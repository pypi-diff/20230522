# Comparing `tmp/django_blob_storage-0.2.0.tar.gz` & `tmp/django_blob_storage-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_blob_storage-0.2.0.tar", max compression
+gzip compressed data, was "django_blob_storage-0.2.1.tar", max compression
```

## Comparing `django_blob_storage-0.2.0.tar` & `django_blob_storage-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1484 2023-05-22 07:37:18.198960 django_blob_storage-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     2281 2023-05-22 09:30:22.377803 django_blob_storage-0.2.0/README.md
--rw-r--r--   0        0        0       54 2023-05-22 07:34:31.578014 django_blob_storage-0.2.0/dbstorage/__init__.py
--rw-r--r--   0        0        0     1021 2023-05-22 08:46:01.182879 django_blob_storage-0.2.0/dbstorage/admin.py
--rw-r--r--   0        0        0      183 2023-05-22 08:38:53.584188 django_blob_storage-0.2.0/dbstorage/apps.py
--rw-r--r--   0        0        0     1662 2023-05-22 07:54:21.902824 django_blob_storage-0.2.0/dbstorage/forms.py
--rw-r--r--   0        0        0      933 2023-05-22 07:34:31.578014 django_blob_storage-0.2.0/dbstorage/migrations/0001_initial.py
--rw-r--r--   0        0        0      822 2023-05-22 09:10:19.182752 django_blob_storage-0.2.0/dbstorage/migrations/0002_remove_dbfile_size_dbfile_accessed_on_and_more.py
--rw-r--r--   0        0        0        0 2023-05-22 07:34:31.578014 django_blob_storage-0.2.0/dbstorage/migrations/__init__.py
--rw-r--r--   0        0        0      927 2023-05-22 09:29:31.291084 django_blob_storage-0.2.0/dbstorage/models.py
--rw-r--r--   0        0        0     1850 2023-05-22 08:56:30.881041 django_blob_storage-0.2.0/dbstorage/storage.py
--rw-r--r--   0        0        0      278 2023-05-22 08:31:20.451175 django_blob_storage-0.2.0/dbstorage/urls.py
--rw-r--r--   0        0        0     1440 2023-05-22 09:01:54.365710 django_blob_storage-0.2.0/dbstorage/views.py
--rw-r--r--   0        0        0      423 2023-05-22 09:30:44.507814 django_blob_storage-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 django_blob_storage-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1484 2023-05-22 07:37:18.198960 django_blob_storage-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     2281 2023-05-22 09:30:22.377803 django_blob_storage-0.2.1/README.md
+-rw-r--r--   0        0        0       54 2023-05-22 07:34:31.578014 django_blob_storage-0.2.1/dbstorage/__init__.py
+-rw-r--r--   0        0        0     1021 2023-05-22 08:46:01.182879 django_blob_storage-0.2.1/dbstorage/admin.py
+-rw-r--r--   0        0        0      183 2023-05-22 08:38:53.584188 django_blob_storage-0.2.1/dbstorage/apps.py
+-rw-r--r--   0        0        0     1662 2023-05-22 07:54:21.902824 django_blob_storage-0.2.1/dbstorage/forms.py
+-rw-r--r--   0        0        0      933 2023-05-22 07:34:31.578014 django_blob_storage-0.2.1/dbstorage/migrations/0001_initial.py
+-rw-r--r--   0        0        0      822 2023-05-22 09:10:19.182752 django_blob_storage-0.2.1/dbstorage/migrations/0002_remove_dbfile_size_dbfile_accessed_on_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-22 07:34:31.578014 django_blob_storage-0.2.1/dbstorage/migrations/__init__.py
+-rw-r--r--   0        0        0      927 2023-05-22 09:29:31.291084 django_blob_storage-0.2.1/dbstorage/models.py
+-rw-r--r--   0        0        0     1850 2023-05-22 08:56:30.881041 django_blob_storage-0.2.1/dbstorage/storage.py
+-rw-r--r--   0        0        0      278 2023-05-22 08:31:20.451175 django_blob_storage-0.2.1/dbstorage/urls.py
+-rw-r--r--   0        0        0     1440 2023-05-22 09:01:54.365710 django_blob_storage-0.2.1/dbstorage/views.py
+-rw-r--r--   0        0        0      423 2023-05-22 09:34:21.450916 django_blob_storage-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2758 1970-01-01 00:00:00.000000 django_blob_storage-0.2.1/PKG-INFO
```

### Comparing `django_blob_storage-0.2.0/LICENSE.md` & `django_blob_storage-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.0/README.md` & `django_blob_storage-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.0/dbstorage/admin.py` & `django_blob_storage-0.2.1/dbstorage/admin.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.0/dbstorage/forms.py` & `django_blob_storage-0.2.1/dbstorage/forms.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.0/dbstorage/migrations/0001_initial.py` & `django_blob_storage-0.2.1/dbstorage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.0/dbstorage/migrations/0002_remove_dbfile_size_dbfile_accessed_on_and_more.py` & `django_blob_storage-0.2.1/dbstorage/migrations/0002_remove_dbfile_size_dbfile_accessed_on_and_more.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.0/dbstorage/models.py` & `django_blob_storage-0.2.1/dbstorage/models.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.0/dbstorage/storage.py` & `django_blob_storage-0.2.1/dbstorage/storage.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.0/dbstorage/views.py` & `django_blob_storage-0.2.1/dbstorage/views.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.0/PKG-INFO` & `django_blob_storage-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-blob-storage
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
-License: MIT
+License: BSD
 Author: alex
 Author-email: devkral@web.de
 Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=3.2)
 Description-Content-Type: text/markdown
```

