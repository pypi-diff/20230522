# Comparing `tmp/huscy.consents-0.7.0a18.tar.gz` & `tmp/huscy.consents-0.8.0a19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.consents-0.7.0a18.tar", last modified: Tue Apr 18 03:17:43 2023, max compression
+gzip compressed data, was "huscy.consents-0.8.0a19.tar", last modified: Mon May 22 14:55:32 2023, max compression
```

## Comparing `huscy.consents-0.7.0a18.tar` & `huscy.consents-0.8.0a19.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.7.0a18/MANIFEST.in
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.7.0a18/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/consents/
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.7.0a18/huscy/consents/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a18/huscy/consents/api_urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.7.0a18/huscy/consents/apps.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/forms.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.602908 huscy.consents-0.7.0a18/huscy/consents/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1519 2023-04-18 03:17:42.000000 huscy.consents-0.7.0a18/huscy/consents/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a18/huscy/consents/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      638 2023-03-10 09:59:30.000000 huscy.consents-0.7.0a18/huscy/consents/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a18/huscy/consents/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     6112 2023-03-10 09:59:30.000000 huscy.consents-0.7.0a18/huscy/consents/services.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/consents/static/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/consents/static/consents/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.606909 huscy.consents-0.7.0a18/huscy/consents/static/consents/css/
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/css/fomantic.min.css
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/css/fomantic2.9.0.min.css
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.606909 huscy.consents-0.7.0a18/huscy/consents/static/consents/img/
--rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/img/logo.svg
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.614909 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/fomantic.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/fomantic2.9.0.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/jquery.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/jquery3.6.1.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/popper.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/static/consents/js/popper1.16.1.min.js
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy/consents/templates/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/huscy/consents/templates/consents/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      599 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/base.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/create_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4342 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/sign_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3129 2023-04-14 09:53:34.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/signed_consent.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/success.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/huscy/consents/templates/consents/text_fragments/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/text_fragments/checkbox.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      111 2023-01-10 14:57:17.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/text_fragments/header.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/text_fragments/paragraph.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/huscy/consents/templates/consents/widgets/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a18/huscy/consents/templates/consents/widgets/select_date.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/huscy/consents/templatetags/
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/templatetags/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/templatetags/dict_extras.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.7.0a18/huscy/consents/urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.7.0a18/huscy/consents/views.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.7.0a18/huscy/consents/viewsets.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-18 03:17:43.594908 huscy.consents-0.7.0a18/huscy.consents.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1621 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      189 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-18 03:17:43.000000 huscy.consents-0.7.0a18/huscy.consents.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-18 03:17:43.618909 huscy.consents-0.7.0a18/setup.cfg
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1736 2023-04-17 17:43:14.000000 huscy.consents-0.7.0a18/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.8.0a19/MANIFEST.in
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a19/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/consents/
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/huscy/consents/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a19/huscy/consents/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a19/huscy/consents/api_urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a19/huscy/consents/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/forms.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.144561 huscy.consents-0.8.0a19/huscy/consents/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1519 2023-05-22 14:55:31.000000 huscy.consents-0.8.0a19/huscy/consents/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a19/huscy/consents/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      638 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a19/huscy/consents/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a19/huscy/consents/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     7037 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/huscy/consents/services.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/consents/static/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/consents/static/consents/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.144561 huscy.consents-0.8.0a19/huscy/consents/static/consents/css/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/css/fomantic.min.css
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/css/fomantic2.9.0.min.css
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.144561 huscy.consents-0.8.0a19/huscy/consents/static/consents/img/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/img/logo.svg
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.152561 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/fomantic.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/fomantic2.9.0.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/jquery.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/jquery3.6.1.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/popper.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/popper1.16.1.min.js
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/consents/templates/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.152561 huscy.consents-0.8.0a19/huscy/consents/templates/consents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      599 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/base.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/create_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4342 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/sign_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3129 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/signed_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/success.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/checkbox.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      113 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/heading.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       72 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/markdown.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/paragraph.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/huscy/consents/templates/consents/widgets/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/widgets/select_date.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/huscy/consents/templatetags/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/templatetags/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/templatetags/dict_extras.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a19/huscy/consents/urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/views.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a19/huscy/consents/viewsets.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy.consents.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1685 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      208 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/setup.cfg
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1766 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/setup.py
```

### Comparing `huscy.consents-0.7.0a18/PKG-INFO` & `huscy.consents-0.8.0a19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.7.0a18
+Version: 0.8.0a19
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
```

### Comparing `huscy.consents-0.7.0a18/huscy/consents/admin.py` & `huscy.consents-0.8.0a19/huscy/consents/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/forms.py` & `huscy.consents-0.8.0a19/huscy/consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/migrations/0001_initial.py` & `huscy.consents-0.8.0a19/huscy/consents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/models.py` & `huscy.consents-0.8.0a19/huscy/consents/models.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/serializer.py` & `huscy.consents-0.8.0a19/huscy/consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/services.py` & `huscy.consents-0.8.0a19/huscy/consents/services.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,14 +66,37 @@
                         },
                     },
                     "required": ["text", "size"],
                 },
             },
             "required": ["properties", "type"],
         },
