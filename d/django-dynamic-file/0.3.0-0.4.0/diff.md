# Comparing `tmp/django-dynamic-file-0.3.0.tar.gz` & `tmp/django-dynamic-file-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dynamic-file-0.3.0.tar", last modified: Mon Jan 23 11:12:29 2023, max compression
+gzip compressed data, was "django-dynamic-file-0.4.0.tar", last modified: Mon May 22 16:34:49 2023, max compression
```

## Comparing `django-dynamic-file-0.3.0.tar` & `django-dynamic-file-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:29.524283 django-dynamic-file-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-01-23 11:12:29.524283 django-dynamic-file-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:29.520283 django-dynamic-file-0.3.0/django_dynamic_file.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-01-23 11:12:29.000000 django-dynamic-file-0.3.0/django_dynamic_file.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-23 11:12:29.000000 django-dynamic-file-0.3.0/django_dynamic_file.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 11:12:29.000000 django-dynamic-file-0.3.0/django_dynamic_file.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-23 11:12:29.000000 django-dynamic-file-0.3.0/django_dynamic_file.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-23 11:12:29.000000 django-dynamic-file-0.3.0/django_dynamic_file.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:29.524283 django-dynamic-file-0.3.0/dynamic_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:29.524283 django-dynamic-file-0.3.0/dynamic_file/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:29.524283 django-dynamic-file-0.3.0/dynamic_file/models/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/models/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:29.524283 django-dynamic-file-0.3.0/dynamic_file/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/serializers/dynamic_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/serializers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:12:29.524283 django-dynamic-file-0.3.0/dynamic_file/views/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/dynamic_file/views/serve_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-01-23 11:12:12.000000 django-dynamic-file-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 11:12:29.524283 django-dynamic-file-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/migrations/0002_alter_dynamicfile_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/models/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/serializers/dynamic_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/serializers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/views/serve_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/tests/test_model_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/tests/test_serializer_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/tests/test_view_serve.py
```

### Comparing `django-dynamic-file-0.3.0/LICENSE` & `django-dynamic-file-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.3.0/PKG-INFO` & `django-dynamic-file-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-file
-Version: 0.3.0
+Version: 0.4.0
 Summary: A flexible approach to handling and serving files with django
 Author-email: Philipp Hafner <philipp@hafner.xyz>
 License: MIT License
         
         Copyright (c) 2022 Philipp Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-dynamic-file-0.3.0/README.rst` & `django-dynamic-file-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.3.0/django_dynamic_file.egg-info/PKG-INFO` & `django-dynamic-file-0.4.0/django_dynamic_file.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-file
-Version: 0.3.0
+Version: 0.4.0
 Summary: A flexible approach to handling and serving files with django
 Author-email: Philipp Hafner <philipp@hafner.xyz>
 License: MIT License
         
         Copyright (c) 2022 Philipp Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-dynamic-file-0.3.0/dynamic_file/config.py` & `django-dynamic-file-0.4.0/dynamic_file/config.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.3.0/dynamic_file/migrations/0001_initial.py` & `django-dynamic-file-0.4.0/dynamic_file/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.3.0/dynamic_file/models/base.py` & `django-dynamic-file-0.4.0/dynamic_file/models/base.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.3.0/dynamic_file/models/file.py` & `django-dynamic-file-0.4.0/dynamic_file/models/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from django.db import models
 from django.utils.translation import gettext as _
 from dynamic_file.models.base import DynamicFileBase
+from dynamic_file.storage import DynamicFileSystemStorage
+
+fs = DynamicFileSystemStorage()
 
 
 class DynamicFile(DynamicFileBase):
     file = models.FileField(
+        storage=fs,
         help_text=_('The uploaded file')
     )
     '''
     The concrete file for this model.
     '''
 
     @property
```

### Comparing `django-dynamic-file-0.3.0/dynamic_file/serializers/fields.py` & `django-dynamic-file-0.4.0/dynamic_file/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.3.0/dynamic_file/views/serve_file.py` & `django-dynamic-file-0.4.0/dynamic_file/views/serve_file.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.3.0/pyproject.toml` & `django-dynamic-file-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-dynamic-file"
-version = "0.3.0"
+version = "0.4.0"
 description = "A flexible approach to handling and serving files with django"
 readme = "README.rst"
 authors = [{ name = "Philipp Hafner", email = "philipp@hafner.xyz" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -31,15 +31,15 @@
 
 [tool.setuptools]
 package-dir = {"dynamic_file" = "dynamic_file"}
 
 
 [tool.bumpver]
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
-current_version = "0.3.0"
+current_version = "0.4.0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

