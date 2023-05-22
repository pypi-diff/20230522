# Comparing `tmp/KegElements-0.9.0.tar.gz` & `tmp/KegElements-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KegElements-0.9.0.tar", last modified: Fri Mar  3 20:15:17 2023, max compression
+gzip compressed data, was "KegElements-0.9.1.tar", last modified: Mon May 22 17:57:59 2023, max compression
```

## Comparing `KegElements-0.9.0.tar` & `KegElements-0.9.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.031174 KegElements-0.9.0/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.015174 KegElements-0.9.0/.ci/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       15 2018-11-13 17:40:23.000000 KegElements-0.9.0/.ci/.gitignore
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      809 2022-12-12 15:57:35.000000 KegElements-0.9.0/.ci/pytest.ini
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.015174 KegElements-0.9.0/.circleci/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2287 2022-12-12 15:57:35.000000 KegElements-0.9.0/.circleci/config.yml
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      122 2021-01-29 21:07:39.000000 KegElements-0.9.0/.gitignore
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      439 2022-12-12 15:57:35.000000 KegElements-0.9.0/.pre-commit-config.yaml
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.015174 KegElements-0.9.0/KegElements.egg-info/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    21018 2023-03-03 20:15:16.000000 KegElements-0.9.0/KegElements.egg-info/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2722 2023-03-03 20:15:16.000000 KegElements-0.9.0/KegElements.egg-info/SOURCES.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-03-03 20:15:16.000000 KegElements-0.9.0/KegElements.egg-info/dependency_links.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2018-11-13 21:38:47.000000 KegElements-0.9.0/KegElements.egg-info/not-zip-safe
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      267 2023-03-03 20:15:16.000000 KegElements-0.9.0/KegElements.egg-info/requires.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       23 2023-03-03 20:15:16.000000 KegElements-0.9.0/KegElements.egg-info/top_level.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       76 2018-11-13 17:40:23.000000 KegElements-0.9.0/MANIFEST.in
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    21018 2023-03-03 20:15:17.031174 KegElements-0.9.0/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    18451 2023-03-03 20:15:02.000000 KegElements-0.9.0/changelog.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.019174 KegElements-0.9.0/keg_elements/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        6 2018-11-13 17:40:23.000000 KegElements-0.9.0/keg_elements/.gitignore
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       92 2021-02-02 19:04:40.000000 KegElements-0.9.0/keg_elements/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      432 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/conftest.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      108 2018-11-13 17:40:23.000000 KegElements-0.9.0/keg_elements/core.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     8742 2021-02-02 19:04:40.000000 KegElements-0.9.0/keg_elements/crypto.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.019174 KegElements-0.9.0/keg_elements/db/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.0/keg_elements/db/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3558 2021-02-02 19:04:40.000000 KegElements-0.9.0/keg_elements/db/columns.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3851 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/db/migrations.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    25756 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/db/mixins.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10163 2021-09-10 20:06:34.000000 KegElements-0.9.0/keg_elements/db/utils.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      862 2018-11-13 17:40:23.000000 KegElements-0.9.0/keg_elements/decorators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      440 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/encoding.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      982 2018-11-13 21:33:50.000000 KegElements-0.9.0/keg_elements/extensions.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.019174 KegElements-0.9.0/keg_elements/forms/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    35660 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/forms/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2147 2020-03-20 14:24:02.000000 KegElements-0.9.0/keg_elements/forms/state_field.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3539 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/forms/validators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      889 2018-11-13 21:33:50.000000 KegElements-0.9.0/keg_elements/http.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.019174 KegElements-0.9.0/keg_elements/i18n/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/i18n/babel.cfg
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.003174 KegElements-0.9.0/keg_elements/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.019174 KegElements-0.9.0/keg_elements/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2627 2022-12-07 20:09:09.000000 KegElements-0.9.0/keg_elements/i18n/es/LC_MESSAGES/keg_elements.mo
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3749 2022-12-07 20:09:09.000000 KegElements-0.9.0/keg_elements/i18n/es/LC_MESSAGES/keg_elements.po
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2573 2022-12-07 20:09:09.000000 KegElements-0.9.0/keg_elements/i18n/keg_elements.pot
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     8009 2021-02-02 19:04:40.000000 KegElements-0.9.0/keg_elements/sentry.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.003174 KegElements-0.9.0/keg_elements/templates/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.023174 KegElements-0.9.0/keg_elements/templates/keg-elements/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      940 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/templates/keg-elements/form-view.html
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.023174 KegElements-0.9.0/keg_elements/templates/keg-elements/forms/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5984 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/templates/keg-elements/forms/datetime-helper.js
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10037 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/templates/keg-elements/forms/horizontal-b3.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11682 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/templates/keg-elements/forms/horizontal-b4.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5456 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/templates/keg-elements/forms/horizontal-static.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      193 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/templates/keg-elements/forms/select2-scripts.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      106 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/templates/keg-elements/forms/select2-styles.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      971 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/templates/keg-elements/grid-view.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    13092 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/testing.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.027174 KegElements-0.9.0/keg_elements/tests/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.0/keg_elements/tests/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4121 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/tests/test_columns.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7725 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/tests/test_crypto.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6423 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/tests/test_db_migrations.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    17932 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/tests/test_db_mixins.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    12725 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/tests/test_db_utils.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1560 2018-11-13 17:40:23.000000 KegElements-0.9.0/keg_elements/tests/test_decorators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      394 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/tests/test_encoding.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.027174 KegElements-0.9.0/keg_elements/tests/test_forms/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.0/keg_elements/tests/test_forms/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    43444 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/tests/test_forms/test_form.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2291 2020-03-20 14:24:02.000000 KegElements-0.9.0/keg_elements/tests/test_forms/test_state_field.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4316 2021-09-10 20:06:34.000000 KegElements-0.9.0/keg_elements/tests/test_forms/test_validators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    13537 2020-09-21 14:19:34.000000 KegElements-0.9.0/keg_elements/tests/test_sentry.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9499 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/tests/test_templates.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3141 2021-09-10 20:06:34.000000 KegElements-0.9.0/keg_elements/tests/test_testing.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.027174 KegElements-0.9.0/keg_elements/tests/test_views/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2021-09-10 20:06:34.000000 KegElements-0.9.0/keg_elements/tests/test_views/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3440 2023-03-03 20:13:24.000000 KegElements-0.9.0/keg_elements/tests/test_views/test_views.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-03-03 20:13:47.000000 KegElements-0.9.0/keg_elements/version.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5555 2022-12-12 15:57:35.000000 KegElements-0.9.0/keg_elements/views.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.031174 KegElements-0.9.0/kegel_app/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.0/kegel_app/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      383 2020-09-21 14:19:34.000000 KegElements-0.9.0/kegel_app/app.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      469 2020-09-21 14:19:34.000000 KegElements-0.9.0/kegel_app/cli.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      613 2023-03-03 20:13:22.000000 KegElements-0.9.0/kegel_app/config.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1265 2021-09-10 20:06:34.000000 KegElements-0.9.0/kegel_app/extensions.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      228 2022-03-04 19:28:09.000000 KegElements-0.9.0/kegel_app/forms.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      222 2020-09-21 14:19:34.000000 KegElements-0.9.0/kegel_app/grids.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.031174 KegElements-0.9.0/kegel_app/model/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.0/kegel_app/model/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9087 2023-03-03 20:13:24.000000 KegElements-0.9.0/kegel_app/model/entities.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.031174 KegElements-0.9.0/kegel_app/templates/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1269 2022-12-12 15:57:35.000000 KegElements-0.9.0/kegel_app/templates/field-macros.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      929 2022-12-12 15:57:35.000000 KegElements-0.9.0/kegel_app/templates/form-field-value-macro.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      388 2022-12-12 15:57:35.000000 KegElements-0.9.0/kegel_app/templates/generic-form.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      295 2022-12-12 15:57:35.000000 KegElements-0.9.0/kegel_app/templates/generic-input-field.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      307 2022-12-12 15:57:35.000000 KegElements-0.9.0/kegel_app/templates/generic-radio-field.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1280 2022-12-12 15:57:35.000000 KegElements-0.9.0/kegel_app/templates/section-macro.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      418 2022-03-04 19:58:11.000000 KegElements-0.9.0/kegel_app/views.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1549 2018-11-13 17:40:23.000000 KegElements-0.9.0/license.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       32 2018-11-13 17:40:23.000000 KegElements-0.9.0/pyp.ini
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1874 2021-02-02 19:04:40.000000 KegElements-0.9.0/readme.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 20:15:17.031174 KegElements-0.9.0/scripts/
--rwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)     3835 2018-11-13 17:40:23.000000 KegElements-0.9.0/scripts/release.sh
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      660 2023-03-03 20:15:17.031174 KegElements-0.9.0/setup.cfg
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1876 2023-03-03 20:13:24.000000 KegElements-0.9.0/setup.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1413 2023-03-03 20:13:24.000000 KegElements-0.9.0/tox.ini
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       77 2018-11-13 17:40:23.000000 KegElements-0.9.0/wheelhouse.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.548277 KegElements-0.9.1/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.524276 KegElements-0.9.1/.ci/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       15 2018-11-13 17:40:23.000000 KegElements-0.9.1/.ci/.gitignore
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      954 2023-05-22 17:57:02.000000 KegElements-0.9.1/.ci/pytest.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.524276 KegElements-0.9.1/.circleci/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2271 2023-05-22 17:57:02.000000 KegElements-0.9.1/.circleci/config.yml
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      122 2021-01-29 21:07:39.000000 KegElements-0.9.1/.gitignore
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      439 2022-12-12 15:57:35.000000 KegElements-0.9.1/.pre-commit-config.yaml
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.524276 KegElements-0.9.1/KegElements.egg-info/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    21191 2023-05-22 17:57:58.000000 KegElements-0.9.1/KegElements.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2722 2023-05-22 17:57:59.000000 KegElements-0.9.1/KegElements.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-22 17:57:58.000000 KegElements-0.9.1/KegElements.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2018-11-13 21:38:47.000000 KegElements-0.9.1/KegElements.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      277 2023-05-22 17:57:59.000000 KegElements-0.9.1/KegElements.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       23 2023-05-22 17:57:59.000000 KegElements-0.9.1/KegElements.egg-info/top_level.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       76 2018-11-13 17:40:23.000000 KegElements-0.9.1/MANIFEST.in
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    21191 2023-05-22 17:57:59.548277 KegElements-0.9.1/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    18624 2023-05-22 17:57:43.000000 KegElements-0.9.1/changelog.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.528276 KegElements-0.9.1/keg_elements/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        6 2018-11-13 17:40:23.000000 KegElements-0.9.1/keg_elements/.gitignore
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       92 2021-02-02 19:04:40.000000 KegElements-0.9.1/keg_elements/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      432 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/conftest.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      108 2018-11-13 17:40:23.000000 KegElements-0.9.1/keg_elements/core.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     8742 2021-02-02 19:04:40.000000 KegElements-0.9.1/keg_elements/crypto.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.532276 KegElements-0.9.1/keg_elements/db/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.1/keg_elements/db/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3558 2021-02-02 19:04:40.000000 KegElements-0.9.1/keg_elements/db/columns.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3851 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/db/migrations.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    25756 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/db/mixins.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10163 2021-09-10 20:06:34.000000 KegElements-0.9.1/keg_elements/db/utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      862 2018-11-13 17:40:23.000000 KegElements-0.9.1/keg_elements/decorators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      440 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/encoding.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      982 2018-11-13 21:33:50.000000 KegElements-0.9.1/keg_elements/extensions.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.532276 KegElements-0.9.1/keg_elements/forms/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    35660 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/forms/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2147 2020-03-20 14:24:02.000000 KegElements-0.9.1/keg_elements/forms/state_field.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3539 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/forms/validators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      889 2018-11-13 21:33:50.000000 KegElements-0.9.1/keg_elements/http.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.532276 KegElements-0.9.1/keg_elements/i18n/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/i18n/babel.cfg
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.512275 KegElements-0.9.1/keg_elements/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.536277 KegElements-0.9.1/keg_elements/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2627 2022-12-07 20:09:09.000000 KegElements-0.9.1/keg_elements/i18n/es/LC_MESSAGES/keg_elements.mo
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3749 2022-12-07 20:09:09.000000 KegElements-0.9.1/keg_elements/i18n/es/LC_MESSAGES/keg_elements.po
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2573 2022-12-07 20:09:09.000000 KegElements-0.9.1/keg_elements/i18n/keg_elements.pot
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    13352 2023-05-22 17:57:02.000000 KegElements-0.9.1/keg_elements/sentry.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.512275 KegElements-0.9.1/keg_elements/templates/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.536277 KegElements-0.9.1/keg_elements/templates/keg-elements/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      940 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/templates/keg-elements/form-view.html
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.536277 KegElements-0.9.1/keg_elements/templates/keg-elements/forms/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5984 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/templates/keg-elements/forms/datetime-helper.js
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10037 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/templates/keg-elements/forms/horizontal-b3.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11682 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/templates/keg-elements/forms/horizontal-b4.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5456 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/templates/keg-elements/forms/horizontal-static.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      193 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/templates/keg-elements/forms/select2-scripts.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      106 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/templates/keg-elements/forms/select2-styles.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      971 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/templates/keg-elements/grid-view.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    13092 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/testing.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.540277 KegElements-0.9.1/keg_elements/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.1/keg_elements/tests/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4121 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/tests/test_columns.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7725 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/tests/test_crypto.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6423 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/tests/test_db_migrations.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    17932 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/tests/test_db_mixins.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    12725 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/tests/test_db_utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1560 2018-11-13 17:40:23.000000 KegElements-0.9.1/keg_elements/tests/test_decorators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      394 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/tests/test_encoding.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.540277 KegElements-0.9.1/keg_elements/tests/test_forms/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.1/keg_elements/tests/test_forms/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    43444 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/tests/test_forms/test_form.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2291 2020-03-20 14:24:02.000000 KegElements-0.9.1/keg_elements/tests/test_forms/test_state_field.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4316 2021-09-10 20:06:34.000000 KegElements-0.9.1/keg_elements/tests/test_forms/test_validators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    21432 2023-05-22 17:57:02.000000 KegElements-0.9.1/keg_elements/tests/test_sentry.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9499 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/tests/test_templates.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3141 2021-09-10 20:06:34.000000 KegElements-0.9.1/keg_elements/tests/test_testing.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.540277 KegElements-0.9.1/keg_elements/tests/test_views/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2021-09-10 20:06:34.000000 KegElements-0.9.1/keg_elements/tests/test_views/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3440 2023-03-03 20:13:24.000000 KegElements-0.9.1/keg_elements/tests/test_views/test_views.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-05-22 17:57:14.000000 KegElements-0.9.1/keg_elements/version.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5555 2022-12-12 15:57:35.000000 KegElements-0.9.1/keg_elements/views.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.544277 KegElements-0.9.1/kegel_app/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.1/kegel_app/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      383 2020-09-21 14:19:34.000000 KegElements-0.9.1/kegel_app/app.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      469 2020-09-21 14:19:34.000000 KegElements-0.9.1/kegel_app/cli.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      613 2023-03-03 20:13:22.000000 KegElements-0.9.1/kegel_app/config.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1265 2021-09-10 20:06:34.000000 KegElements-0.9.1/kegel_app/extensions.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      228 2022-03-04 19:28:09.000000 KegElements-0.9.1/kegel_app/forms.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      222 2020-09-21 14:19:34.000000 KegElements-0.9.1/kegel_app/grids.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.544277 KegElements-0.9.1/kegel_app/model/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-11-13 17:40:23.000000 KegElements-0.9.1/kegel_app/model/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9087 2023-03-03 20:13:24.000000 KegElements-0.9.1/kegel_app/model/entities.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.548277 KegElements-0.9.1/kegel_app/templates/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1269 2022-12-12 15:57:35.000000 KegElements-0.9.1/kegel_app/templates/field-macros.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      929 2022-12-12 15:57:35.000000 KegElements-0.9.1/kegel_app/templates/form-field-value-macro.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      388 2022-12-12 15:57:35.000000 KegElements-0.9.1/kegel_app/templates/generic-form.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      295 2022-12-12 15:57:35.000000 KegElements-0.9.1/kegel_app/templates/generic-input-field.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      307 2022-12-12 15:57:35.000000 KegElements-0.9.1/kegel_app/templates/generic-radio-field.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1280 2022-12-12 15:57:35.000000 KegElements-0.9.1/kegel_app/templates/section-macro.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      418 2022-03-04 19:58:11.000000 KegElements-0.9.1/kegel_app/views.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1549 2018-11-13 17:40:23.000000 KegElements-0.9.1/license.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       32 2018-11-13 17:40:23.000000 KegElements-0.9.1/pyp.ini
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1874 2021-02-02 19:04:40.000000 KegElements-0.9.1/readme.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-22 17:57:59.548277 KegElements-0.9.1/scripts/
+-rwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)     3835 2018-11-13 17:40:23.000000 KegElements-0.9.1/scripts/release.sh
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      660 2023-05-22 17:57:59.548277 KegElements-0.9.1/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1901 2023-05-22 17:57:02.000000 KegElements-0.9.1/setup.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1413 2023-03-03 20:13:24.000000 KegElements-0.9.1/tox.ini
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       77 2018-11-13 17:40:23.000000 KegElements-0.9.1/wheelhouse.ini
```

### Comparing `KegElements-0.9.0/.ci/pytest.ini` & `KegElements-0.9.1/.ci/pytest.ini`

 * *Files 14% similar despite different names*

```diff
@@ -11,7 +11,11 @@
     # ignore:Predicate of partial index.*ignored during reflection
     # ignore:Request.is_xhr is deprecated
     # ignore:Client.get_ident is deprecated. The event ID is now returned as the result of capture.
     # ignore:Using or importing the ABCs from 'collections'
     # ignore::DeprecationWarning:webtest.*:
 
     ignore:.*support Decimal objects natively.*:sqlalchemy.exc.SAWarning
