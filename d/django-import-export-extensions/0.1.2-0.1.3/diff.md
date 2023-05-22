# Comparing `tmp/django_import_export_extensions-0.1.2.tar.gz` & `tmp/django_import_export_extensions-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_import_export_extensions-0.1.2.tar", last modified: Mon May 15 13:17:46 2023, max compression
+gzip compressed data, was "django_import_export_extensions-0.1.3.tar", last modified: Tue May 16 06:29:46 2023, max compression
```

## Comparing `django_import_export_extensions-0.1.2.tar` & `django_import_export_extensions-0.1.3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.799049 django_import_export_extensions-0.1.2/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      176 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/AUTHORS.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3236 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      293 2023-05-15 13:15:23.000000 django_import_export_extensions-0.1.2/HISTORY.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1066 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/LICENSE
--rw-r--r--   0 yalef     (1000) yalef     (1000)      282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/MANIFEST.in
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3343 2023-05-15 13:17:46.802382 django_import_export_extensions-0.1.2/PKG-INFO
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2086 2023-04-27 11:56:03.000000 django_import_export_extensions-0.1.2/README.rst
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.785715 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3343 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/PKG-INFO
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3773 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)       79 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/entry_points.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/not-zip-safe
--rw-r--r--   0 yalef     (1000) yalef     (1000)      126 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/requires.txt
--rw-r--r--   0 yalef     (1000) yalef     (1000)       25 2023-05-15 13:17:46.000000 django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.789049 django_import_export_extensions-0.1.2/docs/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      625 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/Makefile
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.772382 django_import_export_extensions-0.1.2/docs/_build/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.772382 django_import_export_extensions-0.1.2/docs/_build/html/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.789049 django_import_export_extensions-0.1.2/docs/_build/html/_static/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      286 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.2/docs/_build/html/_static/file.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.2/docs/_build/html/_static/plus.png
--rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/authors.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4483 2023-04-27 12:13:39.000000 django_import_export_extensions-0.1.2/docs/conf.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)       33 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/contributing.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/history.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      334 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/index.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2754 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/installation.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)      822 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/make.bat
--rw-r--r--   0 yalef     (1000) yalef     (1000)       27 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/readme.rst
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3447 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/docs/usage.rst
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.789049 django_import_export_extensions-0.1.2/import_export_extensions/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      144 2023-05-15 13:01:32.000000 django_import_export_extensions-0.1.2/import_export_extensions/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.789049 django_import_export_extensions-0.1.2/import_export_extensions/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      166 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      100 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      997 2023-05-02 06:15:21.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/export_admin_form.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1177 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/import_admin_form.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      155 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      797 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/base.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10885 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/export_mixin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      340 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/import_export_mixin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    12731 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/import_mixin.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5715 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/export_job_admin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     7018 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/import_job_admin.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3817 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/mixins.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1394 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/admin/widgets.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/api/
--rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.792382 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      156 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3566 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     3158 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      378 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/progress.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/api/views/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       82 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/views/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     4418 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/views/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     6243 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/api/views/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      716 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/apps.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     7233 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/fields.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1315 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/forms.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/migrations/
--rw-r--r--   0 yalef     (1000) yalef     (1000)    12282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/migrations/0001_initial.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/migrations/__init__.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/models/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       68 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/__init__.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1267 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/core.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    10445 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/export_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    17389 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/import_job.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)      752 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/models/tools.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     8148 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/resources.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.779048 django_import_export_extensions-0.1.2/import_export_extensions/static/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.782382 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.782382 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       67 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/admin/admin.css
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/widgets/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      626 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.782382 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      768 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/admin/admin.js
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.795715 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/widgets/
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1712 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js
--rw-r--r--   0 yalef     (1000) yalef     (1000)      537 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/tasks.py
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.782382 django_import_export_extensions-0.1.2/import_export_extensions/templates/
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.799049 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/
--rw-r--r--   0 yalef     (1000) yalef     (1000)       37 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/base.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1081 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1482 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2440 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export_status.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1215 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5062 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2413 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import_status.html
-drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-15 13:17:46.799049 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/
--rw-r--r--   0 yalef     (1000) yalef     (1000)      391 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_export_item.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_import.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      248 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_import_export.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/change_list/change_list_import_item.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2571 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/import_job_results.html
--rw-r--r--   0 yalef     (1000) yalef     (1000)     5135 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.2/import_export_extensions/utils.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)    11277 2023-05-15 13:15:23.000000 django_import_export_extensions-0.1.2/import_export_extensions/widgets.py
--rw-r--r--   0 yalef     (1000) yalef     (1000)     1791 2023-05-15 13:17:46.805716 django_import_export_extensions-0.1.2/setup.cfg
--rw-r--r--   0 yalef     (1000) yalef     (1000)     2486 2023-05-15 13:15:23.000000 django_import_export_extensions-0.1.2/setup.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      176 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/AUTHORS.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3236 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      398 2023-05-16 06:24:50.000000 django_import_export_extensions-0.1.3/HISTORY.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1066 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/LICENSE
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/MANIFEST.in
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4412 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/PKG-INFO
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2086 2023-04-27 11:56:03.000000 django_import_export_extensions-0.1.3/README.rst
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.361800 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4412 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3685 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        1 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      126 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/requires.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       25 2023-05-16 06:29:46.000000 django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.365133 django_import_export_extensions-0.1.3/docs/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      625 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/Makefile
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.345134 django_import_export_extensions-0.1.3/docs/_build/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.345134 django_import_export_extensions-0.1.3/docs/_build/html/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.368466 django_import_export_extensions-0.1.3/docs/_build/html/_static/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      286 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.3/docs/_build/html/_static/file.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-05 15:45:06.000000 django_import_export_extensions-0.1.3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/authors.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4483 2023-04-27 12:13:39.000000 django_import_export_extensions-0.1.3/docs/conf.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       33 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/contributing.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       28 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/history.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      334 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/index.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2743 2023-05-16 06:24:50.000000 django_import_export_extensions-0.1.3/docs/installation.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      822 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/make.bat
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       27 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/readme.rst
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3447 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/docs/usage.rst
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.368466 django_import_export_extensions-0.1.3/import_export_extensions/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      144 2023-05-16 06:24:50.000000 django_import_export_extensions-0.1.3/import_export_extensions/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.371800 django_import_export_extensions-0.1.3/import_export_extensions/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      166 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.371800 django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      100 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      997 2023-05-02 06:15:21.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/export_admin_form.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1177 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/import_admin_form.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.375133 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      155 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      797 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/base.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    10885 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/export_mixin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      340 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/import_export_mixin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    12731 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/import_mixin.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.375133 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       90 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5715 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/export_job_admin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     7018 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/import_job_admin.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3817 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/mixins.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1394 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/admin/widgets.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.375133 django_import_export_extensions-0.1.3/import_export_extensions/api/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      156 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3566 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3158 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      378 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/progress.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/api/views/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       82 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/views/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     4418 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/views/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     6243 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/api/views/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      716 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/apps.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     7233 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/fields.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1315 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/forms.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/migrations/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    12282 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/migrations/0001_initial.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)        0 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/migrations/__init__.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/models/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       68 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/__init__.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1267 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/core.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    10445 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/export_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    17389 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/import_job.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      752 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/models/tools.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     8148 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/resources.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.348467 django_import_export_extensions-0.1.3/import_export_extensions/static/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.351800 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.351800 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.378466 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       67 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/admin/admin.css
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.381799 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/widgets/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      626 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.351800 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.381799 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      768 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/admin/admin.js
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.381799 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/widgets/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1712 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      537 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/tasks.py
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.355134 django_import_export_extensions-0.1.3/import_export_extensions/templates/
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.381799 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       37 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/base.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1081 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1482 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2440 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export_status.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     1215 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5062 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2413 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import_status.html
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      391 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_export_item.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      183 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_import.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      248 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_import_export.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      171 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/change_list/change_list_import_item.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     2571 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/import_job_results.html
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     5135 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/import_export_extensions/utils.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)    11277 2023-05-15 13:57:42.000000 django_import_export_extensions-0.1.3/import_export_extensions/widgets.py
+-rw-r--r--   0 yalef     (1000) yalef     (1000)     3396 2023-05-16 06:24:50.000000 django_import_export_extensions-0.1.3/pyproject.toml
+drwxr-xr-x   0 yalef     (1000) yalef     (1000)        0 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/requirements/
+-rw-r--r--   0 yalef     (1000) yalef     (1000)      458 2023-04-18 11:22:55.000000 django_import_export_extensions-0.1.3/requirements/production.txt
+-rw-r--r--   0 yalef     (1000) yalef     (1000)       38 2023-05-16 06:29:46.385133 django_import_export_extensions-0.1.3/setup.cfg
```

### Comparing `django_import_export_extensions-0.1.2/CONTRIBUTING.rst` & `django_import_export_extensions-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/LICENSE` & `django_import_export_extensions-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/PKG-INFO` & `django_import_export_extensions-0.1.3/docs/installation.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,105 @@
-Metadata-Version: 2.1
-Name: django_import_export_extensions
-Version: 0.1.2
-Summary: Extend functionality of `django-import-export`
-Home-page: https://github.com/saritasa-nest/django-import-export-extensions
-Author: Saritasa
-Author-email: pypi@saritasa.com
-License: MIT license
-Keywords: django_import_export_extensions
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-===============================
-django-import-export-extensions
-===============================
-
-.. image:: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml/badge.svg
-        :target: https://github.com/saritasa-nest/django-import-export-extensions/actions/workflows/checks.yml
-        :alt: Build status on Github
-
-.. image:: https://img.shields.io/badge/python%20versions-3.9%20%7C%203.10%20%7C%203.11-blue
-        :target: https://pypi.org/project/django-import-export-extensions/
-        :alt: Supported python versions
-
-.. image:: https://img.shields.io/badge/django--versions-3.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-blue
-        :target: https://pypi.org/project/django-import-export-extensions/
-        :alt: Supported django versions
-
-.. image:: https://readthedocs.org/projects/django-import-export-extensions/badge/?version=latest
-    :target: https://django-import-export-extensions.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
-Description
------------
-`django-import-export-extensions` extends the functionality of
-`django-import-export <https://github.com/django-import-export/django-import-export/>`_
-adding the following features:
-
-* Import/export resources in the background via Celery
-* Manage import/export jobs via Django Admin
-* DRF integration that allows to work with import/export jobs via API
-* Support `drf-spectacular <https://github.com/tfranzel/drf-spectacular>`_ generated API schema
-* Additional fields and widgets (FileWidget, IntermediateM2MWidget, M2MField)
-
-Migration from django-import-export
------------------------------------
-Resources migration
-^^^^^^^^^^^^^^^^^^^
-Change ``Resource`` or ``ModelResource`` to
-``CeleryResource`` or ``CeleryModelResource`` respectively.
-
-Admin migration
-^^^^^^^^^^^^^^^
-Change ``ImportMixin``, ``ExportMixin``, ``ImportExportMixin``
-to ``CeleryImportMixin``, ``CeleryExportMixin`` or ``CeleryImportExportMixin`` respectively.
-
-License
--------
-* Free software: MIT license
-* Documentation: https://django-import-export-extensions.readthedocs.io.
-
-
-=======
-History
-=======
-
-0.1.2 (2023-05-12)
-------------------
-
-* Add support for `STORAGES` settings variable
-
-0.1.1 (2023-04-27)
-------------------
+.. highlight:: shell
 
