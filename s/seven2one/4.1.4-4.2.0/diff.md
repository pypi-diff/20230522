# Comparing `tmp/seven2one-4.1.4.tar.gz` & `tmp/seven2one-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seven2one-4.1.4.tar", last modified: Tue Apr 25 15:10:02 2023, max compression
+gzip compressed data, was "seven2one-4.2.0.tar", last modified: Mon May 22 08:35:18 2023, max compression
```

## Comparing `seven2one-4.1.4.tar` & `seven2one-4.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-25 15:10:02.381328 seven2one-4.1.4/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2023-04-14 08:32:42.000000 seven2one-4.1.4/LICENSE
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-14 08:32:42.000000 seven2one-4.1.4/MANIFEST.in
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-04-25 15:10:02.381328 seven2one-4.1.4/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1771 2023-04-14 08:32:42.000000 seven2one-4.1.4/README.md
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-04-25 15:10:02.381328 seven2one-4.1.4/setup.cfg
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1388 2023-04-25 08:08:15.000000 seven2one-4.1.4/setup.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-25 15:10:02.381328 seven2one-4.1.4/seven2one/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-04-25 15:09:58.000000 seven2one-4.1.4/seven2one/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15405 2023-04-25 08:08:15.000000 seven2one-4.1.4/seven2one/authorization.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    10848 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/automation.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    63376 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/core.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/email.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/fileImportService.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/fileimport.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-25 15:10:02.381328 seven2one-4.1.4/seven2one/logging_loki/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/logging_loki/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/logging_loki/const.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/logging_loki/emitter.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/logging_loki/handlers.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/programming.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     9486 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/schedule.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    61479 2023-04-25 08:08:15.000000 seven2one-4.1.4/seven2one/timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-25 15:10:02.381328 seven2one-4.1.4/seven2one/utils/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-04-25 15:09:58.000000 seven2one-4.1.4/seven2one/utils/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35567 2023-04-25 08:08:15.000000 seven2one-4.1.4/seven2one/utils/ut.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/utils/ut_autprog.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/utils/ut_fileimport.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/utils/ut_init.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      989 2023-04-25 08:08:15.000000 seven2one-4.1.4/seven2one/utils/ut_log.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/utils/ut_meta.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2023-04-14 08:32:42.000000 seven2one-4.1.4/seven2one/utils/ut_time.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6567 2023-04-25 08:08:15.000000 seven2one-4.1.4/seven2one/utils/ut_timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-25 15:10:02.381328 seven2one-4.1.4/seven2one.egg-info/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-04-25 15:10:02.000000 seven2one-4.1.4/seven2one.egg-info/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-04-25 15:10:02.000000 seven2one-4.1.4/seven2one.egg-info/SOURCES.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-04-25 15:10:02.000000 seven2one-4.1.4/seven2one.egg-info/dependency_links.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-04-25 15:10:02.000000 seven2one-4.1.4/seven2one.egg-info/not-zip-safe
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       97 2023-04-25 15:10:02.000000 seven2one-4.1.4/seven2one.egg-info/requires.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-04-25 15:10:02.000000 seven2one-4.1.4/seven2one.egg-info/top_level.txt
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.712959 seven2one-4.2.0/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2023-04-14 08:32:42.000000 seven2one-4.2.0/LICENSE
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-14 08:32:42.000000 seven2one-4.2.0/MANIFEST.in
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-05-22 08:35:18.712959 seven2one-4.2.0/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2726 2023-05-22 07:46:14.000000 seven2one-4.2.0/README.md
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-05-22 08:35:18.712959 seven2one-4.2.0/setup.cfg
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1388 2023-04-25 08:08:15.000000 seven2one-4.2.0/setup.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.708959 seven2one-4.2.0/seven2one/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-05-22 08:35:13.000000 seven2one-4.2.0/seven2one/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15405 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/authorization.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    10848 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/automation.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    64496 2023-05-22 07:46:14.000000 seven2one-4.2.0/seven2one/core.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/email.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/fileImportService.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/fileimport.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.712959 seven2one-4.2.0/seven2one/logging_loki/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/logging_loki/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/logging_loki/const.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/logging_loki/emitter.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/logging_loki/handlers.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/programming.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     9486 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/schedule.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    61479 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.712959 seven2one-4.2.0/seven2one/utils/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-05-22 08:35:13.000000 seven2one-4.2.0/seven2one/utils/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35567 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/utils/ut.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_autprog.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_fileimport.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_init.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      989 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/utils/ut_log.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_meta.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_time.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6567 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/utils/ut_timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.712959 seven2one-4.2.0/seven2one.egg-info/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/SOURCES.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/dependency_links.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/not-zip-safe
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       97 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/requires.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/top_level.txt
```

### Comparing `seven2one-4.1.4/LICENSE` & `seven2one-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/PKG-INFO` & `seven2one-4.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.1.4
+Version: 4.2.0
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
@@ -82,7 +82,22 @@
         "fieldDATETIMEOFFSET": "2021-09-14T00:00:00.000Z"
     }
 ]
 
 addBasicItems('testInventory', items)
 
 ```
+
+## Advanced
+
+To change one or more used service endpoints (e.g. for tests against custom deployments) you can overwrite them by environment variables. You have to provide complete URL's.
+
+| Environment variable | Description | Example |
+| -------------------- | --|--|
+| TOKEN_URL                | Access token endpoint | `https://mytechstack/authn/connect/token` |
+| DYNAMIC_OBJECTS_ENDPOINT | DynO graphQL endpoint | `https://run.integrationtest.s2o.dev/itest-375545a3-dynamic-objects/graphql/` |
+| AUTOMATION_ENDPOINT      | Automation service graphQL endpoint |  |
+| SCHEDULE_ENDPOINT        | Schedule service graphQL endpoint | |
+| PROGRAMMING_ENDPOINT     | Programming service graphQL endpoint | |
+| TIMESERIES_ENDPOINT      | TimeSeries gateway graphQL endpoint | |
+| LOGGING_ENDPOINT         | Logging reverse proxy endpoint | `http://mytechstack:8123/loki/api/v1/push` |
+| AUTHORIZATION_ENDPOINT   | Authorization service graphQL endpoint | |
```

### Comparing `seven2one-4.1.4/README.md` & `seven2one-4.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -67,7 +67,22 @@
         "fieldDATETIMEOFFSET": "2021-09-14T00:00:00.000Z"
     }
 ]
 
 addBasicItems('testInventory', items)
 
 ```
+
+## Advanced
+
+To change one or more used service endpoints (e.g. for tests against custom deployments) you can overwrite them by environment variables. You have to provide complete URL's.
+
+| Environment variable | Description | Example |
+| -------------------- | --|--|
+| TOKEN_URL                | Access token endpoint | `https://mytechstack/authn/connect/token` |
+| DYNAMIC_OBJECTS_ENDPOINT | DynO graphQL endpoint | `https://run.integrationtest.s2o.dev/itest-375545a3-dynamic-objects/graphql/` |
+| AUTOMATION_ENDPOINT      | Automation service graphQL endpoint |  |
+| SCHEDULE_ENDPOINT        | Schedule service graphQL endpoint | |
+| PROGRAMMING_ENDPOINT     | Programming service graphQL endpoint | |
+| TIMESERIES_ENDPOINT      | TimeSeries gateway graphQL endpoint | |
+| LOGGING_ENDPOINT         | Logging reverse proxy endpoint | `http://mytechstack:8123/loki/api/v1/push` |
+| AUTHORIZATION_ENDPOINT   | Authorization service graphQL endpoint | |
```

### Comparing `seven2one-4.1.4/setup.py` & `seven2one-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/authorization.py` & `seven2one-4.2.0/seven2one/authorization.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/automation.py` & `seven2one-4.2.0/seven2one/automation.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/core.py` & `seven2one-4.2.0/seven2one/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,31 @@
             dynEndpoint = f'http://{host}:8050/graphql/'
             automationEndpoint = f'http://{host}:8120/graphql/'
             scheduleEndpoint = f'http://{host}:8130/graphql/'
             programmingEndpoint = f'http://{host}:8140/graphql/'
             tsGatewayEndpoint = f'http://{host}:8195/graphql/'
             logEndpoint = f'http://{host}:8175/loki/api/v1/push'
             authzEndpoint = f'http://{host}:8030/graphql/'