+    ignore: pkg_resources is deprecated as an API
+
+    # https://github.com/wtforms/flask-wtf/issues/561
+    ignore:'flask.Markup' is deprecated
```

### Comparing `KegElements-0.9.0/.circleci/config.yml` & `KegElements-0.9.1/.circleci/config.yml`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,20 @@
                 default: tox
         steps:
             - checkout
 
             - run:
                 name: install tox
                 command: >
-                    pip install --upgrade --force-reinstall tox pip
+                    python3.10 -m pip install --upgrade --force-reinstall tox pip
 
             - run:
                 name: version checks
                 command: |
-                    python --version
-                    pip --version
+                    python3.10 --version
                     tox --version
 
             - run:
                 name: run tox
                 command: << parameters.toxcommand >>
 
             - store_test_results:
```

### Comparing `KegElements-0.9.0/KegElements.egg-info/PKG-INFO` & `KegElements-0.9.1/KegElements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KegElements
-Version: 0.9.0
+Version: 0.9.1
 Summary: A testing ground for Keg related code and ideas.
 Home-page: https://github.com/level12/keg-elements
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -92,14 +92,22 @@
 * Keg framework: https://github.com/level12/keg
 * Questions & comments: http://groups.google.com/group/blazelibs
 
 
 Changelog
 =========
 