-* Add package description
-* Add configuration file for read-the-docs service
+==============================
+Installation and Configuration
+==============================
 
-0.1.0 (2023-04-01)
-------------------
 
-* First release on PyPI.
+Stable release
+--------------
+
+To install django-import-export-extensions, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install django-import-export-extensions
+
+This is the preferred method to install django-import-export-extensions, as it will always install the most recent stable release.
+
+If you don't have `pip`_ installed, this `Python installation guide`_ can guide
+you through the process.
+
+.. _pip: https://pip.pypa.io
+.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
+
+
+From sources
+------------
+
+The sources for django-import-export-extensions can be downloaded from the `Github repo`_.
+
+You can either clone the public repository:
+
+.. code-block:: console
+
+    $ git clone https://github.com/saritasa-nest/django-import-export-extensions
+
+Or download the `tarball`_:
+
+.. code-block:: console
+
+    $ curl -OJL https://github.com/saritasa-nest/django-import-export-extensions/tarball/master
+
+Once you have a copy of the source, you can install it with:
+
+.. code-block:: console
+
+    $ make install
+
+
+.. _Github repo: https://github.com/saritasa-nest/django-import-export-extensions
+.. _tarball: https://github.com/saritasa-nest/django-import-export-extensions/tarball/master
+
+
+Add `import_export_extensions` to INSTALLED_APPS
+
+.. code-block:: python
+
+    # settings.py
+    INSTALLED_APPS = (
+        ...
+        'import_export_extensions',
+    )
+
+And then run `migrate` command to create ImportJob/ExportJob models and
+`collectstatic` to let Django collect package static files to use in the admin.
+
+.. code-block:: shell
+
+    $ python manage.py migrate
+    $ python manage.py collectstatic
+
+
+Celery
+------
+
+You need to `set up Celery <https://docs.celeryq.dev/en/latest/getting-started/first-steps-with-celery.html>`_
+to use background import/export. Just plug in Celery and you don't need additional
+settings.
+
+
+Settings
+-------------
+
+You can configure the following in your settings file:
+
+``IMPORT_EXPORT_MAX_DATASET_ROWS``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Sets the maximum number of lines in the file to import in order to avoid memory
+overflow. The default value is 10,000. If there are more lines in the file,
+a ``ValueError`` exception will be raised on import.
+
+``MIME_TYPES_MAP``
+~~~~~~~~~~~~~~~~~~
+
+Mapping file extensions to mime types to import files.
+Default is `mimetypes.types_map`.
+
+
+Settings from django-import-export
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+There are also available `settings from original django-import-export
+<https://django-import-export.readthedocs.io/en/latest/installation.html#settings>`_
+package.
```

### Comparing `django_import_export_extensions-0.1.2/README.rst` & `django_import_export_extensions-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/django_import_export_extensions.egg-info/SOURCES.txt` & `django_import_export_extensions-0.1.3/django_import_export_extensions.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
-setup.py
+pyproject.toml
 django_import_export_extensions.egg-info/PKG-INFO
 django_import_export_extensions.egg-info/SOURCES.txt
 django_import_export_extensions.egg-info/dependency_links.txt
