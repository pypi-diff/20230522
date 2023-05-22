# Comparing `tmp/funding-service-design-utils-2.0.1.tar.gz` & `tmp/funding-service-design-utils-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funding-service-design-utils-2.0.1.tar", last modified: Tue May 16 10:53:05 2023, max compression
+gzip compressed data, was "funding-service-design-utils-2.0.2.tar", last modified: Mon May 22 10:35:15 2023, max compression
```

## Comparing `funding-service-design-utils-2.0.1.tar` & `funding-service-design-utils-2.0.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_test_utils/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/fixtures/db_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_test_utils/test_config/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/test_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/test_config/useful_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/config/commonconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/config/configclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/config/notify_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/devtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/healthchecks/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/healthchecks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/healthchecks/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/healthchecks/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/locale_selector/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/locale_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/locale_selector/get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/locale_selector/set_lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/sentry/init_sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/simple_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/simple_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/simple_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/simple_utils/date_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/toggles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/toggles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/toggles/toggles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.377450 funding-service-design-utils-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-05-22 10:35:15.377450 funding-service-design-utils-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.369450 funding-service-design-utils-2.0.2/fsd_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.369450 funding-service-design-utils-2.0.2/fsd_test_utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_test_utils/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_test_utils/fixtures/db_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.369450 funding-service-design-utils-2.0.2/fsd_test_utils/test_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_test_utils/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_test_utils/test_config/useful_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/authentication/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/authentication/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/authentication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/config/commonconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/config/configclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/config/notify_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/gunicorn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/gunicorn/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/gunicorn/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/gunicorn/config/devtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/gunicorn/config/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/healthchecks/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/healthchecks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/healthchecks/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/healthchecks/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/locale_selector/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/locale_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/locale_selector/get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/locale_selector/set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/sentry/init_sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/simple_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/simple_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/simple_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/simple_utils/date_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.373450 funding-service-design-utils-2.0.2/fsd_utils/toggles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/toggles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/fsd_utils/toggles/toggles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.377450 funding-service-design-utils-2.0.2/funding_service_design_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-05-22 10:35:15.000000 funding-service-design-utils-2.0.2/funding_service_design_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-22 10:35:15.000000 funding-service-design-utils-2.0.2/funding_service_design_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:35:15.000000 funding-service-design-utils-2.0.2/funding_service_design_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-22 10:35:15.000000 funding-service-design-utils-2.0.2/funding_service_design_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 10:35:15.000000 funding-service-design-utils-2.0.2/funding_service_design_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 10:35:15.377450 funding-service-design-utils-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:15.377450 funding-service-design-utils-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/tests/test_get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-22 10:35:02.000000 funding-service-design-utils-2.0.2/tests/test_set_lang.py
```

### Comparing `funding-service-design-utils-2.0.1/LICENSE` & `funding-service-design-utils-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/PKG-INFO` & `funding-service-design-utils-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.1
+Version: 2.0.2
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -166,14 +166,24 @@
 
     FSD_USER_TOKEN_COOKIE_NAME = "fsd_user_token"
     AUTHENTICATOR_HOST = "https://funding-service-design-authenticator-dev.london.cloudapps.digital"
     RSA256_PUBLIC_KEY = "{RSA PUBLIC KEY}"
 
 NOTE: These values (and keys) need to be shared/common across all microservices that use each common authenticator host. If any of the environment *keys* for each of these attributes needs to be modified these can be reconfigured in fsd_utils/authentication/config.py.
 
+To generate new keys in your cwd, you use the following commands:
+```bash
+openssl genrsa -out private_key.pem 2048
+openssl rsa -pubout -in private_key.pem -out public_key.pem
+```
+
+If you're changing keys, you'll need to change them in GitHub secrets across repos.
+Please also add them to BitWarden and let the team know.
+
+
 Then - to use the `@login_required` decorator just add it to routes you need to protect eg:
 
     # in ...routes.py
     from fsd_utils.authentication.decorators import login_required
 
     @login_required
     def example_route(account_id):
