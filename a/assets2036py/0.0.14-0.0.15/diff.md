# Comparing `tmp/assets2036py-0.0.14.tar.gz` & `tmp/assets2036py-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assets2036py-0.0.14.tar", last modified: Mon Nov  7 10:22:50 2022, max compression
+gzip compressed data, was "assets2036py-0.0.15.tar", last modified: Mon May 22 12:07:10 2023, max compression
```

## Comparing `assets2036py-0.0.14.tar` & `assets2036py-0.0.15.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 10:22:50.163215 assets2036py-0.0.14/
--rw-r--r--   0 runner    (1001) docker     (121)    11347 2022-11-07 10:22:36.000000 assets2036py-0.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-11-07 10:22:36.000000 assets2036py-0.0.14/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-11-07 10:22:50.163215 assets2036py-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-11-07 10:22:36.000000 assets2036py-0.0.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 10:22:50.159215 assets2036py-0.0.14/assets2036py/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-11-07 10:22:36.000000 assets2036py-0.0.14/assets2036py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9204 2022-11-07 10:22:36.000000 assets2036py-0.0.14/assets2036py/assetmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)    14611 2022-11-07 10:22:36.000000 assets2036py-0.0.14/assets2036py/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)    11757 2022-11-07 10:22:36.000000 assets2036py-0.0.14/assets2036py/communication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-11-07 10:22:36.000000 assets2036py-0.0.14/assets2036py/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 10:22:50.163215 assets2036py-0.0.14/assets2036py/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-07 10:22:36.000000 assets2036py-0.0.14/assets2036py/resources/_endpoint.json
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-11-07 10:22:36.000000 assets2036py-0.0.14/assets2036py/resources/submodel_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-11-07 10:22:36.000000 assets2036py-0.0.14/assets2036py/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 10:22:50.159215 assets2036py-0.0.14/assets2036py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-11-07 10:22:50.000000 assets2036py-0.0.14/assets2036py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-11-07 10:22:50.000000 assets2036py-0.0.14/assets2036py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 10:22:50.000000 assets2036py-0.0.14/assets2036py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-07 10:22:50.000000 assets2036py-0.0.14/assets2036py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-07 10:22:50.000000 assets2036py-0.0.14/assets2036py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 10:22:50.163215 assets2036py-0.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-11-07 10:22:36.000000 assets2036py-0.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-22 12:06:59.000000 assets2036py-0.0.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-22 12:06:59.000000 assets2036py-0.0.15/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 12:07:10.121992 assets2036py-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-22 12:06:59.000000 assets2036py-0.0.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/assets2036py/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/assetmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/assets2036py/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/resources/_endpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/resources/submodel_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/assets2036py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:07:10.121992 assets2036py-0.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-22 12:06:59.000000 assets2036py-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27893 2023-05-22 12:06:59.000000 assets2036py-0.0.15/tests/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-22 12:06:59.000000 assets2036py-0.0.15/tests/test_assetmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-22 12:06:59.000000 assets2036py-0.0.15/tests/test_utils.py
```

### Comparing `assets2036py-0.0.14/LICENSE` & `assets2036py-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.14/NOTICE` & `assets2036py-0.0.15/NOTICE`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.14/PKG-INFO` & `assets2036py-0.0.15/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assets2036py
-Version: 0.0.14
+Version: 0.0.15
 Summary: helper library to easily implement assets2036
 Home-page: https://github.com/boschresearch/assets2036-submodels
 Author: Daniel Ewert (CR/APA3 G6/BD-BBI)
 Author-email: Daniel.Ewert@de.bosch.com
 License: BIOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `assets2036py-0.0.14/assets2036py/__init__.py` & `assets2036py-0.0.15/assets2036py/__init__.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.14/assets2036py/assetmanager.py` & `assets2036py-0.0.15/assets2036py/assetmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 import ssl
 import json
 import os
 import logging
 from urllib.request import urlopen
 from threading import Thread, Event
-from assets2036py import Asset, Mode
+from assets2036py import Asset, Mode, ProxyAsset
 from assets2036py.exceptions import AssetNotFoundError, OperationTimeoutException
 from assets2036py.communication import CommunicationClient, MQTTClient
 from assets2036py.utilities import get_resource_path
 
 
 logger = logging.getLogger(__name__)
 
-#pylint: disable=line-too-long
+# pylint: disable=line-too-long
 
 
 class AssetManager:
     """Primary entrypoint for working with assets.
     Manages the creation of assets and asset proxies (the latter are used to talk to remote assets).
 
     """
@@ -195,15 +195,15 @@
 
         Returns:
             list: list of found asset names
         """
 
         return self.client.query_asset_names(namespace, *submodel_names)
 
-    def create_asset_proxy(self, namespace: str, name: str) -> Asset:
+    def create_asset_proxy(self, namespace: str, name: str) -> ProxyAsset:
         """Returns the asset with the given name if found, raises AssetNotFoundError otherwise
 
         Args:
             namespace (str): namespace to use
             name (str): name of asset to use
 
         Raises:
