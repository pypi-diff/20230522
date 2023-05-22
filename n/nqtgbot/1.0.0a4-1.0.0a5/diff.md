# Comparing `tmp/nqtgbot-1.0.0a4.tar.gz` & `tmp/nqtgbot-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nqtgbot-1.0.0a4.tar", max compression
+gzip compressed data, was "nqtgbot-1.0.0a5.tar", max compression
```

## Comparing `nqtgbot-1.0.0a4.tar` & `nqtgbot-1.0.0a5.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      556 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a4/LICENSE
--rw-r--r--   0        0        0       94 2022-11-30 22:25:15.578058 nqtgbot-1.0.0a4/README.md
--rw-r--r--   0        0        0        0 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a4/nqtgbot/__init__.py
--rw-r--r--   0        0        0     1174 2022-10-27 17:57:15.551527 nqtgbot-1.0.0a4/nqtgbot/message.py
--rw-r--r--   0        0        0     2253 2022-11-17 19:12:38.249444 nqtgbot-1.0.0a4/nqtgbot/provider.py
--rw-r--r--   0        0        0     1263 2022-11-17 19:12:38.261444 nqtgbot-1.0.0a4/nqtgbot/quotas.py
--rw-r--r--   0        0        0      264 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a4/nqtgbot/resources/config_schema.json
--rw-r--r--   0        0        0     1500 2022-11-30 22:25:15.578058 nqtgbot-1.0.0a4/pyproject.toml
--rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 nqtgbot-1.0.0a4/setup.py
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 nqtgbot-1.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0      557 2023-03-26 09:02:50.446375 nqtgbot-1.0.0a5/LICENSE
+-rw-r--r--   0        0        0      368 2023-05-20 13:15:49.684187 nqtgbot-1.0.0a5/README.md
+-rw-r--r--   0        0        0        0 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a5/nqtgbot/__init__.py
+-rw-r--r--   0        0        0     1174 2022-10-27 17:57:15.551527 nqtgbot-1.0.0a5/nqtgbot/message.py
+-rw-r--r--   0        0        0     2253 2022-11-17 19:12:38.249444 nqtgbot-1.0.0a5/nqtgbot/provider.py
+-rw-r--r--   0        0        0     1336 2023-01-22 20:06:46.830008 nqtgbot-1.0.0a5/nqtgbot/quotas.py
+-rw-r--r--   0        0        0      264 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a5/nqtgbot/resources/config_schema.json
+-rw-r--r--   0        0        0     1294 2023-05-22 11:06:32.697850 nqtgbot-1.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 nqtgbot-1.0.0a5/PKG-INFO
```

### Comparing `nqtgbot-1.0.0a4/LICENSE` & `nqtgbot-1.0.0a5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Copyright (c) 2022 Inqana Ltd.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
-    http://www.apache.org/licenses/LICENSE-2.0
+    https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
```

### Comparing `nqtgbot-1.0.0a4/nqtgbot/message.py` & `nqtgbot-1.0.0a5/nqtgbot/message.py`

 * *Files identical despite different names*

### Comparing `nqtgbot-1.0.0a4/nqtgbot/provider.py` & `nqtgbot-1.0.0a5/nqtgbot/provider.py`

 * *Files identical despite different names*

### Comparing `nqtgbot-1.0.0a4/nqtgbot/quotas.py` & `nqtgbot-1.0.0a5/nqtgbot/quotas.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from nqsdk.abstract.quotas import ProviderDynamicDelayQuota, ProviderStaticQuota
-from nqsdk.enums import QuotaIdentityType
-
+from datetime import datetime, timedelta
 
-class RetryAfterQuota(ProviderDynamicDelayQuota):
-    def __init__(self, delay: int):
-        self._delay = delay
+from nqsdk.abstract.quotas import ProviderDynamicQuota, ProviderStaticQuota
+from nqsdk.enums import QuotaIdentityType
 
-    @property
-    def delay(self) -> int:
-        return self._delay
 
+class RetryAfterQuota(ProviderDynamicQuota):
     @classmethod
     def identity_type(cls) -> QuotaIdentityType:
         return QuotaIdentityType.AUTH_ENTITY
 
+    def __init__(self, delay: int):
+        self._until = datetime.now() + timedelta(seconds=delay)
+
+    @property
+    def until(self) -> datetime:
+        return self._until
+
 
 class PerSecondQuota(ProviderStaticQuota):
     @classmethod
     def identity_type(cls) -> QuotaIdentityType:
         return QuotaIdentityType.AUTH_ENTITY
 
     @property
```

