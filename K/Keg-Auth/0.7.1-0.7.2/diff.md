# Comparing `tmp/Keg-Auth-0.7.1.tar.gz` & `tmp/Keg-Auth-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Keg-Auth-0.7.1.tar", last modified: Fri May 12 19:13:23 2023, max compression
+gzip compressed data, was "Keg-Auth-0.7.2.tar", last modified: Mon May 22 17:08:07 2023, max compression
```

## Comparing `Keg-Auth-0.7.1.tar` & `Keg-Auth-0.7.2.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.798739 Keg-Auth-0.7.1/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.698738 Keg-Auth-0.7.1/.circleci/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1003 2023-05-12 19:12:13.000000 Keg-Auth-0.7.1/.circleci/config.yml
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/.circleci/pytest.ini
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.698738 Keg-Auth-0.7.1/Keg_Auth.egg-info/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19716 2023-05-12 19:13:22.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2754 2023-05-12 19:13:23.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/SOURCES.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-12 19:13:22.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/dependency_links.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2018-06-26 19:41:44.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/not-zip-safe
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      439 2023-05-12 19:13:23.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/requires.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       21 2023-05-12 19:13:23.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/top_level.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      664 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/MANIFEST.in
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19716 2023-05-12 19:13:23.798739 Keg-Auth-0.7.1/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    17004 2023-05-12 19:13:02.000000 Keg-Auth-0.7.1/changelog.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      453 2021-11-29 16:34:48.000000 Keg-Auth-0.7.1/docker-compose.yml
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.702738 Keg-Auth-0.7.1/docs/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      638 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/Makefile
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      799 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/make.bat
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       71 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/docs/requirements.txt
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.714738 Keg-Auth-0.7.1/docs/source/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2579 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/conf.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/core.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/forms.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    25041 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/docs/source/getting-started.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/grids.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      286 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/docs/source/index.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.722739 Keg-Auth-0.7.1/docs/source/libs/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       90 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/libs/authenticators.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       78 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/libs/decorators.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      141 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/libs/index.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       78 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/libs/navigation.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/mail.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.722739 Keg-Auth-0.7.1/docs/source/model/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       94 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/model/entity_registry.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      129 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/model/index.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/model/utils.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/testing.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      866 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/docs/source/upgrade.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/views.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.738739 Keg-Auth-0.7.1/keg_auth/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      932 2022-02-24 20:26:39.000000 Keg-Auth-0.7.1/keg_auth/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4355 2021-07-06 19:42:05.000000 Keg-Auth-0.7.1/keg_auth/cli.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19831 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/core.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1064 2020-04-02 13:20:21.000000 Keg-Auth-0.7.1/keg_auth/extensions.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10715 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/forms.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11025 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/keg_auth/grids.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.738739 Keg-Auth-0.7.1/keg_auth/i18n/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      113 2018-11-14 17:28:05.000000 Keg-Auth-0.7.1/keg_auth/i18n/babel.cfg
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.742739 Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7041 2020-12-08 20:35:04.000000 Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/keg_auth.mo
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11072 2020-12-08 20:35:04.000000 Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/keg_auth.po
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7561 2020-12-08 20:35:04.000000 Keg-Auth-0.7.1/keg_auth/i18n/keg_auth.pot
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.750739 Keg-Auth-0.7.1/keg_auth/libs/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1013 2022-02-24 20:26:39.000000 Keg-Auth-0.7.1/keg_auth/libs/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    45971 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/libs/authenticators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9900 2023-05-12 19:12:13.000000 Keg-Auth-0.7.1/keg_auth/libs/decorators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9648 2022-02-22 19:50:15.000000 Keg-Auth-0.7.1/keg_auth/libs/navigation.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      404 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/keg_auth/libs/templates.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2527 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/mail.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.754739 Keg-Auth-0.7.1/keg_auth/model/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    28459 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/model/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3901 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/keg_auth/model/entity_registry.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      226 2020-04-16 20:22:57.000000 Keg-Auth-0.7.1/keg_auth/model/types.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2474 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/keg_auth/model/utils.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/static/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/static/i18n/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/static/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.758739 Keg-Auth-0.7.1/keg_auth/static/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6521 2020-12-08 20:35:04.000000 Keg-Auth-0.7.1/keg_auth/static/i18n/es/LC_MESSAGES/keg_auth.json
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/templates/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.770739 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      488 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/crud-addedit.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1084 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/crud-list.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      149 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/flash-messages-only.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      369 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/forgot-password.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/i18n.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      453 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/login.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      254 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/multi-part-mail.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1842 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/navigation.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      576 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/new-user-mail.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      624 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/reset-password-mail.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      270 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/set-password.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    58303 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/testing.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.782739 Keg-Auth-0.7.1/keg_auth/tests/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/keg_auth/tests/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      639 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/tests/conftest.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4718 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_auth_manager.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    22575 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/tests/test_authenticators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7666 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/tests/test_cli.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1259 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_core.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    12787 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/tests/test_forms.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2055 2019-06-07 16:29:38.000000 Keg-Auth-0.7.1/keg_auth/tests/test_grids.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2768 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_mail.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    30106 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_model.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    18022 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_navigation.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      187 2022-02-24 20:26:39.000000 Keg-Auth-0.7.1/keg_auth/tests/test_utils.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    59313 2023-05-12 19:12:13.000000 Keg-Auth-0.7.1/keg_auth/tests/test_views.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2201 2022-02-24 20:26:39.000000 Keg-Auth-0.7.1/keg_auth/tests/utils.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-05-12 19:12:32.000000 Keg-Auth-0.7.1/keg_auth/version.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26051 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/views.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.790739 Keg-Auth-0.7.1/keg_auth_ta/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/keg_auth_ta/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      950 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/app.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1119 2020-05-14 15:15:43.000000 Keg-Auth-0.7.1/keg_auth_ta/cli.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      987 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/config.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      986 2022-02-22 19:50:15.000000 Keg-Auth-0.7.1/keg_auth_ta/events.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      802 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/extensions.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      174 2018-08-17 20:04:26.000000 Keg-Auth-0.7.1/keg_auth_ta/grids.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.790739 Keg-Auth-0.7.1/keg_auth_ta/model/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/keg_auth_ta/model/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1526 2020-12-08 18:33:59.000000 Keg-Auth-0.7.1/keg_auth_ta/model/entities.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.794739 Keg-Auth-0.7.1/keg_auth_ta/templates/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      813 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/templates/base-page.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      508 2021-02-02 19:57:35.000000 Keg-Auth-0.7.1/keg_auth_ta/templates/base.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      158 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/templates/email.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      442 2018-08-17 20:04:26.000000 Keg-Auth-0.7.1/keg_auth_ta/templates/home.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6999 2023-05-12 19:12:13.000000 Keg-Auth-0.7.1/keg_auth_ta/views.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      316 2021-11-29 16:34:48.000000 Keg-Auth-0.7.1/keg_auth_ta-config-example.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2141 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/readme.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      655 2023-05-12 19:13:23.798739 Keg-Auth-0.7.1/setup.cfg
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2306 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/setup.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2974 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/todo.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2036 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/tox.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.875892 Keg-Auth-0.7.2/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.839888 Keg-Auth-0.7.2/.circleci/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1003 2023-05-12 19:12:13.000000 Keg-Auth-0.7.2/.circleci/config.yml
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.2/.circleci/pytest.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.839888 Keg-Auth-0.7.2/Keg_Auth.egg-info/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19941 2023-05-22 17:08:07.000000 Keg-Auth-0.7.2/Keg_Auth.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2754 2023-05-22 17:08:07.000000 Keg-Auth-0.7.2/Keg_Auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-22 17:08:07.000000 Keg-Auth-0.7.2/Keg_Auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2018-06-26 19:41:44.000000 Keg-Auth-0.7.2/Keg_Auth.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      439 2023-05-22 17:08:07.000000 Keg-Auth-0.7.2/Keg_Auth.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       21 2023-05-22 17:08:07.000000 Keg-Auth-0.7.2/Keg_Auth.egg-info/top_level.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      664 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/MANIFEST.in
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19941 2023-05-22 17:08:07.875892 Keg-Auth-0.7.2/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    17229 2023-05-22 17:07:47.000000 Keg-Auth-0.7.2/changelog.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      453 2021-11-29 16:34:48.000000 Keg-Auth-0.7.2/docker-compose.yml
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.839888 Keg-Auth-0.7.2/docs/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      638 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/Makefile
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      799 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/make.bat
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       71 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/docs/requirements.txt
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.847889 Keg-Auth-0.7.2/docs/source/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2579 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/conf.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/core.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/forms.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    25041 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/docs/source/getting-started.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/grids.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      286 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/docs/source/index.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.851889 Keg-Auth-0.7.2/docs/source/libs/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       90 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/libs/authenticators.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       78 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/libs/decorators.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      141 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/libs/index.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       78 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/libs/navigation.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/mail.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.851889 Keg-Auth-0.7.2/docs/source/model/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       94 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/model/entity_registry.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      129 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/model/index.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/model/utils.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/testing.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      866 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/docs/source/upgrade.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/docs/source/views.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.855890 Keg-Auth-0.7.2/keg_auth/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      932 2022-02-24 20:26:39.000000 Keg-Auth-0.7.2/keg_auth/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4355 2021-07-06 19:42:05.000000 Keg-Auth-0.7.2/keg_auth/cli.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    20827 2023-05-22 17:07:01.000000 Keg-Auth-0.7.2/keg_auth/core.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1064 2020-04-02 13:20:21.000000 Keg-Auth-0.7.2/keg_auth/extensions.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10715 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/forms.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11025 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/keg_auth/grids.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.859890 Keg-Auth-0.7.2/keg_auth/i18n/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      113 2018-11-14 17:28:05.000000 Keg-Auth-0.7.2/keg_auth/i18n/babel.cfg
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.827886 Keg-Auth-0.7.2/keg_auth/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.859890 Keg-Auth-0.7.2/keg_auth/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7041 2020-12-08 20:35:04.000000 Keg-Auth-0.7.2/keg_auth/i18n/es/LC_MESSAGES/keg_auth.mo
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11072 2020-12-08 20:35:04.000000 Keg-Auth-0.7.2/keg_auth/i18n/es/LC_MESSAGES/keg_auth.po
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7561 2020-12-08 20:35:04.000000 Keg-Auth-0.7.2/keg_auth/i18n/keg_auth.pot
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.859890 Keg-Auth-0.7.2/keg_auth/libs/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1013 2022-02-24 20:26:39.000000 Keg-Auth-0.7.2/keg_auth/libs/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    45971 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/keg_auth/libs/authenticators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9900 2023-05-12 19:12:13.000000 Keg-Auth-0.7.2/keg_auth/libs/decorators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9648 2022-02-22 19:50:15.000000 Keg-Auth-0.7.2/keg_auth/libs/navigation.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      404 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/keg_auth/libs/templates.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2527 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/mail.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.863891 Keg-Auth-0.7.2/keg_auth/model/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    28459 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/keg_auth/model/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3901 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/keg_auth/model/entity_registry.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      226 2020-04-16 20:22:57.000000 Keg-Auth-0.7.2/keg_auth/model/types.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2474 2021-01-29 21:02:21.000000 Keg-Auth-0.7.2/keg_auth/model/utils.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.827886 Keg-Auth-0.7.2/keg_auth/static/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.827886 Keg-Auth-0.7.2/keg_auth/static/i18n/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.827886 Keg-Auth-0.7.2/keg_auth/static/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.863891 Keg-Auth-0.7.2/keg_auth/static/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6521 2020-12-08 20:35:04.000000 Keg-Auth-0.7.2/keg_auth/static/i18n/es/LC_MESSAGES/keg_auth.json
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.827886 Keg-Auth-0.7.2/keg_auth/templates/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.863891 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      488 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/crud-addedit.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1084 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/crud-list.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      149 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/flash-messages-only.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      369 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/forgot-password.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/i18n.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      453 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/login.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      254 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/multi-part-mail.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1842 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/navigation.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      576 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/new-user-mail.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      624 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/reset-password-mail.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      270 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/templates/keg-auth/set-password.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    58303 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/keg_auth/testing.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.867891 Keg-Auth-0.7.2/keg_auth/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.2/keg_auth/tests/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      639 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/keg_auth/tests/conftest.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4718 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/tests/test_auth_manager.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    22575 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/keg_auth/tests/test_authenticators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7666 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/keg_auth/tests/test_cli.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1259 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/tests/test_core.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    12787 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/keg_auth/tests/test_forms.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2055 2019-06-07 16:29:38.000000 Keg-Auth-0.7.2/keg_auth/tests/test_grids.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2768 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/tests/test_mail.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    30106 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/tests/test_model.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    18022 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth/tests/test_navigation.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      187 2022-02-24 20:26:39.000000 Keg-Auth-0.7.2/keg_auth/tests/test_utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    59313 2023-05-12 19:12:13.000000 Keg-Auth-0.7.2/keg_auth/tests/test_views.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2201 2022-02-24 20:26:39.000000 Keg-Auth-0.7.2/keg_auth/tests/utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-05-22 17:07:20.000000 Keg-Auth-0.7.2/keg_auth/version.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26051 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/keg_auth/views.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.871892 Keg-Auth-0.7.2/keg_auth_ta/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.2/keg_auth_ta/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      950 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth_ta/app.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1119 2020-05-14 15:15:43.000000 Keg-Auth-0.7.2/keg_auth_ta/cli.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      987 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth_ta/config.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      986 2022-02-22 19:50:15.000000 Keg-Auth-0.7.2/keg_auth_ta/events.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      802 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth_ta/extensions.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      174 2018-08-17 20:04:26.000000 Keg-Auth-0.7.2/keg_auth_ta/grids.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.871892 Keg-Auth-0.7.2/keg_auth_ta/model/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.2/keg_auth_ta/model/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1526 2020-12-08 18:33:59.000000 Keg-Auth-0.7.2/keg_auth_ta/model/entities.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:08:07.875892 Keg-Auth-0.7.2/keg_auth_ta/templates/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      813 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth_ta/templates/base-page.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      508 2021-02-02 19:57:35.000000 Keg-Auth-0.7.2/keg_auth_ta/templates/base.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      158 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/keg_auth_ta/templates/email.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      442 2018-08-17 20:04:26.000000 Keg-Auth-0.7.2/keg_auth_ta/templates/home.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6999 2023-05-12 19:12:13.000000 Keg-Auth-0.7.2/keg_auth_ta/views.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      316 2021-11-29 16:34:48.000000 Keg-Auth-0.7.2/keg_auth_ta-config-example.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2141 2023-03-03 20:33:36.000000 Keg-Auth-0.7.2/readme.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      655 2023-05-22 17:08:07.875892 Keg-Auth-0.7.2/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2306 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/setup.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2974 2018-06-22 16:02:06.000000 Keg-Auth-0.7.2/todo.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2036 2023-03-03 21:07:57.000000 Keg-Auth-0.7.2/tox.ini
```

### Comparing `Keg-Auth-0.7.1/.circleci/config.yml` & `Keg-Auth-0.7.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/Keg_Auth.egg-info/PKG-INFO` & `Keg-Auth-0.7.2/Keg_Auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Keg-Auth
-Version: 0.7.1
+Version: 0.7.2
 Summary: Authentication plugin for Keg
 Home-page: https://github.com/level12/keg-auth
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -84,14 +84,22 @@
 - `cd keg_auth_ta`
 - `python app.py ...`
 
 
 Changelog
 =========
 
