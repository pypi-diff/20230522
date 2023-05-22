# Comparing `tmp/ppss_auth-0.9.4.4.tar.gz` & `tmp/ppss_auth-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppss_auth-0.9.4.4.tar", last modified: Wed Apr  5 11:27:38 2023, max compression
+gzip compressed data, was "ppss_auth-0.9.5.tar", last modified: Mon May 22 07:24:03 2023, max compression
```

## Comparing `ppss_auth-0.9.4.4.tar` & `ppss_auth-0.9.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.450416 ppss_auth-0.9.4.4/
--rwxrwxrwx   0 dan       (1000) dan       (1000)      159 2021-12-20 10:13:03.000000 ppss_auth-0.9.4.4/MANIFEST.in
--rw-r--r--   0 dan       (1000) dan       (1000)    13538 2023-04-05 11:27:38.450416 ppss_auth-0.9.4.4/PKG-INFO
--rwxrwxrwx   0 dan       (1000) dan       (1000)     6433 2023-04-04 13:50:54.000000 ppss_auth-0.9.4.4/README.md
--rwxrwxrwx   0 dan       (1000) dan       (1000)      266 2021-12-20 10:13:03.000000 ppss_auth-0.9.4.4/babel.ini
--rwxrwxrwx   0 dan       (1000) dan       (1000)      919 2021-12-20 10:13:03.000000 ppss_auth-0.9.4.4/changelog.txt
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.440416 ppss_auth-0.9.4.4/ppss_auth/
--rw-r--r--   0 dan       (1000) dan       (1000)     4192 2023-02-01 09:09:14.000000 ppss_auth-0.9.4.4/ppss_auth/__init__.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.440416 ppss_auth-0.9.4.4/ppss_auth/alembic/
--rw-r--r--   0 dan       (1000) dan       (1000)     2181 2023-01-30 10:16:40.000000 ppss_auth-0.9.4.4/ppss_auth/alembic/alembic.ini
--rwxrwxrwx   0 dan       (1000) dan       (1000)     3298 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/alembic/env.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)      494 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/alembic/script.py.mako
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.440416 ppss_auth-0.9.4.4/ppss_auth/alembic/versions/
--rwxrwxrwx   0 dan       (1000) dan       (1000)      729 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/alembic/versions/20201026_52f4d4eefdfe_unique_permission_name.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)      711 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/alembic/versions/20201120_6c9e84ab8280_unique_user_name.py
--rw-r--r--   0 dan       (1000) dan       (1000)      849 2023-01-30 10:16:40.000000 ppss_auth-0.9.4.4/ppss_auth/alembic/versions/20220329_44fde88fa438_creazione_colonne_per_login_history.py
--rw-r--r--   0 dan       (1000) dan       (1000)      696 2023-01-30 10:16:40.000000 ppss_auth-0.9.4.4/ppss_auth/alembic/versions/20220331_6190d529682d_result_reason.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)     5947 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/alembic/versions/f724fac25359_creation.py
--rw-r--r--   0 dan       (1000) dan       (1000)     7946 2023-01-30 10:16:40.000000 ppss_auth-0.9.4.4/ppss_auth/constants.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.430416 ppss_auth-0.9.4.4/ppss_auth/locale/
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.430416 ppss_auth-0.9.4.4/ppss_auth/locale/en/
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.440416 ppss_auth-0.9.4.4/ppss_auth/locale/en/LC_MESSAGES/
--rwxrwxrwx   0 dan       (1000) dan       (1000)      656 2021-12-20 10:13:03.000000 ppss_auth-0.9.4.4/ppss_auth/locale/en/LC_MESSAGES/ppss_auth.mo
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.430416 ppss_auth-0.9.4.4/ppss_auth/locale/it/
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.440416 ppss_auth-0.9.4.4/ppss_auth/locale/it/LC_MESSAGES/
--rwxrwxrwx   0 dan       (1000) dan       (1000)     2473 2021-12-20 10:13:03.000000 ppss_auth-0.9.4.4/ppss_auth/locale/it/LC_MESSAGES/ppss_auth.mo
--rw-r--r--   0 dan       (1000) dan       (1000)    17232 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/models.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.440416 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_static/
--rwxrwxrwx   0 dan       (1000) dan       (1000)     2331 2020-01-09 13:44:24.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_static/loader.js
--rwxrwxrwx   0 dan       (1000) dan       (1000)      834 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_static/ppssauth.css
--rwxrwxrwx   0 dan       (1000) dan       (1000)     5558 2020-01-09 13:44:24.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_static/ppssauth.js
--rwxrwxrwx   0 dan       (1000) dan       (1000)      930 2020-01-09 13:44:24.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_static/template.html
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.440416 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/
--rwxrwxrwx   0 dan       (1000) dan       (1000)       48 2021-12-20 10:13:03.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/__init__.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)     3076 2021-12-20 10:13:03.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/db.py
--rw-r--r--   0 dan       (1000) dan       (1000)      380 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/emailclient.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)      442 2021-12-20 10:13:03.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/i18n.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)     1499 2021-12-20 10:13:03.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/password.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)      545 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/scriptutils.py
--rw-r--r--   0 dan       (1000) dan       (1000)     4412 2023-01-30 10:16:40.000000 ppss_auth-0.9.4.4/ppss_auth/routes.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.440416 ppss_auth-0.9.4.4/ppss_auth/scripts/
--rwxrwxrwx   0 dan       (1000) dan       (1000)        0 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/scripts/__init__.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)      761 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/scripts/alchemyutils.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)     1167 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/scripts/cleanup_db.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)     4119 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/scripts/create_user.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)     1110 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/scripts/initialize_db.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)       32 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/scripts/sayauth.py
--rwxrwxrwx   0 dan       (1000) dan       (1000)      536 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/scripts/upgrade_db.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.450416 ppss_auth-0.9.4.4/ppss_auth/templates/
--rw-r--r--   0 dan       (1000) dan       (1000)     1384 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/change.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)     1156 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/change.mako
--rw-r--r--   0 dan       (1000) dan       (1000)     4088 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/editgroup.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)     3945 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/editgroup.mako
--rw-r--r--   0 dan       (1000) dan       (1000)      637 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/editperm.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)      589 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/editperm.mako
--rw-r--r--   0 dan       (1000) dan       (1000)     2444 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/edituser.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)     2111 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/edituser.mako
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.450416 ppss_auth-0.9.4.4/ppss_auth/templates/email/
--rwxrwxrwx   0 dan       (1000) dan       (1000)        0 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/templates/email/activation.html
--rw-r--r--   0 dan       (1000) dan       (1000)      358 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/email/activation.mako
--rwxrwxrwx   0 dan       (1000) dan       (1000)        0 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/templates/email/activation.txt
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.450416 ppss_auth-0.9.4.4/ppss_auth/templates/layouts/
--rwxrwxrwx   0 dan       (1000) dan       (1000)     1215 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/templates/layouts/masterlayout.jinja2
--rwxrwxrwx   0 dan       (1000) dan       (1000)     1147 2021-05-11 12:48:04.000000 ppss_auth-0.9.4.4/ppss_auth/templates/layouts/masterlayout.mako
--rw-r--r--   0 dan       (1000) dan       (1000)     1691 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/layouts/midlayout.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)     1548 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/layouts/midlayout.mako
--rwxrwxrwx   0 dan       (1000) dan       (1000)      312 2020-04-06 16:34:12.000000 ppss_auth-0.9.4.4/ppss_auth/templates/layouts/public.jinja2
--rwxrwxrwx   0 dan       (1000) dan       (1000)      296 2020-04-06 16:34:12.000000 ppss_auth-0.9.4.4/ppss_auth/templates/layouts/public.mako
--rw-r--r--   0 dan       (1000) dan       (1000)      919 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/listgroup.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)      869 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/listgroup.mako
--rw-r--r--   0 dan       (1000) dan       (1000)      845 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/listperm.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)      801 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/listperm.mako
--rw-r--r--   0 dan       (1000) dan       (1000)     1276 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/listuser.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)     1201 2023-04-05 11:23:18.000000 ppss_auth-0.9.4.4/ppss_auth/templates/listuser.mako
--rw-r--r--   0 dan       (1000) dan       (1000)     2075 2023-02-23 15:52:02.000000 ppss_auth-0.9.4.4/ppss_auth/templates/login.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)     1954 2023-02-23 15:49:39.000000 ppss_auth-0.9.4.4/ppss_auth/templates/login.mako
--rw-r--r--   0 dan       (1000) dan       (1000)     1216 2023-02-23 15:52:28.000000 ppss_auth-0.9.4.4/ppss_auth/templates/login_nogrid.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)     1132 2023-02-23 15:49:23.000000 ppss_auth-0.9.4.4/ppss_auth/templates/login_nogrid.mako
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.450416 ppss_auth-0.9.4.4/ppss_auth/templates/partials/
--rw-r--r--   0 dan       (1000) dan       (1000)      603 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/partials/userblock.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)      591 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/partials/userblock.mako
--rw-r--r--   0 dan       (1000) dan       (1000)      434 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/partials/usermanage.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)      415 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/partials/usermanage.mako
--rw-r--r--   0 dan       (1000) dan       (1000)     1292 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/registeruser.jinja2
--rw-r--r--   0 dan       (1000) dan       (1000)     1229 2023-02-23 13:56:33.000000 ppss_auth-0.9.4.4/ppss_auth/templates/registeruser.mako
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.450416 ppss_auth-0.9.4.4/ppss_auth/templates/shared/
--rwxrwxrwx   0 dan       (1000) dan       (1000)      211 2020-04-06 16:34:12.000000 ppss_auth-0.9.4.4/ppss_auth/templates/shared/bootstrapcss.html
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.450416 ppss_auth-0.9.4.4/ppss_auth/views/
--rwxrwxrwx   0 dan       (1000) dan       (1000)       36 2020-01-09 13:44:24.000000 ppss_auth-0.9.4.4/ppss_auth/views/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)    26579 2023-01-30 10:16:40.000000 ppss_auth-0.9.4.4/ppss_auth/views/auth.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-04-05 11:27:38.440416 ppss_auth-0.9.4.4/ppss_auth.egg-info/
--rwxrwxrwx   0 dan       (1000) dan       (1000)    13538 2023-04-05 11:27:38.000000 ppss_auth-0.9.4.4/ppss_auth.egg-info/PKG-INFO
--rwxrwxrwx   0 dan       (1000) dan       (1000)     2862 2023-04-05 11:27:38.000000 ppss_auth-0.9.4.4/ppss_auth.egg-info/SOURCES.txt
--rwxrwxrwx   0 dan       (1000) dan       (1000)        1 2023-04-05 11:27:38.000000 ppss_auth-0.9.4.4/ppss_auth.egg-info/dependency_links.txt
--rwxrwxrwx   0 dan       (1000) dan       (1000)      362 2023-04-05 11:27:38.000000 ppss_auth-0.9.4.4/ppss_auth.egg-info/entry_points.txt
--rwxrwxrwx   0 dan       (1000) dan       (1000)       51 2023-04-05 11:27:38.000000 ppss_auth-0.9.4.4/ppss_auth.egg-info/requires.txt
--rwxrwxrwx   0 dan       (1000) dan       (1000)       10 2023-04-05 11:27:38.000000 ppss_auth-0.9.4.4/ppss_auth.egg-info/top_level.txt
--rw-r--r--   0 dan       (1000) dan       (1000)     1388 2023-01-30 10:16:40.000000 ppss_auth-0.9.4.4/readme.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-04-05 11:27:38.450416 ppss_auth-0.9.4.4/setup.cfg
--rw-r--r--   0 dan       (1000) dan       (1000)     1606 2023-04-05 11:27:04.000000 ppss_auth-0.9.4.4/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.716031 ppss_auth-0.9.5/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      159 2021-12-20 10:13:03.000000 ppss_auth-0.9.5/MANIFEST.in
+-rw-r--r--   0 dan       (1000) dan       (1000)    13536 2023-05-22 07:24:03.716031 ppss_auth-0.9.5/PKG-INFO
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     6433 2023-04-04 13:50:54.000000 ppss_auth-0.9.5/README.md
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      266 2021-12-20 10:13:03.000000 ppss_auth-0.9.5/babel.ini
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     1034 2023-05-22 07:18:58.000000 ppss_auth-0.9.5/changelog.txt
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.676031 ppss_auth-0.9.5/ppss_auth/
+-rw-r--r--   0 dan       (1000) dan       (1000)     4192 2023-02-01 09:09:14.000000 ppss_auth-0.9.5/ppss_auth/__init__.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.676031 ppss_auth-0.9.5/ppss_auth/alembic/
+-rw-r--r--   0 dan       (1000) dan       (1000)     2181 2023-01-30 10:16:40.000000 ppss_auth-0.9.5/ppss_auth/alembic/alembic.ini
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     3298 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/alembic/env.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      494 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/alembic/script.py.mako
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.686031 ppss_auth-0.9.5/ppss_auth/alembic/versions/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      729 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/alembic/versions/20201026_52f4d4eefdfe_unique_permission_name.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      711 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/alembic/versions/20201120_6c9e84ab8280_unique_user_name.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      849 2023-01-30 10:16:40.000000 ppss_auth-0.9.5/ppss_auth/alembic/versions/20220329_44fde88fa438_creazione_colonne_per_login_history.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      696 2023-01-30 10:16:40.000000 ppss_auth-0.9.5/ppss_auth/alembic/versions/20220331_6190d529682d_result_reason.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     5947 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/alembic/versions/f724fac25359_creation.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     8487 2023-05-19 10:10:46.000000 ppss_auth-0.9.5/ppss_auth/constants.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.666031 ppss_auth-0.9.5/ppss_auth/locale/
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.666031 ppss_auth-0.9.5/ppss_auth/locale/en/
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.686031 ppss_auth-0.9.5/ppss_auth/locale/en/LC_MESSAGES/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      656 2021-12-20 10:13:03.000000 ppss_auth-0.9.5/ppss_auth/locale/en/LC_MESSAGES/ppss_auth.mo
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.666031 ppss_auth-0.9.5/ppss_auth/locale/it/
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.686031 ppss_auth-0.9.5/ppss_auth/locale/it/LC_MESSAGES/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     2473 2021-12-20 10:13:03.000000 ppss_auth-0.9.5/ppss_auth/locale/it/LC_MESSAGES/ppss_auth.mo
+-rw-r--r--   0 dan       (1000) dan       (1000)    17434 2023-05-17 13:18:07.000000 ppss_auth-0.9.5/ppss_auth/models.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.686031 ppss_auth-0.9.5/ppss_auth/ppss_auth_static/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     2331 2020-01-09 13:44:24.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_static/loader.js
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      834 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_static/ppssauth.css
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     5558 2020-01-09 13:44:24.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_static/ppssauth.js
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      930 2020-01-09 13:44:24.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_static/template.html
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.686031 ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)       48 2021-12-20 10:13:03.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/__init__.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     3076 2021-12-20 10:13:03.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/db.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      380 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/emailclient.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      442 2021-12-20 10:13:03.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/i18n.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     2285 2023-05-19 10:11:31.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/password.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      545 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/scriptutils.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     4415 2023-05-17 13:23:01.000000 ppss_auth-0.9.5/ppss_auth/routes.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.696031 ppss_auth-0.9.5/ppss_auth/scripts/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)        0 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/scripts/__init__.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      761 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/scripts/alchemyutils.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     1167 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/scripts/cleanup_db.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     4119 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/scripts/create_user.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     1110 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/scripts/initialize_db.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)       32 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/scripts/sayauth.py
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      536 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/scripts/upgrade_db.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.706031 ppss_auth-0.9.5/ppss_auth/templates/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1384 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/change.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)     1156 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/change.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)     4088 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/editgroup.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)     3945 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/editgroup.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)      637 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/editperm.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)      589 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/editperm.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)     2444 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/edituser.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)     2111 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/edituser.mako
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.706031 ppss_auth-0.9.5/ppss_auth/templates/email/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)        0 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/templates/email/activation.html
+-rw-r--r--   0 dan       (1000) dan       (1000)      358 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/email/activation.mako
+-rwxrwxrwx   0 dan       (1000) dan       (1000)        0 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/templates/email/activation.txt
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.706031 ppss_auth-0.9.5/ppss_auth/templates/layouts/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     1215 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/templates/layouts/masterlayout.jinja2
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     1147 2021-05-11 12:48:04.000000 ppss_auth-0.9.5/ppss_auth/templates/layouts/masterlayout.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)     1691 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/layouts/midlayout.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)     1548 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/layouts/midlayout.mako
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      312 2020-04-06 16:34:12.000000 ppss_auth-0.9.5/ppss_auth/templates/layouts/public.jinja2
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      296 2020-04-06 16:34:12.000000 ppss_auth-0.9.5/ppss_auth/templates/layouts/public.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)      919 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/listgroup.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)      869 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/listgroup.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)      845 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/listperm.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)      801 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/listperm.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)     1276 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/listuser.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)     1201 2023-04-05 11:23:18.000000 ppss_auth-0.9.5/ppss_auth/templates/listuser.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)     2075 2023-02-23 15:52:02.000000 ppss_auth-0.9.5/ppss_auth/templates/login.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)     1954 2023-02-23 15:49:39.000000 ppss_auth-0.9.5/ppss_auth/templates/login.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)     1216 2023-02-23 15:52:28.000000 ppss_auth-0.9.5/ppss_auth/templates/login_nogrid.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)     1132 2023-02-23 15:49:23.000000 ppss_auth-0.9.5/ppss_auth/templates/login_nogrid.mako
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.706031 ppss_auth-0.9.5/ppss_auth/templates/partials/
+-rw-r--r--   0 dan       (1000) dan       (1000)      603 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/partials/userblock.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)      591 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/partials/userblock.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)      434 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/partials/usermanage.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)      415 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/partials/usermanage.mako
+-rw-r--r--   0 dan       (1000) dan       (1000)     1292 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/registeruser.jinja2
+-rw-r--r--   0 dan       (1000) dan       (1000)     1229 2023-02-23 13:56:33.000000 ppss_auth-0.9.5/ppss_auth/templates/registeruser.mako
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.706031 ppss_auth-0.9.5/ppss_auth/templates/shared/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      211 2020-04-06 16:34:12.000000 ppss_auth-0.9.5/ppss_auth/templates/shared/bootstrapcss.html
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.716031 ppss_auth-0.9.5/ppss_auth/views/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)       36 2020-01-09 13:44:24.000000 ppss_auth-0.9.5/ppss_auth/views/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)    27126 2023-05-19 09:56:21.000000 ppss_auth-0.9.5/ppss_auth/views/auth.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-22 07:24:03.676031 ppss_auth-0.9.5/ppss_auth.egg-info/
+-rwxrwxrwx   0 dan       (1000) dan       (1000)    13536 2023-05-22 07:24:03.000000 ppss_auth-0.9.5/ppss_auth.egg-info/PKG-INFO
+-rwxrwxrwx   0 dan       (1000) dan       (1000)     2862 2023-05-22 07:24:03.000000 ppss_auth-0.9.5/ppss_auth.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dan       (1000) dan       (1000)        1 2023-05-22 07:24:03.000000 ppss_auth-0.9.5/ppss_auth.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dan       (1000) dan       (1000)      362 2023-05-22 07:24:03.000000 ppss_auth-0.9.5/ppss_auth.egg-info/entry_points.txt
+-rwxrwxrwx   0 dan       (1000) dan       (1000)       51 2023-05-22 07:24:03.000000 ppss_auth-0.9.5/ppss_auth.egg-info/requires.txt
+-rwxrwxrwx   0 dan       (1000) dan       (1000)       10 2023-05-22 07:24:03.000000 ppss_auth-0.9.5/ppss_auth.egg-info/top_level.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)     1388 2023-01-30 10:16:40.000000 ppss_auth-0.9.5/readme.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-05-22 07:24:03.716031 ppss_auth-0.9.5/setup.cfg
+-rw-r--r--   0 dan       (1000) dan       (1000)     1604 2023-05-22 07:17:45.000000 ppss_auth-0.9.5/setup.py
```

### Comparing `ppss_auth-0.9.4.4/PKG-INFO` & `ppss_auth-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppss_auth
-Version: 0.9.4.4
+Version: 0.9.5
 Summary: simple auth scheme for pyramid, based on Mako template and sqlalchemy backend
 Home-page: https://bitbucket.org/pingpongstars/ppss_auth/src/master/
 Author: pdepmcp
 Author-email: d.cariboni@pingpongstars.it
 License: MIT
 Keywords: pyramid module authentication accelerator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ppss_auth-0.9.4.4/README.md` & `ppss_auth-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/changelog.txt` & `ppss_auth-0.9.5/changelog.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## v0.9.5