+        
+        if os.getenv("TOKEN_URL") != None:
+            tokenUrl = os.getenv("TOKEN_URL")
+        if os.getenv("DYNAMIC_OBJECTS_ENDPOINT") != None:
+            dynEndpoint = os.getenv("DYNAMIC_OBJECTS_ENDPOINT")
+        if os.getenv("AUTOMATION_ENDPOINT") != None:
+            automationEndpoint = os.getenv("AUTOMATION_ENDPOINT")
+        if os.getenv("SCHEDULE_ENDPOINT") != None:
+            scheduleEndpoint = os.getenv("SCHEDULE_ENDPOINT")
+        if os.getenv("PROGRAMMING_ENDPOINT") != None:
+            programmingEndpoint = os.getenv("PROGRAMMING_ENDPOINT")
+        if os.getenv("TIMESERIES_ENDPOINT") != None:
+            tsGatewayEndpoint = os.getenv("TIMESERIES_ENDPOINT")
+        if os.getenv("LOGGING_ENDPOINT") != None:
+            logEndpoint = os.getenv("LOGGING_ENDPOINT")
+        if os.getenv("AUTHORIZATION_ENDPOINT") != None:
+            authzEndpoint = os.getenv("AUTHORIZATION_ENDPOINT")
 
         token = accessToken if accessToken != None else self._getAccessToken(tokenUrl, user, password, proxies, timeout)
         if token == None:
             return
 
         if logToServer:
             if os.getenv("LOG_SERVER") != None:
