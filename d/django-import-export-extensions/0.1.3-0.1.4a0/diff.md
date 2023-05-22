# Comparing `tmp/django_import_export_extensions-0.1.3.tar.gz` & `tmp/django_import_export_extensions-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_import_export_extensions-0.1.3.tar", last modified: Tue May 16 06:29:46 2023, max compression
+gzip compressed data, was "django_import_export_extensions-0.1.4a0.tar", last modified: Mon May 22 11:38:47 2023, max compression
```

## Comparing `django_import_export_extensions-0.1.3.tar` & `django_import_export_extensions-0.1.4a0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      176 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/AUTHORS.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3236 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      398 2023-05-16 06:24:50.000000 django_import_export_extensions-0.1.3/HISTORY.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1066 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/LICENSE
--rw-r--r--   0 yalef     (1000) yalef     (1000)      282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/MANIFEST.in
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4412 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/PKG-INFO
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2086 2023-04-27 11:56:03.000000 django_import_export_extensions-0.1.3/README.rst
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.361800 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4412 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/PKG-INFO
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3685 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)      126 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/requires.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)       25 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.365133 django_import_export_extensions-0.1.3/docs/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      625 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/Makefile
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.345134 django_import_export_extensions-0.1.3/docs/_build/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.345134 django_import_export_extensions-0.1.3/docs/_build/html/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.368466 django_import_export_extensions-0.1.3/docs/_build/html/_static/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      286 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.3/docs/_build/html/_static/file.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/authors.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4483 2023-04-27 12:13:39.000000 django_import_export_extensions-0.1.3/docs/conf.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)       33 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/contributing.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/history.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      334 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/index.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2743 2023-05-16 06:24:50.000000 django_import_export_extensions-0.1.3/docs/installation.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      822 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/make.bat
--rw-r--r--   0 yalef     (1000) yalef     (1000)       27 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/readme.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3447 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/usage.rst
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.368466 django_import_export_extensions-0.1.3/import_export_extensions/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      144 2023-05-16 06:24:50.000000 django_import_export_extensions-0.1.3/import_export_extensions/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.371800 django_import_export_extensions-0.1.3/import_export_extensions/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      166 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.371800 django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      100 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      997 2023-05-02 06:15:21.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/export_admin_form.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1177 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/import_admin_form.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.375133 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      155 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      797 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/base.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10885 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/export_mixin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      340 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/import_export_mixin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    12731 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/import_mixin.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.375133 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5715 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/export_job_admin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     7018 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/import_job_admin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3817 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/mixins.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1394 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/widgets.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.375133 django_import_export_extensions-0.1.3/import_export_extensions/api/
--rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      156 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3566 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3158 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      378 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/progress.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/api/views/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       82 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/views/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4418 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/views/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     6243 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/views/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      716 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/apps.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     7233 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/fields.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1315 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/forms.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/migrations/
--rw-r--r--   0 yalef     (1000) yalef     (1000)    12282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/migrations/0001_initial.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/migrations/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/models/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       68 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1267 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/core.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10445 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    17389 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      752 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/tools.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     8148 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/resources.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.348467 django_import_export_extensions-0.1.3/import_export_extensions/static/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.351800 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.351800 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       67 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/admin/admin.css
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.381799 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/widgets/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      626 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.351800 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.381799 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      768 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/admin/admin.js
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.381799 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/widgets/
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1712 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js
--rw-r--r--   0 yalef     (1000) yalef     (1000)      537 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/tasks.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.355134 django_import_export_extensions-0.1.3/import_export_extensions/templates/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.381799 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       37 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/base.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1081 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1482 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2440 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export_status.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1215 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5062 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2413 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import_status.html
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      391 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_export_item.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_import.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      248 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_import_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_import_item.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2571 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/import_job_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5135 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/utils.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    11277 2023-05-15 13:57:42.000000 django_import_export_extensions-0.1.3/import_export_extensions/widgets.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3396 2023-05-16 06:24:50.000000 django_import_export_extensions-0.1.3/pyproject.toml
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/requirements/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      458 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/requirements/production.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)       38 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/setup.cfg
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.022684 django_import_export_extensions-0.1.4a0/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      176 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/AUTHORS.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3236 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/CONTRIBUTING.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      460 2023-05-22 10:02:26.000000 django_import_export_extensions-0.1.4a0/HISTORY.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1066 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/LICENSE
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/MANIFEST.in
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4655 2023-05-22 11:38:47.022684 django_import_export_extensions-0.1.4a0/PKG-INFO
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2331 2023-05-22 09:11:05.000000 django_import_export_extensions-0.1.4a0/README.rst
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.989351 django_import_export_extensions-0.1.4a0/django_import_export_extensions.egg-info/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4655 2023-05-22 11:38:46.000000 django_import_export_extensions-0.1.4a0/django_import_export_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3685 2023-05-22 11:38:46.000000 django_import_export_extensions-0.1.4a0/django_import_export_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-05-22 11:38:46.000000 django_import_export_extensions-0.1.4a0/django_import_export_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      126 2023-05-22 11:38:46.000000 django_import_export_extensions-0.1.4a0/django_import_export_extensions.egg-info/requires.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       25 2023-05-22 11:38:46.000000 django_import_export_extensions-0.1.4a0/django_import_export_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.996018 django_import_export_extensions-0.1.4a0/docs/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      625 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/docs/Makefile
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.979351 django_import_export_extensions-0.1.4a0/docs/_build/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.979351 django_import_export_extensions-0.1.4a0/docs/_build/html/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.996018 django_import_export_extensions-0.1.4a0/docs/_build/html/_static/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      286 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.4a0/docs/_build/html/_static/file.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.4a0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.4a0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/docs/authors.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4483 2023-04-27 12:13:39.000000 django_import_export_extensions-0.1.4a0/docs/conf.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       33 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/docs/contributing.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/docs/history.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      334 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/docs/index.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2743 2023-05-16 06:24:50.000000 django_import_export_extensions-0.1.4a0/docs/installation.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      822 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/docs/make.bat
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       27 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/docs/readme.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3447 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/docs/usage.rst
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.006018 django_import_export_extensions-0.1.4a0/import_export_extensions/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      150 2023-05-22 11:33:18.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.006018 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      166 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.009351 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/forms/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      100 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/forms/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1385 2023-05-22 10:17:36.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/forms/export_admin_form.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1592 2023-05-22 10:23:12.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/forms/import_admin_form.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.009351 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/mixins/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      155 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/mixins/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      797 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/mixins/base.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    10885 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/mixins/export_mixin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      340 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/mixins/import_export_mixin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    12731 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/mixins/import_mixin.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.012684 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/model_admins/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/model_admins/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5715 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/model_admins/export_job_admin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     7018 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/model_admins/import_job_admin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3817 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/model_admins/mixins.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1394 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/admin/widgets.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.012684 django_import_export_extensions-0.1.4a0/import_export_extensions/api/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/api/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.012684 django_import_export_extensions-0.1.4a0/import_export_extensions/api/serializers/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      156 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/api/serializers/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3566 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/api/serializers/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3158 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/api/serializers/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      378 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/api/serializers/progress.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.016018 django_import_export_extensions-0.1.4a0/import_export_extensions/api/views/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       82 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/api/views/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4418 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/api/views/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     6243 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/api/views/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      716 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/apps.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     7233 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/fields.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1315 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/forms.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.016018 django_import_export_extensions-0.1.4a0/import_export_extensions/migrations/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    12282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/migrations/0001_initial.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/migrations/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.016018 django_import_export_extensions-0.1.4a0/import_export_extensions/models/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       68 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/models/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1267 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/models/core.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    10445 2023-05-22 10:13:16.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/models/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    17389 2023-05-22 10:13:59.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/models/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      752 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/models/tools.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     8148 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/resources.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.979351 django_import_export_extensions-0.1.4a0/import_export_extensions/static/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.982684 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.982684 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/css/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.019351 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/css/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       67 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/css/admin/admin.css
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.019351 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/css/widgets/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      626 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.982684 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/js/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.019351 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/js/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      768 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/js/admin/admin.js
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.019351 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/js/widgets/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1712 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      537 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/tasks.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:46.982684 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.022684 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       37 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/base.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1081 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1482 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_export_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2440 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_export_status.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1215 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_import.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5062 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_import_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2413 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_import_status.html
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.022684 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/change_list/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      391 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/change_list/change_list.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/change_list/change_list_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/change_list/change_list_export_item.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/change_list/change_list_import.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      248 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/change_list/change_list_import_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/change_list/change_list_import_item.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2571 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/import_job_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5135 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/utils.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    11277 2023-05-15 13:57:42.000000 django_import_export_extensions-0.1.4a0/import_export_extensions/widgets.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3392 2023-05-22 10:31:22.000000 django_import_export_extensions-0.1.4a0/pyproject.toml
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-22 11:38:47.022684 django_import_export_extensions-0.1.4a0/requirements/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      458 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.4a0/requirements/production.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       38 2023-05-22 11:38:47.022684 django_import_export_extensions-0.1.4a0/setup.cfg
```

### Comparing `django_import_export_extensions-0.1.3/CONTRIBUTING.rst` & `django_import_export_extensions-0.1.4a0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/LICENSE` & `django_import_export_extensions-0.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/PKG-INFO` & `django_import_export_extensions-0.1.4a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_import_export_extensions
-Version: 0.1.3
+Version: 0.1.4a0
 Summary: Extend functionality of `django-import-export`
 Author-email: Saritasa <pypi@saritasa.com>
 License: MIT License
         
         Copyright (c) 2022, Saritasa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/saritasa-nest/django-import-export-extensions
 Project-URL: Bug Tracker, https://github.com/saritasa-nest/django-import-export-extensions/issues
 Keywords: django_import_export_extensions
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -50,14 +50,18 @@
 django-import-export-extensions
 ===============================
 
 .. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
         :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
         :alt: Build status on Github
 
