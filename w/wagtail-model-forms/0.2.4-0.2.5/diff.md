# Comparing `tmp/wagtail-model-forms-0.2.4.tar.gz` & `tmp/wagtail-model-forms-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-model-forms-0.2.4.tar", last modified: Mon Apr 24 09:08:24 2023, max compression
+gzip compressed data, was "wagtail-model-forms-0.2.5.tar", last modified: Mon May 22 15:07:08 2023, max compression
```

## Comparing `wagtail-model-forms-0.2.4.tar` & `wagtail-model-forms-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-24 09:08:24.748816 wagtail-model-forms-0.2.4/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1064 2022-07-18 08:50:50.000000 wagtail-model-forms-0.2.4/LICENSE
--rw-r--r--   0 robmoorman   (501) staff       (20)      175 2022-08-04 10:38:05.000000 wagtail-model-forms-0.2.4/MANIFEST.in
--rw-r--r--   0 robmoorman   (501) staff       (20)      553 2023-04-24 09:08:24.748397 wagtail-model-forms-0.2.4/PKG-INFO
--rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-04-24 09:08:24.748916 wagtail-model-forms-0.2.4/setup.cfg
--rw-r--r--   0 robmoorman   (501) staff       (20)      996 2023-04-24 09:06:26.000000 wagtail-model-forms-0.2.4/setup.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-24 09:08:24.741796 wagtail-model-forms-0.2.4/src/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-24 09:08:24.746506 wagtail-model-forms-0.2.4/src/wagtail_model_forms/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1160 2022-08-04 13:25:28.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     1056 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms/blocks.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     1431 2023-04-24 09:03:30.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms/mixins.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     2892 2022-12-13 09:18:55.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms/models.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      390 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms/settings.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-24 09:08:24.742108 wagtail-model-forms-0.2.4/src/wagtail_model_forms/templates/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-24 09:08:24.747304 wagtail-model-forms-0.2.4/src/wagtail_model_forms/templates/wagtail_model_forms/
--rw-r--r--   0 robmoorman   (501) staff       (20)      299 2022-08-04 13:28:34.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms/templates/wagtail_model_forms/form.html
--rw-r--r--   0 robmoorman   (501) staff       (20)     1755 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms/templates/wagtail_model_forms/form_submissions_report.html
--rw-r--r--   0 robmoorman   (501) staff       (20)     1347 2023-04-24 09:04:42.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms/views.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      847 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms/wagtail_hooks.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-24 09:08:24.747751 wagtail-model-forms-0.2.4/src/wagtail_model_forms.egg-info/
--rw-r--r--   0 robmoorman   (501) staff       (20)      423 2023-04-24 09:08:24.000000 wagtail-model-forms-0.2.4/src/wagtail_model_forms.egg-info/SOURCES.txt
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.140406 wagtail-model-forms-0.2.5/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1064 2022-07-18 08:50:50.000000 wagtail-model-forms-0.2.5/LICENSE
+-rw-r--r--   0 robmoorman   (501) staff       (20)      175 2022-08-04 10:38:05.000000 wagtail-model-forms-0.2.5/MANIFEST.in
+-rw-r--r--   0 robmoorman   (501) staff       (20)      553 2023-05-22 15:07:08.140097 wagtail-model-forms-0.2.5/PKG-INFO
+-rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-05-22 15:07:08.140498 wagtail-model-forms-0.2.5/setup.cfg
+-rw-r--r--   0 robmoorman   (501) staff       (20)      996 2023-05-22 15:06:40.000000 wagtail-model-forms-0.2.5/setup.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.135020 wagtail-model-forms-0.2.5/src/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.138605 wagtail-model-forms-0.2.5/src/wagtail_model_forms/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1160 2022-08-04 13:25:28.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1056 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/blocks.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1431 2023-04-24 09:03:30.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/mixins.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2892 2022-12-13 09:18:55.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/models.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      390 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/settings.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.135304 wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.139259 wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/wagtail_model_forms/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      299 2022-08-04 13:28:34.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/wagtail_model_forms/form.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1755 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/wagtail_model_forms/form_submissions_report.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1347 2023-04-24 09:04:42.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/views.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      928 2023-05-22 15:06:49.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/wagtail_hooks.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.139711 wagtail-model-forms-0.2.5/src/wagtail_model_forms.egg-info/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      423 2023-05-22 15:07:08.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms.egg-info/SOURCES.txt
```

### Comparing `wagtail-model-forms-0.2.4/LICENSE` & `wagtail-model-forms-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.4/PKG-INFO` & `wagtail-model-forms-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-model-forms
-Version: 0.2.4
+Version: 0.2.5
 Author: R. Moorman <rob@vicktor.nl>
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `wagtail-model-forms-0.2.4/setup.py` & `wagtail-model-forms-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "pytest",
     "pytest-cov",
     "pytest-django",
 ]
 
 setup(
     name="wagtail-model-forms",
-    version="0.2.4",
+    version="0.2.5",
     description="",
     author="R. Moorman <rob@vicktor.nl>",
     install_requires=install_requires,
     tests_requires=tests_requires,
     extras_require={"test": tests_requires},
     package_dir={"": "src"},
     packages=find_packages("src"),
```

### Comparing `wagtail-model-forms-0.2.4/src/wagtail_model_forms/__init__.py` & `wagtail-model-forms-0.2.5/src/wagtail_model_forms/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.4/src/wagtail_model_forms/blocks.py` & `wagtail-model-forms-0.2.5/src/wagtail_model_forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.4/src/wagtail_model_forms/mixins.py` & `wagtail-model-forms-0.2.5/src/wagtail_model_forms/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.4/src/wagtail_model_forms/models.py` & `wagtail-model-forms-0.2.5/src/wagtail_model_forms/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.4/src/wagtail_model_forms/templates/wagtail_model_forms/form_submissions_report.html` & `wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/wagtail_model_forms/form_submissions_report.html`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.4/src/wagtail_model_forms/views.py` & `wagtail-model-forms-0.2.5/src/wagtail_model_forms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.4/src/wagtail_model_forms/wagtail_hooks.py` & `wagtail-model-forms-0.2.5/src/wagtail_model_forms/wagtail_hooks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from django.urls import path, reverse
-from wagtail.admin.menu import AdminOnlyMenuItem
+from wagtail.admin.menu import MenuItem
 from wagtail.core import hooks
 
 from wagtail_model_forms.settings import REPORTS
 from wagtail_model_forms.views import FormSubmissionReportView
 
+
+class ReportsMenuItem(MenuItem):
+    def is_shown(self, request):
+        return REPORTS
+
+
 if REPORTS:
 
     @hooks.register("register_reports_menu_item")
     def register_report_menu_item():
-        return AdminOnlyMenuItem(
+        return ReportsMenuItem(
             FormSubmissionReportView.title,
             reverse("form_submissions_report"),
             classnames="icon icon-" + FormSubmissionReportView.header_icon,
             order=700,
         )
 
     @hooks.register("register_admin_urls")
```