-django_import_export_extensions.egg-info/entry_points.txt
-django_import_export_extensions.egg-info/not-zip-safe
 django_import_export_extensions.egg-info/requires.txt
 django_import_export_extensions.egg-info/top_level.txt
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
@@ -76,8 +73,9 @@
 import_export_extensions/templates/admin/celery_import_status.html
 import_export_extensions/templates/admin/import_job_results.html
 import_export_extensions/templates/admin/change_list/change_list.html
 import_export_extensions/templates/admin/change_list/change_list_export.html
 import_export_extensions/templates/admin/change_list/change_list_export_item.html
 import_export_extensions/templates/admin/change_list/change_list_import.html
 import_export_extensions/templates/admin/change_list/change_list_import_export.html
-import_export_extensions/templates/admin/change_list/change_list_import_item.html
+import_export_extensions/templates/admin/change_list/change_list_import_item.html
+requirements/production.txt
```

### Comparing `django_import_export_extensions-0.1.2/docs/Makefile` & `django_import_export_extensions-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/docs/conf.py` & `django_import_export_extensions-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/docs/make.bat` & `django_import_export_extensions-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/docs/usage.rst` & `django_import_export_extensions-0.1.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/export_admin_form.py` & `django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/export_admin_form.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/admin/forms/import_admin_form.py` & `django_import_export_extensions-0.1.3/import_export_extensions/admin/forms/import_admin_form.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/base.py` & `django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/base.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/export_mixin.py` & `django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/export_mixin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/admin/mixins/import_mixin.py` & `django_import_export_extensions-0.1.3/import_export_extensions/admin/mixins/import_mixin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/export_job_admin.py` & `django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/export_job_admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/import_job_admin.py` & `django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/import_job_admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/admin/model_admins/mixins.py` & `django_import_export_extensions-0.1.3/import_export_extensions/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/admin/widgets.py` & `django_import_export_extensions-0.1.3/import_export_extensions/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/export_job.py` & `django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/export_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/api/serializers/import_job.py` & `django_import_export_extensions-0.1.3/import_export_extensions/api/serializers/import_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/api/views/export_job.py` & `django_import_export_extensions-0.1.3/import_export_extensions/api/views/export_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/api/views/import_job.py` & `django_import_export_extensions-0.1.3/import_export_extensions/api/views/import_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/apps.py` & `django_import_export_extensions-0.1.3/import_export_extensions/apps.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/fields.py` & `django_import_export_extensions-0.1.3/import_export_extensions/fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/forms.py` & `django_import_export_extensions-0.1.3/import_export_extensions/forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/migrations/0001_initial.py` & `django_import_export_extensions-0.1.3/import_export_extensions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/models/core.py` & `django_import_export_extensions-0.1.3/import_export_extensions/models/core.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/models/export_job.py` & `django_import_export_extensions-0.1.3/import_export_extensions/models/export_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/models/import_job.py` & `django_import_export_extensions-0.1.3/import_export_extensions/models/import_job.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/models/tools.py` & `django_import_export_extensions-0.1.3/import_export_extensions/models/tools.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/resources.py` & `django_import_export_extensions-0.1.3/import_export_extensions/resources.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css` & `django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/css/widgets/progress_bar.css`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/admin/admin.js` & `django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/admin/admin.js`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js` & `django_import_export_extensions-0.1.3/import_export_extensions/static/import_export_jobs/js/widgets/progress_bar.js`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/tasks.py` & `django_import_export_extensions-0.1.3/import_export_extensions/tasks.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export.html` & `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export_results.html` & `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export_results.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_export_status.html` & `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_export_status.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import.html` & `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import_results.html` & `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import_results.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/celery_import_status.html` & `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/celery_import_status.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/templates/admin/import_job_results.html` & `django_import_export_extensions-0.1.3/import_export_extensions/templates/admin/import_job_results.html`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/utils.py` & `django_import_export_extensions-0.1.3/import_export_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/import_export_extensions/widgets.py` & `django_import_export_extensions-0.1.3/import_export_extensions/widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export_extensions-0.1.2/setup.py` & `django_import_export_extensions-0.1.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,145 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import os
-
-from setuptools import find_packages, setup
-
-with open("README.rst") as readme_file:
-    readme = readme_file.read()
-
-with open("HISTORY.rst") as history_file:
-    history = history_file.read()
-
-def strip_comments(line: str) -> str:
-    """Remove comment from the line."""
-    return line.split("#", 1)[0].strip()
-
-
-def _pip_requirement(req: str) -> list[str]:
-    """Handle requirements from files with `-r` key."""
-    if req.startswith("-r "):
-        _, path = req.split()
-        return reqs(*path.split("/"))
-    return [req]
-
-
-def _reqs(file_name: str) -> list[list[str]]:
-    """Handle requirements from other files and remove comments."""
-    return [
-        _pip_requirement(req) for req in (
-            strip_comments(line) for line in open(
-                os.path.join(os.getcwd(), "requirements", file_name),
-            ).readlines()
-        ) if req
-    ]
-
-
-def reqs(file_name: str) -> list[str]:
-    """Get requirements list."""
-    return [req for subreq in _reqs(file_name) for req in subreq]
-
-
-setup(
-    author="Saritasa",
-    author_email="pypi@saritasa.com",
-    python_requires=">=3.9",
-    classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Framework :: Django",
-        "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
-        "Framework :: Django :: 4.1",
-        "Framework :: Django :: 4.2",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
-    description="Extend functionality of `django-import-export`",
-    entry_points={
-        "console_scripts": [
-            "import_export_extensions=import_export_extensions.cli:main",
-        ],
-    },
-    install_requires=reqs("production.txt"),
-    license="MIT license",
-    long_description=readme + "\n\n" + history,
-    include_package_data=True,
-    keywords="django_import_export_extensions",
-    name="django_import_export_extensions",
-    packages=find_packages(include=["import_export_extensions", "import_export_extensions.*"]),
-    test_suite="tests",
-    tests_require=reqs("development.txt"),
-    url="https://github.com/saritasa-nest/django-import-export-extensions",
-    version="0.1.2",
-    zip_safe=False,
-)
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+authors = [
+    {name = "Saritasa", email = "pypi@saritasa.com"},
+]
+requires-python = ">=3.9"
+classifiers = [
+    "Development Status :: 2 - Pre-Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Framework :: Django",
+    "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+description = "Extend functionality of `django-import-export`"
+readme = "README.rst"
+license = {file = "LICENSE"}
+keywords = ["django_import_export_extensions"]
+name = "django_import_export_extensions"
+dynamic = ["dependencies", "version"]
+
+[project.urls]
+"Homepage" = "https://github.com/saritasa-nest/django-import-export-extensions"
+"Bug Tracker" = "https://github.com/saritasa-nest/django-import-export-extensions/issues"
+
+[tool.setuptools.dynamic]
+dependencies = {file = "requirements/production.txt"}
+version = {attr = "import_export_extensions.__version__"}
+
+[tool.setuptools.packages.find]
+include = ["import_export_extensions", "import_export_extensions.*"]
+
+[tool.isort]
+line_length = 79
+multi_line_output = 3
+known_django = "django"
+known_drf = "rest_framework"
+known_apps = "import_export_extensions"
+skip = [
+    "migrations",
+    "_tmp,src",
+    "scripts",
+    ".venv",
+    "node_modules",
+    "config",
+]
+sections = [
+    "FUTURE",
+    "STDLIB",
+    "DJANGO",
+    "DRF",
+    "THIRDPARTY",
+    "FIRSTPARTY",
+    "APPS",
+    "LOCALFOLDER",
+]
+include_trailing_comma = true
+default_section = "THIRDPARTY"
+
+[tool.flake8]
+ignore = [
+    # https://www.flake8rules.com/rules/E126.html
+    "E126",
+    # https://www.flake8rules.com/rules/W503.html
+    "W503",
+    # https://www.flake8rules.com/rules/W504.html
+    "W504",
+    # https://github.com/m-burst/flake8-pytest-style/blob/master/docs/rules/PT004.md
+    "PT004",
+    # http://www.pydocstyle.org/en/latest/error_codes.html
+    "D100",
+    "D106",
+    "D107",
+    "D204",
+    "D301",
+]
+statistics = true
+count = true
+max-complexity = 10
+pytest-fixture-no-parentheses = true
+pytest-parametrize-names-type = "list"
+pytest-parametrize-values-type = "list"
+pytest-parametrize-values-row-type = "list"
+inline-quotes = "double"
+docstring-quotes = "double"
+docstring-convention = "pep257"
+exclude = [
+    "migrations",
+    ".venv",
+    "__init__.py",
+    "docs",
+    "tests/settings.py",
+]
+
+[tool.mypy]
+ignore_missing_imports = true
+implicit_optional = false
+
+warn_no_return = true
+warn_unused_ignores = true
+warn_redundant_casts = true
+warn_unreachable = true
+warn_unused_configs = true
+allow_redefinition = false
+disallow_any_generics = true
+strict_equality = true
+strict_optional = true
+
+ignore_errors = false
+local_partial_types = true
+
+enable_error_code = [
+    "truthy-bool",
+    "redundant-expr",
+]
+
+disable_error_code = [
+    "attr-defined",
+    "index",
+    "annotation-unchecked",
+]
+
+exclude = "settings.py"
+
+[[tool.mypy.overrides]]
+module = "tests.*"
+warn_unreachable = false
+
+[tool.pytest.ini_options]
+DJANGO_SETTINGS_MODULE = "tests.settings"
+python_files = [
+    "tests.py",
+    "test_*.py",
+    "*_tests.py",
+]
```