```

### Comparing `funding-service-design-utils-2.0.1/README.md` & `funding-service-design-utils-2.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -131,14 +131,24 @@
 
     FSD_USER_TOKEN_COOKIE_NAME = "fsd_user_token"
     AUTHENTICATOR_HOST = "https://funding-service-design-authenticator-dev.london.cloudapps.digital"
     RSA256_PUBLIC_KEY = "{RSA PUBLIC KEY}"
 
 NOTE: These values (and keys) need to be shared/common across all microservices that use each common authenticator host. If any of the environment *keys* for each of these attributes needs to be modified these can be reconfigured in fsd_utils/authentication/config.py.
 
+To generate new keys in your cwd, you use the following commands:
+```bash
+openssl genrsa -out private_key.pem 2048
+openssl rsa -pubout -in private_key.pem -out public_key.pem
+```
+
+If you're changing keys, you'll need to change them in GitHub secrets across repos.
+Please also add them to BitWarden and let the team know.
+
+
 Then - to use the `@login_required` decorator just add it to routes you need to protect eg:
 
     # in ...routes.py
     from fsd_utils.authentication.decorators import login_required
 
     @login_required
     def example_route(account_id):
```

### Comparing `funding-service-design-utils-2.0.1/fsd_test_utils/fixtures/db_fixtures.py` & `funding-service-design-utils-2.0.2/fsd_test_utils/fixtures/db_fixtures.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/__init__.py` & `funding-service-design-utils-2.0.2/fsd_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/authentication/config.py` & `funding-service-design-utils-2.0.2/fsd_utils/authentication/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 CONFIGURATION FOR SECURITY UTILITY
 
 To use this utility please ensure that all the
 "config_var_..." keys are set to the correct values
 in the environment of the application that is using
 this utility.
 """
+import enum
+
 config_var_auth_host = "AUTHENTICATOR_HOST"
 config_var_user_token_cookie_name = "FSD_USER_TOKEN_COOKIE_NAME"
 config_var_rs256_public_key = "RSA256_PUBLIC_KEY"
 signout_route = "/sessions/sign-out"
 user_route = "/service/user"
 azure_ad_role_map = {
     "LeadAssessor": "LEAD_ASSESSOR",
     "Assessor": "ASSESSOR",
     "Commenter": "COMMENTER",
 }
+
+
+class SupportedApp(enum.Enum):
+    POST_AWARD_FRONTEND = "post-award-frontend"
```

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/authentication/decorators.py` & `funding-service-design-utils-2.0.2/fsd_utils/authentication/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from functools import wraps
 from typing import List
+from urllib.parse import urlencode
 
 from flask import abort
 from flask import current_app
 from flask import g
 from flask import redirect
 from flask import request
 from fsd_utils.authentication.utils import validate_token_rs256
 from jwt import ExpiredSignatureError
 from jwt import PyJWTError
 
 from .config import config_var_auth_host
 from .config import config_var_user_token_cookie_name
 from .config import signout_route
+from .config import SupportedApp
 from .config import user_route
 from .models import User
 
 
-def _failed_redirect():
-    authenticator_host = current_app.config[config_var_auth_host]
-
-    return abort(redirect(authenticator_host + signout_route))
+def _failed_redirect(return_app: SupportedApp | None):
+    logout_url = _build_logout_url(return_app)
+    return abort(redirect(logout_url))
 
 
 def _failed_roles_redirect(roles_required: List[str]):
     authenticator_host = current_app.config[config_var_auth_host]
 
     return abort(
         redirect(
@@ -32,15 +33,15 @@
             + user_route
             + "?roles_required="
             + "|".join(roles_required)
         )
     )
 
 
-def _check_access_token(auto_redirect=True):
+def _check_access_token(return_app: SupportedApp | None = None, auto_redirect=True):
     """
     Check the expected auth cookie for a
     valid JWT token.
     :param auto_redirect: (bool) redirect on failed authentication if True
     :return:
         - If a valid JWT token is found then return token claims
         - If no valid token is found:
@@ -48,60 +49,76 @@
             -- If auto_redirect is False then return False
     """
     user_token_cookie_name = current_app.config[config_var_user_token_cookie_name]
 
     login_cookie = request.cookies.get(user_token_cookie_name)
     if not login_cookie:
         if auto_redirect:
-            _failed_redirect()
+            _failed_redirect(return_app)
         return False
 
     try:
         return validate_token_rs256(login_cookie)
     except (PyJWTError, ExpiredSignatureError):
         if auto_redirect:
-            _failed_redirect()
+            _failed_redirect(return_app)
         return False
 
 
-def login_required(f=None, roles_required: List[str] = None):
+def _build_logout_url(return_app: SupportedApp | None):
+    authenticator_host = current_app.config[config_var_auth_host]
+    if return_app:
+        return (
+            authenticator_host
+            + signout_route
+            + f"?{urlencode({'return_app': return_app.value})}"
+        )
+    else:
+        return authenticator_host + signout_route
+
+
+def login_required(
+    f=None, roles_required: List[str] = None, return_app: SupportedApp | None = None
+):
     """
      Execute function if request contains valid JWT
      and pass account auth params to route as attributes
      on the flask request global 'g' object:
          - g.account_id: (str) users account id
          - g.is_authenticated: (bool) authentication status
          - g.user - this holds a User object and associated attributes
          - g.logout_url: (str) the service sign-out url
      If no valid auth JWT found then redirect to
      service config invalid login route
     :param f:
+    :param return_app: app to return to after login
     :param roles_required: (List(str), optional) a list of the
             roles required to access the decorated route
     :return:
     """
     if f is None:
-        return lambda f: login_required(f=f, roles_required=roles_required)
+        return lambda f: login_required(
+            f=f, roles_required=roles_required, return_app=return_app
+        )
 
     @wraps(f)
     def _wrapper(*args, **kwargs):
         if (
             current_app.config.get("FLASK_ENV") == "development"
             and current_app.config.get("DEBUG_USER_ROLE")
             and current_app.config.get("DEBUG_USER")
         ):
             g.account_id = "dev-account-id"
             g.user = User(**current_app.config.get("DEBUG_USER"))
         else:
-            token_payload = _check_access_token()
+            token_payload = _check_access_token(return_app=return_app)
             g.account_id = token_payload.get("accountId")
             g.user = User.set_with_token(token_payload)
 
-        authenticator_host = current_app.config[config_var_auth_host]
-        g.logout_url = authenticator_host + signout_route
+        g.logout_url = _build_logout_url(return_app)
         g.is_authenticated = True
         if roles_required:
             if not any(
                 role_required in g.user.roles for role_required in roles_required
             ):
                 _failed_roles_redirect(roles_required)
         return f(*args, **kwargs)
```

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/authentication/models.py` & `funding-service-design-utils-2.0.2/fsd_utils/authentication/models.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/authentication/utils.py` & `funding-service-design-utils-2.0.2/fsd_utils/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/config/commonconfig.py` & `funding-service-design-utils-2.0.2/fsd_utils/config/commonconfig.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/config/configclass.py` & `funding-service-design-utils-2.0.2/fsd_utils/config/configclass.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/config/notify_constants.py` & `funding-service-design-utils-2.0.2/fsd_utils/config/notify_constants.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/devtest.py` & `funding-service-design-utils-2.0.2/fsd_utils/gunicorn/config/devtest.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/local.py` & `funding-service-design-utils-2.0.2/fsd_utils/gunicorn/config/local.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/healthchecks/checkers.py` & `funding-service-design-utils-2.0.2/fsd_utils/healthchecks/checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/healthchecks/healthcheck.py` & `funding-service-design-utils-2.0.2/fsd_utils/healthchecks/healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/locale_selector/get_lang.py` & `funding-service-design-utils-2.0.2/fsd_utils/locale_selector/get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/locale_selector/set_lang.py` & `funding-service-design-utils-2.0.2/fsd_utils/locale_selector/set_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/logging/logging.py` & `funding-service-design-utils-2.0.2/fsd_utils/logging/logging.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/sentry/init_sentry.py` & `funding-service-design-utils-2.0.2/fsd_utils/sentry/init_sentry.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/fsd_utils/toggles/toggles.py` & `funding-service-design-utils-2.0.2/fsd_utils/toggles/toggles.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/PKG-INFO` & `funding-service-design-utils-2.0.2/funding_service_design_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.1
+Version: 2.0.2
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -166,14 +166,24 @@
 
     FSD_USER_TOKEN_COOKIE_NAME = "fsd_user_token"
     AUTHENTICATOR_HOST = "https://funding-service-design-authenticator-dev.london.cloudapps.digital"
     RSA256_PUBLIC_KEY = "{RSA PUBLIC KEY}"
 
 NOTE: These values (and keys) need to be shared/common across all microservices that use each common authenticator host. If any of the environment *keys* for each of these attributes needs to be modified these can be reconfigured in fsd_utils/authentication/config.py.
 
+To generate new keys in your cwd, you use the following commands:
+```bash
+openssl genrsa -out private_key.pem 2048
+openssl rsa -pubout -in private_key.pem -out public_key.pem
+```
+
+If you're changing keys, you'll need to change them in GitHub secrets across repos.
+Please also add them to BitWarden and let the team know.
+
+
 Then - to use the `@login_required` decorator just add it to routes you need to protect eg:
 
     # in ...routes.py
     from fsd_utils.authentication.decorators import login_required
 
     @login_required
     def example_route(account_id):
```

### Comparing `funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/SOURCES.txt` & `funding-service-design-utils-2.0.2/funding_service_design_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/pyproject.toml` & `funding-service-design-utils-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "funding-service-design-utils"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name="DLUHC", email="FundingServiceDesignTeam@levellingup.gov.uk" },
 ]
 description = "Utilities used by the DLUHC Funding Service Design Team"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10,<4.0"
```

### Comparing `funding-service-design-utils-2.0.1/tests/conftest.py` & `funding-service-design-utils-2.0.2/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Contains test configuration.
 """
 from pathlib import Path
 
 import pytest
 from flask import Flask
 from flask import g