+.. image:: https://coveralls.io/repos/github/saritasa-nest/django-import-export-extensions/badge.svg?branch=main
+        :target: https://coveralls.io/github/saritasa-nest/django-import-export-extensions?branch=main
+        :alt: Test coverage
+
 .. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
         :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported python versions
 
 .. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
         :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported django versions
```

### Comparing `django_import_export_extensions-0.1.3/README.rst` & `django_import_export_extensions-0.1.4a0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 django-import-export-extensions
 ===============================
 
 .. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
         :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
         :alt: Build status on Github
 
+.. image:: https://coveralls.io/repos/github/saritasa-nest/django-import-export-extensions/badge.svg?branch=main
+        :target: https://coveralls.io/github/saritasa-nest/django-import-export-extensions?branch=main
+        :alt: Test coverage
+
 .. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
         :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported python versions
 
 .. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
         :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported django versions
```

### Comparing `django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/PKG-INFO` & `django_import_export_extensions-0.1.4a0/django_import_export_extensions.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export-extensions
-Version: 0.1.3
+Version: 0.1.4a0
 Summary: Extend functionality of `django-import-export`
 Author-email: Saritasa <pypi@saritasa.com>
 License: MIT License
         
         Copyright (c) 2022, Saritasa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/saritasa-nest/django-import-export-extensions
 Project-URL: Bug Tracker, https://github.com/saritasa-nest/django-import-export-extensions/issues
 Keywords: django_import_export_extensions
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -50,14 +50,18 @@
 django-import-export-extensions
 ===============================
 
 .. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
         :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
         :alt: Build status on Github
 