+- changed default password re (min length)
+- change session id on succesful login without loosing info
+
+
 ## v0.9.1
 - http header disallowing frame incapsulation
 
 ## v0.9.0
 
 - fix to password expiration cycle
 - fix to special chars.
```

### Comparing `ppss_auth-0.9.4.4/ppss_auth/__init__.py` & `ppss_auth-0.9.5/ppss_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/alembic/alembic.ini` & `ppss_auth-0.9.5/ppss_auth/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/alembic/env.py` & `ppss_auth-0.9.5/ppss_auth/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/alembic/versions/20201026_52f4d4eefdfe_unique_permission_name.py` & `ppss_auth-0.9.5/ppss_auth/alembic/versions/20201026_52f4d4eefdfe_unique_permission_name.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/alembic/versions/20201120_6c9e84ab8280_unique_user_name.py` & `ppss_auth-0.9.5/ppss_auth/alembic/versions/20201120_6c9e84ab8280_unique_user_name.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/alembic/versions/20220329_44fde88fa438_creazione_colonne_per_login_history.py` & `ppss_auth-0.9.5/ppss_auth/alembic/versions/20220329_44fde88fa438_creazione_colonne_per_login_history.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/alembic/versions/20220331_6190d529682d_result_reason.py` & `ppss_auth-0.9.5/ppss_auth/alembic/versions/20220331_6190d529682d_result_reason.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/alembic/versions/f724fac25359_creation.py` & `ppss_auth-0.9.5/ppss_auth/alembic/versions/f724fac25359_creation.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/constants.py` & `ppss_auth-0.9.5/ppss_auth/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,17 +115,20 @@
 
         cls.forbiddentologin = settings.get("ppss_auth.forbidden_to_login", "true").lower() == 'true'
 
         
         
 
         #password enforcement
