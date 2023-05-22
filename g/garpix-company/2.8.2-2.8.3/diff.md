# Comparing `tmp/garpix_company-2.8.2.tar.gz` & `tmp/garpix_company-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_company-2.8.2.tar", last modified: Fri May 12 11:28:53 2023, max compression
+gzip compressed data, was "garpix_company-2.8.3.tar", last modified: Mon May 22 15:06:56 2023, max compression
```

## Comparing `garpix_company-2.8.2.tar` & `garpix_company-2.8.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.999061 garpix_company-2.8.2/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-05-12 11:28:52.000000 garpix_company-2.8.2/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4078 2023-05-12 11:28:52.998932 garpix_company-2.8.2/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.994940 garpix_company-2.8.2/garpix_company/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2760 2023-05-12 11:28:42.000000 garpix_company-2.8.2/garpix_company/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3508 2023-05-11 10:44:26.000000 garpix_company-2.8.2/garpix_company/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.995874 garpix_company-2.8.2/garpix_company/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-11 10:08:25.000000 garpix_company-2.8.2/garpix_company/admin/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.8.2/garpix_company/admin/company_invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/helpers.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.996158 garpix_company-2.8.2/garpix_company/managers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/managers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/managers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/managers/invite.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.996261 garpix_company-2.8.2/garpix_company/migrations/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/migrations/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.996343 garpix_company-2.8.2/garpix_company/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.996537 garpix_company-2.8.2/garpix_company/mixins/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/mixins/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.8.2/garpix_company/mixins/views/company_mixin.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.997053 garpix_company-2.8.2/garpix_company/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-05-05 07:20:15.000000 garpix_company-2.8.2/garpix_company/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6079 2023-05-11 09:19:51.000000 garpix_company-2.8.2/garpix_company/models/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.8.2/garpix_company/models/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4133 2023-05-10 09:40:57.000000 garpix_company-2.8.2/garpix_company/models/user_company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.8.2/garpix_company/models/user_role.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.997594 garpix_company-2.8.2/garpix_company/permissions/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.8.2/garpix_company/permissions/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1035 2023-05-04 14:33:02.000000 garpix_company-2.8.2/garpix_company/permissions/company_admin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      706 2023-05-04 15:00:30.000000 garpix_company-2.8.2/garpix_company/permissions/company_owner.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.8.2/garpix_company/permissions/company_user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      410 2023-05-11 10:44:26.000000 garpix_company-2.8.2/garpix_company/permissions/invite_receiver.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.998202 garpix_company-2.8.2/garpix_company/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.8.2/garpix_company/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.8.2/garpix_company/serializers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5728 2023-05-11 10:44:26.000000 garpix_company-2.8.2/garpix_company/serializers/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.8.2/garpix_company/serializers/role.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.8.2/garpix_company/serializers/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      851 2023-05-04 14:33:02.000000 garpix_company-2.8.2/garpix_company/serializers/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.998383 garpix_company-2.8.2/garpix_company/services/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.8.2/garpix_company/services/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      607 2023-05-10 09:40:24.000000 garpix_company-2.8.2/garpix_company/services/role_service.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.8.2/garpix_company/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-12 11:28:42.000000 garpix_company-2.8.2/garpix_company/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.8.2/garpix_company/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.8.2/garpix_company/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.998782 garpix_company-2.8.2/garpix_company/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.8.2/garpix_company/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6000 2023-05-12 10:59:00.000000 garpix_company-2.8.2/garpix_company/views/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2201 2023-05-12 11:28:16.000000 garpix_company-2.8.2/garpix_company/views/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3645 2023-05-12 10:46:57.000000 garpix_company-2.8.2/garpix_company/views/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 11:28:52.995561 garpix_company-2.8.2/garpix_company.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4078 2023-05-12 11:28:52.000000 garpix_company-2.8.2/garpix_company.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-05-12 11:28:52.000000 garpix_company-2.8.2/garpix_company.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-12 11:28:52.000000 garpix_company-2.8.2/garpix_company.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-12 11:28:52.000000 garpix_company-2.8.2/garpix_company.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-05-12 11:28:52.000000 garpix_company-2.8.2/garpix_company.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-05-12 11:28:52.000000 garpix_company-2.8.2/garpix_company.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-12 11:28:52.999096 garpix_company-2.8.2/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-12 11:28:52.000000 garpix_company-2.8.2/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.139331 garpix_company-2.8.3/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-05-22 15:06:56.000000 garpix_company-2.8.3/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4078 2023-05-22 15:06:56.139170 garpix_company-2.8.3/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.131147 garpix_company-2.8.3/garpix_company/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2820 2023-05-22 15:06:42.000000 garpix_company-2.8.3/garpix_company/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3508 2023-05-11 10:44:26.000000 garpix_company-2.8.3/garpix_company/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.134532 garpix_company-2.8.3/garpix_company/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-11 10:08:25.000000 garpix_company-2.8.3/garpix_company/admin/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.8.3/garpix_company/admin/company_invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/helpers.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.134926 garpix_company-2.8.3/garpix_company/managers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/managers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/managers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/managers/invite.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.135054 garpix_company-2.8.3/garpix_company/migrations/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/migrations/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.135149 garpix_company-2.8.3/garpix_company/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.135371 garpix_company-2.8.3/garpix_company/mixins/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/mixins/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.8.3/garpix_company/mixins/views/company_mixin.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.136132 garpix_company-2.8.3/garpix_company/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-05-05 07:20:15.000000 garpix_company-2.8.3/garpix_company/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6079 2023-05-11 09:19:51.000000 garpix_company-2.8.3/garpix_company/models/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.8.3/garpix_company/models/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4133 2023-05-10 09:40:57.000000 garpix_company-2.8.3/garpix_company/models/user_company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.8.3/garpix_company/models/user_role.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.136774 garpix_company-2.8.3/garpix_company/permissions/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.8.3/garpix_company/permissions/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1035 2023-05-04 14:33:02.000000 garpix_company-2.8.3/garpix_company/permissions/company_admin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      706 2023-05-04 15:00:30.000000 garpix_company-2.8.3/garpix_company/permissions/company_owner.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.8.3/garpix_company/permissions/company_user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      410 2023-05-11 10:44:26.000000 garpix_company-2.8.3/garpix_company/permissions/invite_receiver.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.137710 garpix_company-2.8.3/garpix_company/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.8.3/garpix_company/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.8.3/garpix_company/serializers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5898 2023-05-22 15:06:07.000000 garpix_company-2.8.3/garpix_company/serializers/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.8.3/garpix_company/serializers/role.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.8.3/garpix_company/serializers/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      926 2023-05-12 11:36:47.000000 garpix_company-2.8.3/garpix_company/serializers/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.137950 garpix_company-2.8.3/garpix_company/services/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.8.3/garpix_company/services/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      607 2023-05-10 09:40:24.000000 garpix_company-2.8.3/garpix_company/services/role_service.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.8.3/garpix_company/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-22 15:06:42.000000 garpix_company-2.8.3/garpix_company/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.8.3/garpix_company/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.138983 garpix_company-2.8.3/garpix_company/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.8.3/garpix_company/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6000 2023-05-12 10:59:00.000000 garpix_company-2.8.3/garpix_company/views/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2201 2023-05-12 11:28:16.000000 garpix_company-2.8.3/garpix_company/views/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3645 2023-05-12 10:46:57.000000 garpix_company-2.8.3/garpix_company/views/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.131929 garpix_company-2.8.3/garpix_company.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4078 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-22 15:06:56.139375 garpix_company-2.8.3/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-22 15:06:56.000000 garpix_company-2.8.3/setup.py
```

### Comparing `garpix_company-2.8.2/PKG-INFO` & `garpix_company-2.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_company
-Version: 2.8.2
+Version: 2.8.3
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.8.2/garpix_company/CHANGELOG.md` & `garpix_company-2.8.3/garpix_company/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 2.8.3 (22.05.2023)
+
+- Fixed bug with `invite` endpoint
+
 ### 2.8.2 (12.05.2023)
 
 - Fixed bug with `change_role` endpoint
 - `first_name`, `last_name` company user search added
 - `role` filter added to invites list endpoint
 
 ### 2.8.0-2.8.1 (11.05.2023)