+.. image:: https://coveralls.io/repos/github/saritasa-nest/django-import-export-extensions/badge.svg?branch=main
+        :target: https://coveralls.io/github/saritasa-nest/django-import-export-extensions?branch=main
+        :alt: Test coverage
+
 .. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
         :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported python versions
 
 .. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
         :target: https://pypi.org/project/django-import-export-extensions/
         :alt: Supported django versions
```

### Comparing `django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/SOURCES.txt` & `django_import_export_extensions-0.1.4a0/django_import_export_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/docs/Makefile` & `django_import_export_extensions-0.1.4a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/docs/conf.py` & `django_import_export_extensions-0.1.4a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/docs/installation.rst` & `django_import_export_extensions-0.1.4a0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/docs/make.bat` & `django_import_export_extensions-0.1.4a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/docs/usage.rst` & `django_import_export_extensions-0.1.4a0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/import_admin_form.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/admin/forms/import_admin_form.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,8 +34,24 @@
         )
         self.fields["import_progressbar"].widget = ProgressBarWidget(
             job=instance,
             url=reverse(url_name, args=(instance.id,)),
         )
 
     class Meta:
-        fields = "__all__"
+        fields = (
+            "import_status",
+            "resource_path",
+            "data_file",
+            "resource_kwargs",
+            "traceback",
+            "error_message",
+            "result",
+            "parse_task_id",
+            "import_task_id",
+            "parse_finished",
+            "import_started",
+            "import_finished",
+            "created_by",
+            "created",
+            "modified",
+        )
```

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/base.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/admin/mixins/base.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/export_mixin.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/admin/mixins/export_mixin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/import_mixin.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/admin/mixins/import_mixin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/export_job_admin.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/admin/model_admins/export_job_admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/import_job_admin.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/admin/model_admins/import_job_admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/mixins.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/admin/widgets.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/export_job.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/api/serializers/export_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/import_job.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/api/serializers/import_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/api/views/export_job.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/api/views/export_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/api/views/import_job.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/api/views/import_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/apps.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/apps.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/fields.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/forms.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/migrations/0001_initial.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/models/core.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/models/core.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/models/export_job.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/models/export_job.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -161,14 +161,39 @@
     def __str__(self) -> str:
         """Return string representation."""
         return (
             f"Export job({self.export_status}) <{self.pk}> "
             f"using {self.resource_path}(Format {self.file_format_path})"
         )
 
+    def save(
+        self,
+        force_insert=False,
+        force_update=False,
+        using=None,
+        update_fields=None,
+    ):
+        """Start task for data exporting when ExportJob is created.
+
+        Celery task is manually called with `apply_async`, to provide
+        possibility of custom `task_id` with which task will be run.
+
+        """
+        is_created = self._state.adding
+        super().save(
+            force_insert=force_insert,
+            force_update=force_update,
+            using=using,
+            update_fields=update_fields,
+        )
+        if is_created:
+            self.export_task_id = str(uuid.uuid4())
+            self.save(update_fields=["export_task_id"])
+            transaction.on_commit(self._start_export_data_task)
+
     @property
     def resource(self):
         """Get initialized resource instance."""
         resource_class = module_loading.import_string(self.resource_path)
         resource = resource_class(
             created_by=self.created_by,
             **self.resource_kwargs,
@@ -228,39 +253,14 @@
     @property
     def _incorrect_status_error(self) -> ValueError:
         """Shortcut for raising error when ExportJob is in incorrect state."""
         return ValueError(
             f"Wrong export job status: {self.get_export_status_display()}",
         )
 
-    def save(
-        self,
-        force_insert=False,
-        force_update=False,
-        using=None,
-        update_fields=None,
-    ):
-        """Start task for data exporting when ExportJob is created.
-
-        Celery task is manually called with `apply_async`, to provide
-        possibility of custom `task_id` with which task will be run.
-
-        """
-        is_created = self._state.adding
-        super().save(
-            force_insert=force_insert,
-            force_update=force_update,
-            using=using,
-            update_fields=update_fields,
-        )
-        if is_created:
-            self.export_task_id = str(uuid.uuid4())
-            self.save(update_fields=["export_task_id"])
-            transaction.on_commit(self._start_export_data_task)
-
     def _start_export_data_task(self):
         """Start export data task."""
         from .. import tasks
 
         tasks.export_data_task.apply_async(
             kwargs=dict(job_id=self.pk),
             task_id=self.export_task_id,
```

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/models/import_job.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/models/import_job.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -223,14 +223,39 @@
     def __str__(self) -> str:
         """Return string representation."""
         return (
             f"Import job({self.import_status}) "
             f"<{self.pk}> using {self.resource_path}"
         )
 