+0.9.1 released 2023-05-22
+-------------------------
+
+- support monitoring jobs with Sentry (8bd9cb5_)
+
+.. _8bd9cb5: https://github.com/level12/keg-elements/commit/8bd9cb5
+
+
 0.9.0 released 2023-03-03
 -------------------------
 
 - support SQLAlchemy 2.0 (fce6248_)
 - support keg testing app context changes (4122e9e_)
 - fixed upgrade notes in documentation (514b8ff_)
```

### Comparing `KegElements-0.9.0/KegElements.egg-info/SOURCES.txt` & `KegElements-0.9.1/KegElements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/PKG-INFO` & `KegElements-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KegElements
-Version: 0.9.0
+Version: 0.9.1
 Summary: A testing ground for Keg related code and ideas.
 Home-page: https://github.com/level12/keg-elements
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -92,14 +92,22 @@
 * Keg framework: https://github.com/level12/keg
 * Questions & comments: http://groups.google.com/group/blazelibs
 
 
 Changelog
 =========
 
+0.9.1 released 2023-05-22
+-------------------------
+
+- support monitoring jobs with Sentry (8bd9cb5_)
+
+.. _8bd9cb5: https://github.com/level12/keg-elements/commit/8bd9cb5
+
+
 0.9.0 released 2023-03-03
 -------------------------
 
 - support SQLAlchemy 2.0 (fce6248_)
 - support keg testing app context changes (4122e9e_)
 - fixed upgrade notes in documentation (514b8ff_)
