# Comparing `tmp/plantstar-shared-2.0.2.0.3.tar.gz` & `tmp/plantstar-shared-2.0.2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantstar-shared-2.0.2.0.3.tar", last modified: Tue Dec  6 18:13:05 2022, max compression
+gzip compressed data, was "plantstar-shared-2.0.2.3.2.tar", last modified: Mon May 22 15:46:39 2023, max compression
```

## Comparing `plantstar-shared-2.0.2.0.3.tar` & `plantstar-shared-2.0.2.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:13:05.491906 plantstar-shared-2.0.2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-06 18:13:05.491906 plantstar-shared-2.0.2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:13:05.491906 plantstar-shared-2.0.2.0.3/plantstar_shared/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/DataCollectionModuleProcessNames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/HuskyInterfacePacketTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/MockRawDataProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/RawDataProcessorInterfaceActions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/SysconType.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/add_size_onto_string_and_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/api_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/convert_bytes_to_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/convert_object_to_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/global_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/is_valid_signed_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/syscon_image_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/syscon_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/plantstar_shared/tcp_socket_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:13:05.491906 plantstar-shared-2.0.2.0.3/plantstar_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-06 18:13:05.000000 plantstar-shared-2.0.2.0.3/plantstar_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2022-12-06 18:13:05.000000 plantstar-shared-2.0.2.0.3/plantstar_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 18:13:05.000000 plantstar-shared-2.0.2.0.3/plantstar_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-06 18:13:05.000000 plantstar-shared-2.0.2.0.3/plantstar_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-06 18:13:05.000000 plantstar-shared-2.0.2.0.3/plantstar_shared.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 18:13:05.491906 plantstar-shared-2.0.2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2022-12-06 18:12:51.000000 plantstar-shared-2.0.2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:39.166085 plantstar-shared-2.0.2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 15:46:39.166085 plantstar-shared-2.0.2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:39.166085 plantstar-shared-2.0.2.3.2/plantstar_shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/DataCollectionModuleProcessNames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/HuskyInterfacePacketTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/MockRawDataProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/RawDataProcessorInterfaceActions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/SysconType.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/add_size_onto_string_and_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/api_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/convert_bytes_to_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/convert_object_to_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/global_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/is_valid_signed_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/syscon_image_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/syscon_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/plantstar_shared/tcp_socket_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:39.166085 plantstar-shared-2.0.2.3.2/plantstar_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 15:46:39.000000 plantstar-shared-2.0.2.3.2/plantstar_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-22 15:46:39.000000 plantstar-shared-2.0.2.3.2/plantstar_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:46:39.000000 plantstar-shared-2.0.2.3.2/plantstar_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 15:46:39.000000 plantstar-shared-2.0.2.3.2/plantstar_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 15:46:39.000000 plantstar-shared-2.0.2.3.2/plantstar_shared.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:46:39.166085 plantstar-shared-2.0.2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-22 15:46:27.000000 plantstar-shared-2.0.2.3.2/setup.py
```

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared/HuskyInterfacePacketTypes.py` & `plantstar-shared-2.0.2.3.2/plantstar_shared/HuskyInterfacePacketTypes.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared/MockRawDataProcessor.py` & `plantstar-shared-2.0.2.3.2/plantstar_shared/MockRawDataProcessor.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared/RawDataProcessorInterfaceActions.py` & `plantstar-shared-2.0.2.3.2/plantstar_shared/RawDataProcessorInterfaceActions.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared/SysconType.py` & `plantstar-shared-2.0.2.3.2/plantstar_shared/SysconType.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared/api_types.py` & `plantstar-shared-2.0.2.3.2/plantstar_shared/api_types.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared/global_definitions.py` & `plantstar-shared-2.0.2.3.2/plantstar_shared/global_definitions.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py` & `plantstar-shared-2.0.2.3.2/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared/syscon_json.py` & `plantstar-shared-2.0.2.3.2/plantstar_shared/syscon_json.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared/tcp_socket_utils.py` & `plantstar-shared-2.0.2.3.2/plantstar_shared/tcp_socket_utils.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/plantstar_shared.egg-info/SOURCES.txt` & `plantstar-shared-2.0.2.3.2/plantstar_shared.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.2.0.3/setup.py` & `plantstar-shared-2.0.2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as file_handle:
     long_description = file_handle.read()
 
 setuptools.setup(
     name="plantstar-shared",
     # MAJOR_VERSION.MINOR_VERSION.MAJOR_PATCH_VERSION.MINOR_PATCH_VERSION.SUBVERSION
-    version="2.0.2.0.3",
+    version="2.0.2.3.2",
     author="SYSCON International",
     author_email="dev@syscon-intl.com",
     description="Shared code used in plantstar_apu and plantstar_dcm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SYSCON-International/plantstar_shared",
     packages=setuptools.find_packages(),
```