+        "markdown": {
+            "type": "object",
+            "properties": {
+                "type": {
+                    "description": "The type must be 'markdown'",
+                    "type": "string",
+                    "pattern": "markdown",
+                },
+                "properties": {
+                    "description": "The markdown text has the following properties.",
+                    "type": "object",
+                    "properties": {
+                        "text": {
+                            "description": ("This property contains the displayed text as "
+                                            "markdown text"),
+                            "type": "string",
+                        },
+                    },
+                    "required": ["text"],
+                },
+            },
+            "required": ["properties", "type"],
+        },
         "paragraph": {
             "type": "object",
             "properties": {
                 "type": {
                     "description": "The type must be 'paragraph'.",
                     "type": "string",
                     "pattern": "paragraph",
@@ -105,14 +128,15 @@
     },
 
     "type": "array",
     "items": {
         "anyOf": [
             {"$ref": "#/$defs/checkbox"},
             {"$ref": "#/$defs/heading"},
+            {"$ref": "#/$defs/markdown"},
             {"$ref": "#/$defs/paragraph"},
         ],
     },
     "minItems": 1,
 }
```

### Comparing `huscy.consents-0.7.0a18/huscy/consents/static/consents/css/fomantic.min.css` & `huscy.consents-0.8.0a19/huscy/consents/static/consents/css/fomantic.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/static/consents/css/fomantic2.9.0.min.css` & `huscy.consents-0.8.0a19/huscy/consents/static/consents/css/fomantic2.9.0.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/static/consents/img/logo.svg` & `huscy.consents-0.8.0a19/huscy/consents/static/consents/img/logo.svg`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/fomantic.min.js` & `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/fomantic.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/fomantic2.9.0.min.js` & `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/fomantic2.9.0.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/jquery.min.js` & `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/jquery3.6.1.min.js` & `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/jquery3.6.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/popper.min.js` & `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/static/consents/js/popper1.16.1.min.js` & `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/popper1.16.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/templates/consents/base.html` & `huscy.consents-0.8.0a19/huscy/consents/templates/consents/base.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/templates/consents/create_consent.html` & `huscy.consents-0.8.0a19/huscy/consents/templates/consents/create_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/templates/consents/sign_consent.html` & `huscy.consents-0.8.0a19/huscy/consents/templates/consents/sign_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/templates/consents/signed_consent.html` & `huscy.consents-0.8.0a19/huscy/consents/templates/consents/signed_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/views.py` & `huscy.consents-0.8.0a19/huscy/consents/views.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy/consents/viewsets.py` & `huscy.consents-0.8.0a19/huscy/consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.7.0a18/huscy.consents.egg-info/PKG-INFO` & `huscy.consents-0.8.0a19/huscy.consents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.7.0a18
+Version: 0.8.0a19
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
```

### Comparing `huscy.consents-0.7.0a18/huscy.consents.egg-info/SOURCES.txt` & `huscy.consents-0.8.0a19/huscy.consents.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,12 +30,13 @@
 huscy/consents/static/consents/js/popper1.16.1.min.js
 huscy/consents/templates/consents/base.html
 huscy/consents/templates/consents/create_consent.html
 huscy/consents/templates/consents/sign_consent.html
 huscy/consents/templates/consents/signed_consent.html
 huscy/consents/templates/consents/success.html
 huscy/consents/templates/consents/text_fragments/checkbox.html
-huscy/consents/templates/consents/text_fragments/header.html
+huscy/consents/templates/consents/text_fragments/heading.html
+huscy/consents/templates/consents/text_fragments/markdown.html
 huscy/consents/templates/consents/text_fragments/paragraph.html
 huscy/consents/templates/consents/widgets/select_date.html
 huscy/consents/templatetags/__init__.py
 huscy/consents/templatetags/dict_extras.py
```

### Comparing `huscy.consents-0.7.0a18/setup.py` & `huscy.consents-0.8.0a19/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     packages=find_namespace_packages(include=['huscy.*']),
     include_package_data=True,
 
     install_requires=[
         'Django>=3.2',
         'djangorestframework>=3.11',
         'django-jsignature>=0.9',
+        'django-markdownify',
         'django-phonenumber-field[phonenumberslite]>=5',
         'jsonschema>=3.2',
         'weasyprint',
     ],
     extras_require={
         'development': ['psycopg2-binary'],
         'testing': ['tox', 'watchdog'],
```