-        cls.passwordpreviousdifferent = int(settings.get("ppss_auth.password_previuos_diff","3"))
-        cls.passwordrelist = Conf.conf2list( settings.get("ppss_auth.password_relist",["[A-Z]+","[a-z]+","[0-9]+","[!,\.\?\\/;:_\-+*@\£\$\%\&\(\)\"\'=\^àèìòùé\#§°ç{}]+"]) )
-        cls.passwordwrongmessage = 'La nuova password deve essere differente dalle precedenti 3 e avere almeno una maiuscola, una minuscola, un numero e un carattere fra "!,.?\\/;:_-+*".'
+        cls.passwordpreviousdifferent = int(settings.get("ppss_auth.password_previuos_diff",3))
+        cls.passwordminlen = int(settings.get("ppss_auth.password_min_len",12))
+        cls.passwordrelist = Conf.conf2list( settings.get("ppss_auth.password_relist",["[A-Z]+","[a-z]+","[0-9]+","[!,\.\?\\/;:_\-+*@\£\$\%\&\(\)\"\'=\^àèìòùé\#§°ç{}]+",".{{{len},}}".format(len=cls.passwordminlen)]) )
+        cls.forbiddenpasswordlist = settings.get("ppss_auth.forbidden_password_list","")
+        #cls.passwordwrongmessage = f'La nuova password deve essere differente dalle precedenti {cls.passwordpreviousdifferent} e avere almeno 12 caratteri, una maiuscola, una minuscola, un numero e un carattere fra "!,.?\\/;:_-+*".'
+        cls.passwordwrongmessage = f'The new password must be different from the previous {cls.passwordpreviousdifferent} and should contain at least {cls.passwordminlen} chars, cotaining at least 1 upper case, 1 lower case, 1 number and a special char among these "!,.?\\/;:_-+*".'
         cls.passwordexpiredmessage = 'Password expired. Please change it.'
         cls.passwordexpire =  int(settings.get("ppss_auth.password_expire",0)  )
 
         cls.loginfailthreshold = int(settings.get("ppss_auth.login_fail_threshold",5)  )
         cls.loginfailinterval = int(settings.get("ppss_auth.login_fail_interval",60)  )
 
         ##template path
