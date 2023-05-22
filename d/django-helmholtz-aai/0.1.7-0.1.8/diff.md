# Comparing `tmp/django-helmholtz-aai-0.1.7.tar.gz` & `tmp/django-helmholtz-aai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-helmholtz-aai-0.1.7.tar", last modified: Thu Mar 23 16:55:42 2023, max compression
+gzip compressed data, was "django-helmholtz-aai-0.1.8.tar", last modified: Mon May 22 15:22:01 2023, max compression
```

## Comparing `django-helmholtz-aai-0.1.7.tar` & `django-helmholtz-aai-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)    13827 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2989 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1507 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/
--rw-rw-rw-   0 root         (0) root         (0)     1999 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     9084 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1031 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/management/commands/remove_empty_vos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2782 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/migrations/0002_auto_20220214_1413.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/migrations/0003_auto_20220301_1739.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4982 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     6901 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1568 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/templatetags/helmholtz_aai.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/tests/
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10716 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/tests/test_authentification_view.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    17543 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2989 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1172 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      387 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/django_helmholtz_aai.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-03-23 16:55:42.000000 django-helmholtz-aai-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    80403 2023-03-23 16:55:12.000000 django-helmholtz-aai-0.1.7/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:22:01.022231 django-helmholtz-aai-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)    13827 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-22 15:22:01.022231 django-helmholtz-aai-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:22:01.022231 django-helmholtz-aai-0.1.8/django_helmholtz_aai/
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-22 15:22:01.022231 django-helmholtz-aai-0.1.8/django_helmholtz_aai/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     9084 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:22:01.018231 django-helmholtz-aai-0.1.8/django_helmholtz_aai/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 15:21:40.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:22:01.018231 django-helmholtz-aai-0.1.8/django_helmholtz_aai/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 15:21:40.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/management/commands/remove_empty_vos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:22:01.022231 django-helmholtz-aai-0.1.8/django_helmholtz_aai/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/migrations/0002_auto_20220214_1413.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/migrations/0003_auto_20220301_1739.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4982 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 15:21:40.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     6901 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:22:01.022231 django-helmholtz-aai-0.1.8/django_helmholtz_aai/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 15:21:40.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/templatetags/helmholtz_aai.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:22:01.022231 django-helmholtz-aai-0.1.8/django_helmholtz_aai/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11219 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/tests/test_authentification_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    17543 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:22:01.018231 django-helmholtz-aai-0.1.8/django_helmholtz_aai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-22 15:22:01.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-05-22 15:22:01.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 15:22:01.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-22 15:22:01.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 15:22:01.000000 django-helmholtz-aai-0.1.8/django_helmholtz_aai.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2023-05-22 15:22:01.022231 django-helmholtz-aai-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    80403 2023-05-22 15:21:39.000000 django-helmholtz-aai-0.1.8/versioneer.py
```

### Comparing `django-helmholtz-aai-0.1.7/LICENSE` & `django-helmholtz-aai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/PKG-INFO` & `django-helmholtz-aai-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-helmholtz-aai
-Version: 0.1.7
+Version: 0.1.8
 Summary: A generic Django app to login via Helmholtz AAI
 Home-page: https://gitlab.hzdr.de/HCDC/django/django-helmholtz-aai
 Author: Phiilpp S. Sommer, Housam Dibeh, Hatef Takyar
 Author-email: hcdc_support@hereon.de
 License: EUPL-1.2
 Project-URL: Documentation, https://django-helmholtz-aai.readthedocs.io
 Project-URL: Source, https://gitlab.hzdr.de/hcdc/django/django-helmholtz-aai
```

### Comparing `django-helmholtz-aai-0.1.7/README.rst` & `django-helmholtz-aai-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/__init__.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/__init__.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/admin.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/admin.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/app_settings.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/apps.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/apps.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/management/commands/remove_empty_vos.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/management/commands/remove_empty_vos.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/migrations/0001_initial.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/migrations/0002_auto_20220214_1413.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/migrations/0002_auto_20220214_1413.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/migrations/0003_auto_20220301_1739.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/migrations/0003_auto_20220301_1739.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/migrations/__init__.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/models.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/models.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/signals.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/signals.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/templatetags/helmholtz_aai.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/templatetags/helmholtz_aai.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/tests/__init__.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/tests/test_authentification_view.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/tests/test_authentification_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # program. If not, see https://www.eupl.eu/.
 
 
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Any, Callable
+from unittest import mock
 
 import pytest
 from django.contrib.auth.middleware import AuthenticationMiddleware
 from django.contrib.messages.middleware import MessageMiddleware
 from django.contrib.sessions.middleware import SessionMiddleware
 from django.core.exceptions import PermissionDenied
 from django.utils.functional import cached_property
@@ -88,22 +89,31 @@
 
 
 @pytest.fixture
 def authentification_view(db, rf: RequestFactory, userinfo: dict[str, Any]):
 
     request = rf.get("/helmholtz-aai/auth/")
 
-    session_middleware = SessionMiddleware()
+    # Passing None as the first argument to MiddlewareMixin.__init__() (which
+    # is used by Session-, Authentication- and Message Middleware) is
+    # deprecated from Django 3.1
+    # (https://docs.djangoproject.com/en/4.2/releases/3.1/#id2) and removed
+    # in Django 4.0
+    # (https://docs.djangoproject.com/en/4.2/releases/4.0/#features-removed-in-4-0)
+    # so it has to be mocked in this place
+    get_response = mock.MagicMock()
+
+    session_middleware = SessionMiddleware(get_response)
     session_middleware.process_request(request)
     request.session.save()
 
-    auth_middleware = AuthenticationMiddleware()
+    auth_middleware = AuthenticationMiddleware(get_response)
     auth_middleware.process_request(request)
 
-    message_middleware = MessageMiddleware()
+    message_middleware = MessageMiddleware(get_response)
     message_middleware.process_request(request)
 
     view = PatchedHelmholtzAuthentificationView()
     view._userinfo = userinfo
     view.setup(request)
     return view
```

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/urls.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/urls.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai/views.py` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai/views.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai.egg-info/PKG-INFO` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-helmholtz-aai
-Version: 0.1.7
+Version: 0.1.8
 Summary: A generic Django app to login via Helmholtz AAI
 Home-page: https://gitlab.hzdr.de/HCDC/django/django-helmholtz-aai
 Author: Phiilpp S. Sommer, Housam Dibeh, Hatef Takyar
 Author-email: hcdc_support@hereon.de
 License: EUPL-1.2
 Project-URL: Documentation, https://django-helmholtz-aai.readthedocs.io
 Project-URL: Source, https://gitlab.hzdr.de/hcdc/django/django-helmholtz-aai
```

### Comparing `django-helmholtz-aai-0.1.7/django_helmholtz_aai.egg-info/SOURCES.txt` & `django-helmholtz-aai-0.1.8/django_helmholtz_aai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/setup.cfg` & `django-helmholtz-aai-0.1.8/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 [options]
 include_package_data = true
 python_requires = >=3.7
 packages = find:
 install_requires = 
 	requests
-	Django>=3.1,<3.3
+	Django>=3.1
 	authlib
 
 [options.package_data]
 * = 
 	static/**
 	templates/**
 	py.typed
```

### Comparing `django-helmholtz-aai-0.1.7/setup.py` & `django-helmholtz-aai-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `django-helmholtz-aai-0.1.7/versioneer.py` & `django-helmholtz-aai-0.1.8/versioneer.py`

 * *Files identical despite different names*