```

### Comparing `garpix_company-2.8.2/garpix_company/CONTRIBUTING.md` & `garpix_company-2.8.3/garpix_company/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/README.md` & `garpix_company-2.8.3/garpix_company/README.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/helpers.py` & `garpix_company-2.8.3/garpix_company/helpers.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/models/company.py` & `garpix_company-2.8.3/garpix_company/models/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/models/invite.py` & `garpix_company-2.8.3/garpix_company/models/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/models/user_company.py` & `garpix_company-2.8.3/garpix_company/models/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/models/user_role.py` & `garpix_company-2.8.3/garpix_company/models/user_role.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/permissions/company_admin.py` & `garpix_company-2.8.3/garpix_company/permissions/company_admin.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/permissions/company_owner.py` & `garpix_company-2.8.3/garpix_company/permissions/company_owner.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/serializers/company.py` & `garpix_company-2.8.3/garpix_company/serializers/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/serializers/invite.py` & `garpix_company-2.8.3/garpix_company/serializers/invite.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,42 +26,45 @@
             'role': {'required': True},
         }
 
     def validate_email(self, value):
         User = get_user_model()
         Company = get_company_model()
         company_id = self.context.get("company_id")
-        if not getattr(settings, 'GARPIX_COMPANY_INVITE_NOT_USERS', False):
-            try:
-                user = User.objects.get(email=value)
-                if not Company.check_user_companies_limit(user):
-                    raise ValidationError(_('У пользователя с указанным email превышен лимит количества компаний'))
-                if UserCompany.active_objects.filter(user=user, company_id=company_id).exists():
-                    raise ValidationError(_('Указанный пользователь уже является сотрудником компании'))
-            except User.DoesNotExist:
+        try:
+            user = User.objects.get(email=value)
+            if not Company.check_user_companies_limit(user):
+                raise ValidationError(_('У пользователя с указанным email превышен лимит количества компаний'))
+            if UserCompany.active_objects.filter(user=user, company_id=company_id).exists():
+                raise ValidationError(_('Указанный пользователь уже является сотрудником компании'))
+        except User.DoesNotExist:
+            if getattr(settings, 'GARPIX_COMPANY_INVITE_NOT_USERS', False):
                 raise ValidationError(_('Пользователь с указанным email не зарегистрирован'))
         return value
 
     def validate_user(self, value):
         Company = get_company_model()
         company_id = self.context.get("company_id")
         if not Company.check_user_companies_limit(value):
             raise ValidationError(_('У пользователя с указанным id превышен лимит количества компаний'))
         if UserCompany.active_objects.filter(user=value, company_id=company_id).exists():
             raise ValidationError(_('Указанный пользователь уже является сотрудником компании'))
         return value
 
     def validate(self, data):