@@ -211,17 +211,17 @@
 
         Returns:
             Asset: returns Asset proxy to be used to communicate with remote asset
         """
         submodels = self.client.query_submodels_for_asset(namespace, name)
         if not submodels:
             raise AssetNotFoundError
-        verified_submodels = self._get_submodel_schemata(submodels)
-        return Asset(name, namespace, *verified_submodels, mode=Mode.CONSUMER, communication_client=self.client,
-                     endpoint_name=self.endpoint_name)
+        # verified_submodels = self._get_submodel_schemata(submodels)
+        return ProxyAsset(name, namespace, *submodels.values(), mode=Mode.CONSUMER, communication_client=self.client,
+                          endpoint_name=self.endpoint_name)
 
     def _get_submodel_schemata(self, sub_models):
         # pylint: disable=protected-access,broad-except
         schemata = []
         for meta in sub_models.values():
             try:
                 url = meta["submodel_url"]
```

### Comparing `assets2036py-0.0.14/assets2036py/assets.py` & `assets2036py-0.0.15/assets2036py/assets.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import traceback
 from json import JSONDecodeError
 from urllib.request import urlopen
 from abc import ABC, abstractmethod
 from numbers import Number
 import jsonschema
 from assets2036py.exceptions import InvalidParameterException, NotWritableError
-from .utilities import sanitize
+from .utilities import sanitize, get_resource_path
 
 # pylint: disable=protected-access, line-too-long
 
 
 logger = logging.getLogger(__name__)
 schema_file = path.abspath(path.dirname(__file__)) + \
     "/resources/submodel_schema.json"
@@ -268,14 +268,15 @@
     }
 
     def __init__(self, asset, submodel_definition):
         # pylint: disable=no-member
         self.parent = asset
         self.communication_client = asset.communication_client
         self.name = sanitize(submodel_definition["name"])
+        self._disconnect_callback = None
 
         if asset.access_mode == Mode.OWNER:
 
             meta_prop = WritableProperty("_meta", self, self.meta_property)
 
             setattr(self, "_meta", meta_prop)
 
@@ -290,14 +291,36 @@
             if "properties" in submodel_definition:
                 self._create_readonly_properties(submodel_definition)
             if "operations" in submodel_definition:
                 self._create_callable_operations(submodel_definition)
             if "events" in submodel_definition:
                 self._create_subscribable_events(submodel_definition)
 
+    def _raise_offline_exception(self, online):
+        logger.debug("CALLBACK GOT %s", online)
+        if not online and self._disconnect_callback != None:
+            logger.debug("SEND DISCONNECT FOR %s", self.name)
+            self._disconnect_callback(self.name)
+
+    def on_disconnect(self, callback):
+        self._disconnect_callback = callback
+
+    def register_source(self, source_address):
+        if "/" in source_address:
+            namespace, source_asset = source_address.split("/")
+        else:
+            namespace = self.parent.namespace
+            source_asset = source_address
+        with open(get_resource_path("_endpoint.json")) as file:
+            endpoint_sm_definition = json.load(file)
+        self.endpoint_asset = Asset(source_asset, namespace,
+                                    endpoint_sm_definition, mode=Mode.CONSUMER, communication_client=self.communication_client, endpoint_name="")
+        self.endpoint_asset._endpoint.online.on_change(
+            self._raise_offline_exception)
+
     def delete(self):
         deletables = [getattr(self, prop) for prop in dir(
             self) if type(getattr(self, prop)) == WritableProperty]
         deletables.extend(getattr(self, prop) for prop in dir(
             self) if type(getattr(self, prop)) == BindableOperation)
         for d in deletables:
             d.delete()
@@ -397,7 +420,28 @@
                                   "submodel_url": submodel_url if submodel_url else "file://localhost"}
         submodel_name = submodel_def['name'].replace("-", "_").replace(" ", "")
         self.sub_model_names.append(submodel_name)
         setattr(self, submodel_name, new_sm)
 
     def _get_topic(self):
         return f"{self.namespace}/{self.name}"
+
+
+class ProxyAsset(Asset):
+
+    def __init__(self, name: str, namespace: str, *meta_infos, mode=Mode.CONSUMER, communication_client, endpoint_name) -> None:
+        submodel_defs = []
+        sources = {}
+        for meta_info in meta_infos:
+            sm_def = meta_info["submodel_definition"]
+            submodel_defs.append(sm_def)
+            sources[sm_def["name"]] = meta_info["source"]
+
+        super().__init__(name, namespace, *submodel_defs, mode=mode,
+                         communication_client=communication_client, endpoint_name=endpoint_name)
+        for name, source in sources.items():
+            getattr(self, name).register_source(source)
+            # this is some hacky shit, we need some nicer refactoring here
+
+    def on_disconnect(self, callback):
+        for submodel in self.sub_model_names:
+            getattr(self, submodel).on_disconnect(callback)
```

### Comparing `assets2036py-0.0.14/assets2036py/communication.py` & `assets2036py-0.0.15/assets2036py/communication.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.14/assets2036py/exceptions.py` & `assets2036py-0.0.15/assets2036py/exceptions.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.14/assets2036py/resources/_endpoint.json` & `assets2036py-0.0.15/assets2036py/resources/_endpoint.json`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.14/assets2036py/resources/submodel_schema.json` & `assets2036py-0.0.15/assets2036py/resources/submodel_schema.json`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.14/assets2036py/utilities.py` & `assets2036py-0.0.15/assets2036py/utilities.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.14/assets2036py.egg-info/PKG-INFO` & `assets2036py-0.0.15/assets2036py.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assets2036py
-Version: 0.0.14
+Version: 0.0.15
 Summary: helper library to easily implement assets2036
 Home-page: https://github.com/boschresearch/assets2036-submodels
 Author: Daniel Ewert (CR/APA3 G6/BD-BBI)
 Author-email: Daniel.Ewert@de.bosch.com
 License: BIOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `assets2036py-0.0.14/setup.py` & `assets2036py-0.0.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='assets2036py',
-    version='0.0.14',
+    version='0.0.15',
     url='https://github.com/boschresearch/assets2036-submodels',
     license='BIOS',
     author='Daniel Ewert (CR/APA3 G6/BD-BBI)',
     author_email='Daniel.Ewert@de.bosch.com',
     description='helper library to easily implement assets2036',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

