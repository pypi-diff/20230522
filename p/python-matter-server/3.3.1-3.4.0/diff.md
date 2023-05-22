# Comparing `tmp/python-matter-server-3.3.1.tar.gz` & `tmp/python-matter-server-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.3.1.tar", last modified: Tue Apr 18 09:07:44 2023, max compression
+gzip compressed data, was "python-matter-server-3.4.0.tar", last modified: Mon May 22 13:05:25 2023, max compression
```

## Comparing `python-matter-server-3.3.1.tar` & `python-matter-server-3.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.153157 python-matter-server-3.3.1/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.153157 python-matter-server-3.3.1/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.153157 python-matter-server-3.3.1/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-18 09:07:44.000000 python-matter-server-3.3.1/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:07:41.000000 python-matter-server-3.3.1/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-22 13:05:14.000000 python-matter-server-3.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:05:23.000000 python-matter-server-3.4.0/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 13:05:25.000000 python-matter-server-3.4.0/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 13:05:25.701075 python-matter-server-3.4.0/setup.cfg
```

### Comparing `python-matter-server-3.3.1/LICENSE` & `python-matter-server-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/PKG-INFO` & `python-matter-server-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.3.1
+Version: 3.4.0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.3.1/README.md` & `python-matter-server-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/client/client.py` & `python-matter-server-3.4.0/matter_server/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,24 +133,24 @@
         await self.send_command(APICommand.SET_THREAD_DATASET, dataset=dataset)
 
     async def open_commissioning_window(
         self,
         node_id: int,
         timeout: int = 300,
         iteration: int = 1000,
-        option: int = 0,
+        option: int = 1,
         discriminator: Optional[int] = None,
-    ) -> int:
+    ) -> tuple[int, str]:
         """
         Open a commissioning window to commission a device present on this controller to another.
 
         Returns code to use as discriminator.
         """
         return cast(
-            int,
+            tuple[int, str],
             await self.send_command(
                 APICommand.OPEN_COMMISSIONING_WINDOW,
                 node_id=node_id,
                 timeout=timeout,
                 iteration=iteration,
                 option=option,
                 discriminator=discriminator,
@@ -179,15 +179,15 @@
 
         return [
             MatterFabricData(
                 fabric_id=f.fabricId,
                 vendor_id=f.vendorId,
                 fabric_index=f.fabricIndex,
                 fabric_label=f.label if f.label else None,
-                vendor_name=vendors_map.get(f.vendorId),
+                vendor_name=vendors_map.get(str(f.vendorId)),
             )
             for f in fabrics
         ]
 
     async def remove_matter_fabric(self, node_id: int, fabric_index: int) -> None:
         """Remove Matter fabric from a device."""
         await self.send_device_command(
```

### Comparing `python-matter-server-3.3.1/matter_server/client/connection.py` & `python-matter-server-3.4.0/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/client/exceptions.py` & `python-matter-server-3.4.0/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/client/models/device_types.py` & `python-matter-server-3.4.0/matter_server/client/models/device_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
 
 class BridgedDevice(DeviceType, device_type=0x0013):
     """Bridged Device."""
 
     clusters = {
         all_clusters.Descriptor,
-        all_clusters.BridgedDeviceBasic,
+        all_clusters.BridgedDeviceBasicInformation,
         all_clusters.PowerSourceConfiguration,
         all_clusters.PowerSource,
     }
 
 
 class OnOffLight(DeviceType, device_type=0x0100):
     """On/Off Light."""
```

### Comparing `python-matter-server-3.3.1/matter_server/client/models/node.py` & `python-matter-server-3.4.0/matter_server/client/models/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         Return device info.
 
         If this endpoint represents a BridgedDevice, returns BridgedDeviceBasic.
         If this endpoint represents a ComposedDevice, returns the info of the compose device.
         Otherwise, returns BasicInformation from the Node itself (endpoint 0).
         """
         if self.is_bridged_device:
-            return self.get_cluster(Clusters.BridgedDeviceBasic)
+            return self.get_cluster(Clusters.BridgedDeviceBasicInformation)
         if compose_parent := self.node.get_compose_parent(self.endpoint_id):
             return compose_parent.device_info
         return self.node.device_info
 
     def has_cluster(self, cluster: type[_CLUSTER_T] | int) -> bool:
         """Check if endpoint has a specific cluster."""
         if isinstance(cluster, type):
@@ -196,15 +196,15 @@
         # unwrap cluster and clusterattributes from raw node data attributes
         for attribute_path, attribute_value in attributes_data.items():
             self.set_attribute_value(attribute_path, attribute_value)
         # extract device types from Descriptor Cluster
         cluster = self.get_cluster(Clusters.Descriptor)
         assert cluster is not None
         for dev_info in cluster.deviceTypeList:  # type: ignore[unreachable]
-            device_type = DEVICE_TYPES.get(dev_info.type)
+            device_type = DEVICE_TYPES.get(dev_info.deviceType)
             if device_type is None:
                 LOGGER.debug("Found unknown device type %s", dev_info)
                 continue
             self.device_types.add(device_type)
 
     def __repr__(self) -> str:
         """Return the representation."""
```

### Comparing `python-matter-server-3.3.1/matter_server/common/errors.py` & `python-matter-server-3.4.0/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/common/helpers/api.py` & `python-matter-server-3.4.0/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/common/helpers/json.py` & `python-matter-server-3.4.0/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/common/helpers/util.py` & `python-matter-server-3.4.0/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/common/models.py` & `python-matter-server-3.4.0/matter_server/common/models.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/server/__main__.py` & `python-matter-server-3.4.0/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/server/client_handler.py` & `python-matter-server-3.4.0/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/server/const.py` & `python-matter-server-3.4.0/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/server/device_controller.py` & `python-matter-server-3.4.0/matter_server/server/device_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,37 +236,37 @@
 
     @api_command(APICommand.OPEN_COMMISSIONING_WINDOW)
     async def open_commissioning_window(
         self,
         node_id: int,
         timeout: int = 300,
         iteration: int = 1000,
-        option: int = 0,
+        option: int = 1,
         discriminator: int | None = None,
-    ) -> int:
+    ) -> tuple[int, str]:
         """
         Open a commissioning window to commission a device present on this controller to another.
 
         Returns code to use as discriminator.
         """
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
         if discriminator is None:
             discriminator = 3840  # TODO generate random one
 
-        await self._call_sdk(
+        pin, code = await self._call_sdk(
             self.chip_controller.OpenCommissioningWindow,
             nodeid=node_id,
             timeout=timeout,
             iteration=iteration,
             discriminator=discriminator,
             option=option,
         )
-        return discriminator
+        return pin, code
 
     @api_command(APICommand.DISCOVER)
     async def discover_commissionable_nodes(
         self,
     ) -> CommissionableNode | list[CommissionableNode] | None:
         """Discover Commissionable Nodes (discovered on BLE or mDNS)."""
         if self.chip_controller is None:
```

### Comparing `python-matter-server-3.3.1/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.4.0/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/server/server.py` & `python-matter-server-3.4.0/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/server/stack.py` & `python-matter-server-3.4.0/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/server/storage.py` & `python-matter-server-3.4.0/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.1/matter_server/server/vendor_info.py` & `python-matter-server-3.4.0/matter_server/server/vendor_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     async def get_vendor_names(
         self, filter_vendors: list[int] | None = None
     ) -> dict[int, str]:
         """Get a map of vendor ids to vendor names."""
         if filter_vendors:
             vendors: dict[int, str] = {}
             for vendor_id in filter_vendors:
-                if vendor_id in filter_vendors:
+                if vendor_id in filter_vendors and vendor_id in self._data:
                     vendors[vendor_id] = self._data[vendor_id].vendor_name
             return vendors
 
         return {
             vendor_id: vendor_info.vendor_name
             for vendor_id, vendor_info in self._data.items()
         }
```

### Comparing `python-matter-server-3.3.1/pyproject.toml` & `python-matter-server-3.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.3.1"
+version = "3.4.0"
 license     = {text = "Apache-2.0"}
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
@@ -22,29 +22,29 @@
 ]
 dependencies = [
   "aiohttp",
   "aiorun",
   "coloredlogs",
   "dacite",
   "orjson",
-  "home-assistant-chip-clusters==2023.4.1"
+  "home-assistant-chip-clusters==2023.5.1"
 ]
 
 [project.optional-dependencies]
 server = [
-  "home-assistant-chip-core==2023.4.1",
+  "home-assistant-chip-core==2023.5.1",
   "cryptography==40.0.2"
 ]
 test = [
   "black==23.3.0",
   "flake8==6.0.0",
   "flake8-docstrings==1.7.0",
   "isort==5.12.0",
-  "mypy==1.2.0",
-  "pylint==2.17.2",
+  "mypy==1.3.0",
+  "pylint==2.17.4",
   "pytest==7.3.1",
   "pytest-aiohttp==1.0.4",
   "pytest-cov==4.0.0",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
```

### Comparing `python-matter-server-3.3.1/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.4.0/python_matter_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.3.1
+Version: 3.4.0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.3.1/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.4.0/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