```

### Comparing `ppss_auth-0.9.4.4/ppss_auth/locale/en/LC_MESSAGES/ppss_auth.mo` & `ppss_auth-0.9.5/ppss_auth/locale/en/LC_MESSAGES/ppss_auth.mo`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/locale/it/LC_MESSAGES/ppss_auth.mo` & `ppss_auth-0.9.5/ppss_auth/locale/it/LC_MESSAGES/ppss_auth.mo`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/models.py` & `ppss_auth-0.9.5/ppss_auth/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,27 +265,30 @@
 
     superusercache = None
     permissionscache = None
     permissionsmapcache = None
     groupmapcache = None
 
     @classmethod
-    def checkLogin(cls,user,password,dbsession):
-        return PPSsuser.checkCryptedLogin(user,getPasswordDigest(password),dbsession)
+    def checkLogin(cls,user,password,dbsession,ipaddr = None):
+        return PPSsuser.checkCryptedLogin(user,getPasswordDigest(password),dbsession,ipaddr=ipaddr)
 
     @classmethod
-    def checkCryptedLogin(cls,user,password,dbsession):
+    def checkCryptedLogin(cls,user,password,dbsession,ipaddr = None):
         #.filter(cls.password==password).filter(cls.enabled==1)
         res = dbsession.query(cls).filter(cls.username==user) \
             .options(joinedload('groups')) \
             .options(joinedload('groups.permissions')) \
             .all()
         if len(res)==1:
             res = res[0]
