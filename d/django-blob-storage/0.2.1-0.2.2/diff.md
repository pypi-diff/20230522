# Comparing `tmp/django_blob_storage-0.2.1.tar.gz` & `tmp/django_blob_storage-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_blob_storage-0.2.1.tar", max compression
+gzip compressed data, was "django_blob_storage-0.2.2.tar", max compression
```

## Comparing `django_blob_storage-0.2.1.tar` & `django_blob_storage-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1484 2023-05-22 07:37:18.198960 django_blob_storage-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     2281 2023-05-22 09:30:22.377803 django_blob_storage-0.2.1/README.md
--rw-r--r--   0        0        0       54 2023-05-22 07:34:31.578014 django_blob_storage-0.2.1/dbstorage/__init__.py
--rw-r--r--   0        0        0     1021 2023-05-22 08:46:01.182879 django_blob_storage-0.2.1/dbstorage/admin.py
--rw-r--r--   0        0        0      183 2023-05-22 08:38:53.584188 django_blob_storage-0.2.1/dbstorage/apps.py
--rw-r--r--   0        0        0     1662 2023-05-22 07:54:21.902824 django_blob_storage-0.2.1/dbstorage/forms.py
--rw-r--r--   0        0        0      933 2023-05-22 07:34:31.578014 django_blob_storage-0.2.1/dbstorage/migrations/0001_initial.py
--rw-r--r--   0        0        0      822 2023-05-22 09:10:19.182752 django_blob_storage-0.2.1/dbstorage/migrations/0002_remove_dbfile_size_dbfile_accessed_on_and_more.py
--rw-r--r--   0        0        0        0 2023-05-22 07:34:31.578014 django_blob_storage-0.2.1/dbstorage/migrations/__init__.py
--rw-r--r--   0        0        0      927 2023-05-22 09:29:31.291084 django_blob_storage-0.2.1/dbstorage/models.py
--rw-r--r--   0        0        0     1850 2023-05-22 08:56:30.881041 django_blob_storage-0.2.1/dbstorage/storage.py
--rw-r--r--   0        0        0      278 2023-05-22 08:31:20.451175 django_blob_storage-0.2.1/dbstorage/urls.py
--rw-r--r--   0        0        0     1440 2023-05-22 09:01:54.365710 django_blob_storage-0.2.1/dbstorage/views.py
--rw-r--r--   0        0        0      423 2023-05-22 09:34:21.450916 django_blob_storage-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2758 1970-01-01 00:00:00.000000 django_blob_storage-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1484 2023-05-22 07:37:18.198960 django_blob_storage-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     2281 2023-05-22 09:30:22.377803 django_blob_storage-0.2.2/README.md
+-rw-r--r--   0        0        0       54 2023-05-22 07:34:31.578014 django_blob_storage-0.2.2/dbstorage/__init__.py
+-rw-r--r--   0        0        0     1021 2023-05-22 08:46:01.182879 django_blob_storage-0.2.2/dbstorage/admin.py
+-rw-r--r--   0        0        0      183 2023-05-22 08:38:53.584188 django_blob_storage-0.2.2/dbstorage/apps.py
+-rw-r--r--   0        0        0     1662 2023-05-22 07:54:21.902824 django_blob_storage-0.2.2/dbstorage/forms.py
+-rw-r--r--   0        0        0      933 2023-05-22 07:34:31.578014 django_blob_storage-0.2.2/dbstorage/migrations/0001_initial.py
+-rw-r--r--   0        0        0      822 2023-05-22 09:10:19.182752 django_blob_storage-0.2.2/dbstorage/migrations/0002_remove_dbfile_size_dbfile_accessed_on_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-22 07:34:31.578014 django_blob_storage-0.2.2/dbstorage/migrations/__init__.py
+-rw-r--r--   0        0        0      927 2023-05-22 09:29:31.291084 django_blob_storage-0.2.2/dbstorage/models.py
+-rw-r--r--   0        0        0     1850 2023-05-22 08:56:30.881041 django_blob_storage-0.2.2/dbstorage/storage.py
+-rw-r--r--   0        0        0      278 2023-05-22 08:31:20.451175 django_blob_storage-0.2.2/dbstorage/urls.py
+-rw-r--r--   0        0        0     1440 2023-05-22 09:43:16.662058 django_blob_storage-0.2.2/dbstorage/views.py
+-rw-r--r--   0        0        0      423 2023-05-22 09:43:22.112028 django_blob_storage-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2758 1970-01-01 00:00:00.000000 django_blob_storage-0.2.2/PKG-INFO
```

### Comparing `django_blob_storage-0.2.1/LICENSE.md` & `django_blob_storage-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.1/README.md` & `django_blob_storage-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.1/dbstorage/admin.py` & `django_blob_storage-0.2.2/dbstorage/admin.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.1/dbstorage/forms.py` & `django_blob_storage-0.2.2/dbstorage/forms.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.1/dbstorage/migrations/0001_initial.py` & `django_blob_storage-0.2.2/dbstorage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.1/dbstorage/migrations/0002_remove_dbfile_size_dbfile_accessed_on_and_more.py` & `django_blob_storage-0.2.2/dbstorage/migrations/0002_remove_dbfile_size_dbfile_accessed_on_and_more.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.1/dbstorage/models.py` & `django_blob_storage-0.2.2/dbstorage/models.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.1/dbstorage/storage.py` & `django_blob_storage-0.2.2/dbstorage/storage.py`

 * *Files identical despite different names*

### Comparing `django_blob_storage-0.2.1/dbstorage/views.py` & `django_blob_storage-0.2.2/dbstorage/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import mimetypes
 import time
 
+from django.conf import settings
+from django.db.models.functions import Now
 from django.http.response import FileResponse, HttpResponseNotModified
 from django.shortcuts import get_object_or_404
 from django.utils.http import http_date
 from django.views.generic.base import View
 from django.views.static import was_modified_since
-from django.utils import timezone
-from django.conf import settings
 
 from dbstorage.models import DBFile
 
 
 class DBFileView(View):
     def get(self, request, name):
         """Endpoint to return memory storage file"""
         db_file_query = DBFile.objects.defer("content").filter(name=name)
         db_file = get_object_or_404(db_file_query)
         if getattr(settings, "DJANGO_DBFILE_TRACK_ACCESSED", False):
-            db_file_query.update(accessed_on=timezone.now())
+            db_file_query.update(accessed_on=Now())
 
         mtime = time.mktime(db_file.updated_on.timetuple())
         modified = was_modified_since(
             header=self.request.META.get("HTTP_IF_MODIFIED_SINCE"),
             mtime=mtime,
         )
```

### Comparing `django_blob_storage-0.2.1/PKG-INFO` & `django_blob_storage-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-blob-storage
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 License: BSD
 Author: alex
 Author-email: devkral@web.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

