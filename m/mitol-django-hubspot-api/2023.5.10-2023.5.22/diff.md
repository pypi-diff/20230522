# Comparing `tmp/mitol-django-hubspot-api-2023.5.10.tar.gz` & `tmp/mitol-django-hubspot-api-2023.5.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-hubspot-api-2023.5.10.tar", last modified: Wed May 10 17:42:21 2023, max compression
+gzip compressed data, was "mitol-django-hubspot-api-2023.5.22.tar", last modified: Mon May 22 17:11:53 2023, max compression
```

## Comparing `mitol-django-hubspot-api-2023.5.10.tar` & `mitol-django-hubspot-api-2023.5.22.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.328985 mitol-django-hubspot-api-2023.5.10/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    22389 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      555 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/settings/hubspot_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 17:42:21.328985 mitol-django-hubspot-api-2023.5.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:11:53.659334 mitol-django-hubspot-api-2023.5.22/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-22 17:11:53.655334 mitol-django-hubspot-api-2023.5.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:11:53.655334 mitol-django-hubspot-api-2023.5.22/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:11:53.655334 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22457 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:11:53.655334 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:11:53.655334 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/settings/hubspot_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:11:53.655334 mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-22 17:11:53.000000 mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-22 17:11:53.000000 mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 17:11:53.000000 mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 17:11:53.000000 mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-22 17:11:53.000000 mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 17:11:53.000000 mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 17:11:53.000000 mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 17:11:53.659334 mitol-django-hubspot-api-2023.5.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-05-22 17:11:52.000000 mitol-django-hubspot-api-2023.5.22/setup.py
```

### Comparing `mitol-django-hubspot-api-2023.5.10/PKG-INFO` & `mitol-django-hubspot-api-2023.5.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-hubspot-api
-Version: 2023.5.10
+Version: 2023.5.22
 Summary: Django application for Hubspot API integration
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-hubspot-api-2023.5.10/backend_shim.py` & `mitol-django-hubspot-api-2023.5.22/backend_shim.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/README.md` & `mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/api.py` & `mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,18 +242,19 @@
                 )
                 if secondary_email == user_email:
                     # Retry contact update w/this email
                     retry_update = True
                 elif secondary_email:
                     # Retry contact creation w/this email
                     retry_create = True
-            elif object_id and not ignore_conflict:
-                retry_update = True
-            elif ignore_conflict:
-                return SimplePublicObject(id=hubspot_id)
+            if not retry_create and not retry_update:
+                if object_id and not ignore_conflict:
+                    retry_update = True
+                elif ignore_conflict:
+                    return SimplePublicObject(id=hubspot_id)
             if retry_update:
                 return HubspotApi().crm.objects.basic_api.update(
                     simple_public_object_input=body,
                     object_id=hubspot_id,
                     object_type=hubspot_type,
                 )
             elif retry_create:
```

### Comparing `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/decorators.py` & `mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/decorators.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/factories.py` & `mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/factories.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/migrations/0001_initial.py` & `mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/models.py` & `mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/models.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/settings/hubspot_api.py` & `mitol-django-hubspot-api-2023.5.22/mitol/hubspot_api/settings/hubspot_api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/PKG-INFO` & `mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-hubspot-api
-Version: 2023.5.10
+Version: 2023.5.22
 Summary: Django application for Hubspot API integration
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/SOURCES.txt` & `mitol-django-hubspot-api-2023.5.22/mitol_django_hubspot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-2023.5.10/setup.py` & `mitol-django-hubspot-api-2023.5.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,10 +98,10 @@
     'packages': (
         'mitol',
         'mitol.hubspot_api',
         'mitol.hubspot_api.migrations',
         'mitol.hubspot_api.settings',
     ),
     'python_requires': '>=3.8',
-    'version': '2023.5.10',
+    'version': '2023.5.22',
     'zip_safe': True,
 })
```