+0.7.2 released 2023-05-22
+-------------------------
+
+- handle multiple potential session cookies resulting from werkzeug 2.3 and flask 2.3 changes (8b4680e_)
+
+.. _8b4680e: https://github.com/level12/keg-auth/commit/8b4680e
+
+
 0.7.1 released 2023-05-12
 -------------------------
 
 - allow request loaders to be specified directly to requires decorators (cd42358_)
 
 .. _cd42358: https://github.com/level12/keg-auth/commit/cd42358
```

### Comparing `Keg-Auth-0.7.1/Keg_Auth.egg-info/SOURCES.txt` & `Keg-Auth-0.7.2/Keg_Auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/MANIFEST.in` & `Keg-Auth-0.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/PKG-INFO` & `Keg-Auth-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Keg-Auth
-Version: 0.7.1
+Version: 0.7.2
 Summary: Authentication plugin for Keg
 Home-page: https://github.com/level12/keg-auth
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -84,14 +84,22 @@
 - `cd keg_auth_ta`
 - `python app.py ...`
 
 
 Changelog
 =========
 
+0.7.2 released 2023-05-22
+-------------------------
+
+- handle multiple potential session cookies resulting from werkzeug 2.3 and flask 2.3 changes (8b4680e_)
+
+.. _8b4680e: https://github.com/level12/keg-auth/commit/8b4680e
+
+
 0.7.1 released 2023-05-12
 -------------------------
 
 - allow request loaders to be specified directly to requires decorators (cd42358_)
 
 .. _cd42358: https://github.com/level12/keg-auth/commit/cd42358