@@ -283,20 +300,23 @@
     def updateClient(self) -> None:
         """
         Updates the client scheme and structures, e.g. after adding inventories
         or new inventory properties.
         """
 
         self.client = Utils._create_client(self)
+        graphQLString = Structure._introspectionQueryString()
+        self.scheme = Utils._executeGraphQL(self, graphQLString)
         self.structure = Utils._executeGraphQL(self, Structure.queryStructure)
         self.structure = Structure._fullStructureDict(self.structure)
         self.objects = Structure._fullStructureNT(self.structure)
         self.inventory = Structure._inventoryNT(self.structure)
         self.inventoryProperty = Structure._inventoryPropertyNT(self.structure)
-        self.scheme = self.client.introspection
+        # reninit relevant gateways
+        self.TimeSeries = TimeSeries(self.accessToken, self.TimeSeries.endpoint, self)
 
         return
 
     def inventories(
         self, 
         fields:list=None, 
         where:str=None,
```

### Comparing `seven2one-4.1.4/seven2one/email.py` & `seven2one-4.2.0/seven2one/email.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/fileImportService.py` & `seven2one-4.2.0/seven2one/fileImportService.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/fileimport.py` & `seven2one-4.2.0/seven2one/fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/logging_loki/const.py` & `seven2one-4.2.0/seven2one/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/logging_loki/emitter.py` & `seven2one-4.2.0/seven2one/logging_loki/emitter.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/logging_loki/handlers.py` & `seven2one-4.2.0/seven2one/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/programming.py` & `seven2one-4.2.0/seven2one/programming.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/schedule.py` & `seven2one-4.2.0/seven2one/schedule.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/timeseries.py` & `seven2one-4.2.0/seven2one/timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/utils/ut.py` & `seven2one-4.2.0/seven2one/utils/ut.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/utils/ut_autprog.py` & `seven2one-4.2.0/seven2one/utils/ut_autprog.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/utils/ut_fileimport.py` & `seven2one-4.2.0/seven2one/utils/ut_fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/utils/ut_init.py` & `seven2one-4.2.0/seven2one/utils/ut_init.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/utils/ut_log.py` & `seven2one-4.2.0/seven2one/utils/ut_log.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/utils/ut_meta.py` & `seven2one-4.2.0/seven2one/utils/ut_meta.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/utils/ut_time.py` & `seven2one-4.2.0/seven2one/utils/ut_time.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one/utils/ut_timeseries.py` & `seven2one-4.2.0/seven2one/utils/ut_timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.4/seven2one.egg-info/PKG-INFO` & `seven2one-4.2.0/seven2one.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.1.4
+Version: 4.2.0
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
@@ -82,7 +82,22 @@
         "fieldDATETIMEOFFSET": "2021-09-14T00:00:00.000Z"
     }
 ]
 
 addBasicItems('testInventory', items)
 
 ```
+
+## Advanced
+
+To change one or more used service endpoints (e.g. for tests against custom deployments) you can overwrite them by environment variables. You have to provide complete URL's.
+
+| Environment variable | Description | Example |
+| -------------------- | --|--|
+| TOKEN_URL                | Access token endpoint | `https://mytechstack/authn/connect/token` |
+| DYNAMIC_OBJECTS_ENDPOINT | DynO graphQL endpoint | `https://run.integrationtest.s2o.dev/itest-375545a3-dynamic-objects/graphql/` |
+| AUTOMATION_ENDPOINT      | Automation service graphQL endpoint |  |
+| SCHEDULE_ENDPOINT        | Schedule service graphQL endpoint | |
+| PROGRAMMING_ENDPOINT     | Programming service graphQL endpoint | |
+| TIMESERIES_ENDPOINT      | TimeSeries gateway graphQL endpoint | |
+| LOGGING_ENDPOINT         | Logging reverse proxy endpoint | `http://mytechstack:8123/loki/api/v1/push` |
+| AUTHORIZATION_ENDPOINT   | Authorization service graphQL endpoint | |
```

### Comparing `seven2one-4.1.4/seven2one.egg-info/SOURCES.txt` & `seven2one-4.2.0/seven2one.egg-info/SOURCES.txt`

 * *Files identical despite different names*