+    def save(
+        self,
+        force_insert=False,
+        force_update=False,
+        using=None,
+        update_fields=None,
+    ):
+        """Start task for data parsing when ImportJob is created.
+
+        Celery task is manually called with `apply_async`, to provide
+        possibility of custom `task_id` with which task will be run.
+
+        """
+        is_created = self._state.adding
+        super().save(
+            force_insert=force_insert,
+            force_update=force_update,
+            using=using,
+            update_fields=update_fields,
+        )
+        if is_created:
+            self.parse_task_id = str(uuid.uuid4())
+            self.save(update_fields=["parse_task_id"])
+            transaction.on_commit(self.start_parse_data_task)
+
     @property
     def resource(self):
         """Get initialized resource instance."""
         resource_class = module_loading.import_string(self.resource_path)
         resource = resource_class(
             **self.resource_kwargs,
         )
@@ -286,39 +311,14 @@
     @property
     def _incorrect_status_error(self) -> ValueError:
         """Shortcut for raising error when ImportJob is in incorrect state."""
         return ValueError(
             f"Wrong import job status: {self.get_import_status_display()}",
         )
 
-    def save(
-        self,
-        force_insert=False,
-        force_update=False,
-        using=None,
-        update_fields=None,
-    ):
-        """Start task for data parsing when ImportJob is created.
-
-        Celery task is manually called with `apply_async`, to provide
-        possibility of custom `task_id` with which task will be run.
-
-        """
-        is_created = self._state.adding
-        super().save(
-            force_insert=force_insert,
-            force_update=force_update,
-            using=using,
-            update_fields=update_fields,
-        )
-        if is_created:
-            self.parse_task_id = str(uuid.uuid4())
-            self.save(update_fields=["parse_task_id"])
-            transaction.on_commit(self.start_parse_data_task)
-
     def start_parse_data_task(self):
         """Start parsing task."""
         from .. import tasks
 
         tasks.parse_data_task.apply_async(
             kwargs=dict(job_id=self.pk),
             task_id=self.parse_task_id,
```

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/models/tools.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/models/tools.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/resources.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/resources.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css` & `django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/admin/admin.js` & `django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/js/admin/admin.js`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js` & `django_import_export_extensions-0.1.4a0/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/tasks.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/tasks.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export.html` & `django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_export.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export_results.html` & `django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_export_results.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export_status.html` & `django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_export_status.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import.html` & `django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_import.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import_results.html` & `django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_import_results.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import_status.html` & `django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/celery_import_status.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/import_job_results.html` & `django_import_export_extensions-0.1.4a0/import_export_extensions/templates/admin/import_job_results.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/utils.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/import_export_extensions/widgets.py` & `django_import_export_extensions-0.1.4a0/import_export_extensions/widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.3/pyproject.toml` & `django_import_export_extensions-0.1.4a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 authors = [
     {name = "Saritasa", email = "pypi@saritasa.com"},
 ]
 requires-python = ">=3.9"
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
```