-            failcount = dbsession.query(PPSsloginhistory).filter(PPSsloginhistory.user_id == res.id).filter(PPSsloginhistory.result==0).filter(PPSsloginhistory.insertdt > datetime.now()-timedelta(minutes=Conf.loginfailinterval)).count()
+            failcountquery = dbsession.query(PPSsloginhistory).filter(PPSsloginhistory.user_id == res.id).filter(PPSsloginhistory.result==0).filter(PPSsloginhistory.insertdt > datetime.now()-timedelta(minutes=Conf.loginfailinterval))
+            if ipaddr:
+                failcountquery = failcountquery.filter(PPSsloginhistory.ipaddress == ipaddr)
+            failcount = failcountquery.count()
             valid = LoginError(res.password == password, res.enabled == 1,failcount<Conf.loginfailthreshold)
             #res.password == password and res.enabled == 1
         else:
             res = None
             valid = LoginError(None,None,None)
         return res,valid
         #return res[0] if len(res)==1 else None
```

### Comparing `ppss_auth-0.9.4.4/ppss_auth/ppss_auth_static/loader.js` & `ppss_auth-0.9.5/ppss_auth/ppss_auth_static/loader.js`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/ppss_auth_static/ppssauth.css` & `ppss_auth-0.9.5/ppss_auth/ppss_auth_static/ppssauth.css`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/ppss_auth_static/ppssauth.js` & `ppss_auth-0.9.5/ppss_auth/ppss_auth_static/ppssauth.js`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/ppss_auth_static/template.html` & `ppss_auth-0.9.5/ppss_auth/ppss_auth_static/template.html`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/db.py` & `ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/db.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/password.py` & `ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/password.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .. import constants
 from .i18n import _,__
 import re
 import hashlib
 