```

### Comparing `KegElements-0.9.0/changelog.rst` & `KegElements-0.9.1/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.9.1 released 2023-05-22
+-------------------------
+
+- support monitoring jobs with Sentry (8bd9cb5_)
+
+.. _8bd9cb5: https://github.com/level12/keg-elements/commit/8bd9cb5
+
+
 0.9.0 released 2023-03-03
 -------------------------
 
 - support SQLAlchemy 2.0 (fce6248_)
 - support keg testing app context changes (4122e9e_)
 - fixed upgrade notes in documentation (514b8ff_)
```

### Comparing `KegElements-0.9.0/keg_elements/crypto.py` & `KegElements-0.9.1/keg_elements/crypto.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/db/columns.py` & `KegElements-0.9.1/keg_elements/db/columns.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/db/migrations.py` & `KegElements-0.9.1/keg_elements/db/migrations.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/db/mixins.py` & `KegElements-0.9.1/keg_elements/db/mixins.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/db/utils.py` & `KegElements-0.9.1/keg_elements/db/utils.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/decorators.py` & `KegElements-0.9.1/keg_elements/decorators.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/extensions.py` & `KegElements-0.9.1/keg_elements/extensions.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/forms/__init__.py` & `KegElements-0.9.1/keg_elements/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/forms/state_field.py` & `KegElements-0.9.1/keg_elements/forms/state_field.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/forms/validators.py` & `KegElements-0.9.1/keg_elements/forms/validators.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/http.py` & `KegElements-0.9.1/keg_elements/http.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/i18n/es/LC_MESSAGES/keg_elements.mo` & `KegElements-0.9.1/keg_elements/i18n/es/LC_MESSAGES/keg_elements.mo`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/i18n/es/LC_MESSAGES/keg_elements.po` & `KegElements-0.9.1/keg_elements/i18n/es/LC_MESSAGES/keg_elements.po`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/i18n/keg_elements.pot` & `KegElements-0.9.1/keg_elements/i18n/keg_elements.pot`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/templates/keg-elements/form-view.html` & `KegElements-0.9.1/keg_elements/templates/keg-elements/form-view.html`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/templates/keg-elements/forms/datetime-helper.js` & `KegElements-0.9.1/keg_elements/templates/keg-elements/forms/datetime-helper.js`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/templates/keg-elements/forms/horizontal-b3.html` & `KegElements-0.9.1/keg_elements/templates/keg-elements/forms/horizontal-b3.html`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/templates/keg-elements/forms/horizontal-b4.html` & `KegElements-0.9.1/keg_elements/templates/keg-elements/forms/horizontal-b4.html`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/templates/keg-elements/forms/horizontal-static.html` & `KegElements-0.9.1/keg_elements/templates/keg-elements/forms/horizontal-static.html`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/templates/keg-elements/grid-view.html` & `KegElements-0.9.1/keg_elements/templates/keg-elements/grid-view.html`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/testing.py` & `KegElements-0.9.1/keg_elements/testing.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_columns.py` & `KegElements-0.9.1/keg_elements/tests/test_columns.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_crypto.py` & `KegElements-0.9.1/keg_elements/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_db_migrations.py` & `KegElements-0.9.1/keg_elements/tests/test_db_migrations.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_db_mixins.py` & `KegElements-0.9.1/keg_elements/tests/test_db_mixins.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_db_utils.py` & `KegElements-0.9.1/keg_elements/tests/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_decorators.py` & `KegElements-0.9.1/keg_elements/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_forms/test_form.py` & `KegElements-0.9.1/keg_elements/tests/test_forms/test_form.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_forms/test_state_field.py` & `KegElements-0.9.1/keg_elements/tests/test_forms/test_state_field.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_forms/test_validators.py` & `KegElements-0.9.1/keg_elements/tests/test_forms/test_validators.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_templates.py` & `KegElements-0.9.1/keg_elements/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_testing.py` & `KegElements-0.9.1/keg_elements/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/tests/test_views/test_views.py` & `KegElements-0.9.1/keg_elements/tests/test_views/test_views.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/keg_elements/views.py` & `KegElements-0.9.1/keg_elements/views.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/kegel_app/config.py` & `KegElements-0.9.1/kegel_app/config.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/kegel_app/extensions.py` & `KegElements-0.9.1/kegel_app/extensions.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/kegel_app/model/entities.py` & `KegElements-0.9.1/kegel_app/model/entities.py`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/kegel_app/templates/field-macros.html` & `KegElements-0.9.1/kegel_app/templates/field-macros.html`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/kegel_app/templates/form-field-value-macro.html` & `KegElements-0.9.1/kegel_app/templates/form-field-value-macro.html`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/kegel_app/templates/section-macro.html` & `KegElements-0.9.1/kegel_app/templates/section-macro.html`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/license.txt` & `KegElements-0.9.1/license.txt`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/readme.rst` & `KegElements-0.9.1/readme.rst`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/scripts/release.sh` & `KegElements-0.9.1/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/setup.cfg` & `KegElements-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `KegElements-0.9.0/setup.py` & `KegElements-0.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             'pre-commit',
             'psycopg2-binary',
             'pyquery',
             'pytest',
             'pytest-cov',
             # pinned to version in our package index.
             'pyodbc==4.0.34',
+            'responses',
             'sqlalchemy_pyodbc_mssql',
             'tox',
             'freezegun',
             'webgrid',
             'xlsxwriter',
         ],
         'i18n': [
```

### Comparing `KegElements-0.9.0/tox.ini` & `KegElements-0.9.1/tox.ini`

 * *Files identical despite different names*