+        User = get_user_model()
         validated_data = super().validate(data)
         user = validated_data.get('user', None)
         email = validated_data.get('email', None)
         if not user and not email:
             raise ValidationError(_('Укажите email или id пользователя'))
         if user:
-            data['email'] = user.email
+            validated_data['email'] = user.email
+        elif not getattr(settings, 'GARPIX_COMPANY_INVITE_NOT_USERS', False):
+            validated_data['user'] = User.objects.filter(email=email).first()
         return data
 
     def create(self, validated_data):
         Role = get_company_role_model()
         request = self.context.get("request")
         company_id = self.context.get("company_id")
         if role := validated_data.get('role', None):
```

### Comparing `garpix_company-2.8.2/garpix_company/serializers/user_company.py` & `garpix_company-2.8.3/garpix_company/serializers/user_company.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,7 +21,10 @@
 
 
 class ChangeUserRoleSerializer(serializers.ModelSerializer):
 
     class Meta:
         model = UserCompany
         fields = ('role',)
+        extra_kwargs = {
+            'role': {'required': False}
+        }
```

### Comparing `garpix_company-2.8.2/garpix_company/services/role_service.py` & `garpix_company-2.8.3/garpix_company/services/role_service.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/settings.py` & `garpix_company-2.8.3/garpix_company/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/setup.py` & `garpix_company-2.8.3/garpix_company/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.8.2',
+    version='2.8.3',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_company-2.8.2/garpix_company/urls.py` & `garpix_company-2.8.3/garpix_company/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/views/company.py` & `garpix_company-2.8.3/garpix_company/views/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/views/invite.py` & `garpix_company-2.8.3/garpix_company/views/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company/views/user_company.py` & `garpix_company-2.8.3/garpix_company/views/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/garpix_company.egg-info/PKG-INFO` & `garpix_company-2.8.3/garpix_company.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-company
-Version: 2.8.2
+Version: 2.8.3
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.8.2/garpix_company.egg-info/SOURCES.txt` & `garpix_company-2.8.3/garpix_company.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.2/setup.py` & `garpix_company-2.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.8.2',
+    version='2.8.3',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