+
 import os,datetime,logging
 l = logging.getLogger('ppssauth')
 
 class chkResult():
   def __init__(self,b,m,*args,**kwargs):
     self.b = b
     self.m = m
@@ -20,26 +21,42 @@
   def getMsg(self,request):
     if request:
       return __(request,self.m ).format(*self.args,**self.kwargs)
     else:
       return self.m.format(*self.args,**self.kwargs)
 
 def checkPassword(user,newpassword):
+  l.info("checking new password...")
   prevpasslist = user.passowrdhistory
   passworddig = getPasswordDigest(newpassword)
+  if newpassword.lower() == user.username.lower():
+    return chkResult(False,"password can not be equal to username" )
   for prevpass in prevpasslist[0:constants.Conf.passwordpreviousdifferent]:
     l.debug("\n{}\n vs \n{}".format(passworddig, prevpass.password))
     if passworddig == prevpass.password:
       l.warn("password already used on {}".format(prevpass.insertdt))
       return chkResult(False,"password already used on {}",prevpass.insertdt )
+  l.warn(f"password re list: {constants.Conf.passwordrelist}")
   for reexp in constants.Conf.passwordrelist:
+    l.info(f"checking against {reexp}")
     myre = re.compile(reexp)
     if myre.search(newpassword) is None:
-      l.info("password {} don't match constaint:{}".format(newpassword,reexp))
+      l.info("password {} doesn't match constaint:{}".format(newpassword,reexp))
       return chkResult(False, "password for user '{}' don't match constaint:{}",user.username,reexp )