+from fsd_utils.authentication.config import SupportedApp
 from fsd_utils.authentication.decorators import login_requested
 from fsd_utils.authentication.decorators import login_required
 
 
 def create_app():
     app = Flask("test")
     return app
@@ -53,14 +54,21 @@
             mock_login_required_roles_route,
         )
         app_context.app.add_url_rule(
             "/mock_login_required_admin_roles_route",
             "mock_login_required_admin_roles_route",
             mock_login_required_admin_roles_route,
         )
+
+        app_context.app.add_url_rule(
+            "/mock_login_requested_return_app_route",
+            "mock_login_requested_return_app_route",
+            mock_login_requested_return_app_route,
+        )
+
         with app_context.app.test_client() as test_client:
             yield test_client
 
 
 @pytest.fixture(scope="function")
 def flask_test_development_client():
     """
@@ -201,7 +209,36 @@
             full_name="Test User",
             highest_role="LEAD_ASSESSOR",
             roles=["LEAD_ASSESSOR", "ASSESSOR", "COMMENTER"]
         )
     :return: the Flask g variable serialised as a dict/json
     """
     return vars(g)
+
+
+@login_required(return_app=SupportedApp.POST_AWARD_FRONTEND)
+def mock_login_requested_return_app_route():
+    """
+    A mock route function decorated with @login_requested
+    Here we expect a logged in user to have the required
+    Flask request g variables set as below:
+    NOTE: the logout_url should end with the query string "?return_app=post-award-frontend" in both cases.
+    g: {
+        "is_authenticated": True,
+        "logout_url": "https://authenticator/sessions/sign-out?return_app=post-award-frontend",
+        "account_id": "test-user",
+        "user": User(
+            email="test@example.com",
+            full_name="Test User",
+            highest_role="LEAD_ASSESSOR",
+            roles=["LEAD_ASSESSOR", "ASSESSOR", "COMMENTER"]
+        )
+    and a non logged in user to have the Flask request g variables
+    set as below:
+    g: {
+        "is_authenticated": False,
+        "logout_url": "https://authenticator/sessions/sign-out?return_app=post-award-frontend",
+        "account_id": None,
+    }
+    :return: the Flask g variable serialised as a dict/json
+    """
+    return vars(g)
```

### Comparing `funding-service-design-utils-2.0.1/tests/test_authentication.py` & `funding-service-design-utils-2.0.2/tests/test_authentication.py`

 * *Files 13% similar despite different names*

```diff
@@ -203,7 +203,66 @@
             "/mock_login_required_roles_route"
         )
         assert mock_request.status_code == 302
         assert (
             mock_request.location
             == "https://authenticator/service/user?roles_required=COMMENTER"
         )
