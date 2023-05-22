# Comparing `tmp/django-workos-0.4.8.tar.gz` & `tmp/django-workos-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-workos-0.4.8.tar", last modified: Mon Feb 27 00:55:07 2023, max compression
+gzip compressed data, was "django-workos-0.5.0.tar", last modified: Mon May 22 04:34:32 2023, max compression
```

## Comparing `django-workos-0.4.8.tar` & `django-workos-0.5.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-02-27 00:55:07.329600 django-workos-0.4.8/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1484 2022-08-09 22:13:18.000000 django-workos-0.4.8/LICENSE
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      121 2022-08-15 04:11:13.000000 django-workos-0.4.8/MANIFEST.in
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20115 2023-02-27 00:55:07.329600 django-workos-0.4.8/PKG-INFO
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    19671 2023-02-27 00:53:08.000000 django-workos-0.4.8/README.md
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-02-27 00:55:07.319600 django-workos-0.4.8/django_workos.egg-info/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20115 2023-02-27 00:55:07.000000 django-workos-0.4.8/django_workos.egg-info/PKG-INFO
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2996 2023-02-27 00:55:07.000000 django-workos-0.4.8/django_workos.egg-info/SOURCES.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)        1 2023-02-27 00:55:07.000000 django-workos-0.4.8/django_workos.egg-info/dependency_links.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-02-27 00:55:07.000000 django-workos-0.4.8/django_workos.egg-info/requires.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-02-27 00:55:07.000000 django-workos-0.4.8/django_workos.egg-info/top_level.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      585 2023-02-27 00:54:02.000000 django-workos-0.4.8/pyproject.toml
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       73 2023-02-27 00:55:07.329600 django-workos-0.4.8/setup.cfg
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-02-27 00:55:07.319600 django-workos-0.4.8/workos_login/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.4.8/workos_login/__init__.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1799 2023-02-27 00:17:50.000000 django-workos-0.4.8/workos_login/admin.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1505 2022-08-13 16:56:52.000000 django-workos-0.4.8/workos_login/admin_site.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1045 2022-10-05 00:27:58.000000 django-workos-0.4.8/workos_login/apps.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2562 2022-10-17 23:02:26.000000 django-workos-0.4.8/workos_login/conf.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       99 2022-10-09 19:59:00.000000 django-workos-0.4.8/workos_login/exceptions.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     5731 2023-02-27 00:17:50.000000 django-workos-0.4.8/workos_login/forms.py
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-02-27 00:55:07.329600 django-workos-0.4.8/workos_login/migrations/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     3267 2022-08-15 00:43:37.000000 django-workos-0.4.8/workos_login/migrations/0001_initial.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      629 2022-08-13 00:41:11.000000 django-workos-0.4.8/workos_login/migrations/0002_auto_20220803_2242.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      563 2022-09-20 04:37:45.000000 django-workos-0.4.8/workos_login/migrations/0003_loginrule_jit_username_format.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      908 2022-10-04 22:32:58.000000 django-workos-0.4.8/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      655 2022-10-05 06:11:28.000000 django-workos-0.4.8/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      542 2023-02-27 00:19:33.000000 django-workos-0.4.8/workos_login/migrations/0006_loginrule_jit_creation_type.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      475 2023-02-27 00:25:07.000000 django-workos-0.4.8/workos_login/migrations/0007_auto_20230227_0020.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:25:13.000000 django-workos-0.4.8/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.4.8/workos_login/migrations/__init__.py
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-02-27 00:55:07.329600 django-workos-0.4.8/workos_login/migrations/__pycache__/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2654 2022-08-15 00:43:43.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      817 2022-08-13 00:41:12.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      788 2022-09-20 04:37:55.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1012 2022-08-06 22:56:24.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1192 2022-08-10 00:17:47.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1049 2022-10-04 22:32:58.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      720 2022-08-12 22:31:04.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      874 2022-10-05 06:14:09.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:20:58.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      784 2023-02-27 00:25:13.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      950 2023-02-27 00:26:25.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      166 2022-07-28 06:31:59.000000 django-workos-0.4.8/workos_login/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    11311 2023-02-27 00:36:18.000000 django-workos-0.4.8/workos_login/models.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      200 2022-10-17 23:45:50.000000 django-workos-0.4.8/workos_login/signals.py
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-02-27 00:55:07.319600 django-workos-0.4.8/workos_login/templates/
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-02-27 00:55:07.329600 django-workos-0.4.8/workos_login/templates/registration/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4413 2022-10-21 22:15:20.000000 django-workos-0.4.8/workos_login/templates/registration/base_login.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1720 2022-09-19 21:22:58.000000 django-workos-0.4.8/workos_login/templates/registration/base_registration.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      307 2022-08-13 17:15:38.000000 django-workos-0.4.8/workos_login/templates/registration/bootstrap.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      498 2022-08-10 00:23:34.000000 django-workos-0.4.8/workos_login/templates/registration/form.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       47 2022-10-21 22:11:19.000000 django-workos-0.4.8/workos_login/templates/registration/login.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       46 2022-08-13 18:16:16.000000 django-workos-0.4.8/workos_login/templates/registration/logo.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      278 2022-08-13 02:40:24.000000 django-workos-0.4.8/workos_login/templates/registration/magic_link_complete.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      394 2022-08-09 05:19:03.000000 django-workos-0.4.8/workos_login/templates/registration/messages.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1397 2022-10-21 22:15:37.000000 django-workos-0.4.8/workos_login/templates/registration/mfa_enroll.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2122 2022-08-09 04:14:47.000000 django-workos-0.4.8/workos_login/templates/registration/mfa_enroll_start.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      678 2022-10-21 22:17:30.000000 django-workos-0.4.8/workos_login/templates/registration/mfa_verify.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      316 2022-09-15 22:29:19.000000 django-workos-0.4.8/workos_login/templates/registration/password_reset_complete.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      666 2022-09-15 22:32:39.000000 django-workos-0.4.8/workos_login/templates/registration/password_reset_confirm.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      493 2022-09-15 22:32:39.000000 django-workos-0.4.8/workos_login/templates/registration/password_reset_done.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      501 2022-09-15 22:24:22.000000 django-workos-0.4.8/workos_login/templates/registration/password_reset_form.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1589 2022-10-21 21:39:41.000000 django-workos-0.4.8/workos_login/templates/registration/style.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4718 2022-10-17 23:00:04.000000 django-workos-0.4.8/workos_login/tests.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2073 2023-02-23 05:45:24.000000 django-workos-0.4.8/workos_login/urls.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    10399 2023-02-23 07:23:03.000000 django-workos-0.4.8/workos_login/utils.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    21106 2023-02-27 00:36:18.000000 django-workos-0.4.8/workos_login/views.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-22 04:34:32.759254 django-workos-0.5.0/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1484 2022-08-09 22:13:18.000000 django-workos-0.5.0/LICENSE
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      121 2022-08-15 04:11:13.000000 django-workos-0.5.0/MANIFEST.in
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20115 2023-05-22 04:34:32.759254 django-workos-0.5.0/PKG-INFO
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    19671 2023-02-27 00:53:08.000000 django-workos-0.5.0/README.md
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-22 04:34:32.749254 django-workos-0.5.0/django_workos.egg-info/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20115 2023-05-22 04:34:32.000000 django-workos-0.5.0/django_workos.egg-info/PKG-INFO
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2996 2023-05-22 04:34:32.000000 django-workos-0.5.0/django_workos.egg-info/SOURCES.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)        1 2023-05-22 04:34:32.000000 django-workos-0.5.0/django_workos.egg-info/dependency_links.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-05-22 04:34:32.000000 django-workos-0.5.0/django_workos.egg-info/requires.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-05-22 04:34:32.000000 django-workos-0.5.0/django_workos.egg-info/top_level.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      585 2023-05-22 04:33:46.000000 django-workos-0.5.0/pyproject.toml
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       73 2023-05-22 04:34:32.759254 django-workos-0.5.0/setup.cfg
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-22 04:34:32.749254 django-workos-0.5.0/workos_login/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.0/workos_login/__init__.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1799 2023-02-27 00:17:50.000000 django-workos-0.5.0/workos_login/admin.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1505 2022-08-13 16:56:52.000000 django-workos-0.5.0/workos_login/admin_site.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1045 2022-10-05 00:27:58.000000 django-workos-0.5.0/workos_login/apps.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2650 2023-05-22 03:56:47.000000 django-workos-0.5.0/workos_login/conf.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       99 2022-10-09 19:59:00.000000 django-workos-0.5.0/workos_login/exceptions.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     5731 2023-02-27 00:17:50.000000 django-workos-0.5.0/workos_login/forms.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-22 04:34:32.749254 django-workos-0.5.0/workos_login/migrations/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     3267 2022-08-15 00:43:37.000000 django-workos-0.5.0/workos_login/migrations/0001_initial.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      629 2022-08-13 00:41:11.000000 django-workos-0.5.0/workos_login/migrations/0002_auto_20220803_2242.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      563 2022-09-20 04:37:45.000000 django-workos-0.5.0/workos_login/migrations/0003_loginrule_jit_username_format.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      908 2022-10-04 22:32:58.000000 django-workos-0.5.0/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      655 2022-10-05 06:11:28.000000 django-workos-0.5.0/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      542 2023-02-27 00:19:33.000000 django-workos-0.5.0/workos_login/migrations/0006_loginrule_jit_creation_type.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      475 2023-02-27 00:25:07.000000 django-workos-0.5.0/workos_login/migrations/0007_auto_20230227_0020.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:25:13.000000 django-workos-0.5.0/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.0/workos_login/migrations/__init__.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-22 04:34:32.759254 django-workos-0.5.0/workos_login/migrations/__pycache__/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2654 2022-08-15 00:43:43.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      817 2022-08-13 00:41:12.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      788 2022-09-20 04:37:55.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1012 2022-08-06 22:56:24.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1192 2022-08-10 00:17:47.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1049 2022-10-04 22:32:58.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      720 2022-08-12 22:31:04.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      874 2022-10-05 06:14:09.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:20:58.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      784 2023-02-27 00:25:13.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      950 2023-02-27 00:26:25.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      166 2022-07-28 06:31:59.000000 django-workos-0.5.0/workos_login/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    11410 2023-05-22 04:01:58.000000 django-workos-0.5.0/workos_login/models.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      200 2022-10-17 23:45:50.000000 django-workos-0.5.0/workos_login/signals.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-22 04:34:32.749254 django-workos-0.5.0/workos_login/templates/
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-05-22 04:34:32.759254 django-workos-0.5.0/workos_login/templates/registration/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4439 2023-05-22 03:56:47.000000 django-workos-0.5.0/workos_login/templates/registration/base_login.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1720 2022-09-19 21:22:58.000000 django-workos-0.5.0/workos_login/templates/registration/base_registration.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      307 2022-08-13 17:15:38.000000 django-workos-0.5.0/workos_login/templates/registration/bootstrap.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      498 2022-08-10 00:23:34.000000 django-workos-0.5.0/workos_login/templates/registration/form.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       47 2022-10-21 22:11:19.000000 django-workos-0.5.0/workos_login/templates/registration/login.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       46 2022-08-13 18:16:16.000000 django-workos-0.5.0/workos_login/templates/registration/logo.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      276 2023-05-22 04:27:37.000000 django-workos-0.5.0/workos_login/templates/registration/magic_link_complete.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      394 2022-08-09 05:19:03.000000 django-workos-0.5.0/workos_login/templates/registration/messages.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1397 2022-10-21 22:15:37.000000 django-workos-0.5.0/workos_login/templates/registration/mfa_enroll.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2122 2022-08-09 04:14:47.000000 django-workos-0.5.0/workos_login/templates/registration/mfa_enroll_start.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      678 2022-10-21 22:17:30.000000 django-workos-0.5.0/workos_login/templates/registration/mfa_verify.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      316 2022-09-15 22:29:19.000000 django-workos-0.5.0/workos_login/templates/registration/password_reset_complete.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      666 2022-09-15 22:32:39.000000 django-workos-0.5.0/workos_login/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      493 2022-09-15 22:32:39.000000 django-workos-0.5.0/workos_login/templates/registration/password_reset_done.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      501 2022-09-15 22:24:22.000000 django-workos-0.5.0/workos_login/templates/registration/password_reset_form.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1589 2022-10-21 21:39:41.000000 django-workos-0.5.0/workos_login/templates/registration/style.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4718 2022-10-17 23:00:04.000000 django-workos-0.5.0/workos_login/tests.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2073 2023-02-23 05:45:24.000000 django-workos-0.5.0/workos_login/urls.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    10399 2023-02-23 07:23:03.000000 django-workos-0.5.0/workos_login/utils.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    21142 2023-05-22 03:56:47.000000 django-workos-0.5.0/workos_login/views.py
```

### Comparing `django-workos-0.4.8/LICENSE` & `django-workos-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/PKG-INFO` & `django-workos-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-workos
-Version: 0.4.8
+Version: 0.5.0
 Summary: Enabling SSO, MFA and passwordless login for Django projects by using WorkOS.
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/surefyresystems/django-workos
 Keywords: django,sso,workos,mfa
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `django-workos-0.4.8/README.md` & `django-workos-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/django_workos.egg-info/PKG-INFO` & `django-workos-0.5.0/django_workos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-workos
-Version: 0.4.8
+Version: 0.5.0
 Summary: Enabling SSO, MFA and passwordless login for Django projects by using WorkOS.
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/surefyresystems/django-workos
 Keywords: django,sso,workos,mfa
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `django-workos-0.4.8/django_workos.egg-info/SOURCES.txt` & `django-workos-0.5.0/django_workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/pyproject.toml` & `django-workos-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-workos"
-version = "0.4.8"
+version = "0.5.0"
 description = "Enabling SSO, MFA and passwordless login for Django projects by using WorkOS."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["django", "sso", "workos", "mfa"]
 license = {text = "BSD 3-Clause License"}
 classifiers = [
     "Framework :: Django",
```

### Comparing `django-workos-0.4.8/workos_login/admin.py` & `django-workos-0.5.0/workos_login/admin.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/admin_site.py` & `django-workos-0.5.0/workos_login/admin_site.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/apps.py` & `django-workos-0.5.0/workos_login/apps.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/conf.py` & `django-workos-0.5.0/workos_login/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,18 @@
         return "MicrosoftOAuth"
 
     @property
     def WORKOS_METHOD_MFA(self) -> str:
         return "mfa"
 
     @property
+    def WORKOS_METHOD_EMAIL_MFA(self) -> str:
+        return "email_mfa"
+
+    @property
     def WORKOS_METHOD_MAGIC(self) -> str:
         return "magic"
 
     @property
     def WORKOS_SSO_REDIRECT_URI(self) -> Optional[str]:
         return getattr(settings, "WORKOS_SSO_REDIRECT_URI", None)
```

### Comparing `django-workos-0.4.8/workos_login/forms.py` & `django-workos-0.5.0/workos_login/forms.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/0001_initial.py` & `django-workos-0.5.0/workos_login/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/0002_auto_20220803_2242.py` & `django-workos-0.5.0/workos_login/migrations/0002_auto_20220803_2242.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/0003_loginrule_jit_username_format.py` & `django-workos-0.5.0/workos_login/migrations/0003_loginrule_jit_username_format.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py` & `django-workos-0.5.0/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py` & `django-workos-0.5.0/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/0006_loginrule_jit_creation_type.py` & `django-workos-0.5.0/workos_login/migrations/0006_loginrule_jit_creation_type.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py` & `django-workos-0.5.0/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc` & `django-workos-0.5.0/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/models.py` & `django-workos-0.5.0/workos_login/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                 return rule
 
         return None
 
 
 class LoginMethods(models.TextChoices):
     MFA = conf.WORKOS_METHOD_MFA, "MFA"
+    EMAIL_MFA = conf.WORKOS_METHOD_EMAIL_MFA, "Email MFA"
     MAGIC_LINK = conf.WORKOS_METHOD_MAGIC, "Passwordless Email"
     GOOGLE_SSO = conf.WORKOS_METHOD_GOOGLE_OAUTH, "Google SSO"
     MICROSOFT_SSO = conf.WORKOS_METHOD_MICROSOFT_OAUTH, "Microsoft SSO"
     SAML_SSO = conf.WORKOS_METHOD_SSO, "SAML SSO"
     USERNAME = conf.WORKOS_METHOD_EMAIL, "Username/Password"
 
     @property
@@ -137,15 +138,15 @@
 
     @property
     def username(self) -> bool:
         return self.method == LoginMethods.USERNAME
 
     @property
     def requires_password(self) -> bool:
-        return self.mfa or self.username
+        return self.mfa or self.username or self.method == LoginMethods.EMAIL_MFA
 
     def clean(self):
         errors = {}
 
         if self.totp_organization_name and not self.mfa:
             errors["totp_organization_name"] = _("Organization name only valid for MFA")
```

### Comparing `django-workos-0.4.8/workos_login/templates/registration/base_login.html` & `django-workos-0.5.0/workos_login/templates/registration/base_login.html`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
       })
     }
 
     function reqListener () {
       const response = JSON.parse(this.responseText);
       const rule = response.rule;
       const method = response.method;
-      if(method === 'username' || method === 'mfa'){
+      if(method === 'username' || method === 'mfa' || method === 'email_mfa'){
         showInput('id_password');
         showItem('forgot-password');
       }
       incrementStep();
       if(method === 'sso' || method === 'magic'){
         // No more work to do - go next again
         next()
```

### Comparing `django-workos-0.4.8/workos_login/templates/registration/base_registration.html` & `django-workos-0.5.0/workos_login/templates/registration/base_registration.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/templates/registration/mfa_enroll.html` & `django-workos-0.5.0/workos_login/templates/registration/mfa_enroll.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/templates/registration/mfa_enroll_start.html` & `django-workos-0.5.0/workos_login/templates/registration/mfa_enroll_start.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/templates/registration/mfa_verify.html` & `django-workos-0.5.0/workos_login/templates/registration/mfa_verify.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/templates/registration/password_reset_confirm.html` & `django-workos-0.5.0/workos_login/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/templates/registration/style.html` & `django-workos-0.5.0/workos_login/templates/registration/style.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/tests.py` & `django-workos-0.5.0/workos_login/tests.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/urls.py` & `django-workos-0.5.0/workos_login/urls.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/utils.py` & `django-workos-0.5.0/workos_login/utils.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.4.8/workos_login/views.py` & `django-workos-0.5.0/workos_login/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
                 return redirect('mfa_verify')
             else:
                 return redirect('mfa_enroll')
         elif method == LoginMethods.USERNAME:
             # This will log in the user - clear the workos session vars
             clear_session_vars(self.request)
             return super(WorkosLoginView, self).form_valid(form)
-        elif method == LoginMethods.MAGIC_LINK:
+        elif method == LoginMethods.MAGIC_LINK or method == LoginMethods.EMAIL_MFA:
             email = user.email
             uri = conf.WORKOS_MAGIC_REDIRECT_URI if conf.WORKOS_MAGIC_REDIRECT_URI else self.request.build_absolute_uri(reverse("magic_callback"))
             session = workos.client.passwordless.create_session({
                 'email': email,
                 'redirect_uri': uri,
                 'state': state,
                 'type': 'MagicLink'})
```