+    else:
+      l.debug("password {} matches constraint:{}".format(newpassword,reexp))
+  if constants.Conf.forbiddenpasswordlist:
+    with open(constants.Conf.forbiddenpasswordlist, 'r') as fp:
+      lowernp = newpassword.lower()
+      for l_no, line in enumerate(fp):
+          # search string
+          if lowernp in line.lower():
+              l.warn("password found in forbidden list")
+              return chkResult(False, "password for user '{}' found in forbidden password list",user.username )
+              #break
   return chkResult(True,"ok")
 
 
 def getPasswordDigest(password):
   s = hashlib.sha512(password.encode('utf-8'))
   dig = s.hexdigest()
   return dig
```

### Comparing `ppss_auth-0.9.4.4/ppss_auth/ppss_auth_utils/scriptutils.py` & `ppss_auth-0.9.5/ppss_auth/ppss_auth_utils/scriptutils.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/routes.py` & `ppss_auth-0.9.5/ppss_auth/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
   config.add_route('ppss:user:changepassword', '/password/change')
   config.add_route('ppss:user:resetpassword', '/password/change/{magicnumber}')
   
   config.add_route('ppss:user:list', '/user/list')
   config.add_route('ppss:user:editself', '/user/modify/me')
   config.add_route('ppss:user:edit', '/user/modify/{elementid}')
   config.add_route('ppss:user:search', '/user/search/')
+  config.add_route('ppss:user:remove', '/user/remove/{userid}/{groupid}')
+  config.add_route('ppss:user:checkpassword', '/user/checkpassword/{userid}')
 
   config.add_route('ppss:group:list', '/group/list')
   config.add_route('ppss:group:edit', '/group/modify/{elementid}')
   
   config.add_route('ppss:group:removeuser', '/group/removeuser/{elementid}/{targetid}')
   config.add_route('ppss:group:adduser', '/group/adduser/{elementid}/{targetid}')
   config.add_route('ppss:group:removeperm', '/group/removeperm/{elementid}/{targetid}')
@@ -30,16 +32,15 @@
   config.add_route('ppss:group:search', '/group/search/')
 
   config.add_route('ppss:perm:list',   '/perm/list')
   config.add_route('ppss:perm:edit',   '/perm/modify/{elementid}')
   config.add_route('ppss:perm:delete', '/perm/delete/{elementid}')
   config.add_route('ppss:perm:search', '/perm/search/')
 
-  config.add_route('ppss:user:remove', '/user/remove/{userid}/{groupid}')
-  config.add_route('ppss:user:checkpassword', '/user/checkpassword/{userid}')
+  
 
   config.add_route('test:test',Conf.testurl)
 
 
   config.add_route('oauth:callback',"/oauth/callback")
 
   ########views
