# Comparing `tmp/half_orm-0.9.0.tar.gz` & `tmp/half_orm-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "half_orm-0.9.0.tar", last modified: Fri May 12 08:38:28 2023, max compression
+gzip compressed data, was "half_orm-0.9.1.tar", last modified: Mon May 22 08:19:19 2023, max compression
```

## Comparing `half_orm-0.9.0.tar` & `half_orm-0.9.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.598108 half_orm-0.9.0/
--rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-02-02 08:59:25.000000 half_orm-0.9.0/AUTHORS
--rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-02-02 08:59:25.000000 half_orm-0.9.0/LICENSE
--rw-r--r--   0 joel      (1000) joel      (1000)    27298 2023-05-12 08:38:28.598108 half_orm-0.9.0/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)    26357 2023-05-12 08:37:33.000000 half_orm-0.9.0/README.md
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.582109 half_orm-0.9.0/half_orm/
--rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-02-02 08:59:25.000000 half_orm-0.9.0/half_orm/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     5495 2023-05-12 08:02:28.000000 half_orm-0.9.0/half_orm/field.py
--rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-02-02 08:59:25.000000 half_orm-0.9.0/half_orm/field_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     5558 2023-05-12 08:04:47.000000 half_orm-0.9.0/half_orm/fkey.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3513 2023-05-12 08:00:34.000000 half_orm-0.9.0/half_orm/hotest.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)    14440 2023-04-21 09:03:14.000000 half_orm-0.9.0/half_orm/model.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1143 2023-03-21 09:29:02.000000 half_orm-0.9.0/half_orm/model_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)      405 2023-03-18 07:38:44.000000 half_orm-0.9.0/half_orm/null.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.590108 half_orm-0.9.0/half_orm/packager/
--rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3780 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/changelog.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4470 2023-05-12 08:15:08.000000 half_orm-0.9.0/half_orm/packager/database.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4685 2023-04-21 09:03:14.000000 half_orm-0.9.0/half_orm/packager/db_conn.py
--rw-r--r--   0 joel      (1000) joel      (1000)     7522 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/hgit.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     5335 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/hop.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1274 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/manifest.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     8882 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/modules.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)    13522 2023-03-17 13:09:31.000000 half_orm-0.9.0/half_orm/packager/patch.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.590108 half_orm-0.9.0/half_orm/packager/patches/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.574109 half_orm-0.9.0/half_orm/packager/patches/0/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.574109 half_orm-0.9.0/half_orm/packager/patches/0/1/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.594108 half_orm-0.9.0/half_orm/packager/patches/0/1/0/
--rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
--rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
--rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/patches/log
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.594108 half_orm-0.9.0/half_orm/packager/patches/sql/
--rw-r--r--   0 joel      (1000) joel      (1000)     4197 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/patches/sql/half_orm_meta.sql
--rw-r--r--   0 joel      (1000) joel      (1000)     8297 2023-04-21 09:03:14.000000 half_orm-0.9.0/half_orm/packager/repo.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.598108 half_orm-0.9.0/half_orm/packager/templates/
--rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/.gitignore
--rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/MANIFEST.in
--rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/Pipfile
--rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/README
--rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/base_test
--rw-r--r--   0 joel      (1000) joel      (1000)      437 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/db_connector.py
--rw-r--r--   0 joel      (1000) joel      (1000)      246 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/module_template_1
--rw-r--r--   0 joel      (1000) joel      (1000)      120 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/module_template_2
--rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/module_template_3
--rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/relation_test
--rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/setup.py
--rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/warning
--rw-r--r--   0 joel      (1000) joel      (1000)     2099 2023-04-20 09:30:05.000000 half_orm-0.9.0/half_orm/packager/utils.py
--rw-r--r--   0 joel      (1000) joel      (1000)        8 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/version.txt
--rw-r--r--   0 joel      (1000) joel      (1000)    17049 2023-04-20 09:30:05.000000 half_orm-0.9.0/half_orm/pg_meta.py
--rw-r--r--   0 joel      (1000) joel      (1000)    39274 2023-05-12 08:04:42.000000 half_orm-0.9.0/half_orm/relation.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1520 2023-05-12 08:00:34.000000 half_orm-0.9.0/half_orm/relation_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3876 2023-05-12 08:00:07.000000 half_orm-0.9.0/half_orm/relation_factory.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2743 2023-03-21 09:29:02.000000 half_orm-0.9.0/half_orm/transaction.py
--rw-r--r--   0 joel      (1000) joel      (1000)        6 2023-05-12 08:37:35.000000 half_orm-0.9.0/half_orm/version.txt
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.586109 half_orm-0.9.0/half_orm.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)    27298 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)     1582 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       51 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/entry_points.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       46 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       27 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-01-04 14:18:53.000000 half_orm-0.9.0/pyproject.toml
--rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-05-12 08:38:28.598108 half_orm-0.9.0/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-03-06 08:18:37.000000 half_orm-0.9.0/setup.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/
+-rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-02-02 08:59:25.000000 half_orm-0.9.1/AUTHORS
+-rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-02-02 08:59:25.000000 half_orm-0.9.1/LICENSE
+-rw-r--r--   0 joel      (1000) joel      (1000)    27388 2023-05-22 08:19:19.000856 half_orm-0.9.1/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)    26447 2023-05-22 08:13:46.000000 half_orm-0.9.1/README.md
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:18.996856 half_orm-0.9.1/half_orm/
+-rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-02-02 08:59:25.000000 half_orm-0.9.1/half_orm/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     5495 2023-05-12 08:02:28.000000 half_orm-0.9.1/half_orm/field.py
+-rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-02-02 08:59:25.000000 half_orm-0.9.1/half_orm/field_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     5558 2023-05-12 08:04:47.000000 half_orm-0.9.1/half_orm/fkey.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3513 2023-05-12 08:00:34.000000 half_orm-0.9.1/half_orm/hotest.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)    14440 2023-04-21 09:03:14.000000 half_orm-0.9.1/half_orm/model.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1143 2023-03-21 09:29:02.000000 half_orm-0.9.1/half_orm/model_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      405 2023-03-18 07:38:44.000000 half_orm-0.9.1/half_orm/null.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/
+-rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3794 2023-05-19 09:57:24.000000 half_orm-0.9.1/half_orm/packager/changelog.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4536 2023-05-19 08:11:53.000000 half_orm-0.9.1/half_orm/packager/database.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4652 2023-05-19 09:54:22.000000 half_orm-0.9.1/half_orm/packager/db_conn.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     7522 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/hgit.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     5373 2023-05-19 07:56:23.000000 half_orm-0.9.1/half_orm/packager/hop.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1274 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/manifest.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     8882 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/modules.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)    13389 2023-05-19 09:54:16.000000 half_orm-0.9.1/half_orm/packager/patch.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/patches/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:18.992856 half_orm-0.9.1/half_orm/packager/patches/0/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:18.992856 half_orm-0.9.1/half_orm/packager/patches/0/1/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/patches/0/1/0/
+-rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)      306 2023-05-22 07:11:49.000000 half_orm-0.9.1/half_orm/packager/patches/0/1/0/02_half_orm_meta.view.hop_penultimate_release.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/patches/log
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/patches/sql/
+-rw-r--r--   0 joel      (1000) joel      (1000)     5864 2023-05-22 07:14:29.000000 half_orm-0.9.1/half_orm/packager/patches/sql/half_orm_meta.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)     8618 2023-05-19 07:57:31.000000 half_orm-0.9.1/half_orm/packager/repo.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:19.000856 half_orm-0.9.1/half_orm/packager/templates/
+-rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/.gitignore
+-rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/MANIFEST.in
+-rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/Pipfile
+-rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/README
+-rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/base_test
+-rw-r--r--   0 joel      (1000) joel      (1000)      437 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/db_connector.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      246 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/module_template_1
+-rw-r--r--   0 joel      (1000) joel      (1000)      120 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/module_template_2
+-rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/module_template_3
+-rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/relation_test
+-rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/setup.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/templates/warning
+-rw-r--r--   0 joel      (1000) joel      (1000)     2099 2023-04-20 09:30:05.000000 half_orm-0.9.1/half_orm/packager/utils.py
+-rw-r--r--   0 joel      (1000) joel      (1000)        8 2023-02-28 10:33:54.000000 half_orm-0.9.1/half_orm/packager/version.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)    17049 2023-04-20 09:30:05.000000 half_orm-0.9.1/half_orm/pg_meta.py
+-rw-r--r--   0 joel      (1000) joel      (1000)    39274 2023-05-12 08:04:42.000000 half_orm-0.9.1/half_orm/relation.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1520 2023-05-12 08:00:34.000000 half_orm-0.9.1/half_orm/relation_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3876 2023-05-12 08:00:07.000000 half_orm-0.9.1/half_orm/relation_factory.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2743 2023-03-21 09:29:02.000000 half_orm-0.9.1/half_orm/transaction.py
+-rw-r--r--   0 joel      (1000) joel      (1000)        6 2023-05-22 08:12:53.000000 half_orm-0.9.1/half_orm/version.txt
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-22 08:19:18.996856 half_orm-0.9.1/half_orm.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)    27388 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)     1664 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       51 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/entry_points.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       46 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       27 2023-05-22 08:19:18.000000 half_orm-0.9.1/half_orm.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-01-04 14:18:53.000000 half_orm-0.9.1/pyproject.toml
+-rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-05-22 08:19:19.000856 half_orm-0.9.1/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-03-06 08:18:37.000000 half_orm-0.9.1/setup.py
```

### Comparing `half_orm-0.9.0/LICENSE` & `half_orm-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/PKG-INFO` & `half_orm-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half_orm
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -18,24 +18,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-# A simple PostgreSQL to Python mapper [0.9.0] and its packager [0.1.0a2]
+# A simple PostgreSQL to Python mapper [0.9.1] and its packager [0.1.0a3]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
-![Python versions](https://img.shields.io/pypi/pyversions/half_orm)
+![Python versions](https://img.shields.io/badge/Python-%20&ge;%203.7-blue)
+![PostgreSQL versions](https://img.shields.io/badge/PostgreSQL-%20&ge;%209.6-blue)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
 ![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
 ![Contributors](https://img.shields.io/github/contributors/collorg/halform)
 
-You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data. If you want to build or patch a model, you might be interested in the [`half_orm packager`](#next-hop-the-gitops-half_orm-packager-wipalpha).
+You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.7). `Half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data. If you want to build or patch a model, you might be interested in the [`half_orm packager`](#next-hop-the-gitops-half_orm-packager-wipalpha).
 
 The 'half' part of `half_orm` name indicates that it only deals with the data manipulation language ([DML](https://www.postgresql.org/docs/current/dml.html)) part of SQL. Basically the [`INSERT`](https://www.postgresql.org/docs/current/sql-insert.html), [`SELECT`](https://www.postgresql.org/docs/current/sql-select.html), [`UPDATE`](https://www.postgresql.org/docs/current/sql-update.html) and [`DELETE`](https://www.postgresql.org/docs/current/sql-delete.html) commands. This is what makes `half_orm` so easy to learn an use.
 
 Here is what coding with `half_orm` looks like :
 
 ```python
 from half_orm.model import Model
```

### Comparing `half_orm-0.9.0/README.md` & `half_orm-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# A simple PostgreSQL to Python mapper [0.9.0] and its packager [0.1.0a2]
+# A simple PostgreSQL to Python mapper [0.9.1] and its packager [0.1.0a3]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
-![Python versions](https://img.shields.io/pypi/pyversions/half_orm)
+![Python versions](https://img.shields.io/badge/Python-%20&ge;%203.7-blue)
+![PostgreSQL versions](https://img.shields.io/badge/PostgreSQL-%20&ge;%209.6-blue)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
 ![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
 ![Contributors](https://img.shields.io/github/contributors/collorg/halform)
 
-You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data. If you want to build or patch a model, you might be interested in the [`half_orm packager`](#next-hop-the-gitops-half_orm-packager-wipalpha).
+You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.7). `Half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data. If you want to build or patch a model, you might be interested in the [`half_orm packager`](#next-hop-the-gitops-half_orm-packager-wipalpha).
 
 The 'half' part of `half_orm` name indicates that it only deals with the data manipulation language ([DML](https://www.postgresql.org/docs/current/dml.html)) part of SQL. Basically the [`INSERT`](https://www.postgresql.org/docs/current/sql-insert.html), [`SELECT`](https://www.postgresql.org/docs/current/sql-select.html), [`UPDATE`](https://www.postgresql.org/docs/current/sql-update.html) and [`DELETE`](https://www.postgresql.org/docs/current/sql-delete.html) commands. This is what makes `half_orm` so easy to learn an use.
 
 Here is what coding with `half_orm` looks like :
 
 ```python
 from half_orm.model import Model
```

### Comparing `half_orm-0.9.0/half_orm/field.py` & `half_orm-0.9.1/half_orm/field.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/fkey.py` & `half_orm-0.9.1/half_orm/fkey.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/hotest.py` & `half_orm-0.9.1/half_orm/hotest.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/model.py` & `half_orm-0.9.1/half_orm/model.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/model_errors.py` & `half_orm-0.9.1/half_orm/model_errors.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/packager/changelog.py` & `half_orm-0.9.1/half_orm/packager/changelog.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,32 +49,32 @@
             else:
                 utils.write(self.__file, f'{utils.hop_version()}\t{release}\t\t\n', mode='a+')
         self.__seq()
 
     def update_release(self, release, commit, previous_commit):
         "Add the commit sha1 to the release in the .hop/CHANGELOG file"
         out = []
-        previous = self.previous(release)
+        previous = self.previous(release, 1)
         for line in utils.readlines(self.__file):
             if line and line.split()[1] not in {release, previous}:
                 out.append(line)
             elif line.split()[1] == previous:
                 elt = line.split()
                 out.append(f'{elt[0]}\t{elt[1]}\t{elt[2]}\t{previous_commit}\n')
             else:
                 out.append(f'{utils.hop_version()}\t{release}\t{commit}\t\n')
         utils.write(self.__file, ''.join(out))
         self.__repo.hgit.add(self.__file)
         # self.__repo.hgit.commit('-m', f'[hop][{release}] CHANGELOG')
         self.__seq()
 
-    def previous(self, release):
+    def previous(self, release, index):
         "Return previous release of release."
         index_of_release = self.__releases.index(release)
-        return self.__releases[index_of_release - 1]
+        return self.__releases[index_of_release - index]
 
     @property
     def file(self):
         "Return the name of the changelog file"
         return self.__file
 
     @property
```

### Comparing `half_orm-0.9.0/half_orm/packager/database.py` & `half_orm-0.9.1/half_orm/packager/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,17 @@
         self.__model = None
         self.__last_release = None
         self.__connection_params: DbConn = DbConn(self.__repo.name)
         if self.__repo.name:
             try:
                 self.__model = Model(self.__repo.name)
                 self.__init(self.__repo.name)
-            except OperationalError:
-                pass
+            except OperationalError as err:
+                if not self.__repo.new:
+                    utils.error(err, 1)
 
     def __call__(self, name):
         return self.__class__(self.__repo)
 
     def __init(self, name, get_release=True):
         self.__name = name
         self.__connection_params = DbConn(name)
```

### Comparing `half_orm-0.9.0/half_orm/packager/db_conn.py` & `half_orm-0.9.1/half_orm/packager/db_conn.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,14 @@
         if self.__port:
             cmd_list += ['-p', self.__port]
         if self.__host:
             cmd_list += ['-h', self.__host]
         cmd_list.append(self.__name)
         if args:
             cmd_list += args
-        # print('XXX', cmd_list)
         try:
             subprocess.run(
                 cmd_list, env=env, shell=False, check=True,
                 # stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                 **kwargs)
         except subprocess.CalledProcessError as err:
             utils.error(f'{err.stderr} with user: {self.__user}, host: {self.__host}, port: {self.__port}\n', exit_code=err.returncode)
```

### Comparing `half_orm-0.9.0/half_orm/packager/hgit.py` & `half_orm-0.9.1/half_orm/packager/hgit.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/packager/hop.py` & `half_orm-0.9.1/half_orm/packager/hop.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         "Adds the commands to the main click group."
         @click.command()
         @click.argument('package_name')
         @click.option('-d', '--devel', is_flag=True, help="Development mode")
         def new(package_name, devel=False):
             """ Creates a new hop project named <package_name>.
             """
-            self.__repo.new(package_name, devel)
+            self.__repo.init(package_name, devel)
 
 
         @click.command()
         @click.option(
             '-l', '--level',
             type=click.Choice(['patch', 'minor', 'major']), help="Release level.")
         @click.option('-m', '--message', type=str, help="The git commit message")
@@ -154,15 +154,16 @@
 def main(ctx):
     """
     Generates/Synchronises/Patches a python package from a PostgreSQL database
     """
     if hop.repo_checked and ctx.invoked_subcommand is None:
         click.echo(hop.state)
     elif not hop.repo_checked and ctx.invoked_subcommand != 'new':
-        utils.error(
-            "You're not in a hop repository.\n"
-            "Try `hop new <package name>` or change directory.\n", exit_code=1)
+        click.echo(hop.state)
+        print(
+            "\nNot in a hop repository.\n"
+            f"Try {utils.Color.bold('hop new [--devel] <package name>')} or change directory.\n")
 
 hop.add_commands(main)
 
 if __name__ == '__main__':
     main({})
```

### Comparing `half_orm-0.9.0/half_orm/packager/manifest.py` & `half_orm-0.9.1/half_orm/packager/manifest.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/packager/modules.py` & `half_orm-0.9.1/half_orm/packager/modules.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/packager/patch.py` & `half_orm-0.9.1/half_orm/packager/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
     @classmethod
     @property
     def levels(cls):
         "Returns the levels"
         return cls.__levels
 
-    def previous(self, release):
+    def previous(self, release, index=0):
         "Return .hop/CHANGELOG second to last line."
-        return self.__changelog.previous(release)
+        return self.__changelog.previous(release, index)
 
     @property
     def __next_releases(self):
         db_last_release = self.__repo.database.last_release_s
         ch_last_release = self.__changelog.last_release
         if db_last_release != ch_last_release:
             utils.error(
@@ -162,57 +162,56 @@
         self.__repo.model.disconnect()
         self.__repo.database.execute_pg_command('dropdb')
         self.__repo.database.execute_pg_command('createdb')
         self.__repo.database.execute_pg_command(
             'psql', '-f', self.__backup_file('Backups', release), stdout=subprocess.DEVNULL)
         self.__repo.model.ping()
 
+    def __restore_previous_release(self):
+        db_release = self.__repo.database.last_release_s
+        previous_release = self.previous(db_release, 1)
+        self.__restore_db(db_release)
+        os.remove(self.__backup_file('Backups', db_release))
+        sys.exit(1)
+
     def __execute_sql(self, file_):
         "Execute sql query contained in sql file_"
         query = utils.read(file_.path).replace('%', '%%')
         if len(query) == 0:
             return
         try:
             self.__repo.model.execute_query(query)
         except (psycopg2.Error, psycopg2.OperationalError, psycopg2.InterfaceError) as err:
             utils.error(f'Problem with query in {file_.name}\n{err}\n')
-            db_release = self.__repo.database.last_release_s
-            previous_release = self.previous(db_release)
-            self.__restore_db(previous_release)
-            os.remove(self.__backup_file('Backups', previous_release))
-            sys.exit(1)
+            self.__restore_previous_release()
 
     def __execute_script(self, file_):
         try:
             subprocess.run(
                 ['python', file_.path],
                 env=os.environ.update({'PYTHONPATH': self.__repo.base_dir}),
                 shell=False, check=True)
         except subprocess.CalledProcessError as err:
             utils.error(f'Problem with script {file_}\n{err}\n')
-            db_release = self.__repo.database.last_release_s
-            previous_release = self.previous(db_release)
-            self.__restore_db(previous_release)
-            os.remove(self.__backup_file('Backups', previous_release))
-            sys.exit(1)
+            self.__restore_previous_release()
 
     def apply(self, release, force=False, save_db=True):
         "Apply the release in 'path'"
         if self.__repo.hgit.repos_is_clean():
             self.__repo.hgit.rebase('hop_main')
         db_release = self.__repo.database.last_release_s
         changelog_msg = ''
         if self.__check_apply_or_re_apply() == 'apply' and save_db:
             self.__save_db(db_release)
         elif not self.__repo.production:
             if not force:
                 okay = input(f'Do you want to re-apply the release {release} [y/N]?') or 'y'
                 if okay.upper() != 'Y':
                     sys.exit()
-            self.__restore_db(self.previous(db_release))
+            self.__restore_db(self.previous(db_release, 1))
         app_upg = utils.Color.green('Upgrading to') if self.__repo.production else utils.Color.bold('Applying')
         print(f'{app_upg} {utils.Color.bold(release)}')
         files = []
         major, minor, patch = release.split('.')
         path = os.path.join(self.__patches_base_dir, major, minor, patch)
         for file_ in os.scandir(path):
             files.append({'name': file_.name, 'file': file_})
@@ -253,15 +252,15 @@
             resp = ['This repo is not in developement mode.']
         return '\n'.join(resp)
 
 
     def undo(self, database_only=False):
         "Undo a patch."
         db_release = self.__repo.database.last_release_s
-        previous_release = self.previous(db_release)
+        previous_release = self.previous(db_release, 1)
         self.__restore_db(previous_release)
         if not database_only:
             modules.generate(self.__repo)
         os.remove(self.__backup_file('Backups', previous_release))
 
     def sync_package(self):
         "Synchronise the package with the current database model"
```

### Comparing `half_orm-0.9.0/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql` & `half_orm-0.9.1/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/packager/patches/sql/half_orm_meta.sql` & `half_orm-0.9.1/half_orm/packager/patches/sql/half_orm_meta.sql`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 --
 -- PostgreSQL database dump
 --
 
--- Dumped from database version 15.1 (Debian 15.1-1.pgdg110+1)
--- Dumped by pg_dump version 15.1 (Debian 15.1-1.pgdg110+1)
+-- Dumped from database version 13.11 (Debian 13.11-1.pgdg110+1)
+-- Dumped by pg_dump version 13.11 (Debian 13.11-1.pgdg110+1)
 
 SET statement_timeout = 0;
 SET lock_timeout = 0;
 SET idle_in_transaction_session_timeout = 0;
 SET client_encoding = 'UTF8';
 SET standard_conforming_strings = on;
 SELECT pg_catalog.set_config('search_path', '', false);
@@ -26,32 +26,84 @@
 --
 -- Name: half_orm_meta.view; Type: SCHEMA; Schema: -; Owner: -
 --
 
 CREATE SCHEMA "half_orm_meta.view";
 
 
+--
+-- Name: check_database(text); Type: FUNCTION; Schema: half_orm_meta; Owner: -
+--
+
+CREATE FUNCTION half_orm_meta.check_database(old_dbid text DEFAULT NULL::text) RETURNS text
+    LANGUAGE plpgsql
+    AS $$
+DECLARE
+    dbname text;
+    dbid text;
+BEGIN
+    select current_database() into dbname;
+    --XXX: use a materialized view.
+    BEGIN
+        select encode(hmac(dbname, pg_read_file('hop_key'), 'sha1'), 'hex') into dbid;
+    EXCEPTION
+        when undefined_file then
+            raise NOTICE 'No hop_key file for the cluster. Will use % for dbid', dbname;
+            dbid := dbname;
+    END;
+    if old_dbid is not null and old_dbid != dbid
+    then
+        raise Exception 'Not the same database!';
+    end if;
+    return dbid;
+END;
+$$;
+
+
 SET default_tablespace = '';
 
 SET default_table_access_method = heap;
 
 --
+-- Name: database; Type: TABLE; Schema: half_orm_meta; Owner: -
+--
+
+CREATE TABLE half_orm_meta.database (
+    id text NOT NULL,
+    name text NOT NULL,
+    description text
+);
+
+
+--
+-- Name: TABLE database; Type: COMMENT; Schema: half_orm_meta; Owner: -
+--
+
+COMMENT ON TABLE half_orm_meta.database IS '
+id identifies the database in the cluster. It uses the key
+in hop_key.
+';
+
+
+--
 -- Name: hop_release; Type: TABLE; Schema: half_orm_meta; Owner: -
 --
 
 CREATE TABLE half_orm_meta.hop_release (
     major integer NOT NULL,
     minor integer NOT NULL,
     patch integer NOT NULL,
     pre_release text DEFAULT ''::text NOT NULL,
     pre_release_num text DEFAULT ''::text NOT NULL,
     date date DEFAULT CURRENT_DATE,
     "time" time(0) with time zone DEFAULT CURRENT_TIME,
     changelog text,
     commit text,
+    dbid text,
+    hop_release text,
     CONSTRAINT hop_release_major_check CHECK ((major >= 0)),
     CONSTRAINT hop_release_minor_check CHECK ((minor >= 0)),
     CONSTRAINT hop_release_patch_check CHECK ((patch >= 0)),
     CONSTRAINT hop_release_pre_release_check CHECK ((pre_release = ANY (ARRAY['alpha'::text, 'beta'::text, 'rc'::text, ''::text]))),
     CONSTRAINT hop_release_pre_release_num_check CHECK (((pre_release_num = ''::text) OR (pre_release_num ~ '^\d+$'::text)))
 );
 
@@ -93,26 +145,33 @@
 
 
 --
 -- Name: hop_penultimate_release; Type: VIEW; Schema: half_orm_meta.view; Owner: -
 --
 
 CREATE VIEW "half_orm_meta.view".hop_penultimate_release AS
- WITH sub AS (
-         SELECT hop_release.major,
+ SELECT penultimate.major,
+    penultimate.minor,
+    penultimate.patch
+   FROM ( SELECT hop_release.major,
             hop_release.minor,
-            hop_release.patch,
-            row_number() OVER (ORDER BY hop_release.major DESC, hop_release.minor DESC, hop_release.patch DESC) AS rn
+            hop_release.patch
            FROM half_orm_meta.hop_release
-        )
- SELECT sub.major,
-    sub.minor,
-    sub.patch
-   FROM sub
-  WHERE (sub.rn = 2);
+          ORDER BY hop_release.major DESC, hop_release.minor DESC, hop_release.patch DESC
+         LIMIT 2) penultimate
+  ORDER BY penultimate.major, penultimate.minor, penultimate.patch
+ LIMIT 1;
+
+
+--
+-- Name: database database_pkey; Type: CONSTRAINT; Schema: half_orm_meta; Owner: -
+--
+
+ALTER TABLE ONLY half_orm_meta.database
+    ADD CONSTRAINT database_pkey PRIMARY KEY (id);
 
 
 --
 -- Name: hop_release_issue hop_release_issue_pkey; Type: CONSTRAINT; Schema: half_orm_meta; Owner: -
 --
 
 ALTER TABLE ONLY half_orm_meta.hop_release_issue
@@ -124,14 +183,22 @@
 --
 
 ALTER TABLE ONLY half_orm_meta.hop_release
     ADD CONSTRAINT hop_release_pkey PRIMARY KEY (major, minor, patch, pre_release, pre_release_num);
 
 
 --
+-- Name: hop_release hop_release_dbid_fkey; Type: FK CONSTRAINT; Schema: half_orm_meta; Owner: -
+--
+
+ALTER TABLE ONLY half_orm_meta.hop_release
+    ADD CONSTRAINT hop_release_dbid_fkey FOREIGN KEY (dbid) REFERENCES half_orm_meta.database(id) ON UPDATE CASCADE;
+
+
+--
 -- Name: hop_release_issue hop_release_issue_release_major_release_minor_release_patc_fkey; Type: FK CONSTRAINT; Schema: half_orm_meta; Owner: -
 --
 
 ALTER TABLE ONLY half_orm_meta.hop_release_issue
     ADD CONSTRAINT hop_release_issue_release_major_release_minor_release_patc_fkey FOREIGN KEY (release_major, release_minor, release_patch, release_pre_release, release_pre_release_num) REFERENCES half_orm_meta.hop_release(major, minor, patch, pre_release, pre_release_num);
```

### Comparing `half_orm-0.9.0/half_orm/packager/repo.py` & `half_orm-0.9.1/half_orm/packager/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,23 +79,29 @@
     @devel.setter
     def devel(self, devel):
         self.__devel = devel
 
 class Repo:
     """Reads and writes the hop repo conf file.
     """
+    __new = False
     __checked: bool = False
     __base_dir: str = None
     __config: Config = None
     database: Database = NotImplementedError()
     hgit: HGit = None
     def __init__(self):
         self.__check()
 
     @property
+    def new(self):
+        "Returns if the repo is being created or not."
+        return Repo.__new
+
+    @property
     def checked(self):
         "Returns if the Repo is OK."
         return self.__checked
 
     @property
     def production(self):
         "Returns the production status of the database"
@@ -159,31 +165,34 @@
     @property
     def devel(self):
         return self.__config.devel
 
     @property
     def state(self):
         "Returns the state (str) of the repository."
-        res = [f'Half-ORM packager: {utils.hop_version()}\n']
-        hop_version = utils.Color.red(self.__config.hop_version) if \
-            self.__hop_version_mismatch() else \
-            utils.Color.green(self.__config.hop_version)
-        res += [
-            '[Hop repository]',
-            f'- base directory: {self.__base_dir}',
-            f'- package name: {self.__config.name}',
-            f'- hop version: {hop_version}'
-        ]
-        res.append(self.database.state)
-        res.append(str(self.hgit))
-        res.append(Patch(self).state)
+        res = [f'hop version: {utils.Color.bold(utils.hop_version())}']
+        res += [f'half-orm version: {utils.Color.bold(half_orm.VERSION)}\n']
+        if self.__config:
+            hop_version = utils.Color.red(self.__config.hop_version) if \
+                self.__hop_version_mismatch() else \
+                utils.Color.green(self.__config.hop_version)
+            res += [
+                '[Hop repository]',
+                f'- base directory: {self.__base_dir}',
+                f'- package name: {self.__config.name}',
+                f'- hop version: {hop_version}'
+            ]
+            res.append(self.database.state)
+            res.append(str(self.hgit))
+            res.append(Patch(self).state)
         return '\n'.join(res)
 
-    def new(self, package_name, devel):
+    def init(self, package_name, devel):
         "Create a new hop repository"
+        Repo.__new = True
         cur_dir = os.path.abspath(os.path.curdir)
         self.__base_dir = os.path.join(cur_dir, package_name)
         self.__config = Config(self.__base_dir, name=package_name, devel=devel)
         self.database = Database(self).init(self.__config.name)
         print(f"Installing new hop repo in {self.__base_dir}.")
 
         if not os.path.exists(self.__base_dir):
```

### Comparing `half_orm-0.9.0/half_orm/packager/templates/README` & `half_orm-0.9.1/half_orm/packager/templates/README`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/packager/templates/setup.py` & `half_orm-0.9.1/half_orm/packager/templates/setup.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/packager/utils.py` & `half_orm-0.9.1/half_orm/packager/utils.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/pg_meta.py` & `half_orm-0.9.1/half_orm/pg_meta.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/relation.py` & `half_orm-0.9.1/half_orm/relation.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/relation_errors.py` & `half_orm-0.9.1/half_orm/relation_errors.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/relation_factory.py` & `half_orm-0.9.1/half_orm/relation_factory.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm/transaction.py` & `half_orm-0.9.1/half_orm/transaction.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.0/half_orm.egg-info/PKG-INFO` & `half_orm-0.9.1/half_orm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half-orm
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -18,24 +18,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-# A simple PostgreSQL to Python mapper [0.9.0] and its packager [0.1.0a2]
+# A simple PostgreSQL to Python mapper [0.9.1] and its packager [0.1.0a3]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
-![Python versions](https://img.shields.io/pypi/pyversions/half_orm)
+![Python versions](https://img.shields.io/badge/Python-%20&ge;%203.7-blue)
+![PostgreSQL versions](https://img.shields.io/badge/PostgreSQL-%20&ge;%209.6-blue)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
 ![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
 ![Contributors](https://img.shields.io/github/contributors/collorg/halform)
 
-You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data. If you want to build or patch a model, you might be interested in the [`half_orm packager`](#next-hop-the-gitops-half_orm-packager-wipalpha).
+You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.7). `Half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data. If you want to build or patch a model, you might be interested in the [`half_orm packager`](#next-hop-the-gitops-half_orm-packager-wipalpha).
 
 The 'half' part of `half_orm` name indicates that it only deals with the data manipulation language ([DML](https://www.postgresql.org/docs/current/dml.html)) part of SQL. Basically the [`INSERT`](https://www.postgresql.org/docs/current/sql-insert.html), [`SELECT`](https://www.postgresql.org/docs/current/sql-select.html), [`UPDATE`](https://www.postgresql.org/docs/current/sql-update.html) and [`DELETE`](https://www.postgresql.org/docs/current/sql-delete.html) commands. This is what makes `half_orm` so easy to learn an use.
 
 Here is what coding with `half_orm` looks like :
 
 ```python
 from half_orm.model import Model
```

### Comparing `half_orm-0.9.0/half_orm.egg-info/SOURCES.txt` & `half_orm-0.9.1/half_orm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 half_orm/packager/patch.py
 half_orm/packager/repo.py
 half_orm/packager/utils.py
 half_orm/packager/version.txt
 half_orm/packager/patches/log
 half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
 half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
+half_orm/packager/patches/0/1/0/02_half_orm_meta.view.hop_penultimate_release.sql
 half_orm/packager/patches/sql/half_orm_meta.sql
 half_orm/packager/templates/.gitignore
 half_orm/packager/templates/MANIFEST.in
 half_orm/packager/templates/Pipfile
 half_orm/packager/templates/README
 half_orm/packager/templates/base_test
 half_orm/packager/templates/db_connector.py
```

### Comparing `half_orm-0.9.0/setup.py` & `half_orm-0.9.1/setup.py`

 * *Files identical despite different names*