```

### Comparing `Keg-Auth-0.7.1/changelog.rst` & `Keg-Auth-0.7.2/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.7.2 released 2023-05-22
+-------------------------
+
+- handle multiple potential session cookies resulting from werkzeug 2.3 and flask 2.3 changes (8b4680e_)
+
+.. _8b4680e: https://github.com/level12/keg-auth/commit/8b4680e
+
+
 0.7.1 released 2023-05-12
 -------------------------
 
 - allow request loaders to be specified directly to requires decorators (cd42358_)
 
 .. _cd42358: https://github.com/level12/keg-auth/commit/cd42358
```

### Comparing `Keg-Auth-0.7.1/docs/Makefile` & `Keg-Auth-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/docs/make.bat` & `Keg-Auth-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/docs/source/conf.py` & `Keg-Auth-0.7.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/docs/source/getting-started.rst` & `Keg-Auth-0.7.2/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/docs/source/upgrade.rst` & `Keg-Auth-0.7.2/docs/source/upgrade.rst`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/__init__.py` & `Keg-Auth-0.7.2/keg_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/cli.py` & `Keg-Auth-0.7.2/keg_auth/cli.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/core.py` & `Keg-Auth-0.7.2/keg_auth/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -433,10 +433,36 @@
 
 
 def clear_session(app, user):
     if app.config.get('KEGAUTH_LOGOUT_CLEAR_SESSION'):
         flask.session.clear()
 
 
+def fix_session_cookies(app, **extra):
+    cookie_values = flask.request.cookies.getlist(
+        app.config.get('SESSION_COOKIE_NAME')
+    )
+    server_name = app.config.get('SERVER_NAME')
+    if len(cookie_values) > 1 and server_name:
+        # werkzeug update has breaking session, since it matches both
+        # and doesn't remove the old value...
+
+        # chop off the port which is usually not supported by browsers
+        cookie_domain = server_name.rsplit(':', 1)[0].lstrip('.')
+        if flask.helpers.is_ip(cookie_domain):
+            return
+
+        cookie_domain = '.' + cookie_domain
+
+        # old werkzeug before 2.3 put a leading dot, new does not. Delete
+        # the old cookie.
+        resp = flask.redirect(flask.request.url)
+        resp.delete_cookie(app.config.get('SESSION_COOKIE_NAME'), domain=cookie_domain)
+
+        # redirect to the same page, so the proper cookie value gets loaded
+        flask.abort(resp)
+
+
 flask_login.signals.user_logged_in.connect(on_login)
 flask_login.signals.user_logged_out.connect(refresh_session_menus)
 flask_login.signals.user_logged_out.connect(clear_session)
+flask.request_started.connect(fix_session_cookies)
```

