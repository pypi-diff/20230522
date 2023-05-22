# Comparing `tmp/flunt-1.0.0.tar.gz` & `tmp/flunt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flunt-1.0.0.tar", max compression
+gzip compressed data, was "flunt-1.0.1.tar", max compression
```

## Comparing `flunt-1.0.0.tar` & `flunt-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1085 2023-05-22 02:18:14.799811 flunt-1.0.0/LICENSE
--rw-r--r--   0        0        0       46 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/__init__.py
--rw-r--r--   0        0        0       46 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/localization/__init__.py
--rw-r--r--   0        0        0     2082 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/localization/flunt_regex_patterns.py
--rw-r--r--   0        0        0       46 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/notifications/__init__.py
--rw-r--r--   0        0        0      344 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/notifications/interface.py
--rw-r--r--   0        0        0     1795 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/notifications/notifiable.py
--rw-r--r--   0        0        0      411 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/notifications/notification.py
--rw-r--r--   0        0        0       46 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/validations/__init__.py
--rw-r--r--   0        0        0     2512 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/validations/bool_validation_contract.py
--rw-r--r--   0        0        0      795 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/validations/contract.py
--rw-r--r--   0        0        0     3492 2023-05-22 02:18:14.803811 flunt-1.0.0/flunt/validations/email_validation_contract.py
--rw-r--r--   0        0        0    15883 2023-05-22 02:18:14.803811 flunt-1.0.0/flunt/validations/strings_validation_contract.py
--rw-r--r--   0        0        0      670 2023-05-22 02:18:14.803811 flunt-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 flunt-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-22 03:13:24.536957 flunt-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2615 2023-05-22 03:13:24.536957 flunt-1.0.1/README.md
+-rw-r--r--   0        0        0       46 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/__init__.py
+-rw-r--r--   0        0        0       46 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/localization/__init__.py
+-rw-r--r--   0        0        0     2082 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/localization/flunt_regex_patterns.py
+-rw-r--r--   0        0        0       46 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/notifications/__init__.py
+-rw-r--r--   0        0        0      344 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/notifications/interface.py
+-rw-r--r--   0        0        0     1795 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/notifications/notifiable.py
+-rw-r--r--   0        0        0      411 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/notifications/notification.py
+-rw-r--r--   0        0        0       46 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/validations/__init__.py
+-rw-r--r--   0        0        0     2512 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/validations/bool_validation_contract.py
+-rw-r--r--   0        0        0      795 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/validations/contract.py
+-rw-r--r--   0        0        0     3492 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/validations/email_validation_contract.py
+-rw-r--r--   0        0        0    15883 2023-05-22 03:13:24.536957 flunt-1.0.1/flunt/validations/strings_validation_contract.py
+-rw-r--r--   0        0        0     1097 2023-05-22 03:13:24.536957 flunt-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 flunt-1.0.1/PKG-INFO
```

### Comparing `flunt-1.0.0/LICENSE` & `flunt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flunt-1.0.0/flunt/localization/flunt_regex_patterns.py` & `flunt-1.0.1/flunt/localization/flunt_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `flunt-1.0.0/flunt/notifications/notifiable.py` & `flunt-1.0.1/flunt/notifications/notifiable.py`

 * *Files identical despite different names*

### Comparing `flunt-1.0.0/flunt/validations/bool_validation_contract.py` & `flunt-1.0.1/flunt/validations/bool_validation_contract.py`

 * *Files identical despite different names*

### Comparing `flunt-1.0.0/flunt/validations/contract.py` & `flunt-1.0.1/flunt/validations/contract.py`

 * *Files identical despite different names*

### Comparing `flunt-1.0.0/flunt/validations/email_validation_contract.py` & `flunt-1.0.1/flunt/validations/email_validation_contract.py`

 * *Files identical despite different names*

### Comparing `flunt-1.0.0/flunt/validations/strings_validation_contract.py` & `flunt-1.0.1/flunt/validations/strings_validation_contract.py`

 * *Files identical despite different names*