+
+    def test_login_required_with_return_app_redirects_to_signed_out_without_token(
+        self, flask_test_client
+    ):
+        """
+        GIVEN a flask_test_client and
+            route decorated with @login_required decorator with the "return_app" parameter set to "post-award-frontend"
+        WHEN a request is made without any "fsd-user-token" cookie
+        THEN the route redirects to the authenticator /sessions/sign-out url with correct return_app query param
+        :param flask_test_client:
+        """
+        mock_request = flask_test_client.get("/mock_login_requested_return_app_route")
+
+        assert mock_request.status_code == 302
+        assert (
+            mock_request.location
+            == "https://authenticator/sessions/sign-out?return_app=post-award-frontend"
+        )
+
+    def test_login_required_with_return_app_redirects_to_signed_out_with_invalid_token(
+        self, flask_test_client
+    ):
+        """
+        GIVEN a flask_test_client and
+            route decorated with @login_required decorator with the "return_app" parameter set to "post-award-frontend"
+        WHEN a request is made with a correctly formatted
+            but invalidly signed "fsd-user-token" cookie
+        THEN the route redirects to the authenticator /sessions/sign-out url with correct return_app query param
+        :param flask_test_client:
+        """
+        invalid_token = self._create_invalid_token()
+        flask_test_client.set_cookie("localhost", "fsd-user-token", invalid_token)
+        mock_request = flask_test_client.get("/mock_login_requested_return_app_route")
+
+        assert mock_request.status_code == 302
+        assert (
+            mock_request.location
+            == "https://authenticator/sessions/sign-out?return_app=post-award-frontend"
+        )
+
+    def test_login_required_with_return_app_sets_user_attributes_with_valid_token(
+        self, flask_test_client
+    ):
+        """
+        GIVEN a flask_test_client and
+            route decorated with @login_required decorator with the "return_app" parameter set to "post-award-frontend"
+        WHEN a request is made with a correctly formatted
+            and signed "fsd-user-token" cookie
+        THEN the route returns with the g variable "logout_url" set correctly
+        :param flask_test_client:
+        """
+        valid_token = self._create_valid_token()
+        flask_test_client.set_cookie("localhost", "fsd-user-token", valid_token)
+        mock_request = flask_test_client.get("/mock_login_requested_return_app_route")
+        assert mock_request.status_code == 200
+        assert (
+            mock_request.json["logout_url"]
+            == "https://authenticator/sessions/sign-out?return_app=post-award-frontend"
+        )
```

### Comparing `funding-service-design-utils-2.0.1/tests/test_checkers.py` & `funding-service-design-utils-2.0.2/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/tests/test_data_utils.py` & `funding-service-design-utils-2.0.2/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/tests/test_get_lang.py` & `funding-service-design-utils-2.0.2/tests/test_get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/tests/test_healthcheck.py` & `funding-service-design-utils-2.0.2/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.1/tests/test_set_lang.py` & `funding-service-design-utils-2.0.2/tests/test_set_lang.py`

 * *Files identical despite different names*