### Comparing `Keg-Auth-0.7.1/keg_auth/extensions.py` & `Keg-Auth-0.7.2/keg_auth/extensions.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/forms.py` & `Keg-Auth-0.7.2/keg_auth/forms.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/grids.py` & `Keg-Auth-0.7.2/keg_auth/grids.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/keg_auth.mo` & `Keg-Auth-0.7.2/keg_auth/i18n/es/LC_MESSAGES/keg_auth.mo`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/keg_auth.po` & `Keg-Auth-0.7.2/keg_auth/i18n/es/LC_MESSAGES/keg_auth.po`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/i18n/keg_auth.pot` & `Keg-Auth-0.7.2/keg_auth/i18n/keg_auth.pot`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/libs/__init__.py` & `Keg-Auth-0.7.2/keg_auth/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/libs/authenticators.py` & `Keg-Auth-0.7.2/keg_auth/libs/authenticators.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/libs/decorators.py` & `Keg-Auth-0.7.2/keg_auth/libs/decorators.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/libs/navigation.py` & `Keg-Auth-0.7.2/keg_auth/libs/navigation.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/mail.py` & `Keg-Auth-0.7.2/keg_auth/mail.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/model/__init__.py` & `Keg-Auth-0.7.2/keg_auth/model/__init__.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/model/entity_registry.py` & `Keg-Auth-0.7.2/keg_auth/model/entity_registry.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/model/utils.py` & `Keg-Auth-0.7.2/keg_auth/model/utils.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/static/i18n/es/LC_MESSAGES/keg_auth.json` & `Keg-Auth-0.7.2/keg_auth/static/i18n/es/LC_MESSAGES/keg_auth.json`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/templates/keg-auth/crud-list.html` & `Keg-Auth-0.7.2/keg_auth/templates/keg-auth/crud-list.html`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/templates/keg-auth/navigation.html` & `Keg-Auth-0.7.2/keg_auth/templates/keg-auth/navigation.html`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/templates/keg-auth/new-user-mail.j2` & `Keg-Auth-0.7.2/keg_auth/templates/keg-auth/new-user-mail.j2`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/templates/keg-auth/reset-password-mail.j2` & `Keg-Auth-0.7.2/keg_auth/templates/keg-auth/reset-password-mail.j2`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/testing.py` & `Keg-Auth-0.7.2/keg_auth/testing.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/conftest.py` & `Keg-Auth-0.7.2/keg_auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_auth_manager.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_auth_manager.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_authenticators.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_authenticators.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_cli.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_core.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_forms.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_grids.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_grids.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_mail.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_model.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_navigation.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_navigation.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/test_views.py` & `Keg-Auth-0.7.2/keg_auth/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/tests/utils.py` & `Keg-Auth-0.7.2/keg_auth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth/views.py` & `Keg-Auth-0.7.2/keg_auth/views.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth_ta/app.py` & `Keg-Auth-0.7.2/keg_auth_ta/app.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth_ta/cli.py` & `Keg-Auth-0.7.2/keg_auth_ta/cli.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth_ta/config.py` & `Keg-Auth-0.7.2/keg_auth_ta/config.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth_ta/events.py` & `Keg-Auth-0.7.2/keg_auth_ta/events.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth_ta/extensions.py` & `Keg-Auth-0.7.2/keg_auth_ta/extensions.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth_ta/model/entities.py` & `Keg-Auth-0.7.2/keg_auth_ta/model/entities.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth_ta/templates/base-page.html` & `Keg-Auth-0.7.2/keg_auth_ta/templates/base-page.html`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/keg_auth_ta/views.py` & `Keg-Auth-0.7.2/keg_auth_ta/views.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/readme.rst` & `Keg-Auth-0.7.2/readme.rst`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/setup.cfg` & `Keg-Auth-0.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/setup.py` & `Keg-Auth-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/todo.txt` & `Keg-Auth-0.7.2/todo.txt`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.1/tox.ini` & `Keg-Auth-0.7.2/tox.ini`

 * *Files identical despite different names*