```

### Comparing `ppss_auth-0.9.4.4/ppss_auth/scripts/alchemyutils.py` & `ppss_auth-0.9.5/ppss_auth/scripts/alchemyutils.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/scripts/cleanup_db.py` & `ppss_auth-0.9.5/ppss_auth/scripts/cleanup_db.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/scripts/create_user.py` & `ppss_auth-0.9.5/ppss_auth/scripts/create_user.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/scripts/initialize_db.py` & `ppss_auth-0.9.5/ppss_auth/scripts/initialize_db.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/scripts/upgrade_db.py` & `ppss_auth-0.9.5/ppss_auth/scripts/upgrade_db.py`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/change.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/change.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/change.mako` & `ppss_auth-0.9.5/ppss_auth/templates/change.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/editgroup.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/editgroup.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/editgroup.mako` & `ppss_auth-0.9.5/ppss_auth/templates/editgroup.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/editperm.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/editperm.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/editperm.mako` & `ppss_auth-0.9.5/ppss_auth/templates/editperm.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/edituser.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/edituser.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/edituser.mako` & `ppss_auth-0.9.5/ppss_auth/templates/edituser.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/layouts/masterlayout.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/layouts/masterlayout.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/layouts/masterlayout.mako` & `ppss_auth-0.9.5/ppss_auth/templates/layouts/masterlayout.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/layouts/midlayout.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/layouts/midlayout.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/layouts/midlayout.mako` & `ppss_auth-0.9.5/ppss_auth/templates/layouts/midlayout.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/listgroup.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/listgroup.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/listgroup.mako` & `ppss_auth-0.9.5/ppss_auth/templates/listgroup.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/listperm.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/listperm.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/listperm.mako` & `ppss_auth-0.9.5/ppss_auth/templates/listperm.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/listuser.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/listuser.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/listuser.mako` & `ppss_auth-0.9.5/ppss_auth/templates/listuser.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/login.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/login.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/login.mako` & `ppss_auth-0.9.5/ppss_auth/templates/login.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/login_nogrid.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/login_nogrid.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/login_nogrid.mako` & `ppss_auth-0.9.5/ppss_auth/templates/login_nogrid.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/partials/userblock.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/partials/userblock.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/partials/userblock.mako` & `ppss_auth-0.9.5/ppss_auth/templates/partials/userblock.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/registeruser.jinja2` & `ppss_auth-0.9.5/ppss_auth/templates/registeruser.jinja2`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/templates/registeruser.mako` & `ppss_auth-0.9.5/ppss_auth/templates/registeruser.mako`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/ppss_auth/views/auth.py` & `ppss_auth-0.9.5/ppss_auth/views/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,28 +177,33 @@
         if r.POST:
             username = r.params.get("username",u"")
             password = r.params.get("password",u"")
             superuser = False
             res = None
             l.info("Login attempt: u={username}".format(username=username))
             if res is None:
-                res,valid = PPSsuser.checkLogin(username,password,r.dbsession)
+                res,valid = PPSsuser.checkLogin(username,password,r.dbsession,ipaddr = self.request.remote_addr)
                 self.logloginattempt(res,valid,username)
             if res and valid:
                 res.getPermissionsMap()
-                self.setPrincipalsInSession(res,superuser,res.passwordExpired())
+                sessionvals = self.getSessionVals(self.setPrincipalsInSession(res,superuser,res.passwordExpired()))                
                 r.dbsession.expunge(res)
+                l.info(f"session keys:{sessionvals}")
+
 
                 ## log the last login
                 llogin = PPSsuser.byId(res.id,r.dbsession)
                 llogin.lastlogin = datetime.datetime.now()  
                 l.debug("last login:{}".format(llogin.lastlogin))
-
+                r.session.invalidate()
+                
+                r.session.update(sessionvals)                
                 r.session[Conf.sessionuser] = {'id':res.id,'name':username,'user':res}
                 headers = remember(r, res.id)
+                r.session.save()
                 if res.passwordExpired(): 
                     return HTTPFound(r.route_url("ppss:user:changepassword"))
                 return HTTPFound(postloginpage,headers=headers)
             #wrong password or disabled user
             
             l.warn("Login attempt failed for user {user}".format(user=username))
             if valid.blocked():
@@ -320,15 +325,20 @@
             r.session['admin'] = True
             r.session['principals'] = ["g:admin","g:sysadmin"]
         else:
             r.session['principals'] = user.getPrincipals(passwordExpired) 
             r.session['admin'] = False
         l.info("permissions for {}({},{}):{}".format(user.username,isSuperUser,passwordExpired,r.session['principals'])  )
         r.session.changed()
+        return r.session
 
+    def getSessionVals(self,session,all=False):
+        allvals = {k:session.get(k) for k in session.keys() if (not k.startswith("_")) or all }
+        l.debug(f"all session vals:{allvals}")
+        return allvals
 
     def listUser(self):
         elements = self.request.dbsession.query(PPSsuser).all()
         retdict = {'elements':elements}
         retdict.update(self.retdict)
         return retdict
 
@@ -424,15 +434,15 @@
                         retdict['msg'] = __(self.request,"Password updated.")
                         canenable = True
                     else:
                         retdict['msg'] = res.getMsg(self.request)
                         #__(self.request,"New password doesn't match constraints." )
                 else:
                     retdict['msg'] = __(self.request,"New password doesn't match confirmation field.")
-            user.enabled = 1 if self.request.params.get("enabled")=="1" and canenable else 0
+            user.enabled = 1 if self.request.params.get("enabled")=="1" and canenable and user.password else 0
             
             groups=map(int,self.request.params.getall("allgroups"))
             l.debug("group={groups}".format(groups=groups ))
             usergroups = [PPSsgroup.byId(groupid,self.request.dbsession) for groupid in groups if groupid in set([g.id for g in editablegroups ])]
             user.groups = usergroups
             self.request.dbsession.flush()
             #return HTTPFound(self.request.route_url('ppss:user:edit',elementid = user.id) )
```

### Comparing `ppss_auth-0.9.4.4/ppss_auth.egg-info/PKG-INFO` & `ppss_auth-0.9.5/ppss_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppss-auth
-Version: 0.9.4.4
+Version: 0.9.5
 Summary: simple auth scheme for pyramid, based on Mako template and sqlalchemy backend
 Home-page: https://bitbucket.org/pingpongstars/ppss_auth/src/master/
 Author: pdepmcp
 Author-email: d.cariboni@pingpongstars.it
 License: MIT
 Keywords: pyramid module authentication accelerator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ppss_auth-0.9.4.4/ppss_auth.egg-info/SOURCES.txt` & `ppss_auth-0.9.5/ppss_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/readme.txt` & `ppss_auth-0.9.5/readme.txt`

 * *Files identical despite different names*

### Comparing `ppss_auth-0.9.4.4/setup.py` & `ppss_auth-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 here = os.path.abspath(os.path.dirname(__file__))
 readme = open(os.path.join(here, 'README.md'), 'r').read()
 changelog = open(os.path.join(here, 'README.md'), 'r').read()
 
 setup(name='ppss_auth',
-  version='0.9.4.4',
+  version='0.9.5',
   description='simple auth scheme for pyramid, based on Mako template and sqlalchemy backend',
   long_description=readme + "\n\n\n" + changelog,
   long_description_content_type="text/markdown",
   author='pdepmcp',
   author_email='d.cariboni@pingpongstars.it',
   license='MIT',
   classifiers=[
```

