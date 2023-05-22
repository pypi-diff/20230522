# Comparing `tmp/Flunt-0.2.0.tar.gz` & `tmp/flunt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flunt-0.2.0.tar", max compression
+gzip compressed data, was "flunt-1.0.0.tar", max compression
```

## Comparing `Flunt-0.2.0.tar` & `flunt-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,15 @@
--rw-r--r--   0        0        0     1085 2021-11-23 02:26:46.818699 Flunt-0.2.0/LICENSE
--rw-r--r--   0        0        0       46 2021-11-23 02:26:46.818699 Flunt-0.2.0/flunt/__init__.py
--rw-r--r--   0        0        0     2960 2021-11-23 02:26:46.818699 Flunt-0.2.0/flunt/contract.py
--rw-r--r--   0        0        0     1668 2021-11-23 02:26:46.818699 Flunt-0.2.0/flunt/notifiable.py
--rw-r--r--   0        0        0      411 2021-11-23 02:26:46.818699 Flunt-0.2.0/flunt/notification.py
--rw-r--r--   0        0        0      491 2021-11-23 02:26:46.818699 Flunt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      764 2021-11-23 02:27:40.431926 Flunt-0.2.0/setup.py
--rw-r--r--   0        0        0      495 2021-11-23 02:27:40.432158 Flunt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-22 02:18:14.799811 flunt-1.0.0/LICENSE
+-rw-r--r--   0        0        0       46 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/__init__.py
+-rw-r--r--   0        0        0       46 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/localization/__init__.py
+-rw-r--r--   0        0        0     2082 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/localization/flunt_regex_patterns.py
+-rw-r--r--   0        0        0       46 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/notifications/__init__.py
+-rw-r--r--   0        0        0      344 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/notifications/interface.py
+-rw-r--r--   0        0        0     1795 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/notifications/notifiable.py
+-rw-r--r--   0        0        0      411 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/notifications/notification.py
+-rw-r--r--   0        0        0       46 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/validations/__init__.py
+-rw-r--r--   0        0        0     2512 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/validations/bool_validation_contract.py
+-rw-r--r--   0        0        0      795 2023-05-22 02:18:14.799811 flunt-1.0.0/flunt/validations/contract.py
+-rw-r--r--   0        0        0     3492 2023-05-22 02:18:14.803811 flunt-1.0.0/flunt/validations/email_validation_contract.py
+-rw-r--r--   0        0        0    15883 2023-05-22 02:18:14.803811 flunt-1.0.0/flunt/validations/strings_validation_contract.py
+-rw-r--r--   0        0        0      670 2023-05-22 02:18:14.803811 flunt-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 flunt-1.0.0/PKG-INFO
```

### Comparing `Flunt-0.2.0/LICENSE` & `flunt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flunt-0.2.0/flunt/notifiable.py` & `flunt-1.0.0/flunt/notifications/notifiable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Module Notifiable."""
-from flunt.notification import Notification
+from interface import implements
 
+from flunt.notifications.interface import INotifiable
+from flunt.notifications.notification import Notification
 
-class Notifiable(Notification):
+
+class Notifiable(implements(INotifiable), Notification):
     """Class Notifiable."""
 
     def __init__(self) -> None:
         """Found 'Constructor'."""
         self._notifications: list = []
 
     def add_notification(self, notification: Notification):
```

