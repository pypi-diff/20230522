# Comparing `tmp/azure-mgmt-appcontainers-2.0.0b2.zip` & `tmp/azure-mgmt-appcontainers-3.0.0b1.zip`

## zipinfo {}

```diff
@@ -1,87 +1,93 @@
-Zip file size: 225548 bytes, number of entries: 85
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure/
--rw-rw-r--  2.0 unx    15997 b- defN 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/PKG-INFO
--rw-rw-r--  2.0 unx     2832 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/setup.py
--rw-rw-r--  2.0 unx      219 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/MANIFEST.in
--rw-rw-r--  2.0 unx       38 b- defN 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/setup.cfg
--rw-rw-r--  2.0 unx     2143 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/README.md
--rw-rw-r--  2.0 unx      614 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/_meta.json
--rw-rw-r--  2.0 unx    12953 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/CHANGELOG.md
--rw-rw-r--  2.0 unx     1074 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/LICENSE
--rw-rw-r--  2.0 unx    15997 b- defN 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx      116 b- defN 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/requires.txt
--rw-rw-r--  2.0 unx     4388 b- defN 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        1 b- defN 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/top_level.txt
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/
--rw-rw-r--  2.0 unx       65 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/
--rw-rw-r--  2.0 unx     3741 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_configuration.py
--rw-rw-r--  2.0 unx    77872 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_serialization.py
--rw-rw-r--  2.0 unx    11427 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_container_apps_api_client.py
--rw-rw-r--  2.0 unx       26 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/py.typed
--rw-rw-r--  2.0 unx     1169 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_vendor.py
--rw-rw-r--  2.0 unx      488 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_version.py
--rw-rw-r--  2.0 unx     1530 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_patch.py
--rw-rw-r--  2.0 unx      907 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/__init__.py
--rw-rw-r--  2.0 unx    28036 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_diagnostics_operations.py
--rw-rw-r--  2.0 unx     6007 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_billing_meters_operations.py
--rw-rw-r--  2.0 unx     6721 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environments_diagnostics_operations.py
--rw-rw-r--  2.0 unx     6743 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_operations.py
--rw-rw-r--  2.0 unx    60048 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environments_operations.py
--rw-rw-r--  2.0 unx    50649 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_operations.py
--rw-rw-r--  2.0 unx    62915 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_operations.py
--rw-rw-r--  2.0 unx     7722 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_available_workload_profiles_operations.py
--rw-rw-r--  2.0 unx    10870 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_namespaces_operations.py
--rw-rw-r--  2.0 unx    11909 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_revision_replicas_operations.py
--rw-rw-r--  2.0 unx    24430 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environments_storages_operations.py
--rw-rw-r--  2.0 unx    30537 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_dapr_components_operations.py
--rw-rw-r--  2.0 unx    26079 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_auth_configs_operations.py
--rw-rw-r--  2.0 unx    34615 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_certificates_operations.py
--rw-rw-r--  2.0 unx    35434 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_certificates_operations.py
--rw-rw-r--  2.0 unx    25014 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_storages_operations.py
--rw-rw-r--  2.0 unx    31236 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_dapr_components_operations.py
--rw-rw-r--  2.0 unx    26578 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_revisions_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_patch.py
--rw-rw-r--  2.0 unx    34289 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_source_controls_operations.py
--rw-rw-r--  2.0 unx    11399 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environment_diagnostics_operations.py
--rw-rw-r--  2.0 unx     3147 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-30 03:00 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/
--rw-rw-r--  2.0 unx     3789 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/_configuration.py
--rw-rw-r--  2.0 unx    11634 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/_container_apps_api_client.py
--rw-rw-r--  2.0 unx     1530 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/_patch.py
--rw-rw-r--  2.0 unx      854 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/__init__.py
--rw-rw-r--  2.0 unx    20647 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_diagnostics_operations.py
--rw-rw-r--  2.0 unx     4808 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_billing_meters_operations.py
--rw-rw-r--  2.0 unx     5282 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environments_diagnostics_operations.py
--rw-rw-r--  2.0 unx     6039 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    49509 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environments_operations.py
--rw-rw-r--  2.0 unx    41117 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_operations.py
--rw-rw-r--  2.0 unx    50692 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_operations.py
--rw-rw-r--  2.0 unx     6542 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_available_workload_profiles_operations.py
--rw-rw-r--  2.0 unx     9191 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_namespaces_operations.py
--rw-rw-r--  2.0 unx     8696 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_revision_replicas_operations.py
--rw-rw-r--  2.0 unx    18248 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environments_storages_operations.py
--rw-rw-r--  2.0 unx    22870 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_dapr_components_operations.py
--rw-rw-r--  2.0 unx    19933 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_auth_configs_operations.py
--rw-rw-r--  2.0 unx    26717 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_certificates_operations.py
--rw-rw-r--  2.0 unx    27231 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_certificates_operations.py
--rw-rw-r--  2.0 unx    18634 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_storages_operations.py
--rw-rw-r--  2.0 unx    23328 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_dapr_components_operations.py
--rw-rw-r--  2.0 unx    18983 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_revisions_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    28319 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_source_controls_operations.py
--rw-rw-r--  2.0 unx     8452 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environment_diagnostics_operations.py
--rw-rw-r--  2.0 unx     3147 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   287908 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/_models_py3.py
--rw-rw-r--  2.0 unx     8459 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/_container_apps_api_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/_patch.py
--rw-rw-r--  2.0 unx    14467 b- defN 22-Dec-30 02:59 azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/__init__.py
-85 files, 1437095 bytes uncompressed, 204366 bytes compressed:  85.8%
+Zip file size: 254073 bytes, number of entries: 91
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/
+-rw-rw-r--  2.0 unx    17172 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx      219 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx    20245 b- defN 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx     1074 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/LICENSE
+-rw-rw-r--  2.0 unx     2172 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/README.md
+-rw-rw-r--  2.0 unx     2840 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/setup.py
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/setup.cfg
+-rw-rw-r--  2.0 unx      614 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/_meta.json
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/py.typed
+-rw-rw-r--  2.0 unx     3508 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_configuration.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_serialization.py
+-rw-rw-r--  2.0 unx      907 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/__init__.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_patch.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_vendor.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_version.py
+-rw-rw-r--  2.0 unx    12360 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_container_apps_api_client.py
+-rw-rw-r--  2.0 unx    16235 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/_patch.py
+-rw-rw-r--  2.0 unx     8829 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/_container_apps_api_client_enums.py
+-rw-rw-r--  2.0 unx   331104 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/
+-rw-rw-r--  2.0 unx     3556 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/_configuration.py
+-rw-rw-r--  2.0 unx      854 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/__init__.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/_patch.py
+-rw-rw-r--  2.0 unx    12584 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/_container_apps_api_client.py
+-rw-rw-r--  2.0 unx     5799 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx     8438 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_revision_replicas_operations.py
+-rw-rw-r--  2.0 unx    26952 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_certificates_operations.py
+-rw-rw-r--  2.0 unx    19656 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_auth_configs_operations.py
+-rw-rw-r--  2.0 unx     3425 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    41122 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_operations.py
+-rw-rw-r--  2.0 unx    18687 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_revisions_operations.py
+-rw-rw-r--  2.0 unx    18370 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_storages_operations.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_available_workload_profiles_operations.py
+-rw-rw-r--  2.0 unx    71800 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_jobs_operations.py
+-rw-rw-r--  2.0 unx    20355 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_diagnostics_operations.py
+-rw-rw-r--  2.0 unx    32916 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_certificates_operations.py
+-rw-rw-r--  2.0 unx    27965 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_source_controls_operations.py
+-rw-rw-r--  2.0 unx     4564 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_billing_meters_operations.py
+-rw-rw-r--  2.0 unx    50792 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_operations.py
+-rw-rw-r--  2.0 unx    23040 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_dapr_components_operations.py
+-rw-rw-r--  2.0 unx    49069 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environments_operations.py
+-rw-rw-r--  2.0 unx     8970 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    26438 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_certificates_operations.py
+-rw-rw-r--  2.0 unx    22582 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_dapr_components_operations.py
+-rw-rw-r--  2.0 unx    17982 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environments_storages_operations.py
+-rw-rw-r--  2.0 unx     5038 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environments_diagnostics_operations.py
+-rw-rw-r--  2.0 unx     8194 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environment_diagnostics_operations.py
+-rw-rw-r--  2.0 unx     6615 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_jobs_executions_operations.py
+-rw-rw-r--  2.0 unx     6493 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_operations.py
+-rw-rw-r--  2.0 unx    11631 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_revision_replicas_operations.py
+-rw-rw-r--  2.0 unx    35105 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_certificates_operations.py
+-rw-rw-r--  2.0 unx    25762 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_auth_configs_operations.py
+-rw-rw-r--  2.0 unx     3425 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_patch.py
+-rw-rw-r--  2.0 unx    50567 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_operations.py
+-rw-rw-r--  2.0 unx    26232 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_revisions_operations.py
+-rw-rw-r--  2.0 unx    24710 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_storages_operations.py
+-rw-rw-r--  2.0 unx     7472 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_available_workload_profiles_operations.py
+-rw-rw-r--  2.0 unx    85023 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_jobs_operations.py
+-rw-rw-r--  2.0 unx    27694 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_diagnostics_operations.py
+-rw-rw-r--  2.0 unx    40778 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_certificates_operations.py
+-rw-rw-r--  2.0 unx    33895 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_source_controls_operations.py
+-rw-rw-r--  2.0 unx     5753 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_billing_meters_operations.py
+-rw-rw-r--  2.0 unx    62941 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_operations.py
+-rw-rw-r--  2.0 unx    30898 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_dapr_components_operations.py
+-rw-rw-r--  2.0 unx    59561 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environments_operations.py
+-rw-rw-r--  2.0 unx    10639 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    34286 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_certificates_operations.py
+-rw-rw-r--  2.0 unx    30199 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_dapr_components_operations.py
+-rw-rw-r--  2.0 unx    24124 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environments_storages_operations.py
+-rw-rw-r--  2.0 unx     6467 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environments_diagnostics_operations.py
+-rw-rw-r--  2.0 unx    11121 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environment_diagnostics_operations.py
+-rw-rw-r--  2.0 unx     8122 b- defN 23-May-22 09:10 azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_jobs_executions_operations.py
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx    20245 b- defN 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx     4790 b- defN 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx      124 b- defN 23-May-22 09:11 azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/requires.txt
+91 files, 1733311 bytes uncompressed, 231247 bytes compressed:  86.7%
```

## zipnote {}

```diff
@@ -1,256 +1,274 @@
-Filename: azure-mgmt-appcontainers-2.0.0b2/
+Filename: azure-mgmt-appcontainers-3.0.0b1/
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/PKG-INFO
+Filename: azure-mgmt-appcontainers-3.0.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/setup.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/MANIFEST.in
+Filename: azure-mgmt-appcontainers-3.0.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/setup.cfg
+Filename: azure-mgmt-appcontainers-3.0.0b1/LICENSE
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/README.md
+Filename: azure-mgmt-appcontainers-3.0.0b1/README.md
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/_meta.json
+Filename: azure-mgmt-appcontainers-3.0.0b1/setup.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/CHANGELOG.md
+Filename: azure-mgmt-appcontainers-3.0.0b1/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/LICENSE
+Filename: azure-mgmt-appcontainers-3.0.0b1/_meta.json
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/PKG-INFO
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/requires.txt
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/SOURCES.txt
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/not-zip-safe
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/dependency_links.txt
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/top_level.txt
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/__init__.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/py.typed
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/__init__.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/__init__.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_patch.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_configuration.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_version.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_serialization.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_container_apps_api_client.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_container_apps_api_client.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/py.typed
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_vendor.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/_container_apps_api_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_version.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_patch.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/__init__.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_diagnostics_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_billing_meters_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environments_diagnostics_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/_container_apps_api_client.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environments_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_revision_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_certificates_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_auth_configs_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_available_workload_profiles_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_namespaces_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_revision_replicas_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environments_storages_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_revisions_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_dapr_components_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_storages_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_auth_configs_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_available_workload_profiles_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_certificates_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_jobs_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_certificates_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_diagnostics_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_storages_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_certificates_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_dapr_components_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_source_controls_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_revisions_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_billing_meters_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_patch.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_source_controls_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_dapr_components_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environment_diagnostics_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environments_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/__init__.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_certificates_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/_configuration.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_dapr_components_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/_container_apps_api_client.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environments_storages_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/_patch.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environments_diagnostics_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/__init__.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environment_diagnostics_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_diagnostics_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_jobs_executions_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_billing_meters_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environments_diagnostics_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_revision_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_certificates_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environments_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_auth_configs_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_available_workload_profiles_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_namespaces_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_revisions_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_revision_replicas_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_storages_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environments_storages_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_available_workload_profiles_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_dapr_components_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_jobs_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_auth_configs_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_diagnostics_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_certificates_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_certificates_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_certificates_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_source_controls_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_storages_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_billing_meters_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_dapr_components_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_revisions_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_dapr_components_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_patch.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environments_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_source_controls_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environment_diagnostics_operations.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_certificates_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/__init__.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_dapr_components_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/_models_py3.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environments_storages_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/_container_apps_api_client_enums.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environments_diagnostics_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/_patch.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environment_diagnostics_operations.py
 Comment: 
 
-Filename: azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/__init__.py
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_jobs_executions_operations.py
+Comment: 
+
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/dependency_links.txt
+Comment: 
+
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/PKG-INFO
+Comment: 
+
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/not-zip-safe
+Comment: 
+
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/requires.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/PKG-INFO` & `azure-mgmt-appcontainers-3.0.0b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-appcontainers
-Version: 2.0.0b2
+Version: 3.0.0b1
 Summary: Microsoft Azure Appcontainers Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -64,16 +64,17 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = ContainerAppsAPIClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Appcontainers Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Appcontainers Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
@@ -84,14 +85,95 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-appcontainers%2FREADME.png)
 
 
 # Release History
 
+## 3.0.0b1 (2023-05-20)
+
+### Features Added
+
+  - Added operation group JobsExecutionsOperations
+  - Added operation group JobsOperations
+  - Added operation group ManagedCertificatesOperations
+  - Model AvailableWorkloadProfileProperties has a new parameter category
+  - Model ContainerApp has a new parameter managed_by
+  - Model ContainerApp has a new parameter workload_profile_name
+  - Model ContainerAppSecret has a new parameter identity
+  - Model ContainerAppSecret has a new parameter key_vault_url
+  - Model Ingress has a new parameter sticky_sessions
+  - Model ManagedEnvironment has a new parameter dapr_configuration
+  - Model ManagedEnvironment has a new parameter infrastructure_resource_group
+  - Model ManagedEnvironment has a new parameter keda_configuration
+  - Model Secret has a new parameter identity
+  - Model Secret has a new parameter key_vault_url
+  - Model Volume has a new parameter secrets
+
+### Breaking Changes
+
+  - Model AvailableWorkloadProfileProperties no longer has parameter billing_meter_category
+  - Model ContainerApp no longer has parameter workload_profile_type
+  - Model ManagedEnvironment no longer has parameter sku
+  - Model VnetConfiguration no longer has parameter outbound_settings
+  - Model VnetConfiguration no longer has parameter runtime_subnet_id
+  - Model WorkloadProfile has a new required parameter name
+
+## 2.0.0 (2023-03-20)
+
+### Features Added
+
+  - Added operation ContainerAppsOperations.get_auth_token
+  - Added operation ManagedEnvironmentsOperations.get_auth_token
+  - Added operation ManagedEnvironmentsOperations.list_workload_profile_states
+  - Added operation group AvailableWorkloadProfilesOperations
+  - Added operation group BillingMetersOperations
+  - Added operation group ConnectedEnvironmentsCertificatesOperations
+  - Added operation group ConnectedEnvironmentsDaprComponentsOperations
+  - Added operation group ConnectedEnvironmentsOperations
+  - Added operation group ConnectedEnvironmentsStoragesOperations
+  - Added operation group ContainerAppsDiagnosticsOperations
+  - Added operation group ManagedEnvironmentDiagnosticsOperations
+  - Added operation group ManagedEnvironmentsDiagnosticsOperations
+  - Model CertificateProperties has a new parameter subject_alternative_names
+  - Model Configuration has a new parameter max_inactive_revisions
+  - Model ContainerApp has a new parameter environment_id
+  - Model ContainerApp has a new parameter event_stream_endpoint
+  - Model ContainerApp has a new parameter extended_location
+  - Model ContainerApp has a new parameter latest_ready_revision_name
+  - Model ContainerApp has a new parameter workload_profile_type
+  - Model CustomHostnameAnalysisResult has a new parameter conflict_with_environment_custom_domain
+  - Model Dapr has a new parameter enable_api_logging
+  - Model Dapr has a new parameter http_max_request_size
+  - Model Dapr has a new parameter http_read_buffer_size
+  - Model Dapr has a new parameter log_level
+  - Model DaprComponent has a new parameter secret_store_component
+  - Model Ingress has a new parameter client_certificate_mode
+  - Model Ingress has a new parameter cors_policy
+  - Model Ingress has a new parameter exposed_port
+  - Model Ingress has a new parameter ip_security_restrictions
+  - Model ManagedEnvironment has a new parameter custom_domain_configuration
+  - Model ManagedEnvironment has a new parameter event_stream_endpoint
+  - Model ManagedEnvironment has a new parameter kind
+  - Model ManagedEnvironment has a new parameter sku
+  - Model ManagedEnvironment has a new parameter workload_profiles
+  - Model ReplicaContainer has a new parameter exec_endpoint
+  - Model ReplicaContainer has a new parameter log_stream_endpoint
+  - Model Revision has a new parameter last_active_time
+  - Model ScaleRule has a new parameter tcp
+  - Model Template has a new parameter init_containers
+  - Model VnetConfiguration has a new parameter outbound_settings
+
+### Breaking Changes
+
+  - Model CustomHostnameAnalysisResult no longer has parameter id
+  - Model CustomHostnameAnalysisResult no longer has parameter name
+  - Model CustomHostnameAnalysisResult no longer has parameter system_data
+  - Model CustomHostnameAnalysisResult no longer has parameter type
+
 ## 2.0.0b2 (2022-12-29)
 
 ### Features Added
 
   - Added operation ContainerAppsOperations.get_auth_token
   - Added operation ManagedEnvironmentsOperations.get_auth_token
   - Added operation ManagedEnvironmentsOperations.list_workload_profile_states
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/setup.py` & `azure-mgmt-appcontainers-3.0.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,14 @@
         'azure.mgmt',
     ]),
     include_package_data=True,
     package_data={
         'pytyped': ['py.typed'],
     },
     install_requires=[
-        "msrest>=0.7.1",
+        "isodate<1.0.0,>=0.6.1",
         "azure-common~=1.1",
         "azure-mgmt-core>=1.3.2,<2.0.0",
         "typing-extensions>=4.3.0; python_version<'3.8.0'",
     ],
     python_requires=">=3.7"
 )
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/README.md` & `azure-mgmt-appcontainers-3.0.0b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,17 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = ContainerAppsAPIClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Appcontainers Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Appcontainers Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/_meta.json` & `azure-mgmt-appcontainers-3.0.0b1/_meta.json`

 * *Files 10% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/app/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.4.8 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'3c639105c011765893db51cbb0dda056e34dc994'",*

 * * "'use'": "{insert: [(0 […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/app/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.2.7 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "f38115ac455af89493b0a0719d9a987404560dda",
+    "autorest_command": "autorest specification/app/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.8 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "3c639105c011765893db51cbb0dda056e34dc994",
     "readme": "specification/app/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.2.7",
+        "@autorest/python@6.4.8",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/CHANGELOG.md` & `azure-mgmt-appcontainers-3.0.0b1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,90 @@
 # Release History
 
+## 3.0.0b1 (2023-05-20)
+
+### Features Added
+
+  - Added operation group JobsExecutionsOperations
+  - Added operation group JobsOperations
+  - Added operation group ManagedCertificatesOperations
+  - Model AvailableWorkloadProfileProperties has a new parameter category
+  - Model ContainerApp has a new parameter managed_by
+  - Model ContainerApp has a new parameter workload_profile_name
+  - Model ContainerAppSecret has a new parameter identity
+  - Model ContainerAppSecret has a new parameter key_vault_url
+  - Model Ingress has a new parameter sticky_sessions
+  - Model ManagedEnvironment has a new parameter dapr_configuration
+  - Model ManagedEnvironment has a new parameter infrastructure_resource_group
+  - Model ManagedEnvironment has a new parameter keda_configuration
+  - Model Secret has a new parameter identity
+  - Model Secret has a new parameter key_vault_url
+  - Model Volume has a new parameter secrets
+
+### Breaking Changes
+
+  - Model AvailableWorkloadProfileProperties no longer has parameter billing_meter_category
+  - Model ContainerApp no longer has parameter workload_profile_type
+  - Model ManagedEnvironment no longer has parameter sku
+  - Model VnetConfiguration no longer has parameter outbound_settings
+  - Model VnetConfiguration no longer has parameter runtime_subnet_id
+  - Model WorkloadProfile has a new required parameter name
+
+## 2.0.0 (2023-03-20)
+
+### Features Added
+
+  - Added operation ContainerAppsOperations.get_auth_token
+  - Added operation ManagedEnvironmentsOperations.get_auth_token
+  - Added operation ManagedEnvironmentsOperations.list_workload_profile_states
+  - Added operation group AvailableWorkloadProfilesOperations
+  - Added operation group BillingMetersOperations
+  - Added operation group ConnectedEnvironmentsCertificatesOperations
+  - Added operation group ConnectedEnvironmentsDaprComponentsOperations
+  - Added operation group ConnectedEnvironmentsOperations
+  - Added operation group ConnectedEnvironmentsStoragesOperations
+  - Added operation group ContainerAppsDiagnosticsOperations
+  - Added operation group ManagedEnvironmentDiagnosticsOperations
+  - Added operation group ManagedEnvironmentsDiagnosticsOperations
+  - Model CertificateProperties has a new parameter subject_alternative_names
+  - Model Configuration has a new parameter max_inactive_revisions
+  - Model ContainerApp has a new parameter environment_id
+  - Model ContainerApp has a new parameter event_stream_endpoint
+  - Model ContainerApp has a new parameter extended_location
+  - Model ContainerApp has a new parameter latest_ready_revision_name
+  - Model ContainerApp has a new parameter workload_profile_type
+  - Model CustomHostnameAnalysisResult has a new parameter conflict_with_environment_custom_domain
+  - Model Dapr has a new parameter enable_api_logging
+  - Model Dapr has a new parameter http_max_request_size
+  - Model Dapr has a new parameter http_read_buffer_size
+  - Model Dapr has a new parameter log_level
+  - Model DaprComponent has a new parameter secret_store_component
+  - Model Ingress has a new parameter client_certificate_mode
+  - Model Ingress has a new parameter cors_policy
+  - Model Ingress has a new parameter exposed_port
+  - Model Ingress has a new parameter ip_security_restrictions
+  - Model ManagedEnvironment has a new parameter custom_domain_configuration
+  - Model ManagedEnvironment has a new parameter event_stream_endpoint
+  - Model ManagedEnvironment has a new parameter kind
+  - Model ManagedEnvironment has a new parameter sku
+  - Model ManagedEnvironment has a new parameter workload_profiles
+  - Model ReplicaContainer has a new parameter exec_endpoint
+  - Model ReplicaContainer has a new parameter log_stream_endpoint
+  - Model Revision has a new parameter last_active_time
+  - Model ScaleRule has a new parameter tcp
+  - Model Template has a new parameter init_containers
+  - Model VnetConfiguration has a new parameter outbound_settings
+
+### Breaking Changes
+
+  - Model CustomHostnameAnalysisResult no longer has parameter id
+  - Model CustomHostnameAnalysisResult no longer has parameter name
+  - Model CustomHostnameAnalysisResult no longer has parameter system_data
+  - Model CustomHostnameAnalysisResult no longer has parameter type
+
 ## 2.0.0b2 (2022-12-29)
 
 ### Features Added
 
   - Added operation ContainerAppsOperations.get_auth_token
   - Added operation ManagedEnvironmentsOperations.get_auth_token
   - Added operation ManagedEnvironmentsOperations.list_workload_profile_states
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/LICENSE` & `azure-mgmt-appcontainers-3.0.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/PKG-INFO` & `azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-appcontainers
-Version: 2.0.0b2
+Version: 3.0.0b1
 Summary: Microsoft Azure Appcontainers Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -64,16 +64,17 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = ContainerAppsAPIClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Appcontainers Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Appcontainers Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
@@ -84,14 +85,95 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-appcontainers%2FREADME.png)
 
 
 # Release History
 
+## 3.0.0b1 (2023-05-20)
+
+### Features Added
+
+  - Added operation group JobsExecutionsOperations
+  - Added operation group JobsOperations
+  - Added operation group ManagedCertificatesOperations
+  - Model AvailableWorkloadProfileProperties has a new parameter category
+  - Model ContainerApp has a new parameter managed_by
+  - Model ContainerApp has a new parameter workload_profile_name
+  - Model ContainerAppSecret has a new parameter identity
+  - Model ContainerAppSecret has a new parameter key_vault_url
+  - Model Ingress has a new parameter sticky_sessions
+  - Model ManagedEnvironment has a new parameter dapr_configuration
+  - Model ManagedEnvironment has a new parameter infrastructure_resource_group
+  - Model ManagedEnvironment has a new parameter keda_configuration
+  - Model Secret has a new parameter identity
+  - Model Secret has a new parameter key_vault_url
+  - Model Volume has a new parameter secrets
+
+### Breaking Changes
+
+  - Model AvailableWorkloadProfileProperties no longer has parameter billing_meter_category
+  - Model ContainerApp no longer has parameter workload_profile_type
+  - Model ManagedEnvironment no longer has parameter sku
+  - Model VnetConfiguration no longer has parameter outbound_settings
+  - Model VnetConfiguration no longer has parameter runtime_subnet_id
+  - Model WorkloadProfile has a new required parameter name
+
+## 2.0.0 (2023-03-20)
+
+### Features Added
+
+  - Added operation ContainerAppsOperations.get_auth_token
+  - Added operation ManagedEnvironmentsOperations.get_auth_token
+  - Added operation ManagedEnvironmentsOperations.list_workload_profile_states
+  - Added operation group AvailableWorkloadProfilesOperations
+  - Added operation group BillingMetersOperations
+  - Added operation group ConnectedEnvironmentsCertificatesOperations
+  - Added operation group ConnectedEnvironmentsDaprComponentsOperations
+  - Added operation group ConnectedEnvironmentsOperations
+  - Added operation group ConnectedEnvironmentsStoragesOperations
+  - Added operation group ContainerAppsDiagnosticsOperations
+  - Added operation group ManagedEnvironmentDiagnosticsOperations
+  - Added operation group ManagedEnvironmentsDiagnosticsOperations
+  - Model CertificateProperties has a new parameter subject_alternative_names
+  - Model Configuration has a new parameter max_inactive_revisions
+  - Model ContainerApp has a new parameter environment_id
+  - Model ContainerApp has a new parameter event_stream_endpoint
+  - Model ContainerApp has a new parameter extended_location
+  - Model ContainerApp has a new parameter latest_ready_revision_name
+  - Model ContainerApp has a new parameter workload_profile_type
+  - Model CustomHostnameAnalysisResult has a new parameter conflict_with_environment_custom_domain
+  - Model Dapr has a new parameter enable_api_logging
+  - Model Dapr has a new parameter http_max_request_size
+  - Model Dapr has a new parameter http_read_buffer_size
+  - Model Dapr has a new parameter log_level
+  - Model DaprComponent has a new parameter secret_store_component
+  - Model Ingress has a new parameter client_certificate_mode
+  - Model Ingress has a new parameter cors_policy
+  - Model Ingress has a new parameter exposed_port
+  - Model Ingress has a new parameter ip_security_restrictions
+  - Model ManagedEnvironment has a new parameter custom_domain_configuration
+  - Model ManagedEnvironment has a new parameter event_stream_endpoint
+  - Model ManagedEnvironment has a new parameter kind
+  - Model ManagedEnvironment has a new parameter sku
+  - Model ManagedEnvironment has a new parameter workload_profiles
+  - Model ReplicaContainer has a new parameter exec_endpoint
+  - Model ReplicaContainer has a new parameter log_stream_endpoint
+  - Model Revision has a new parameter last_active_time
+  - Model ScaleRule has a new parameter tcp
+  - Model Template has a new parameter init_containers
+  - Model VnetConfiguration has a new parameter outbound_settings
+
+### Breaking Changes
+
+  - Model CustomHostnameAnalysisResult no longer has parameter id
+  - Model CustomHostnameAnalysisResult no longer has parameter name
+  - Model CustomHostnameAnalysisResult no longer has parameter system_data
+  - Model CustomHostnameAnalysisResult no longer has parameter type
+
 ## 2.0.0b2 (2022-12-29)
 
 ### Features Added
 
   - Added operation ContainerAppsOperations.get_auth_token
   - Added operation ManagedEnvironmentsOperations.get_auth_token
   - Added operation ManagedEnvironmentsOperations.list_workload_profile_states
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure_mgmt_appcontainers.egg-info/SOURCES.txt` & `azure-mgmt-appcontainers-3.0.0b1/azure_mgmt_appcontainers.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 azure/mgmt/appcontainers/aio/operations/_container_apps_auth_configs_operations.py
 azure/mgmt/appcontainers/aio/operations/_container_apps_diagnostics_operations.py
 azure/mgmt/appcontainers/aio/operations/_container_apps_operations.py
 azure/mgmt/appcontainers/aio/operations/_container_apps_revision_replicas_operations.py
 azure/mgmt/appcontainers/aio/operations/_container_apps_revisions_operations.py
 azure/mgmt/appcontainers/aio/operations/_container_apps_source_controls_operations.py
 azure/mgmt/appcontainers/aio/operations/_dapr_components_operations.py
+azure/mgmt/appcontainers/aio/operations/_jobs_executions_operations.py
+azure/mgmt/appcontainers/aio/operations/_jobs_operations.py
+azure/mgmt/appcontainers/aio/operations/_managed_certificates_operations.py
 azure/mgmt/appcontainers/aio/operations/_managed_environment_diagnostics_operations.py
 azure/mgmt/appcontainers/aio/operations/_managed_environments_diagnostics_operations.py
 azure/mgmt/appcontainers/aio/operations/_managed_environments_operations.py
 azure/mgmt/appcontainers/aio/operations/_managed_environments_storages_operations.py
 azure/mgmt/appcontainers/aio/operations/_namespaces_operations.py
 azure/mgmt/appcontainers/aio/operations/_operations.py
 azure/mgmt/appcontainers/aio/operations/_patch.py
@@ -55,14 +58,17 @@
 azure/mgmt/appcontainers/operations/_container_apps_auth_configs_operations.py
 azure/mgmt/appcontainers/operations/_container_apps_diagnostics_operations.py
 azure/mgmt/appcontainers/operations/_container_apps_operations.py
 azure/mgmt/appcontainers/operations/_container_apps_revision_replicas_operations.py
 azure/mgmt/appcontainers/operations/_container_apps_revisions_operations.py
 azure/mgmt/appcontainers/operations/_container_apps_source_controls_operations.py
 azure/mgmt/appcontainers/operations/_dapr_components_operations.py
+azure/mgmt/appcontainers/operations/_jobs_executions_operations.py
+azure/mgmt/appcontainers/operations/_jobs_operations.py
+azure/mgmt/appcontainers/operations/_managed_certificates_operations.py
 azure/mgmt/appcontainers/operations/_managed_environment_diagnostics_operations.py
 azure/mgmt/appcontainers/operations/_managed_environments_diagnostics_operations.py
 azure/mgmt/appcontainers/operations/_managed_environments_operations.py
 azure/mgmt/appcontainers/operations/_managed_environments_storages_operations.py
 azure/mgmt/appcontainers/operations/_namespaces_operations.py
 azure/mgmt/appcontainers/operations/_operations.py
 azure/mgmt/appcontainers/operations/_patch.py
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_configuration.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,22 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
 from ._version import VERSION
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class ContainerAppsAPIClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for ContainerAppsAPIClient.
@@ -31,22 +25,22 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-10-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(ContainerAppsAPIClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-10-01"] = kwargs.pop("api_version", "2022-10-01")
+        api_version: str = kwargs.pop("api_version", "2022-11-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_serialization.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,47 @@
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
-from typing import Optional, Union, AnyStr, IO, Mapping
+from typing import (
+    Dict,
+    Any,
+    cast,
+    Optional,
+    Union,
+    AnyStr,
+    IO,
+    Mapping,
+    Callable,
+    TypeVar,
+    MutableMapping,
+    Type,
+    List,
+    Mapping,
+)
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from typing import Dict, Any, cast
-
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
+
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
@@ -273,43 +290,43 @@
     serialization and deserialization.
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs):
-        self.additional_properties = {}
+    def __init__(self, **kwargs: Any) -> None:
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls):
+    def enable_additional_properties_sending(cls) -> None:
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls):
+    def is_xml_model(cls) -> bool:
         try:
             cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
@@ -318,30 +335,35 @@
         try:
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly=False, **kwargs):
+    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
-        """Return a dict that can be JSONify using json.dump.
+    def as_dict(
+        self,
+        keep_readonly: bool = True,
+        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
+        **kwargs: Any
+    ) -> JSON:
+        """Return a dict that can be serialized using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -380,41 +402,46 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls, data, content_type=None):
+    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(cls, data, key_extractors=None, content_type=None):
+    def from_dict(
+        cls: Type[ModelType],
+        data: Any,
+        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
+        content_type: Optional[str] = None,
+    ) -> ModelType:
         """Parse a dict using given key extractor return a model.
 
         By default consider key
         extractors (rest_key_case_insensitive_extractor, attribute_key_case_insensitive_extractor
         and last_rest_key_case_insensitive_extractor)
 
         :param dict data: A dict using RestAPI structure
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        deserializer.key_extractors = (
-            [
+        deserializer.key_extractors = (  # type: ignore
+            [  # type: ignore
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -514,15 +541,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -530,15 +557,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -598,15 +625,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -622,16 +649,15 @@
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
                         for k in keys:  # type: ignore
                             if k not in _serialized:
                                 _serialized.update(_new_attr)  # type: ignore
                             _new_attr = _new_attr[k]  # type: ignore
@@ -652,16 +678,16 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type, None)
+        internal_data_type_str = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type_str, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
@@ -773,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -1157,15 +1185,16 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        dict_keys = _FLATTEN.split(key)
+        # Need the cast, as for some reasons "split" is typed as list[str | Any]
+        dict_keys = cast(List[str], _FLATTEN.split(key))
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1238,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1262,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
@@ -1328,15 +1357,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1348,15 +1377,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1467,40 +1496,40 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
         if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
             target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
-        return target, target.__class__.__name__
+        return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
             _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_container_apps_api_client.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_container_apps_api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     ContainerAppsAuthConfigsOperations,
     ContainerAppsDiagnosticsOperations,
     ContainerAppsOperations,
     ContainerAppsRevisionReplicasOperations,
     ContainerAppsRevisionsOperations,
     ContainerAppsSourceControlsOperations,
     DaprComponentsOperations,
+    JobsExecutionsOperations,
+    JobsOperations,
+    ManagedCertificatesOperations,
     ManagedEnvironmentDiagnosticsOperations,
     ManagedEnvironmentsDiagnosticsOperations,
     ManagedEnvironmentsOperations,
     ManagedEnvironmentsStoragesOperations,
     NamespacesOperations,
     Operations,
 )
@@ -66,14 +69,18 @@
     :vartype connected_environments_dapr_components:
      azure.mgmt.appcontainers.operations.ConnectedEnvironmentsDaprComponentsOperations
     :ivar connected_environments_storages: ConnectedEnvironmentsStoragesOperations operations
     :vartype connected_environments_storages:
      azure.mgmt.appcontainers.operations.ConnectedEnvironmentsStoragesOperations
     :ivar container_apps: ContainerAppsOperations operations
     :vartype container_apps: azure.mgmt.appcontainers.operations.ContainerAppsOperations
+    :ivar jobs: JobsOperations operations
+    :vartype jobs: azure.mgmt.appcontainers.operations.JobsOperations
+    :ivar jobs_executions: JobsExecutionsOperations operations
+    :vartype jobs_executions: azure.mgmt.appcontainers.operations.JobsExecutionsOperations
     :ivar container_apps_revisions: ContainerAppsRevisionsOperations operations
     :vartype container_apps_revisions:
      azure.mgmt.appcontainers.operations.ContainerAppsRevisionsOperations
     :ivar container_apps_revision_replicas: ContainerAppsRevisionReplicasOperations operations
     :vartype container_apps_revision_replicas:
      azure.mgmt.appcontainers.operations.ContainerAppsRevisionReplicasOperations
     :ivar container_apps_diagnostics: ContainerAppsDiagnosticsOperations operations
@@ -88,14 +95,17 @@
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.appcontainers.operations.Operations
     :ivar managed_environments: ManagedEnvironmentsOperations operations
     :vartype managed_environments:
      azure.mgmt.appcontainers.operations.ManagedEnvironmentsOperations
     :ivar certificates: CertificatesOperations operations
     :vartype certificates: azure.mgmt.appcontainers.operations.CertificatesOperations
+    :ivar managed_certificates: ManagedCertificatesOperations operations
+    :vartype managed_certificates:
+     azure.mgmt.appcontainers.operations.ManagedCertificatesOperations
     :ivar namespaces: NamespacesOperations operations
     :vartype namespaces: azure.mgmt.appcontainers.operations.NamespacesOperations
     :ivar dapr_components: DaprComponentsOperations operations
     :vartype dapr_components: azure.mgmt.appcontainers.operations.DaprComponentsOperations
     :ivar managed_environments_storages: ManagedEnvironmentsStoragesOperations operations
     :vartype managed_environments_storages:
      azure.mgmt.appcontainers.operations.ManagedEnvironmentsStoragesOperations
@@ -104,16 +114,16 @@
      azure.mgmt.appcontainers.operations.ContainerAppsSourceControlsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-10-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -121,15 +131,15 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = ContainerAppsAPIClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.container_apps_auth_configs = ContainerAppsAuthConfigsOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -147,14 +157,16 @@
         self.connected_environments_dapr_components = ConnectedEnvironmentsDaprComponentsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.connected_environments_storages = ConnectedEnvironmentsStoragesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.container_apps = ContainerAppsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.jobs = JobsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.jobs_executions = JobsExecutionsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.container_apps_revisions = ContainerAppsRevisionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.container_apps_revision_replicas = ContainerAppsRevisionReplicasOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.container_apps_diagnostics = ContainerAppsDiagnosticsOperations(
@@ -167,14 +179,17 @@
             self._client, self._config, self._serialize, self._deserialize
         )
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.managed_environments = ManagedEnvironmentsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.certificates = CertificatesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.managed_certificates = ManagedCertificatesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.namespaces = NamespacesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.dapr_components = DaprComponentsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.managed_environments_storages = ManagedEnvironmentsStoragesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.container_apps_source_controls = ContainerAppsSourceControlsOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -205,9 +220,9 @@
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "ContainerAppsAPIClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details) -> None:
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_vendor.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_vendor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from typing import List, cast
+
 from azure.core.pipeline.transport import HttpRequest
 
 
 def _convert_request(request, files=None):
     data = request.content if not files else None
     request = HttpRequest(method=request.method, url=request.url, headers=request.headers, data=data)
     if files:
@@ -18,10 +20,11 @@
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            formatted_components = template.split("/")
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
             components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/_patch.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/__init__.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_diagnostics_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_diagnostics_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,32 +25,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_detectors_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/detectors",
     )  # pylint: disable=line-too-long
@@ -76,15 +71,15 @@
 
 def build_get_detector_request(
     resource_group_name: str, container_app_name: str, detector_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/detectors/{detectorName}",
     )  # pylint: disable=line-too-long
@@ -115,15 +110,15 @@
     *,
     filter: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/detectorProperties/revisionsApi/revisions/",
     )  # pylint: disable=line-too-long
@@ -150,15 +145,15 @@
 
 def build_get_revision_request(
     resource_group_name: str, container_app_name: str, revision_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/detectorProperties/revisionsApi/revisions/{revisionName}",
     )  # pylint: disable=line-too-long
@@ -184,15 +179,15 @@
 
 def build_get_root_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/detectorProperties/rootApi/",
     )  # pylint: disable=line-too-long
@@ -252,17 +247,15 @@
         :return: An iterator like instance of either Diagnostics or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.Diagnostics]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DiagnosticsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -308,16 +301,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -357,17 +351,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Diagnostics] = kwargs.pop("cls", None)
 
         request = build_get_detector_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             detector_name=detector_name,
             subscription_id=self._config.subscription_id,
@@ -375,16 +367,17 @@
             template_url=self.get_detector.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -420,17 +413,15 @@
         :return: An iterator like instance of either Revision or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.Revision]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.RevisionCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -477,16 +468,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -526,17 +518,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Revision] = kwargs.pop("cls", None)
 
         request = build_get_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -544,16 +534,17 @@
             template_url=self.get_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -593,33 +584,32 @@
             404: lambda response: ResourceNotFoundError(response=response, error_format=ARMErrorFormat),
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
 
         request = build_get_root_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get_root.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_billing_meters_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_billing_meters_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,30 +23,26 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.App/locations/{location}/billingMeters"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -105,32 +100,31 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BillingMeterCollection] = kwargs.pop("cls", None)
 
         request = build_get_request(
             location=location,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environments_diagnostics_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environments_diagnostics_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,32 +23,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_root_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/detectorProperties/rootApi/",
     )  # pylint: disable=line-too-long
@@ -114,33 +109,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
 
         request = build_get_root_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get_root.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,30 +25,26 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.App/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -87,17 +82,15 @@
         :return: An iterator like instance of either OperationDetail or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.OperationDetail]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AvailableOperations] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -140,16 +133,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environments_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environments_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,30 +27,26 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.App/managedEnvironments")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -67,15 +62,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments",
     )  # pylint: disable=line-too-long
@@ -99,15 +94,15 @@
 
 def build_get_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}",
     )  # pylint: disable=line-too-long
@@ -132,15 +127,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}",
@@ -168,15 +163,15 @@
 
 def build_delete_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}",
     )  # pylint: disable=line-too-long
@@ -201,15 +196,15 @@
 
 def build_update_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}",
@@ -237,15 +232,15 @@
 
 def build_get_auth_token_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/getAuthtoken",
     )  # pylint: disable=line-too-long
@@ -264,21 +259,21 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_workload_profile_states_request(
+def build_list_workload_profile_states_request(  # pylint: disable=name-too-long
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/workloadProfileStates",
     )  # pylint: disable=line-too-long
@@ -330,17 +325,15 @@
         :return: An iterator like instance of either ManagedEnvironment or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.ManagedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironmentsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -384,16 +377,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -419,17 +413,15 @@
         :return: An iterator like instance of either ManagedEnvironment or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.ManagedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironmentsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -474,16 +466,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -519,33 +512,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -576,17 +568,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(environment_envelope, (IO, bytes)):
@@ -605,16 +595,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -724,16 +715,16 @@
         Creates or updates a Managed Environment used to host container apps.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Environment. Required.
         :type environment_name: str
-        :param environment_envelope: Configuration details of the Environment. Is either a model type
-         or a IO type. Required.
+        :param environment_envelope: Configuration details of the Environment. Is either a
+         ManagedEnvironment type or a IO type. Required.
         :type environment_envelope: ~azure.mgmt.appcontainers.models.ManagedEnvironment or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -746,17 +737,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.appcontainers.models.ManagedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -807,33 +796,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -868,17 +856,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -928,17 +914,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.ManagedEnvironment]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(environment_envelope, (IO, bytes)):
@@ -957,16 +941,17 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -1074,16 +1059,16 @@
         Patches a Managed Environment using JSON Merge Patch.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Environment. Required.
         :type environment_name: str
-        :param environment_envelope: Configuration details of the Environment. Is either a model type
-         or a IO type. Required.
+        :param environment_envelope: Configuration details of the Environment. Is either a
+         ManagedEnvironment type or a IO type. Required.
         :type environment_envelope: ~azure.mgmt.appcontainers.models.ManagedEnvironment or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1096,17 +1081,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.appcontainers.models.ManagedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._update_initial(
@@ -1172,33 +1155,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.EnvironmentAuthToken] = kwargs.pop("cls", None)
 
         request = build_get_auth_token_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get_auth_token.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -1215,17 +1197,17 @@
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/getAuthtoken"
     }
 
     @distributed_trace
     def list_workload_profile_states(
         self, resource_group_name: str, environment_name: str, **kwargs: Any
     ) -> Iterable["_models.WorkloadProfileStates"]:
-        """Get all workload Profile States for a Premium Managed Environment..
+        """Get all workload Profile States for a Managed Environment..
 
-        Get all workload Profile States for a Premium Managed Environment.
+        Get all workload Profile States for a Managed Environment.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1233,17 +1215,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.WorkloadProfileStates]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.WorkloadProfileStatesCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1289,16 +1269,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,30 +27,26 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.App/connectedEnvironments")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -67,15 +62,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments",
     )  # pylint: disable=line-too-long
@@ -99,21 +94,21 @@
 
 def build_get_request(
     resource_group_name: str, connected_environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "connectedEnvironmentName": _SERIALIZER.url("connected_environment_name", connected_environment_name, "str"),
@@ -132,22 +127,22 @@
 
 def build_create_or_update_request(
     resource_group_name: str, connected_environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "connectedEnvironmentName": _SERIALIZER.url("connected_environment_name", connected_environment_name, "str"),
@@ -168,21 +163,21 @@
 
 def build_delete_request(
     resource_group_name: str, connected_environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "connectedEnvironmentName": _SERIALIZER.url("connected_environment_name", connected_environment_name, "str"),
@@ -201,21 +196,21 @@
 
 def build_update_request(
     resource_group_name: str, connected_environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "connectedEnvironmentName": _SERIALIZER.url("connected_environment_name", connected_environment_name, "str"),
@@ -234,15 +229,15 @@
 
 def build_check_name_availability_request(
     resource_group_name: str, connected_environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/checkNameAvailability",
@@ -298,17 +293,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.ConnectedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironmentCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -352,16 +345,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -388,17 +382,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.ConnectedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironmentCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -443,16 +435,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -488,33 +481,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironment] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -524,15 +516,15 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         connected_environment_name: str,
         environment_envelope: Union[_models.ConnectedEnvironment, IO],
@@ -545,17 +537,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConnectedEnvironment] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(environment_envelope, (IO, bytes)):
@@ -574,16 +564,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -597,15 +588,15 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         connected_environment_name: str,
@@ -688,15 +679,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the connectedEnvironment. Required.
         :type connected_environment_name: str
         :param environment_envelope: Configuration details of the connectedEnvironment. Is either a
-         model type or a IO type. Required.
+         ConnectedEnvironment type or a IO type. Required.
         :type environment_envelope: ~azure.mgmt.appcontainers.models.ConnectedEnvironment or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -709,17 +700,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.appcontainers.models.ConnectedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConnectedEnvironment] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -738,30 +727,32 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ConnectedEnvironment", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, connected_environment_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
@@ -770,47 +761,50 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, connected_environment_name: str, **kwargs: Any) -> LROPoller[None]:
         """Delete an connectedEnvironment.
 
         Delete an connectedEnvironment.
@@ -831,17 +825,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -855,30 +847,32 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     @distributed_trace
     def update(
         self, resource_group_name: str, connected_environment_name: str, **kwargs: Any
     ) -> _models.ConnectedEnvironment:
         """Update connected Environment's properties.
@@ -902,33 +896,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironment] = kwargs.pop("cls", None)
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -938,15 +931,15 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     @overload
     def check_name_availability(
         self,
         resource_group_name: str,
         connected_environment_name: str,
@@ -1022,15 +1015,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the Managed Environment. Required.
         :type connected_environment_name: str
         :param check_name_availability_request: The check connectedEnvironmentName availability
-         request. Is either a model type or a IO type. Required.
+         request. Is either a CheckNameAvailabilityRequest type or a IO type. Required.
         :type check_name_availability_request:
          ~azure.mgmt.appcontainers.models.CheckNameAvailabilityRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResponse or the result of cls(response)
@@ -1044,17 +1037,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CheckNameAvailabilityResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(check_name_availability_request, (IO, bytes)):
@@ -1073,16 +1064,17 @@
             template_url=self.check_name_availability.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,30 +27,26 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.App/containerApps")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -67,15 +62,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps",
     )  # pylint: disable=line-too-long
@@ -99,15 +94,15 @@
 
 def build_get_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}",
     )  # pylint: disable=line-too-long
@@ -132,15 +127,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}",
@@ -168,15 +163,15 @@
 
 def build_delete_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}",
     )  # pylint: disable=line-too-long
@@ -201,15 +196,15 @@
 
 def build_update_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}",
@@ -231,26 +226,26 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_custom_host_name_analysis_request(
+def build_list_custom_host_name_analysis_request(  # pylint: disable=name-too-long
     resource_group_name: str,
     container_app_name: str,
     subscription_id: str,
     *,
     custom_hostname: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/listCustomHostNameAnalysis",
     )  # pylint: disable=line-too-long
@@ -277,15 +272,15 @@
 
 def build_list_secrets_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/listSecrets",
     )  # pylint: disable=line-too-long
@@ -310,15 +305,15 @@
 
 def build_get_auth_token_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/getAuthtoken",
     )  # pylint: disable=line-too-long
@@ -370,17 +365,15 @@
         :return: An iterator like instance of either ContainerApp or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.ContainerApp]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerAppCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -424,16 +417,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -457,17 +451,15 @@
         :return: An iterator like instance of either ContainerApp or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.ContainerApp]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerAppCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -512,16 +504,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -557,33 +550,32 @@
             404: lambda response: ResourceNotFoundError(response=response, error_format=ARMErrorFormat),
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -614,17 +606,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(container_app_envelope, (IO, bytes)):
@@ -643,16 +633,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -762,16 +753,16 @@
         Create or update a Container App.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param container_app_name: Name of the Container App. Required.
         :type container_app_name: str
-        :param container_app_envelope: Properties used to create a container app. Is either a model
-         type or a IO type. Required.
+        :param container_app_envelope: Properties used to create a container app. Is either a
+         ContainerApp type or a IO type. Required.
         :type container_app_envelope: ~azure.mgmt.appcontainers.models.ContainerApp or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -784,17 +775,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.appcontainers.models.ContainerApp]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -813,15 +802,17 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ContainerApp", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
@@ -845,44 +836,47 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _delete_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}"
     }
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, container_app_name: str, **kwargs: Any) -> LROPoller[None]:
@@ -906,17 +900,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -930,15 +922,17 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
@@ -966,17 +960,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.ContainerApp]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(container_app_envelope, (IO, bytes)):
@@ -995,31 +987,36 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("ContainerApp", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
     _update_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}"
     }
 
@@ -1113,15 +1110,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param container_app_name: Name of the Container App. Required.
         :type container_app_name: str
         :param container_app_envelope: Properties of a Container App that need to be updated. Is either
-         a model type or a IO type. Required.
+         a ContainerApp type or a IO type. Required.
         :type container_app_envelope: ~azure.mgmt.appcontainers.models.ContainerApp or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1134,17 +1131,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.appcontainers.models.ContainerApp]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._update_initial(
@@ -1212,17 +1207,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CustomHostnameAnalysisResult] = kwargs.pop("cls", None)
 
         request = build_list_custom_host_name_analysis_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             custom_hostname=custom_hostname,
@@ -1230,16 +1223,17 @@
             template_url=self.list_custom_host_name_analysis.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -1281,33 +1275,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SecretsCollection] = kwargs.pop("cls", None)
 
         request = build_list_secrets_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list_secrets.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -1349,33 +1342,32 @@
             404: lambda response: ResourceNotFoundError(response=response, error_format=ARMErrorFormat),
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerAppAuthToken] = kwargs.pop("cls", None)
 
         request = build_get_auth_token_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get_auth_token.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_available_workload_profiles_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_available_workload_profiles_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,30 +25,26 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.App/locations/{location}/availableManagedEnvironmentsWorkloadProfileTypes",
     )  # pylint: disable=line-too-long
@@ -101,17 +96,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.AvailableWorkloadProfile]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AvailableWorkloadProfilesCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -156,16 +149,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_namespaces_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_namespaces_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,32 +23,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_check_name_availability_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/checkNameAvailability",
@@ -168,16 +163,16 @@
         Checks if resource name is available.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
-        :param check_name_availability_request: The check name availability request. Is either a model
-         type or a IO type. Required.
+        :param check_name_availability_request: The check name availability request. Is either a
+         CheckNameAvailabilityRequest type or a IO type. Required.
         :type check_name_availability_request:
          ~azure.mgmt.appcontainers.models.CheckNameAvailabilityRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResponse or the result of cls(response)
@@ -191,17 +186,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CheckNameAvailabilityResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(check_name_availability_request, (IO, bytes)):
@@ -220,16 +213,17 @@
             template_url=self.check_name_availability.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_revision_replicas_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_revision_replicas_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,18 +23,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -46,15 +41,15 @@
     replica_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/revisions/{revisionName}/replicas/{replicaName}",
     )  # pylint: disable=line-too-long
@@ -81,15 +76,15 @@
 
 def build_list_replicas_request(
     resource_group_name: str, container_app_name: str, revision_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/revisions/{revisionName}/replicas",
     )  # pylint: disable=line-too-long
@@ -161,17 +156,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Replica] = kwargs.pop("cls", None)
 
         request = build_get_replica_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             replica_name=replica_name,
@@ -180,16 +173,17 @@
             template_url=self.get_replica.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -233,17 +227,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ReplicaCollection] = kwargs.pop("cls", None)
 
         request = build_list_replicas_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -251,16 +243,17 @@
             template_url=self.list_replicas.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environments_storages_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environments_storages_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,32 +23,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/storages",
     )  # pylint: disable=line-too-long
@@ -74,15 +69,15 @@
 
 def build_get_request(
     resource_group_name: str, environment_name: str, storage_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/storages/{storageName}",
     )  # pylint: disable=line-too-long
@@ -108,15 +103,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, environment_name: str, storage_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/storages/{storageName}",
@@ -145,15 +140,15 @@
 
 def build_delete_request(
     resource_group_name: str, environment_name: str, storage_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/storages/{storageName}",
     )  # pylint: disable=line-too-long
@@ -221,33 +216,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironmentStoragesCollection] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -291,17 +285,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironmentStorage] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             storage_name=storage_name,
             subscription_id=self._config.subscription_id,
@@ -309,16 +301,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -417,16 +410,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Environment. Required.
         :type environment_name: str
         :param storage_name: Name of the storage. Required.
         :type storage_name: str
-        :param storage_envelope: Configuration details of storage. Is either a model type or a IO type.
-         Required.
+        :param storage_envelope: Configuration details of storage. Is either a
+         ManagedEnvironmentStorage type or a IO type. Required.
         :type storage_envelope: ~azure.mgmt.appcontainers.models.ManagedEnvironmentStorage or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ManagedEnvironmentStorage or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.ManagedEnvironmentStorage
@@ -439,17 +432,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ManagedEnvironmentStorage] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(storage_envelope, (IO, bytes)):
@@ -469,16 +460,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -522,17 +514,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             storage_name=storage_name,
             subscription_id=self._config.subscription_id,
@@ -540,16 +530,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_dapr_components_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_dapr_components_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,32 +25,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/daprComponents",
     )  # pylint: disable=line-too-long
@@ -76,15 +71,15 @@
 
 def build_get_request(
     resource_group_name: str, environment_name: str, component_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/daprComponents/{componentName}",
     )  # pylint: disable=line-too-long
@@ -110,15 +105,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, environment_name: str, component_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/daprComponents/{componentName}",
@@ -147,15 +142,15 @@
 
 def build_delete_request(
     resource_group_name: str, environment_name: str, component_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/daprComponents/{componentName}",
     )  # pylint: disable=line-too-long
@@ -181,15 +176,15 @@
 
 def build_list_secrets_request(
     resource_group_name: str, environment_name: str, component_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/daprComponents/{componentName}/listSecrets",
     )  # pylint: disable=line-too-long
@@ -247,17 +242,15 @@
         :return: An iterator like instance of either DaprComponent or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.DaprComponent]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprComponentsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -303,16 +296,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -352,17 +346,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprComponent] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -370,16 +362,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -478,16 +471,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
         :param component_name: Name of the Dapr Component. Required.
         :type component_name: str
-        :param dapr_component_envelope: Configuration details of the Dapr Component. Is either a model
-         type or a IO type. Required.
+        :param dapr_component_envelope: Configuration details of the Dapr Component. Is either a
+         DaprComponent type or a IO type. Required.
         :type dapr_component_envelope: ~azure.mgmt.appcontainers.models.DaprComponent or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DaprComponent or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.DaprComponent
@@ -500,17 +493,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DaprComponent] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(dapr_component_envelope, (IO, bytes)):
@@ -530,16 +521,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -583,17 +575,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -601,16 +591,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -650,17 +641,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprSecretsCollection] = kwargs.pop("cls", None)
 
         request = build_list_secrets_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -668,16 +657,17 @@
             template_url=self.list_secrets.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_auth_configs_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_auth_configs_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,32 +25,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_container_app_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/authConfigs",
     )  # pylint: disable=line-too-long
@@ -76,15 +71,15 @@
 
 def build_get_request(
     resource_group_name: str, container_app_name: str, auth_config_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/authConfigs/{authConfigName}",
     )  # pylint: disable=line-too-long
@@ -110,15 +105,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, container_app_name: str, auth_config_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/authConfigs/{authConfigName}",
@@ -147,15 +142,15 @@
 
 def build_delete_request(
     resource_group_name: str, container_app_name: str, auth_config_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/authConfigs/{authConfigName}",
     )  # pylint: disable=line-too-long
@@ -215,17 +210,15 @@
         :return: An iterator like instance of either AuthConfig or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.AuthConfig]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AuthConfigCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -271,16 +264,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -320,17 +314,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AuthConfig] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             auth_config_name=auth_config_name,
             subscription_id=self._config.subscription_id,
@@ -338,16 +330,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -447,15 +440,15 @@
          Required.
         :type resource_group_name: str
         :param container_app_name: Name of the Container App. Required.
         :type container_app_name: str
         :param auth_config_name: Name of the Container App AuthConfig. Required.
         :type auth_config_name: str
         :param auth_config_envelope: Properties used to create a Container App AuthConfig. Is either a
-         model type or a IO type. Required.
+         AuthConfig type or a IO type. Required.
         :type auth_config_envelope: ~azure.mgmt.appcontainers.models.AuthConfig or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AuthConfig or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.AuthConfig
@@ -468,17 +461,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AuthConfig] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(auth_config_envelope, (IO, bytes)):
@@ -498,16 +489,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -551,17 +543,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             auth_config_name=auth_config_name,
             subscription_id=self._config.subscription_id,
@@ -569,16 +559,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_certificates_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_certificates_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,32 +25,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/certificates",
     )  # pylint: disable=line-too-long
@@ -76,15 +71,15 @@
 
 def build_get_request(
     resource_group_name: str, environment_name: str, certificate_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/certificates/{certificateName}",
     )  # pylint: disable=line-too-long
@@ -110,15 +105,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, environment_name: str, certificate_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/certificates/{certificateName}",
@@ -147,15 +142,15 @@
 
 def build_delete_request(
     resource_group_name: str, environment_name: str, certificate_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/certificates/{certificateName}",
     )  # pylint: disable=line-too-long
@@ -181,15 +176,15 @@
 
 def build_update_request(
     resource_group_name: str, environment_name: str, certificate_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/certificates/{certificateName}",
@@ -250,17 +245,15 @@
         :return: An iterator like instance of either Certificate or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.Certificate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CertificateCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -306,16 +299,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -355,17 +349,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
@@ -373,16 +365,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -481,16 +474,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
         :param certificate_name: Name of the Certificate. Required.
         :type certificate_name: str
-        :param certificate_envelope: Certificate to be created or updated. Is either a model type or a
-         IO type. Default value is None.
+        :param certificate_envelope: Certificate to be created or updated. Is either a Certificate type
+         or a IO type. Default value is None.
         :type certificate_envelope: ~azure.mgmt.appcontainers.models.Certificate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Certificate or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.Certificate
@@ -503,17 +496,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(certificate_envelope, (IO, bytes)):
@@ -536,16 +527,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -589,17 +581,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
@@ -607,16 +597,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -712,15 +703,15 @@
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
         :param certificate_name: Name of the Certificate. Required.
         :type certificate_name: str
         :param certificate_envelope: Properties of a certificate that need to be updated. Is either a
-         model type or a IO type. Required.
+         CertificatePatch type or a IO type. Required.
         :type certificate_envelope: ~azure.mgmt.appcontainers.models.CertificatePatch or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Certificate or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.Certificate
@@ -733,17 +724,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(certificate_envelope, (IO, bytes)):
@@ -763,16 +752,17 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_certificates_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_certificates_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,32 +25,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, connected_environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/certificates",
     )  # pylint: disable=line-too-long
@@ -80,15 +75,15 @@
     certificate_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/certificates/{certificateName}",
     )  # pylint: disable=line-too-long
@@ -118,15 +113,15 @@
     certificate_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/certificates/{certificateName}",
@@ -159,15 +154,15 @@
     certificate_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/certificates/{certificateName}",
     )  # pylint: disable=line-too-long
@@ -197,15 +192,15 @@
     certificate_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/certificates/{certificateName}",
@@ -268,17 +263,15 @@
         :return: An iterator like instance of either Certificate or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.Certificate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CertificateCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -324,16 +317,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -373,17 +367,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
@@ -391,16 +383,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -499,16 +492,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the Connected Environment. Required.
         :type connected_environment_name: str
         :param certificate_name: Name of the Certificate. Required.
         :type certificate_name: str
-        :param certificate_envelope: Certificate to be created or updated. Is either a model type or a
-         IO type. Default value is None.
+        :param certificate_envelope: Certificate to be created or updated. Is either a Certificate type
+         or a IO type. Default value is None.
         :type certificate_envelope: ~azure.mgmt.appcontainers.models.Certificate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Certificate or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.Certificate
@@ -521,17 +514,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(certificate_envelope, (IO, bytes)):
@@ -554,16 +545,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -607,17 +599,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
@@ -625,16 +615,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -730,15 +721,15 @@
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the Connected Environment. Required.
         :type connected_environment_name: str
         :param certificate_name: Name of the Certificate. Required.
         :type certificate_name: str
         :param certificate_envelope: Properties of a certificate that need to be updated. Is either a
-         model type or a IO type. Required.
+         CertificatePatch type or a IO type. Required.
         :type certificate_envelope: ~azure.mgmt.appcontainers.models.CertificatePatch or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Certificate or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.Certificate
@@ -751,17 +742,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(certificate_envelope, (IO, bytes)):
@@ -781,16 +770,17 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_storages_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_storages_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,32 +23,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, connected_environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/storages",
     )  # pylint: disable=line-too-long
@@ -74,15 +69,15 @@
 
 def build_get_request(
     resource_group_name: str, connected_environment_name: str, storage_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/storages/{storageName}",
     )  # pylint: disable=line-too-long
@@ -108,15 +103,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, connected_environment_name: str, storage_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/storages/{storageName}",
@@ -145,15 +140,15 @@
 
 def build_delete_request(
     resource_group_name: str, connected_environment_name: str, storage_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/storages/{storageName}",
     )  # pylint: disable=line-too-long
@@ -221,33 +216,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironmentStoragesCollection] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -291,17 +285,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironmentStorage] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             storage_name=storage_name,
             subscription_id=self._config.subscription_id,
@@ -309,16 +301,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -417,16 +410,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the Environment. Required.
         :type connected_environment_name: str
         :param storage_name: Name of the storage. Required.
         :type storage_name: str
-        :param storage_envelope: Configuration details of storage. Is either a model type or a IO type.
-         Required.
+        :param storage_envelope: Configuration details of storage. Is either a
+         ConnectedEnvironmentStorage type or a IO type. Required.
         :type storage_envelope: ~azure.mgmt.appcontainers.models.ConnectedEnvironmentStorage or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConnectedEnvironmentStorage or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.ConnectedEnvironmentStorage
@@ -439,17 +432,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConnectedEnvironmentStorage] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(storage_envelope, (IO, bytes)):
@@ -469,16 +460,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -522,17 +514,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             storage_name=storage_name,
             subscription_id=self._config.subscription_id,
@@ -540,16 +530,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_connected_environments_dapr_components_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_connected_environments_dapr_components_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,32 +25,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, connected_environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/daprComponents",
     )  # pylint: disable=line-too-long
@@ -76,15 +71,15 @@
 
 def build_get_request(
     resource_group_name: str, connected_environment_name: str, component_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/daprComponents/{componentName}",
     )  # pylint: disable=line-too-long
@@ -110,15 +105,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, connected_environment_name: str, component_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/daprComponents/{componentName}",
@@ -147,15 +142,15 @@
 
 def build_delete_request(
     resource_group_name: str, connected_environment_name: str, component_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/daprComponents/{componentName}",
     )  # pylint: disable=line-too-long
@@ -181,15 +176,15 @@
 
 def build_list_secrets_request(
     resource_group_name: str, connected_environment_name: str, component_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}/daprComponents/{componentName}/listSecrets",
     )  # pylint: disable=line-too-long
@@ -249,17 +244,15 @@
         :return: An iterator like instance of either DaprComponent or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.DaprComponent]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprComponentsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -305,16 +298,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -354,17 +348,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprComponent] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -372,16 +364,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -480,16 +473,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the connected environment. Required.
         :type connected_environment_name: str
         :param component_name: Name of the Dapr Component. Required.
         :type component_name: str
-        :param dapr_component_envelope: Configuration details of the Dapr Component. Is either a model
-         type or a IO type. Required.
+        :param dapr_component_envelope: Configuration details of the Dapr Component. Is either a
+         DaprComponent type or a IO type. Required.
         :type dapr_component_envelope: ~azure.mgmt.appcontainers.models.DaprComponent or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DaprComponent or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.DaprComponent
@@ -502,17 +495,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DaprComponent] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(dapr_component_envelope, (IO, bytes)):
@@ -532,16 +523,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -585,17 +577,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -603,16 +593,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -652,17 +643,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprSecretsCollection] = kwargs.pop("cls", None)
 
         request = build_list_secrets_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -670,16 +659,17 @@
             template_url=self.list_secrets.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_revisions_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_revisions_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,18 +25,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -48,15 +43,15 @@
     *,
     filter: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/revisions",
     )  # pylint: disable=line-too-long
@@ -83,15 +78,15 @@
 
 def build_get_revision_request(
     resource_group_name: str, container_app_name: str, revision_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/revisions/{revisionName}",
     )  # pylint: disable=line-too-long
@@ -117,15 +112,15 @@
 
 def build_activate_revision_request(
     resource_group_name: str, container_app_name: str, revision_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/revisions/{revisionName}/activate",
     )  # pylint: disable=line-too-long
@@ -151,15 +146,15 @@
 
 def build_deactivate_revision_request(
     resource_group_name: str, container_app_name: str, revision_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/revisions/{revisionName}/deactivate",
     )  # pylint: disable=line-too-long
@@ -185,15 +180,15 @@
 
 def build_restart_revision_request(
     resource_group_name: str, container_app_name: str, revision_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/revisions/{revisionName}/restart",
     )  # pylint: disable=line-too-long
@@ -255,17 +250,15 @@
         :return: An iterator like instance of either Revision or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.Revision]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.RevisionCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -312,16 +305,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -361,17 +355,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Revision] = kwargs.pop("cls", None)
 
         request = build_get_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -379,16 +371,17 @@
             template_url=self.get_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -432,17 +425,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_activate_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -450,16 +441,17 @@
             template_url=self.activate_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -499,17 +491,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_deactivate_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -517,16 +507,17 @@
             template_url=self.deactivate_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -566,17 +557,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_restart_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -584,16 +573,17 @@
             template_url=self.restart_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_patch.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_container_apps_source_controls_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_container_apps_source_controls_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,32 +27,28 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_container_app_request(
     resource_group_name: str, container_app_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/sourcecontrols",
     )  # pylint: disable=line-too-long
@@ -78,15 +73,15 @@
 
 def build_get_request(
     resource_group_name: str, container_app_name: str, source_control_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/sourcecontrols/{sourceControlName}",
     )  # pylint: disable=line-too-long
@@ -112,15 +107,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, container_app_name: str, source_control_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/sourcecontrols/{sourceControlName}",
@@ -149,15 +144,15 @@
 
 def build_delete_request(
     resource_group_name: str, container_app_name: str, source_control_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}/sourcecontrols/{sourceControlName}",
     )  # pylint: disable=line-too-long
@@ -217,17 +212,15 @@
         :return: An iterator like instance of either SourceControl or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.appcontainers.models.SourceControl]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SourceControlCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -273,16 +266,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -322,17 +316,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SourceControl] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             source_control_name=source_control_name,
             subscription_id=self._config.subscription_id,
@@ -340,16 +332,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -381,17 +374,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SourceControl] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(source_control_envelope, (IO, bytes)):
@@ -411,16 +402,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -542,15 +534,15 @@
          Required.
         :type resource_group_name: str
         :param container_app_name: Name of the Container App. Required.
         :type container_app_name: str
         :param source_control_name: Name of the Container App SourceControl. Required.
         :type source_control_name: str
         :param source_control_envelope: Properties used to create a Container App SourceControl. Is
-         either a model type or a IO type. Required.
+         either a SourceControl type or a IO type. Required.
         :type source_control_envelope: ~azure.mgmt.appcontainers.models.SourceControl or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -563,17 +555,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.appcontainers.models.SourceControl]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SourceControl] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -625,17 +615,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             source_control_name=source_control_name,
             subscription_id=self._config.subscription_id,
@@ -643,16 +631,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -691,17 +680,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/_managed_environment_diagnostics_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_managed_environment_diagnostics_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,32 +23,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_detectors_request(
     resource_group_name: str, environment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/detectors",
     )  # pylint: disable=line-too-long
@@ -74,15 +69,15 @@
 
 def build_get_detector_request(
     resource_group_name: str, environment_name: str, detector_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-10-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/detectors/{detectorName}",
     )  # pylint: disable=line-too-long
@@ -150,33 +145,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DiagnosticsCollection] = kwargs.pop("cls", None)
 
         request = build_list_detectors_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list_detectors.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -220,17 +214,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Diagnostics] = kwargs.pop("cls", None)
 
         request = build_get_detector_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             detector_name=detector_name,
             subscription_id=self._config.subscription_id,
@@ -238,16 +230,17 @@
             template_url=self.get_detector.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/operations/__init__.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,25 @@
 from ._available_workload_profiles_operations import AvailableWorkloadProfilesOperations
 from ._billing_meters_operations import BillingMetersOperations
 from ._connected_environments_operations import ConnectedEnvironmentsOperations
 from ._connected_environments_certificates_operations import ConnectedEnvironmentsCertificatesOperations
 from ._connected_environments_dapr_components_operations import ConnectedEnvironmentsDaprComponentsOperations
 from ._connected_environments_storages_operations import ConnectedEnvironmentsStoragesOperations
 from ._container_apps_operations import ContainerAppsOperations
+from ._jobs_operations import JobsOperations
+from ._jobs_executions_operations import JobsExecutionsOperations
 from ._container_apps_revisions_operations import ContainerAppsRevisionsOperations
 from ._container_apps_revision_replicas_operations import ContainerAppsRevisionReplicasOperations
 from ._container_apps_diagnostics_operations import ContainerAppsDiagnosticsOperations
 from ._managed_environment_diagnostics_operations import ManagedEnvironmentDiagnosticsOperations
 from ._managed_environments_diagnostics_operations import ManagedEnvironmentsDiagnosticsOperations
 from ._operations import Operations
 from ._managed_environments_operations import ManagedEnvironmentsOperations
 from ._certificates_operations import CertificatesOperations
+from ._managed_certificates_operations import ManagedCertificatesOperations
 from ._namespaces_operations import NamespacesOperations
 from ._dapr_components_operations import DaprComponentsOperations
 from ._managed_environments_storages_operations import ManagedEnvironmentsStoragesOperations
 from ._container_apps_source_controls_operations import ContainerAppsSourceControlsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
@@ -36,22 +39,25 @@
     "AvailableWorkloadProfilesOperations",
     "BillingMetersOperations",
     "ConnectedEnvironmentsOperations",
     "ConnectedEnvironmentsCertificatesOperations",
     "ConnectedEnvironmentsDaprComponentsOperations",
     "ConnectedEnvironmentsStoragesOperations",
     "ContainerAppsOperations",
+    "JobsOperations",
+    "JobsExecutionsOperations",
     "ContainerAppsRevisionsOperations",
     "ContainerAppsRevisionReplicasOperations",
     "ContainerAppsDiagnosticsOperations",
     "ManagedEnvironmentDiagnosticsOperations",
     "ManagedEnvironmentsDiagnosticsOperations",
     "Operations",
     "ManagedEnvironmentsOperations",
     "CertificatesOperations",
+    "ManagedCertificatesOperations",
     "NamespacesOperations",
     "DaprComponentsOperations",
     "ManagedEnvironmentsStoragesOperations",
     "ContainerAppsSourceControlsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/_configuration.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,22 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class ContainerAppsAPIClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for ContainerAppsAPIClient.
@@ -31,22 +25,22 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-10-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(ContainerAppsAPIClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-10-01"] = kwargs.pop("api_version", "2022-10-01")
+        api_version: str = kwargs.pop("api_version", "2022-11-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/_container_apps_api_client.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/_container_apps_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     ContainerAppsAuthConfigsOperations,
     ContainerAppsDiagnosticsOperations,
     ContainerAppsOperations,
     ContainerAppsRevisionReplicasOperations,
     ContainerAppsRevisionsOperations,
     ContainerAppsSourceControlsOperations,
     DaprComponentsOperations,
+    JobsExecutionsOperations,
+    JobsOperations,
+    ManagedCertificatesOperations,
     ManagedEnvironmentDiagnosticsOperations,
     ManagedEnvironmentsDiagnosticsOperations,
     ManagedEnvironmentsOperations,
     ManagedEnvironmentsStoragesOperations,
     NamespacesOperations,
     Operations,
 )
@@ -66,14 +69,18 @@
     :vartype connected_environments_dapr_components:
      azure.mgmt.appcontainers.aio.operations.ConnectedEnvironmentsDaprComponentsOperations
     :ivar connected_environments_storages: ConnectedEnvironmentsStoragesOperations operations
     :vartype connected_environments_storages:
      azure.mgmt.appcontainers.aio.operations.ConnectedEnvironmentsStoragesOperations
     :ivar container_apps: ContainerAppsOperations operations
     :vartype container_apps: azure.mgmt.appcontainers.aio.operations.ContainerAppsOperations
+    :ivar jobs: JobsOperations operations
+    :vartype jobs: azure.mgmt.appcontainers.aio.operations.JobsOperations
+    :ivar jobs_executions: JobsExecutionsOperations operations
+    :vartype jobs_executions: azure.mgmt.appcontainers.aio.operations.JobsExecutionsOperations
     :ivar container_apps_revisions: ContainerAppsRevisionsOperations operations
     :vartype container_apps_revisions:
      azure.mgmt.appcontainers.aio.operations.ContainerAppsRevisionsOperations
     :ivar container_apps_revision_replicas: ContainerAppsRevisionReplicasOperations operations
     :vartype container_apps_revision_replicas:
      azure.mgmt.appcontainers.aio.operations.ContainerAppsRevisionReplicasOperations
     :ivar container_apps_diagnostics: ContainerAppsDiagnosticsOperations operations
@@ -88,14 +95,17 @@
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.appcontainers.aio.operations.Operations
     :ivar managed_environments: ManagedEnvironmentsOperations operations
     :vartype managed_environments:
      azure.mgmt.appcontainers.aio.operations.ManagedEnvironmentsOperations
     :ivar certificates: CertificatesOperations operations
     :vartype certificates: azure.mgmt.appcontainers.aio.operations.CertificatesOperations
+    :ivar managed_certificates: ManagedCertificatesOperations operations
+    :vartype managed_certificates:
+     azure.mgmt.appcontainers.aio.operations.ManagedCertificatesOperations
     :ivar namespaces: NamespacesOperations operations
     :vartype namespaces: azure.mgmt.appcontainers.aio.operations.NamespacesOperations
     :ivar dapr_components: DaprComponentsOperations operations
     :vartype dapr_components: azure.mgmt.appcontainers.aio.operations.DaprComponentsOperations
     :ivar managed_environments_storages: ManagedEnvironmentsStoragesOperations operations
     :vartype managed_environments_storages:
      azure.mgmt.appcontainers.aio.operations.ManagedEnvironmentsStoragesOperations
@@ -104,16 +114,16 @@
      azure.mgmt.appcontainers.aio.operations.ContainerAppsSourceControlsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-10-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -121,15 +131,15 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = ContainerAppsAPIClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.container_apps_auth_configs = ContainerAppsAuthConfigsOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -147,14 +157,16 @@
         self.connected_environments_dapr_components = ConnectedEnvironmentsDaprComponentsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.connected_environments_storages = ConnectedEnvironmentsStoragesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.container_apps = ContainerAppsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.jobs = JobsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.jobs_executions = JobsExecutionsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.container_apps_revisions = ContainerAppsRevisionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.container_apps_revision_replicas = ContainerAppsRevisionReplicasOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.container_apps_diagnostics = ContainerAppsDiagnosticsOperations(
@@ -167,14 +179,17 @@
             self._client, self._config, self._serialize, self._deserialize
         )
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.managed_environments = ManagedEnvironmentsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.certificates = CertificatesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.managed_certificates = ManagedCertificatesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.namespaces = NamespacesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.dapr_components = DaprComponentsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.managed_environments_storages = ManagedEnvironmentsStoragesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.container_apps_source_controls = ContainerAppsSourceControlsOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -205,9 +220,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "ContainerAppsAPIClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/_patch.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/__init__.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_diagnostics_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_diagnostics_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -33,18 +32,14 @@
     build_get_detector_request,
     build_get_revision_request,
     build_get_root_request,
     build_list_detectors_request,
     build_list_revisions_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ContainerAppsDiagnosticsOperations:
     """
     .. warning::
@@ -82,17 +77,15 @@
         :return: An iterator like instance of either Diagnostics or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.Diagnostics]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DiagnosticsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -138,16 +131,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -187,17 +181,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Diagnostics] = kwargs.pop("cls", None)
 
         request = build_get_detector_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             detector_name=detector_name,
             subscription_id=self._config.subscription_id,
@@ -205,16 +197,17 @@
             template_url=self.get_detector.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -250,17 +243,15 @@
         :return: An iterator like instance of either Revision or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.Revision]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.RevisionCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -307,16 +298,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -356,17 +348,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Revision] = kwargs.pop("cls", None)
 
         request = build_get_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -374,16 +364,17 @@
             template_url=self.get_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -423,33 +414,32 @@
             404: lambda response: ResourceNotFoundError(response=response, error_format=ARMErrorFormat),
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
 
         request = build_get_root_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get_root.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_billing_meters_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_billing_meters_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,18 +23,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._billing_meters_operations import build_get_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class BillingMetersOperations:
     """
     .. warning::
@@ -75,32 +70,31 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BillingMeterCollection] = kwargs.pop("cls", None)
 
         request = build_get_request(
             location=location,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environments_diagnostics_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environments_diagnostics_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,18 +23,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._managed_environments_diagnostics_operations import build_get_root_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ManagedEnvironmentsDiagnosticsOperations:
     """
     .. warning::
@@ -80,33 +75,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
 
         request = build_get_root_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get_root.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -26,18 +25,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class Operations:
     """
     .. warning::
@@ -66,17 +61,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.OperationDetail]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AvailableOperations] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -119,16 +112,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environments_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environments_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -38,18 +37,14 @@
     build_get_request,
     build_list_by_resource_group_request,
     build_list_by_subscription_request,
     build_list_workload_profile_states_request,
     build_update_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ManagedEnvironmentsOperations:
     """
     .. warning::
@@ -80,17 +75,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.ManagedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironmentsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -134,16 +127,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -172,17 +166,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.ManagedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironmentsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -227,16 +219,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -272,33 +265,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -329,17 +321,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(environment_envelope, (IO, bytes)):
@@ -358,16 +348,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -477,16 +468,16 @@
         Creates or updates a Managed Environment used to host container apps.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Environment. Required.
         :type environment_name: str
-        :param environment_envelope: Configuration details of the Environment. Is either a model type
-         or a IO type. Required.
+        :param environment_envelope: Configuration details of the Environment. Is either a
+         ManagedEnvironment type or a IO type. Required.
         :type environment_envelope: ~azure.mgmt.appcontainers.models.ManagedEnvironment or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -499,17 +490,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.appcontainers.models.ManagedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -560,33 +549,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -623,17 +611,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -683,17 +669,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.ManagedEnvironment]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(environment_envelope, (IO, bytes)):
@@ -712,16 +696,17 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -829,16 +814,16 @@
         Patches a Managed Environment using JSON Merge Patch.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Environment. Required.
         :type environment_name: str
-        :param environment_envelope: Configuration details of the Environment. Is either a model type
-         or a IO type. Required.
+        :param environment_envelope: Configuration details of the Environment. Is either a
+         ManagedEnvironment type or a IO type. Required.
         :type environment_envelope: ~azure.mgmt.appcontainers.models.ManagedEnvironment or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -851,17 +836,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.appcontainers.models.ManagedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ManagedEnvironment] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._update_initial(
@@ -927,33 +910,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.EnvironmentAuthToken] = kwargs.pop("cls", None)
 
         request = build_get_auth_token_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get_auth_token.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -970,17 +952,17 @@
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/managedEnvironments/{environmentName}/getAuthtoken"
     }
 
     @distributed_trace
     def list_workload_profile_states(
         self, resource_group_name: str, environment_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.WorkloadProfileStates"]:
-        """Get all workload Profile States for a Premium Managed Environment..
+        """Get all workload Profile States for a Managed Environment..
 
-        Get all workload Profile States for a Premium Managed Environment.
+        Get all workload Profile States for a Managed Environment.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -989,17 +971,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.WorkloadProfileStates]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.WorkloadProfileStatesCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1045,16 +1025,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -37,18 +36,14 @@
     build_delete_request,
     build_get_request,
     build_list_by_resource_group_request,
     build_list_by_subscription_request,
     build_update_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ConnectedEnvironmentsOperations:
     """
     .. warning::
@@ -80,17 +75,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.ConnectedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironmentCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -134,16 +127,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -171,17 +165,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.ConnectedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironmentCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -226,16 +218,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -271,33 +264,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironment] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -307,15 +299,15 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         connected_environment_name: str,
         environment_envelope: Union[_models.ConnectedEnvironment, IO],
@@ -328,17 +320,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConnectedEnvironment] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(environment_envelope, (IO, bytes)):
@@ -357,16 +347,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -380,15 +371,15 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         connected_environment_name: str,
@@ -473,15 +464,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the connectedEnvironment. Required.
         :type connected_environment_name: str
         :param environment_envelope: Configuration details of the connectedEnvironment. Is either a
-         model type or a IO type. Required.
+         ConnectedEnvironment type or a IO type. Required.
         :type environment_envelope: ~azure.mgmt.appcontainers.models.ConnectedEnvironment or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -495,17 +486,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.appcontainers.models.ConnectedEnvironment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConnectedEnvironment] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -524,30 +513,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ConnectedEnvironment", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, connected_environment_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
@@ -556,47 +548,50 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, connected_environment_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete an connectedEnvironment.
@@ -619,17 +614,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -643,30 +636,32 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     @distributed_trace_async
     async def update(
         self, resource_group_name: str, connected_environment_name: str, **kwargs: Any
     ) -> _models.ConnectedEnvironment:
         """Update connected Environment's properties.
@@ -690,33 +685,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironment] = kwargs.pop("cls", None)
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -726,15 +720,15 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/connectedEnvironments/{connectedEnvironmentName}"
     }
 
     @overload
     async def check_name_availability(
         self,
         resource_group_name: str,
         connected_environment_name: str,
@@ -810,15 +804,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the Managed Environment. Required.
         :type connected_environment_name: str
         :param check_name_availability_request: The check connectedEnvironmentName availability
-         request. Is either a model type or a IO type. Required.
+         request. Is either a CheckNameAvailabilityRequest type or a IO type. Required.
         :type check_name_availability_request:
          ~azure.mgmt.appcontainers.models.CheckNameAvailabilityRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResponse or the result of cls(response)
@@ -832,17 +826,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CheckNameAvailabilityResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(check_name_availability_request, (IO, bytes)):
@@ -861,16 +853,17 @@
             template_url=self.check_name_availability.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -39,18 +38,14 @@
     build_list_by_resource_group_request,
     build_list_by_subscription_request,
     build_list_custom_host_name_analysis_request,
     build_list_secrets_request,
     build_update_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ContainerAppsOperations:
     """
     .. warning::
@@ -80,17 +75,15 @@
         :return: An iterator like instance of either ContainerApp or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.ContainerApp]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerAppCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -134,16 +127,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -167,17 +161,15 @@
         :return: An iterator like instance of either ContainerApp or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.ContainerApp]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerAppCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -222,16 +214,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -267,33 +260,32 @@
             404: lambda response: ResourceNotFoundError(response=response, error_format=ARMErrorFormat),
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -324,17 +316,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(container_app_envelope, (IO, bytes)):
@@ -353,16 +343,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -472,16 +463,16 @@
         Create or update a Container App.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param container_app_name: Name of the Container App. Required.
         :type container_app_name: str
-        :param container_app_envelope: Properties used to create a container app. Is either a model
-         type or a IO type. Required.
+        :param container_app_envelope: Properties used to create a container app. Is either a
+         ContainerApp type or a IO type. Required.
         :type container_app_envelope: ~azure.mgmt.appcontainers.models.ContainerApp or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -494,17 +485,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.appcontainers.models.ContainerApp]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -523,15 +512,18 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ContainerApp", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
@@ -555,44 +547,47 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _delete_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}"
     }
 
     @distributed_trace_async
     async def begin_delete(
@@ -618,17 +613,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -642,15 +635,17 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
@@ -678,17 +673,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.ContainerApp]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(container_app_envelope, (IO, bytes)):
@@ -707,31 +700,36 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("ContainerApp", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
     _update_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.App/containerApps/{containerAppName}"
     }
 
@@ -825,15 +823,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param container_app_name: Name of the Container App. Required.
         :type container_app_name: str
         :param container_app_envelope: Properties of a Container App that need to be updated. Is either
-         a model type or a IO type. Required.
+         a ContainerApp type or a IO type. Required.
         :type container_app_envelope: ~azure.mgmt.appcontainers.models.ContainerApp or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -846,17 +844,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.appcontainers.models.ContainerApp]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ContainerApp] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._update_initial(
@@ -924,17 +920,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CustomHostnameAnalysisResult] = kwargs.pop("cls", None)
 
         request = build_list_custom_host_name_analysis_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             custom_hostname=custom_hostname,
@@ -942,16 +936,17 @@
             template_url=self.list_custom_host_name_analysis.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -993,33 +988,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SecretsCollection] = kwargs.pop("cls", None)
 
         request = build_list_secrets_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list_secrets.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -1061,33 +1055,32 @@
             404: lambda response: ResourceNotFoundError(response=response, error_format=ARMErrorFormat),
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ContainerAppAuthToken] = kwargs.pop("cls", None)
 
         request = build_get_auth_token_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get_auth_token.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_available_workload_profiles_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_available_workload_profiles_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -26,18 +25,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._available_workload_profiles_operations import build_get_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class AvailableWorkloadProfilesOperations:
     """
     .. warning::
@@ -71,17 +66,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.AvailableWorkloadProfile]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AvailableWorkloadProfilesCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -126,16 +119,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_namespaces_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_namespaces_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,18 +23,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._namespaces_operations import build_check_name_availability_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class NamespacesOperations:
     """
     .. warning::
@@ -129,16 +124,16 @@
         Checks if resource name is available.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
-        :param check_name_availability_request: The check name availability request. Is either a model
-         type or a IO type. Required.
+        :param check_name_availability_request: The check name availability request. Is either a
+         CheckNameAvailabilityRequest type or a IO type. Required.
         :type check_name_availability_request:
          ~azure.mgmt.appcontainers.models.CheckNameAvailabilityRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResponse or the result of cls(response)
@@ -152,17 +147,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CheckNameAvailabilityResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(check_name_availability_request, (IO, bytes)):
@@ -181,16 +174,17 @@
             template_url=self.check_name_availability.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_revision_replicas_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_revision_replicas_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -27,18 +26,14 @@
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._container_apps_revision_replicas_operations import (
     build_get_replica_request,
     build_list_replicas_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ContainerAppsRevisionReplicasOperations:
     """
     .. warning::
@@ -87,17 +82,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Replica] = kwargs.pop("cls", None)
 
         request = build_get_replica_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             replica_name=replica_name,
@@ -106,16 +99,17 @@
             template_url=self.get_replica.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -159,17 +153,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ReplicaCollection] = kwargs.pop("cls", None)
 
         request = build_list_replicas_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -177,16 +169,17 @@
             template_url=self.list_replicas.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environments_storages_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environments_storages_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -29,18 +28,14 @@
 from ...operations._managed_environments_storages_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ManagedEnvironmentsStoragesOperations:
     """
     .. warning::
@@ -85,33 +80,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironmentStoragesCollection] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -155,17 +149,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ManagedEnvironmentStorage] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             storage_name=storage_name,
             subscription_id=self._config.subscription_id,
@@ -173,16 +165,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -281,16 +274,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Environment. Required.
         :type environment_name: str
         :param storage_name: Name of the storage. Required.
         :type storage_name: str
-        :param storage_envelope: Configuration details of storage. Is either a model type or a IO type.
-         Required.
+        :param storage_envelope: Configuration details of storage. Is either a
+         ManagedEnvironmentStorage type or a IO type. Required.
         :type storage_envelope: ~azure.mgmt.appcontainers.models.ManagedEnvironmentStorage or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ManagedEnvironmentStorage or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.ManagedEnvironmentStorage
@@ -303,17 +296,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ManagedEnvironmentStorage] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(storage_envelope, (IO, bytes)):
@@ -333,16 +324,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -386,17 +378,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             storage_name=storage_name,
             subscription_id=self._config.subscription_id,
@@ -404,16 +394,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_dapr_components_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_dapr_components_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -33,18 +32,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
     build_list_secrets_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DaprComponentsOperations:
     """
     .. warning::
@@ -81,17 +76,15 @@
         :return: An iterator like instance of either DaprComponent or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.DaprComponent]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprComponentsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -137,16 +130,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -186,17 +180,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprComponent] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -204,16 +196,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -312,16 +305,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
         :param component_name: Name of the Dapr Component. Required.
         :type component_name: str
-        :param dapr_component_envelope: Configuration details of the Dapr Component. Is either a model
-         type or a IO type. Required.
+        :param dapr_component_envelope: Configuration details of the Dapr Component. Is either a
+         DaprComponent type or a IO type. Required.
         :type dapr_component_envelope: ~azure.mgmt.appcontainers.models.DaprComponent or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DaprComponent or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.DaprComponent
@@ -334,17 +327,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DaprComponent] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(dapr_component_envelope, (IO, bytes)):
@@ -364,16 +355,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -417,17 +409,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -435,16 +425,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -484,17 +475,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprSecretsCollection] = kwargs.pop("cls", None)
 
         request = build_list_secrets_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -502,16 +491,17 @@
             template_url=self.list_secrets.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_auth_configs_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_auth_configs_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -32,18 +31,14 @@
 from ...operations._container_apps_auth_configs_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_container_app_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ContainerAppsAuthConfigsOperations:
     """
     .. warning::
@@ -80,17 +75,15 @@
         :return: An iterator like instance of either AuthConfig or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.AuthConfig]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AuthConfigCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -136,16 +129,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -185,17 +179,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AuthConfig] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             auth_config_name=auth_config_name,
             subscription_id=self._config.subscription_id,
@@ -203,16 +195,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -312,15 +305,15 @@
          Required.
         :type resource_group_name: str
         :param container_app_name: Name of the Container App. Required.
         :type container_app_name: str
         :param auth_config_name: Name of the Container App AuthConfig. Required.
         :type auth_config_name: str
         :param auth_config_envelope: Properties used to create a Container App AuthConfig. Is either a
-         model type or a IO type. Required.
+         AuthConfig type or a IO type. Required.
         :type auth_config_envelope: ~azure.mgmt.appcontainers.models.AuthConfig or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AuthConfig or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.AuthConfig
@@ -333,17 +326,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AuthConfig] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(auth_config_envelope, (IO, bytes)):
@@ -363,16 +354,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -416,17 +408,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             auth_config_name=auth_config_name,
             subscription_id=self._config.subscription_id,
@@ -434,16 +424,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_certificates_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_certificates_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -33,18 +32,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
     build_update_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class CertificatesOperations:
     """
     .. warning::
@@ -81,17 +76,15 @@
         :return: An iterator like instance of either Certificate or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.Certificate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CertificateCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -137,16 +130,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -186,17 +180,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
@@ -204,16 +196,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -312,16 +305,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
         :param certificate_name: Name of the Certificate. Required.
         :type certificate_name: str
-        :param certificate_envelope: Certificate to be created or updated. Is either a model type or a
-         IO type. Default value is None.
+        :param certificate_envelope: Certificate to be created or updated. Is either a Certificate type
+         or a IO type. Default value is None.
         :type certificate_envelope: ~azure.mgmt.appcontainers.models.Certificate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Certificate or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.Certificate
@@ -334,17 +327,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(certificate_envelope, (IO, bytes)):
@@ -367,16 +358,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -420,17 +412,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
@@ -438,16 +428,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -543,15 +534,15 @@
          Required.
         :type resource_group_name: str
         :param environment_name: Name of the Managed Environment. Required.
         :type environment_name: str
         :param certificate_name: Name of the Certificate. Required.
         :type certificate_name: str
         :param certificate_envelope: Properties of a certificate that need to be updated. Is either a
-         model type or a IO type. Required.
+         CertificatePatch type or a IO type. Required.
         :type certificate_envelope: ~azure.mgmt.appcontainers.models.CertificatePatch or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Certificate or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.Certificate
@@ -564,17 +555,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(certificate_envelope, (IO, bytes)):
@@ -594,16 +583,17 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_certificates_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_certificates_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -33,18 +32,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
     build_update_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ConnectedEnvironmentsCertificatesOperations:
     """
     .. warning::
@@ -81,17 +76,15 @@
         :return: An iterator like instance of either Certificate or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.Certificate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CertificateCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -137,16 +130,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -186,17 +180,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
@@ -204,16 +196,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -312,16 +305,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the Connected Environment. Required.
         :type connected_environment_name: str
         :param certificate_name: Name of the Certificate. Required.
         :type certificate_name: str
-        :param certificate_envelope: Certificate to be created or updated. Is either a model type or a
-         IO type. Default value is None.
+        :param certificate_envelope: Certificate to be created or updated. Is either a Certificate type
+         or a IO type. Default value is None.
         :type certificate_envelope: ~azure.mgmt.appcontainers.models.Certificate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Certificate or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.Certificate
@@ -334,17 +327,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(certificate_envelope, (IO, bytes)):
@@ -367,16 +358,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -420,17 +412,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
@@ -438,16 +428,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -543,15 +534,15 @@
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the Connected Environment. Required.
         :type connected_environment_name: str
         :param certificate_name: Name of the Certificate. Required.
         :type certificate_name: str
         :param certificate_envelope: Properties of a certificate that need to be updated. Is either a
-         model type or a IO type. Required.
+         CertificatePatch type or a IO type. Required.
         :type certificate_envelope: ~azure.mgmt.appcontainers.models.CertificatePatch or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Certificate or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.Certificate
@@ -564,17 +555,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Certificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(certificate_envelope, (IO, bytes)):
@@ -594,16 +583,17 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_storages_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_storages_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -29,18 +28,14 @@
 from ...operations._connected_environments_storages_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ConnectedEnvironmentsStoragesOperations:
     """
     .. warning::
@@ -85,33 +80,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironmentStoragesCollection] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -155,17 +149,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConnectedEnvironmentStorage] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             storage_name=storage_name,
             subscription_id=self._config.subscription_id,
@@ -173,16 +165,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -281,16 +274,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the Environment. Required.
         :type connected_environment_name: str
         :param storage_name: Name of the storage. Required.
         :type storage_name: str
-        :param storage_envelope: Configuration details of storage. Is either a model type or a IO type.
-         Required.
+        :param storage_envelope: Configuration details of storage. Is either a
+         ConnectedEnvironmentStorage type or a IO type. Required.
         :type storage_envelope: ~azure.mgmt.appcontainers.models.ConnectedEnvironmentStorage or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConnectedEnvironmentStorage or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.ConnectedEnvironmentStorage
@@ -303,17 +296,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConnectedEnvironmentStorage] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(storage_envelope, (IO, bytes)):
@@ -333,16 +324,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -386,17 +378,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             storage_name=storage_name,
             subscription_id=self._config.subscription_id,
@@ -404,16 +394,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_connected_environments_dapr_components_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_connected_environments_dapr_components_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -33,18 +32,14 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
     build_list_secrets_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ConnectedEnvironmentsDaprComponentsOperations:
     """
     .. warning::
@@ -81,17 +76,15 @@
         :return: An iterator like instance of either DaprComponent or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.DaprComponent]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprComponentsCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -137,16 +130,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -186,17 +180,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprComponent] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -204,16 +196,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -312,16 +305,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param connected_environment_name: Name of the connected environment. Required.
         :type connected_environment_name: str
         :param component_name: Name of the Dapr Component. Required.
         :type component_name: str
-        :param dapr_component_envelope: Configuration details of the Dapr Component. Is either a model
-         type or a IO type. Required.
+        :param dapr_component_envelope: Configuration details of the Dapr Component. Is either a
+         DaprComponent type or a IO type. Required.
         :type dapr_component_envelope: ~azure.mgmt.appcontainers.models.DaprComponent or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DaprComponent or the result of cls(response)
         :rtype: ~azure.mgmt.appcontainers.models.DaprComponent
@@ -334,17 +327,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DaprComponent] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(dapr_component_envelope, (IO, bytes)):
@@ -364,16 +355,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -417,17 +409,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -435,16 +425,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -484,17 +475,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DaprSecretsCollection] = kwargs.pop("cls", None)
 
         request = build_list_secrets_request(
             resource_group_name=resource_group_name,
             connected_environment_name=connected_environment_name,
             component_name=component_name,
             subscription_id=self._config.subscription_id,
@@ -502,16 +491,17 @@
             template_url=self.list_secrets.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_revisions_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_revisions_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -33,18 +32,14 @@
     build_activate_revision_request,
     build_deactivate_revision_request,
     build_get_revision_request,
     build_list_revisions_request,
     build_restart_revision_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ContainerAppsRevisionsOperations:
     """
     .. warning::
@@ -83,17 +78,15 @@
         :return: An iterator like instance of either Revision or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.Revision]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.RevisionCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -140,16 +133,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -189,17 +183,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Revision] = kwargs.pop("cls", None)
 
         request = build_get_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -207,16 +199,17 @@
             template_url=self.get_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -260,17 +253,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_activate_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -278,16 +269,17 @@
             template_url=self.activate_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -327,17 +319,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_deactivate_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -345,16 +335,17 @@
             template_url=self.deactivate_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -394,17 +385,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_restart_revision_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             revision_name=revision_name,
             subscription_id=self._config.subscription_id,
@@ -412,16 +401,17 @@
             template_url=self.restart_revision.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_patch.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_container_apps_source_controls_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_container_apps_source_controls_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -34,18 +33,14 @@
 from ...operations._container_apps_source_controls_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_container_app_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ContainerAppsSourceControlsOperations:
     """
     .. warning::
@@ -82,17 +77,15 @@
         :return: An iterator like instance of either SourceControl or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.appcontainers.models.SourceControl]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SourceControlCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -138,16 +131,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -187,17 +181,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SourceControl] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             source_control_name=source_control_name,
             subscription_id=self._config.subscription_id,
@@ -205,16 +197,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -246,17 +239,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SourceControl] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(source_control_envelope, (IO, bytes)):
@@ -276,16 +267,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -407,15 +399,15 @@
          Required.
         :type resource_group_name: str
         :param container_app_name: Name of the Container App. Required.
         :type container_app_name: str
         :param source_control_name: Name of the Container App SourceControl. Required.
         :type source_control_name: str
         :param source_control_envelope: Properties used to create a Container App SourceControl. Is
-         either a model type or a IO type. Required.
+         either a SourceControl type or a IO type. Required.
         :type source_control_envelope: ~azure.mgmt.appcontainers.models.SourceControl or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -428,17 +420,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.appcontainers.models.SourceControl]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SourceControl] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -490,17 +480,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             container_app_name=container_app_name,
             source_control_name=source_control_name,
             subscription_id=self._config.subscription_id,
@@ -508,16 +496,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -556,17 +545,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/_managed_environment_diagnostics_operations.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/aio/operations/_managed_environment_diagnostics_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -27,18 +26,14 @@
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._managed_environment_diagnostics_operations import (
     build_get_detector_request,
     build_list_detectors_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ManagedEnvironmentDiagnosticsOperations:
     """
     .. warning::
@@ -83,33 +78,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DiagnosticsCollection] = kwargs.pop("cls", None)
 
         request = build_list_detectors_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list_detectors.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
@@ -153,17 +147,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-10-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Diagnostics] = kwargs.pop("cls", None)
 
         request = build_get_detector_request(
             resource_group_name=resource_group_name,
             environment_name=environment_name,
             detector_name=detector_name,
             subscription_id=self._config.subscription_id,
@@ -171,16 +163,17 @@
             template_url=self.get_detector.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.DefaultErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/aio/operations/__init__.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,25 @@
 from ._available_workload_profiles_operations import AvailableWorkloadProfilesOperations
 from ._billing_meters_operations import BillingMetersOperations
 from ._connected_environments_operations import ConnectedEnvironmentsOperations
 from ._connected_environments_certificates_operations import ConnectedEnvironmentsCertificatesOperations
 from ._connected_environments_dapr_components_operations import ConnectedEnvironmentsDaprComponentsOperations
 from ._connected_environments_storages_operations import ConnectedEnvironmentsStoragesOperations
 from ._container_apps_operations import ContainerAppsOperations
+from ._jobs_operations import JobsOperations
+from ._jobs_executions_operations import JobsExecutionsOperations
 from ._container_apps_revisions_operations import ContainerAppsRevisionsOperations
 from ._container_apps_revision_replicas_operations import ContainerAppsRevisionReplicasOperations
 from ._container_apps_diagnostics_operations import ContainerAppsDiagnosticsOperations
 from ._managed_environment_diagnostics_operations import ManagedEnvironmentDiagnosticsOperations
 from ._managed_environments_diagnostics_operations import ManagedEnvironmentsDiagnosticsOperations
 from ._operations import Operations
 from ._managed_environments_operations import ManagedEnvironmentsOperations
 from ._certificates_operations import CertificatesOperations
+from ._managed_certificates_operations import ManagedCertificatesOperations
 from ._namespaces_operations import NamespacesOperations
 from ._dapr_components_operations import DaprComponentsOperations
 from ._managed_environments_storages_operations import ManagedEnvironmentsStoragesOperations
 from ._container_apps_source_controls_operations import ContainerAppsSourceControlsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
@@ -36,22 +39,25 @@
     "AvailableWorkloadProfilesOperations",
     "BillingMetersOperations",
     "ConnectedEnvironmentsOperations",
     "ConnectedEnvironmentsCertificatesOperations",
     "ConnectedEnvironmentsDaprComponentsOperations",
     "ConnectedEnvironmentsStoragesOperations",
     "ContainerAppsOperations",
+    "JobsOperations",
+    "JobsExecutionsOperations",
     "ContainerAppsRevisionsOperations",
     "ContainerAppsRevisionReplicasOperations",
     "ContainerAppsDiagnosticsOperations",
     "ManagedEnvironmentDiagnosticsOperations",
     "ManagedEnvironmentsDiagnosticsOperations",
     "Operations",
     "ManagedEnvironmentsOperations",
     "CertificatesOperations",
+    "ManagedCertificatesOperations",
     "NamespacesOperations",
     "DaprComponentsOperations",
     "ManagedEnvironmentsStoragesOperations",
     "ContainerAppsSourceControlsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/_models_py3.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/_models_py3.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     :vartype allowed_audiences: list[str]
     """
 
     _attribute_map = {
         "allowed_audiences": {"key": "allowedAudiences", "type": "[str]"},
     }
 
-    def __init__(self, *, allowed_audiences: Optional[List[str]] = None, **kwargs):
+    def __init__(self, *, allowed_audiences: Optional[List[str]] = None, **kwargs: Any) -> None:
         """
         :keyword allowed_audiences: The configuration settings of the allowed list of audiences from
          which to validate the JWT token.
         :paramtype allowed_audiences: list[str]
         """
         super().__init__(**kwargs)
         self.allowed_audiences = allowed_audiences
@@ -60,15 +60,17 @@
     """
 
     _attribute_map = {
         "groups": {"key": "groups", "type": "[str]"},
         "identities": {"key": "identities", "type": "[str]"},
     }
 
-    def __init__(self, *, groups: Optional[List[str]] = None, identities: Optional[List[str]] = None, **kwargs):
+    def __init__(
+        self, *, groups: Optional[List[str]] = None, identities: Optional[List[str]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword groups: The list of the allowed groups.
         :paramtype groups: list[str]
         :keyword identities: The list of the allowed identities.
         :paramtype identities: list[str]
         """
         super().__init__(**kwargs)
@@ -96,16 +98,16 @@
 
     def __init__(
         self,
         *,
         enabled: Optional[bool] = None,
         registration: Optional["_models.AppleRegistration"] = None,
         login: Optional["_models.LoginScopes"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: :code:`<code>false</code>` if the Apple provider should not be enabled
          despite the set registration; otherwise, :code:`<code>true</code>`.
         :paramtype enabled: bool
         :keyword registration: The configuration settings of the Apple registration.
         :paramtype registration: ~azure.mgmt.appcontainers.models.AppleRegistration
         :keyword login: The configuration settings of the login flow.
@@ -127,15 +129,17 @@
     """
 
     _attribute_map = {
         "client_id": {"key": "clientId", "type": "str"},
         "client_secret_setting_name": {"key": "clientSecretSettingName", "type": "str"},
     }
 
-    def __init__(self, *, client_id: Optional[str] = None, client_secret_setting_name: Optional[str] = None, **kwargs):
+    def __init__(
+        self, *, client_id: Optional[str] = None, client_secret_setting_name: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword client_id: The Client ID of the app used for login.
         :paramtype client_id: str
         :keyword client_secret_setting_name: The app setting name that contains the client secret.
         :paramtype client_secret_setting_name: str
         """
         super().__init__(**kwargs)
@@ -159,43 +163,46 @@
     }
 
     def __init__(
         self,
         *,
         destination: Optional[str] = None,
         log_analytics_configuration: Optional["_models.LogAnalyticsConfiguration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword destination: Logs destination.
         :paramtype destination: str
         :keyword log_analytics_configuration: Log Analytics configuration.
         :paramtype log_analytics_configuration:
          ~azure.mgmt.appcontainers.models.LogAnalyticsConfiguration
         """
         super().__init__(**kwargs)
         self.destination = destination
         self.log_analytics_configuration = log_analytics_configuration
 
 
 class AppRegistration(_serialization.Model):
-    """The configuration settings of the app registration for providers that have app ids and app secrets.
+    """The configuration settings of the app registration for providers that have app ids and app
+    secrets.
 
     :ivar app_id: The App ID of the app used for login.
     :vartype app_id: str
     :ivar app_secret_setting_name: The app setting name that contains the app secret.
     :vartype app_secret_setting_name: str
     """
 
     _attribute_map = {
         "app_id": {"key": "appId", "type": "str"},
         "app_secret_setting_name": {"key": "appSecretSettingName", "type": "str"},
     }
 
-    def __init__(self, *, app_id: Optional[str] = None, app_secret_setting_name: Optional[str] = None, **kwargs):
+    def __init__(
+        self, *, app_id: Optional[str] = None, app_secret_setting_name: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword app_id: The App ID of the app used for login.
         :paramtype app_id: str
         :keyword app_secret_setting_name: The app setting name that contains the app secret.
         :paramtype app_secret_setting_name: str
         """
         super().__init__(**kwargs)
@@ -231,25 +238,26 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.system_data = None
 
 
 class ProxyResource(Resource):
-    """The resource model definition for a Azure Resource Manager proxy resource. It will not have tags and a location.
+    """The resource model definition for a Azure Resource Manager proxy resource. It will not have
+    tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
     :vartype id: str
     :ivar name: The name of the resource.
@@ -272,21 +280,22 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
 
 
 class AuthConfig(ProxyResource):
-    """Configuration settings for the Azure ContainerApp Service Authentication / Authorization feature.
+    """Configuration settings for the Azure ContainerApp Service Authentication / Authorization
+    feature.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
     :vartype id: str
     :ivar name: The name of the resource.
@@ -337,16 +346,16 @@
         self,
         *,
         platform: Optional["_models.AuthPlatform"] = None,
         global_validation: Optional["_models.GlobalValidation"] = None,
         identity_providers: Optional["_models.IdentityProviders"] = None,
         login: Optional["_models.Login"] = None,
         http_settings: Optional["_models.HttpSettings"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword platform: The configuration settings of the platform of ContainerApp Service
          Authentication/Authorization.
         :paramtype platform: ~azure.mgmt.appcontainers.models.AuthPlatform
         :keyword global_validation: The configuration settings that determines the validation flow of
          users using  Service Authentication/Authorization.
         :paramtype global_validation: ~azure.mgmt.appcontainers.models.GlobalValidation
@@ -387,26 +396,27 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[AuthConfig]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.AuthConfig"], **kwargs):
+    def __init__(self, *, value: List["_models.AuthConfig"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.AuthConfig]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
 
 
 class AuthPlatform(_serialization.Model):
-    """The configuration settings of the platform of ContainerApp Service Authentication/Authorization.
+    """The configuration settings of the platform of ContainerApp Service
+    Authentication/Authorization.
 
     :ivar enabled: :code:`<code>true</code>` if the Authentication / Authorization feature is
      enabled for the current app; otherwise, :code:`<code>false</code>`.
     :vartype enabled: bool
     :ivar runtime_version: The RuntimeVersion of the Authentication / Authorization feature in use
      for the current app.
      The setting in this value can control the behavior of certain features in the Authentication /
@@ -415,15 +425,15 @@
     """
 
     _attribute_map = {
         "enabled": {"key": "enabled", "type": "bool"},
         "runtime_version": {"key": "runtimeVersion", "type": "str"},
     }
 
-    def __init__(self, *, enabled: Optional[bool] = None, runtime_version: Optional[str] = None, **kwargs):
+    def __init__(self, *, enabled: Optional[bool] = None, runtime_version: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword enabled: :code:`<code>true</code>` if the Authentication / Authorization feature is
          enabled for the current app; otherwise, :code:`<code>false</code>`.
         :paramtype enabled: bool
         :keyword runtime_version: The RuntimeVersion of the Authentication / Authorization feature in
          use for the current app.
          The setting in this value can control the behavior of certain features in the Authentication /
@@ -447,30 +457,30 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[OperationDetail]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.OperationDetail"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self, *, value: Optional[List["_models.OperationDetail"]] = None, next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: Collection of available operation details.
         :paramtype value: list[~azure.mgmt.appcontainers.models.OperationDetail]
         :keyword next_link: URL client should use to fetch the next page (per server side paging).
          It's null for now, added for future use.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
 class AvailableWorkloadProfile(ProxyResource):
-    """A premium workload profile.
+    """A workload profile with specific hardware configure to run container apps.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
     :vartype id: str
     :ivar name: The name of the resource.
@@ -504,79 +514,76 @@
     }
 
     def __init__(
         self,
         *,
         location: Optional[str] = None,
         properties: Optional["_models.AvailableWorkloadProfileProperties"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword location: Region of the workload profile.
         :paramtype location: str
         :keyword properties: Revision resource specific properties.
         :paramtype properties: ~azure.mgmt.appcontainers.models.AvailableWorkloadProfileProperties
         """
         super().__init__(**kwargs)
         self.location = location
         self.properties = properties
 
 
 class AvailableWorkloadProfileProperties(_serialization.Model):
     """Revision resource specific properties.
 
-    :ivar billing_meter_category: Used to map workload profile types to billing meter. Known values
-     are: "PremiumSkuGeneralPurpose", "PremiumSkuMemoryOptimized", and "PremiumSkuComputeOptimized".
-    :vartype billing_meter_category: str or ~azure.mgmt.appcontainers.models.Category
+    :ivar category: Used to categorize workload profiles.
+    :vartype category: str
     :ivar applicability: indicates whether the profile is default for the location. Known values
      are: "LocationDefault" and "Custom".
     :vartype applicability: str or ~azure.mgmt.appcontainers.models.Applicability
     :ivar cores: Number of cores in CPU.
     :vartype cores: int
     :ivar memory_gi_b: Memory in GiB.
     :vartype memory_gi_b: int
     :ivar display_name: The everyday name of the workload profile.
     :vartype display_name: str
     """
 
     _attribute_map = {
-        "billing_meter_category": {"key": "billingMeterCategory", "type": "str"},
+        "category": {"key": "category", "type": "str"},
         "applicability": {"key": "applicability", "type": "str"},
         "cores": {"key": "cores", "type": "int"},
         "memory_gi_b": {"key": "memoryGiB", "type": "int"},
         "display_name": {"key": "displayName", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        billing_meter_category: Optional[Union[str, "_models.Category"]] = None,
+        category: Optional[str] = None,
         applicability: Optional[Union[str, "_models.Applicability"]] = None,
         cores: Optional[int] = None,
         memory_gi_b: Optional[int] = None,
         display_name: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword billing_meter_category: Used to map workload profile types to billing meter. Known
-         values are: "PremiumSkuGeneralPurpose", "PremiumSkuMemoryOptimized", and
-         "PremiumSkuComputeOptimized".
-        :paramtype billing_meter_category: str or ~azure.mgmt.appcontainers.models.Category
+        :keyword category: Used to categorize workload profiles.
+        :paramtype category: str
         :keyword applicability: indicates whether the profile is default for the location. Known values
          are: "LocationDefault" and "Custom".
         :paramtype applicability: str or ~azure.mgmt.appcontainers.models.Applicability
         :keyword cores: Number of cores in CPU.
         :paramtype cores: int
         :keyword memory_gi_b: Memory in GiB.
         :paramtype memory_gi_b: int
         :keyword display_name: The everyday name of the workload profile.
         :paramtype display_name: str
         """
         super().__init__(**kwargs)
-        self.billing_meter_category = billing_meter_category
+        self.category = category
         self.applicability = applicability
         self.cores = cores
         self.memory_gi_b = memory_gi_b
         self.display_name = display_name
 
 
 class AvailableWorkloadProfilesCollection(_serialization.Model):
@@ -598,15 +605,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[AvailableWorkloadProfile]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.AvailableWorkloadProfile"], **kwargs):
+    def __init__(self, *, value: List["_models.AvailableWorkloadProfile"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of workload profiles. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.AvailableWorkloadProfile]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -645,16 +652,16 @@
         self,
         *,
         enabled: Optional[bool] = None,
         registration: Optional["_models.AzureActiveDirectoryRegistration"] = None,
         login: Optional["_models.AzureActiveDirectoryLogin"] = None,
         validation: Optional["_models.AzureActiveDirectoryValidation"] = None,
         is_auto_provisioned: Optional[bool] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: :code:`<code>false</code>` if the Azure Active Directory provider should not
          be enabled despite the set registration; otherwise, :code:`<code>true</code>`.
         :paramtype enabled: bool
         :keyword registration: The configuration settings of the Azure Active Directory app
          registration.
         :paramtype registration: ~azure.mgmt.appcontainers.models.AzureActiveDirectoryRegistration
@@ -692,16 +699,20 @@
 
     _attribute_map = {
         "login_parameters": {"key": "loginParameters", "type": "[str]"},
         "disable_www_authenticate": {"key": "disableWWWAuthenticate", "type": "bool"},
     }
 
     def __init__(
-        self, *, login_parameters: Optional[List[str]] = None, disable_www_authenticate: Optional[bool] = None, **kwargs
-    ):
+        self,
+        *,
+        login_parameters: Optional[List[str]] = None,
+        disable_www_authenticate: Optional[bool] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword login_parameters: Login parameters to send to the OpenID Connect authorization
          endpoint when
          a user logs in. Each parameter must be in the form "key=value".
         :paramtype login_parameters: list[str]
         :keyword disable_www_authenticate: :code:`<code>true</code>` if the www-authenticate provider
          should be omitted from the request; otherwise, :code:`<code>false</code>`.
@@ -764,16 +775,16 @@
         *,
         open_id_issuer: Optional[str] = None,
         client_id: Optional[str] = None,
         client_secret_setting_name: Optional[str] = None,
         client_secret_certificate_thumbprint: Optional[str] = None,
         client_secret_certificate_subject_alternative_name: Optional[str] = None,
         client_secret_certificate_issuer: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword open_id_issuer: The OpenID Connect Issuer URI that represents the entity which issues
          access tokens for this application.
          When using Azure Active Directory, this value is the URI of the directory tenant, e.g.
          https://login.microsoftonline.com/v2.0/{tenant-guid}/.
          This URI is a case-sensitive identifier for the token issuer.
          More information on OpenID Connect Discovery:
@@ -834,16 +845,16 @@
 
     def __init__(
         self,
         *,
         jwt_claim_checks: Optional["_models.JwtClaimChecks"] = None,
         allowed_audiences: Optional[List[str]] = None,
         default_authorization_policy: Optional["_models.DefaultAuthorizationPolicy"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword jwt_claim_checks: The configuration settings of the checks that should be made while
          validating the JWT Claims.
         :paramtype jwt_claim_checks: ~azure.mgmt.appcontainers.models.JwtClaimChecks
         :keyword allowed_audiences: The list of audiences that can make successful
          authentication/authorization requests.
         :paramtype allowed_audiences: list[str]
@@ -881,16 +892,16 @@
     def __init__(
         self,
         *,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         tenant_id: Optional[str] = None,
         subscription_id: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword client_id: Client Id.
         :paramtype client_id: str
         :keyword client_secret: Client Secret.
         :paramtype client_secret: str
         :keyword tenant_id: Tenant Id.
         :paramtype tenant_id: str
@@ -927,16 +938,16 @@
     def __init__(
         self,
         *,
         account_name: Optional[str] = None,
         account_key: Optional[str] = None,
         access_mode: Optional[Union[str, "_models.AccessMode"]] = None,
         share_name: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword account_name: Storage account name for azure file.
         :paramtype account_name: str
         :keyword account_key: Storage account key for azure file.
         :paramtype account_key: str
         :keyword access_mode: Access mode for storage. Known values are: "ReadOnly" and "ReadWrite".
         :paramtype access_mode: str or ~azure.mgmt.appcontainers.models.AccessMode
@@ -966,16 +977,16 @@
     }
 
     def __init__(
         self,
         *,
         enabled: Optional[bool] = None,
         registration: Optional["_models.AzureStaticWebAppsRegistration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: :code:`<code>false</code>` if the Azure Static Web Apps provider should not
          be enabled despite the set registration; otherwise, :code:`<code>true</code>`.
         :paramtype enabled: bool
         :keyword registration: The configuration settings of the Azure Static Web Apps registration.
         :paramtype registration: ~azure.mgmt.appcontainers.models.AzureStaticWebAppsRegistration
         """
@@ -991,15 +1002,15 @@
     :vartype client_id: str
     """
 
     _attribute_map = {
         "client_id": {"key": "clientId", "type": "str"},
     }
 
-    def __init__(self, *, client_id: Optional[str] = None, **kwargs):
+    def __init__(self, *, client_id: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword client_id: The Client ID of the app used for login.
         :paramtype client_id: str
         """
         super().__init__(**kwargs)
         self.client_id = client_id
 
@@ -1039,16 +1050,16 @@
         image: Optional[str] = None,
         name: Optional[str] = None,
         command: Optional[List[str]] = None,
         args: Optional[List[str]] = None,
         env: Optional[List["_models.EnvironmentVar"]] = None,
         resources: Optional["_models.ContainerResources"] = None,
         volume_mounts: Optional[List["_models.VolumeMount"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword image: Container image tag.
         :paramtype image: str
         :keyword name: Custom container name.
         :paramtype name: str
         :keyword command: Container start command.
         :paramtype command: list[str]
@@ -1068,15 +1079,15 @@
         self.args = args
         self.env = env
         self.resources = resources
         self.volume_mounts = volume_mounts
 
 
 class BillingMeter(ProxyResource):
-    """A premium billing meter.
+    """Billing meter.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
     :vartype id: str
     :ivar name: The name of the resource.
@@ -1106,29 +1117,33 @@
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "location": {"key": "location", "type": "str"},
         "properties": {"key": "properties", "type": "BillingMeterProperties"},
     }
 
     def __init__(
-        self, *, location: Optional[str] = None, properties: Optional["_models.BillingMeterProperties"] = None, **kwargs
-    ):
+        self,
+        *,
+        location: Optional[str] = None,
+        properties: Optional["_models.BillingMeterProperties"] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword location: Region for the billing meter.
         :paramtype location: str
         :keyword properties: Revision resource specific properties.
         :paramtype properties: ~azure.mgmt.appcontainers.models.BillingMeterProperties
         """
         super().__init__(**kwargs)
         self.location = location
         self.properties = properties
 
 
 class BillingMeterCollection(_serialization.Model):
-    """Collection of premium workload billing meters.
+    """Collection of billing meters.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: Collection of billing meters. Required.
     :vartype value: list[~azure.mgmt.appcontainers.models.BillingMeter]
     """
 
@@ -1136,29 +1151,28 @@
         "value": {"required": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[BillingMeter]"},
     }
 
-    def __init__(self, *, value: List["_models.BillingMeter"], **kwargs):
+    def __init__(self, *, value: List["_models.BillingMeter"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of billing meters. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.BillingMeter]
         """
         super().__init__(**kwargs)
         self.value = value
 
 
 class BillingMeterProperties(_serialization.Model):
     """Revision resource specific properties.
 
-    :ivar category: Used to map workload profile types to billing meter. Known values are:
-     "PremiumSkuGeneralPurpose", "PremiumSkuMemoryOptimized", and "PremiumSkuComputeOptimized".
-    :vartype category: str or ~azure.mgmt.appcontainers.models.Category
+    :ivar category: Used to categorize billing meters.
+    :vartype category: str
     :ivar meter_type: Billing meter type.
     :vartype meter_type: str
     :ivar display_name: The everyday name of the billing meter.
     :vartype display_name: str
     """
 
     _attribute_map = {
@@ -1166,36 +1180,36 @@
         "meter_type": {"key": "meterType", "type": "str"},
         "display_name": {"key": "displayName", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        category: Optional[Union[str, "_models.Category"]] = None,
+        category: Optional[str] = None,
         meter_type: Optional[str] = None,
         display_name: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword category: Used to map workload profile types to billing meter. Known values are:
-         "PremiumSkuGeneralPurpose", "PremiumSkuMemoryOptimized", and "PremiumSkuComputeOptimized".
-        :paramtype category: str or ~azure.mgmt.appcontainers.models.Category
+        :keyword category: Used to categorize billing meters.
+        :paramtype category: str
         :keyword meter_type: Billing meter type.
         :paramtype meter_type: str
         :keyword display_name: The everyday name of the billing meter.
         :paramtype display_name: str
         """
         super().__init__(**kwargs)
         self.category = category
         self.meter_type = meter_type
         self.display_name = display_name
 
 
 class TrackedResource(Resource):
-    """The resource model definition for an Azure Resource Manager tracked top level resource which has 'tags' and a 'location'.
+    """The resource model definition for an Azure Resource Manager tracked top level resource which
+    has 'tags' and a 'location'.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
@@ -1227,15 +1241,15 @@
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
     }
 
-    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         """
         super().__init__(**kwargs)
@@ -1289,16 +1303,16 @@
 
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
         properties: Optional["_models.CertificateProperties"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword properties: Certificate resource specific properties.
         :paramtype properties: ~azure.mgmt.appcontainers.models.CertificateProperties
@@ -1326,15 +1340,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Certificate]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.Certificate"], **kwargs):
+    def __init__(self, *, value: List["_models.Certificate"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.Certificate]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -1347,15 +1361,15 @@
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "tags": {"key": "tags", "type": "{str}"},
     }
 
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Application-specific metadata in the form of key-value pairs.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.tags = tags
 
@@ -1413,15 +1427,15 @@
         "issue_date": {"key": "issueDate", "type": "iso-8601"},
         "expiration_date": {"key": "expirationDate", "type": "iso-8601"},
         "thumbprint": {"key": "thumbprint", "type": "str"},
         "valid": {"key": "valid", "type": "bool"},
         "public_key_hash": {"key": "publicKeyHash", "type": "str"},
     }
 
-    def __init__(self, *, password: Optional[str] = None, value: Optional[bytes] = None, **kwargs):
+    def __init__(self, *, password: Optional[str] = None, value: Optional[bytes] = None, **kwargs: Any) -> None:
         """
         :keyword password: Certificate password.
         :paramtype password: str
         :keyword value: PFX or PEM blob.
         :paramtype value: bytes
         """
         super().__init__(**kwargs)
@@ -1448,15 +1462,15 @@
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, type: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, type: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: The name of the resource for which availability needs to be checked.
         :paramtype name: str
         :keyword type: The resource type.
         :paramtype type: str
         """
         super().__init__(**kwargs)
@@ -1484,16 +1498,16 @@
 
     def __init__(
         self,
         *,
         name_available: Optional[bool] = None,
         reason: Optional[Union[str, "_models.CheckNameAvailabilityReason"]] = None,
         message: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name_available: Indicates if the resource name is available.
         :paramtype name_available: bool
         :keyword reason: The reason why the given name is not available. Known values are: "Invalid"
          and "AlreadyExists".
         :paramtype reason: str or ~azure.mgmt.appcontainers.models.CheckNameAvailabilityReason
         :keyword message: Detailed reason why the given name is available.
@@ -1502,41 +1516,45 @@
         super().__init__(**kwargs)
         self.name_available = name_available
         self.reason = reason
         self.message = message
 
 
 class ClientRegistration(_serialization.Model):
-    """The configuration settings of the app registration for providers that have client ids and client secrets.
+    """The configuration settings of the app registration for providers that have client ids and
+    client secrets.
 
     :ivar client_id: The Client ID of the app used for login.
     :vartype client_id: str
     :ivar client_secret_setting_name: The app setting name that contains the client secret.
     :vartype client_secret_setting_name: str
     """
 
     _attribute_map = {
         "client_id": {"key": "clientId", "type": "str"},
         "client_secret_setting_name": {"key": "clientSecretSettingName", "type": "str"},
     }
 
-    def __init__(self, *, client_id: Optional[str] = None, client_secret_setting_name: Optional[str] = None, **kwargs):
+    def __init__(
+        self, *, client_id: Optional[str] = None, client_secret_setting_name: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword client_id: The Client ID of the app used for login.
         :paramtype client_id: str
         :keyword client_secret_setting_name: The app setting name that contains the client secret.
         :paramtype client_secret_setting_name: str
         """
         super().__init__(**kwargs)
         self.client_id = client_id
         self.client_secret_setting_name = client_secret_setting_name
 
 
 class Configuration(_serialization.Model):
-    """Non versioned Container App configuration properties that define the mutable settings of a Container app.
+    """Non versioned Container App configuration properties that define the mutable settings of a
+    Container app.
 
     :ivar secrets: Collection of secrets used by a Container app.
     :vartype secrets: list[~azure.mgmt.appcontainers.models.Secret]
     :ivar active_revisions_mode: ActiveRevisionsMode controls how active revisions are handled for
      the Container app:
 
 
@@ -1571,16 +1589,16 @@
         *,
         secrets: Optional[List["_models.Secret"]] = None,
         active_revisions_mode: Union[str, "_models.ActiveRevisionsMode"] = "Single",
         ingress: Optional["_models.Ingress"] = None,
         registries: Optional[List["_models.RegistryCredentials"]] = None,
         dapr: Optional["_models.Dapr"] = None,
         max_inactive_revisions: Optional[int] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword secrets: Collection of secrets used by a Container app.
         :paramtype secrets: list[~azure.mgmt.appcontainers.models.Secret]
         :keyword active_revisions_mode: ActiveRevisionsMode controls how active revisions are handled
          for the Container app:
 
 
@@ -1687,16 +1705,16 @@
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
         extended_location: Optional["_models.ExtendedLocation"] = None,
         static_ip: Optional[str] = None,
         dapr_ai_connection_string: Optional[str] = None,
         custom_domain_configuration: Optional["_models.CustomDomainConfiguration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword extended_location: The complex type of the extended location.
         :paramtype extended_location: ~azure.mgmt.appcontainers.models.ExtendedLocation
@@ -1735,15 +1753,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[ConnectedEnvironment]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.ConnectedEnvironment"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.ConnectedEnvironment"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources.
         :paramtype value: list[~azure.mgmt.appcontainers.models.ConnectedEnvironment]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -1780,15 +1798,17 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "ConnectedEnvironmentStorageProperties"},
     }
 
-    def __init__(self, *, properties: Optional["_models.ConnectedEnvironmentStorageProperties"] = None, **kwargs):
+    def __init__(
+        self, *, properties: Optional["_models.ConnectedEnvironmentStorageProperties"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword properties: Storage properties.
         :paramtype properties: ~azure.mgmt.appcontainers.models.ConnectedEnvironmentStorageProperties
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -1800,15 +1820,15 @@
     :vartype azure_file: ~azure.mgmt.appcontainers.models.AzureFileProperties
     """
 
     _attribute_map = {
         "azure_file": {"key": "azureFile", "type": "AzureFileProperties"},
     }
 
-    def __init__(self, *, azure_file: Optional["_models.AzureFileProperties"] = None, **kwargs):
+    def __init__(self, *, azure_file: Optional["_models.AzureFileProperties"] = None, **kwargs: Any) -> None:
         """
         :keyword azure_file: Azure file properties.
         :paramtype azure_file: ~azure.mgmt.appcontainers.models.AzureFileProperties
         """
         super().__init__(**kwargs)
         self.azure_file = azure_file
 
@@ -1826,15 +1846,15 @@
         "value": {"required": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[ConnectedEnvironmentStorage]"},
     }
 
-    def __init__(self, *, value: List["_models.ConnectedEnvironmentStorage"], **kwargs):
+    def __init__(self, *, value: List["_models.ConnectedEnvironmentStorage"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of storage resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.ConnectedEnvironmentStorage]
         """
         super().__init__(**kwargs)
         self.value = value
 
@@ -1878,16 +1898,16 @@
         name: Optional[str] = None,
         command: Optional[List[str]] = None,
         args: Optional[List[str]] = None,
         env: Optional[List["_models.EnvironmentVar"]] = None,
         resources: Optional["_models.ContainerResources"] = None,
         volume_mounts: Optional[List["_models.VolumeMount"]] = None,
         probes: Optional[List["_models.ContainerAppProbe"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword image: Container image tag.
         :paramtype image: str
         :keyword name: Custom container name.
         :paramtype name: str
         :keyword command: Container start command.
         :paramtype command: list[str]
@@ -1938,24 +1958,29 @@
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
     :ivar extended_location: The complex type of the extended location.
     :vartype extended_location: ~azure.mgmt.appcontainers.models.ExtendedLocation
     :ivar identity: managed identities for the Container App to interact with other Azure services
      without maintaining any secrets or credentials in code.
     :vartype identity: ~azure.mgmt.appcontainers.models.ManagedServiceIdentity
+    :ivar managed_by: The fully qualified resource ID of the resource that manages this resource.
+     Indicates if this resource is managed by another Azure resource. If this is present, complete
+     mode deployment will not delete the resource if it is removed from the template since it is
+     managed by another resource.
+    :vartype managed_by: str
     :ivar provisioning_state: Provisioning state of the Container App. Known values are:
      "InProgress", "Succeeded", "Failed", "Canceled", and "Deleting".
     :vartype provisioning_state: str or
      ~azure.mgmt.appcontainers.models.ContainerAppProvisioningState
     :ivar managed_environment_id: Deprecated. Resource ID of the Container App's environment.
     :vartype managed_environment_id: str
     :ivar environment_id: Resource ID of environment.
     :vartype environment_id: str
-    :ivar workload_profile_type: Workload profile type to pin for container app execution.
-    :vartype workload_profile_type: str
+    :ivar workload_profile_name: Workload profile name to pin for container app execution.
+    :vartype workload_profile_name: str
     :ivar latest_revision_name: Name of the latest revision of the Container App.
     :vartype latest_revision_name: str
     :ivar latest_ready_revision_name: Name of the latest ready revision of the Container App.
     :vartype latest_ready_revision_name: str
     :ivar latest_revision_fqdn: Fully Qualified Domain Name of the latest revision of the Container
      App.
     :vartype latest_revision_fqdn: str
@@ -1991,18 +2016,19 @@
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "extended_location": {"key": "extendedLocation", "type": "ExtendedLocation"},
         "identity": {"key": "identity", "type": "ManagedServiceIdentity"},
+        "managed_by": {"key": "managedBy", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "managed_environment_id": {"key": "properties.managedEnvironmentId", "type": "str"},
         "environment_id": {"key": "properties.environmentId", "type": "str"},
-        "workload_profile_type": {"key": "properties.workloadProfileType", "type": "str"},
+        "workload_profile_name": {"key": "properties.workloadProfileName", "type": "str"},
         "latest_revision_name": {"key": "properties.latestRevisionName", "type": "str"},
         "latest_ready_revision_name": {"key": "properties.latestReadyRevisionName", "type": "str"},
         "latest_revision_fqdn": {"key": "properties.latestRevisionFqdn", "type": "str"},
         "custom_domain_verification_id": {"key": "properties.customDomainVerificationId", "type": "str"},
         "configuration": {"key": "properties.configuration", "type": "Configuration"},
         "template": {"key": "properties.template", "type": "Template"},
         "outbound_ip_addresses": {"key": "properties.outboundIpAddresses", "type": "[str]"},
@@ -2012,49 +2038,56 @@
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
         extended_location: Optional["_models.ExtendedLocation"] = None,
         identity: Optional["_models.ManagedServiceIdentity"] = None,
+        managed_by: Optional[str] = None,
         managed_environment_id: Optional[str] = None,
         environment_id: Optional[str] = None,
-        workload_profile_type: Optional[str] = None,
+        workload_profile_name: Optional[str] = None,
         configuration: Optional["_models.Configuration"] = None,
         template: Optional["_models.Template"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword extended_location: The complex type of the extended location.
         :paramtype extended_location: ~azure.mgmt.appcontainers.models.ExtendedLocation
         :keyword identity: managed identities for the Container App to interact with other Azure
          services without maintaining any secrets or credentials in code.
         :paramtype identity: ~azure.mgmt.appcontainers.models.ManagedServiceIdentity
+        :keyword managed_by: The fully qualified resource ID of the resource that manages this
+         resource. Indicates if this resource is managed by another Azure resource. If this is present,
+         complete mode deployment will not delete the resource if it is removed from the template since
+         it is managed by another resource.
+        :paramtype managed_by: str
         :keyword managed_environment_id: Deprecated. Resource ID of the Container App's environment.
         :paramtype managed_environment_id: str
         :keyword environment_id: Resource ID of environment.
         :paramtype environment_id: str
-        :keyword workload_profile_type: Workload profile type to pin for container app execution.
-        :paramtype workload_profile_type: str
+        :keyword workload_profile_name: Workload profile name to pin for container app execution.
+        :paramtype workload_profile_name: str
         :keyword configuration: Non versioned Container App configuration properties.
         :paramtype configuration: ~azure.mgmt.appcontainers.models.Configuration
         :keyword template: Container App versioned application definition.
         :paramtype template: ~azure.mgmt.appcontainers.models.Template
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.extended_location = extended_location
         self.identity = identity
+        self.managed_by = managed_by
         self.provisioning_state = None
         self.managed_environment_id = managed_environment_id
         self.environment_id = environment_id
-        self.workload_profile_type = workload_profile_type
+        self.workload_profile_name = workload_profile_name
         self.latest_revision_name = None
         self.latest_ready_revision_name = None
         self.latest_revision_fqdn = None
         self.custom_domain_verification_id = None
         self.configuration = configuration
         self.template = template
         self.outbound_ip_addresses = None
@@ -2106,15 +2139,15 @@
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "token": {"key": "properties.token", "type": "str"},
         "expires": {"key": "properties.expires", "type": "iso-8601"},
     }
 
-    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         """
         super().__init__(tags=tags, location=location, **kwargs)
@@ -2141,26 +2174,60 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[ContainerApp]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.ContainerApp"], **kwargs):
+    def __init__(self, *, value: List["_models.ContainerApp"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.ContainerApp]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
 
 
+class ContainerAppJobExecutions(_serialization.Model):
+    """Container App executions collection ARM resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar value: Collection of resources. Required.
+    :vartype value: list[~azure.mgmt.appcontainers.models.JobExecution]
+    :ivar next_link: Link to next page of resources.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "value": {"required": True},
+        "next_link": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[JobExecution]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(self, *, value: List["_models.JobExecution"], **kwargs: Any) -> None:
+        """
+        :keyword value: Collection of resources. Required.
+        :paramtype value: list[~azure.mgmt.appcontainers.models.JobExecution]
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = None
+
+
 class ContainerAppProbe(_serialization.Model):
-    """Probe describes a health check to be performed against a container to determine whether it is alive or ready to receive traffic.
+    """Probe describes a health check to be performed against a container to determine whether it is
+    alive or ready to receive traffic.
 
     :ivar failure_threshold: Minimum consecutive failures for the probe to be considered failed
      after having succeeded. Defaults to 3. Minimum value is 1. Maximum value is 10.
     :vartype failure_threshold: int
     :ivar http_get: HTTPGet specifies the http request to perform.
     :vartype http_get: ~azure.mgmt.appcontainers.models.ContainerAppProbeHttpGet
     :ivar initial_delay_seconds: Number of seconds after the container has started before liveness
@@ -2213,16 +2280,16 @@
         initial_delay_seconds: Optional[int] = None,
         period_seconds: Optional[int] = None,
         success_threshold: Optional[int] = None,
         tcp_socket: Optional["_models.ContainerAppProbeTcpSocket"] = None,
         termination_grace_period_seconds: Optional[int] = None,
         timeout_seconds: Optional[int] = None,
         type: Optional[Union[str, "_models.Type"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword failure_threshold: Minimum consecutive failures for the probe to be considered failed
          after having succeeded. Defaults to 3. Minimum value is 1. Maximum value is 10.
         :paramtype failure_threshold: int
         :keyword http_get: HTTPGet specifies the http request to perform.
         :paramtype http_get: ~azure.mgmt.appcontainers.models.ContainerAppProbeHttpGet
         :keyword initial_delay_seconds: Number of seconds after the container has started before
@@ -2303,16 +2370,16 @@
         self,
         *,
         port: int,
         host: Optional[str] = None,
         http_headers: Optional[List["_models.ContainerAppProbeHttpGetHttpHeadersItem"]] = None,
         path: Optional[str] = None,
         scheme: Optional[Union[str, "_models.Scheme"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword host: Host name to connect to, defaults to the pod IP. You probably want to set "Host"
          in httpHeaders instead.
         :paramtype host: str
         :keyword http_headers: Custom headers to set in the request. HTTP allows repeated headers.
         :paramtype http_headers:
          list[~azure.mgmt.appcontainers.models.ContainerAppProbeHttpGetHttpHeadersItem]
@@ -2350,15 +2417,15 @@
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "value": {"key": "value", "type": "str"},
     }
 
-    def __init__(self, *, name: str, value: str, **kwargs):
+    def __init__(self, *, name: str, value: str, **kwargs: Any) -> None:
         """
         :keyword name: The header field name. Required.
         :paramtype name: str
         :keyword value: The header field value. Required.
         :paramtype value: str
         """
         super().__init__(**kwargs)
@@ -2383,15 +2450,15 @@
     }
 
     _attribute_map = {
         "host": {"key": "host", "type": "str"},
         "port": {"key": "port", "type": "int"},
     }
 
-    def __init__(self, *, port: int, host: Optional[str] = None, **kwargs):
+    def __init__(self, *, port: int, host: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword host: Optional: Host name to connect to, defaults to the pod IP.
         :paramtype host: str
         :keyword port: Number or name of the port to access on the container. Number must be in the
          range 1 to 65535. Name must be an IANA_SVC_NAME. Required.
         :paramtype port: int
         """
@@ -2405,31 +2472,43 @@
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar name: Secret Name.
     :vartype name: str
     :ivar value: Secret Value.
     :vartype value: str
+    :ivar identity: Resource ID of a managed identity to authenticate with Azure Key Vault, or
+     System to use a system-assigned identity.
+    :vartype identity: str
+    :ivar key_vault_url: Azure Key Vault URL pointing to the secret referenced by the container
+     app.
+    :vartype key_vault_url: str
     """
 
     _validation = {
         "name": {"readonly": True},
         "value": {"readonly": True},
+        "identity": {"readonly": True},
+        "key_vault_url": {"readonly": True},
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "value": {"key": "value", "type": "str"},
+        "identity": {"key": "identity", "type": "str"},
+        "key_vault_url": {"key": "keyVaultUrl", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.name = None
         self.value = None
+        self.identity = None
+        self.key_vault_url = None
 
 
 class ContainerResources(_serialization.Model):
     """Container App container resource requirements.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -2447,15 +2526,15 @@
 
     _attribute_map = {
         "cpu": {"key": "cpu", "type": "float"},
         "memory": {"key": "memory", "type": "str"},
         "ephemeral_storage": {"key": "ephemeralStorage", "type": "str"},
     }
 
-    def __init__(self, *, cpu: Optional[float] = None, memory: Optional[str] = None, **kwargs):
+    def __init__(self, *, cpu: Optional[float] = None, memory: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword cpu: Required CPU in cores, e.g. 0.5.
         :paramtype cpu: float
         :keyword memory: Required memory, e.g. "250Mb".
         :paramtype memory: str
         """
         super().__init__(**kwargs)
@@ -2481,16 +2560,16 @@
     }
 
     def __init__(
         self,
         *,
         convention: Optional[Union[str, "_models.CookieExpirationConvention"]] = None,
         time_to_expiration: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword convention: The convention used when determining the session cookie's expiration.
          Known values are: "FixedTime" and "IdentityProviderDerived".
         :paramtype convention: str or ~azure.mgmt.appcontainers.models.CookieExpirationConvention
         :keyword time_to_expiration: The time after the request is made when the session cookie should
          expire.
         :paramtype time_to_expiration: str
@@ -2501,25 +2580,26 @@
 
 
 class CorsPolicy(_serialization.Model):
     """Cross-Origin-Resource-Sharing policy.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar allowed_origins: allowed origins. Required.
+    :ivar allowed_origins: Specifies the content for the access-control-allow-origins header.
+     Required.
     :vartype allowed_origins: list[str]
-    :ivar allowed_methods: allowed HTTP methods.
+    :ivar allowed_methods: Specifies the content for the access-control-allow-methods header.
     :vartype allowed_methods: list[str]
-    :ivar allowed_headers: allowed HTTP headers.
+    :ivar allowed_headers: Specifies the content for the access-control-allow-headers header.
     :vartype allowed_headers: list[str]
-    :ivar expose_headers: expose HTTP headers.
+    :ivar expose_headers: Specifies the content for the access-control-expose-headers header.
     :vartype expose_headers: list[str]
-    :ivar max_age: max time client can cache the result.
+    :ivar max_age: Specifies the content for the access-control-max-age header.
     :vartype max_age: int
-    :ivar allow_credentials: allow credential or not.
+    :ivar allow_credentials: Specifies whether the resource allows credentials.
     :vartype allow_credentials: bool
     """
 
     _validation = {
         "allowed_origins": {"required": True},
     }
 
@@ -2537,28 +2617,29 @@
         *,
         allowed_origins: List[str],
         allowed_methods: Optional[List[str]] = None,
         allowed_headers: Optional[List[str]] = None,
         expose_headers: Optional[List[str]] = None,
         max_age: Optional[int] = None,
         allow_credentials: Optional[bool] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword allowed_origins: allowed origins. Required.
+        :keyword allowed_origins: Specifies the content for the access-control-allow-origins header.
+         Required.
         :paramtype allowed_origins: list[str]
-        :keyword allowed_methods: allowed HTTP methods.
+        :keyword allowed_methods: Specifies the content for the access-control-allow-methods header.
         :paramtype allowed_methods: list[str]
-        :keyword allowed_headers: allowed HTTP headers.
+        :keyword allowed_headers: Specifies the content for the access-control-allow-headers header.
         :paramtype allowed_headers: list[str]
-        :keyword expose_headers: expose HTTP headers.
+        :keyword expose_headers: Specifies the content for the access-control-expose-headers header.
         :paramtype expose_headers: list[str]
-        :keyword max_age: max time client can cache the result.
+        :keyword max_age: Specifies the content for the access-control-max-age header.
         :paramtype max_age: int
-        :keyword allow_credentials: allow credential or not.
+        :keyword allow_credentials: Specifies whether the resource allows credentials.
         :paramtype allow_credentials: bool
         """
         super().__init__(**kwargs)
         self.allowed_origins = allowed_origins
         self.allowed_methods = allowed_methods
         self.allowed_headers = allowed_headers
         self.expose_headers = expose_headers
@@ -2572,45 +2653,44 @@
     All required parameters must be populated in order to send to Azure.
 
     :ivar name: Hostname. Required.
     :vartype name: str
     :ivar binding_type: Custom Domain binding type. Known values are: "Disabled" and "SniEnabled".
     :vartype binding_type: str or ~azure.mgmt.appcontainers.models.BindingType
     :ivar certificate_id: Resource Id of the Certificate to be bound to this hostname. Must exist
-     in the Managed Environment. Required.
+     in the Managed Environment.
     :vartype certificate_id: str
     """
 
     _validation = {
         "name": {"required": True},
-        "certificate_id": {"required": True},
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "binding_type": {"key": "bindingType", "type": "str"},
         "certificate_id": {"key": "certificateId", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         name: str,
-        certificate_id: str,
         binding_type: Optional[Union[str, "_models.BindingType"]] = None,
-        **kwargs
-    ):
+        certificate_id: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Hostname. Required.
         :paramtype name: str
         :keyword binding_type: Custom Domain binding type. Known values are: "Disabled" and
          "SniEnabled".
         :paramtype binding_type: str or ~azure.mgmt.appcontainers.models.BindingType
         :keyword certificate_id: Resource Id of the Certificate to be bound to this hostname. Must
-         exist in the Managed Environment. Required.
+         exist in the Managed Environment.
         :paramtype certificate_id: str
         """
         super().__init__(**kwargs)
         self.name = name
         self.binding_type = binding_type
         self.certificate_id = certificate_id
 
@@ -2655,16 +2735,16 @@
 
     def __init__(
         self,
         *,
         dns_suffix: Optional[str] = None,
         certificate_value: Optional[bytes] = None,
         certificate_password: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword dns_suffix: Dns suffix for the environment domain.
         :paramtype dns_suffix: str
         :keyword certificate_value: PFX or PEM blob.
         :paramtype certificate_value: bytes
         :keyword certificate_password: Certificate password.
         :paramtype certificate_password: str
@@ -2751,16 +2831,16 @@
         self,
         *,
         c_name_records: Optional[List[str]] = None,
         txt_records: Optional[List[str]] = None,
         a_records: Optional[List[str]] = None,
         alternate_c_name_records: Optional[List[str]] = None,
         alternate_txt_records: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword c_name_records: CName records visible for this hostname.
         :paramtype c_name_records: list[str]
         :keyword txt_records: TXT records visible for this hostname.
         :paramtype txt_records: list[str]
         :keyword a_records: A records visible for this hostname.
         :paramtype a_records: list[str]
@@ -2818,16 +2898,16 @@
 
     def __init__(
         self,
         *,
         details: Optional[
             List["_models.CustomHostnameAnalysisResultCustomDomainVerificationFailureInfoDetailsItem"]
         ] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword details: Details or the error.
         :paramtype details:
          list[~azure.mgmt.appcontainers.models.CustomHostnameAnalysisResultCustomDomainVerificationFailureInfoDetailsItem]
         """
         super().__init__(**kwargs)
         self.code = None
@@ -2857,15 +2937,15 @@
 
     _attribute_map = {
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
         self.target = None
 
 
@@ -2891,16 +2971,16 @@
 
     def __init__(
         self,
         *,
         enabled: Optional[bool] = None,
         registration: Optional["_models.OpenIdConnectRegistration"] = None,
         login: Optional["_models.OpenIdConnectLogin"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: :code:`<code>false</code>` if the custom Open ID provider provider should not
          be enabled; otherwise, :code:`<code>true</code>`.
         :paramtype enabled: bool
         :keyword registration: The configuration settings of the app registration for the custom Open
          ID Connect provider.
         :paramtype registration: ~azure.mgmt.appcontainers.models.OpenIdConnectRegistration
@@ -2934,16 +3014,16 @@
 
     def __init__(
         self,
         *,
         type: Optional[str] = None,
         metadata: Optional[Dict[str, str]] = None,
         auth: Optional[List["_models.ScaleRuleAuth"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword type: Type of the custom scale rule
          eg: azure-servicebus, redis etc.
         :paramtype type: str
         :keyword metadata: Metadata properties to describe custom scale rule.
         :paramtype metadata: dict[str, str]
         :keyword auth: Authentication secrets for the custom scale rule.
@@ -2998,16 +3078,16 @@
         app_id: Optional[str] = None,
         app_protocol: Union[str, "_models.AppProtocol"] = "http",
         app_port: Optional[int] = None,
         http_read_buffer_size: Optional[int] = None,
         http_max_request_size: Optional[int] = None,
         log_level: Optional[Union[str, "_models.LogLevel"]] = None,
         enable_api_logging: Optional[bool] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: Boolean indicating if the Dapr side car is enabled.
         :paramtype enabled: bool
         :keyword app_id: Dapr application identifier.
         :paramtype app_id: str
         :keyword app_protocol: Tells Dapr which protocol your application is using. Valid options are
          http and grpc. Default is http. Known values are: "http" and "grpc".
@@ -3100,16 +3180,16 @@
         version: Optional[str] = None,
         ignore_errors: bool = False,
         init_timeout: Optional[str] = None,
         secrets: Optional[List["_models.Secret"]] = None,
         secret_store_component: Optional[str] = None,
         metadata: Optional[List["_models.DaprMetadata"]] = None,
         scopes: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword component_type: Component type.
         :paramtype component_type: str
         :keyword version: Component version.
         :paramtype version: str
         :keyword ignore_errors: Boolean describing if the component errors are ignores.
         :paramtype ignore_errors: bool
@@ -3154,24 +3234,47 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[DaprComponent]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.DaprComponent"], **kwargs):
+    def __init__(self, *, value: List["_models.DaprComponent"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.DaprComponent]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
 
 
+class DaprConfiguration(_serialization.Model):
+    """Configuration properties Dapr component.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar version: The version of Dapr.
+    :vartype version: str
+    """
+
+    _validation = {
+        "version": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "version": {"key": "version", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.version = None
+
+
 class DaprMetadata(_serialization.Model):
     """Dapr component metadata.
 
     :ivar name: Metadata property name.
     :vartype name: str
     :ivar value: Metadata property value.
     :vartype value: str
@@ -3183,16 +3286,21 @@
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "value": {"key": "value", "type": "str"},
         "secret_ref": {"key": "secretRef", "type": "str"},
     }
 
     def __init__(
-        self, *, name: Optional[str] = None, value: Optional[str] = None, secret_ref: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        name: Optional[str] = None,
+        value: Optional[str] = None,
+        secret_ref: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Metadata property name.
         :paramtype name: str
         :keyword value: Metadata property value.
         :paramtype value: str
         :keyword secret_ref: Name of the Dapr Component secret from which to pull the metadata property
          value.
@@ -3221,15 +3329,15 @@
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "value": {"key": "value", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.name = None
         self.value = None
 
 
 class DaprSecretsCollection(_serialization.Model):
@@ -3245,15 +3353,15 @@
         "value": {"required": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[DaprSecret]"},
     }
 
-    def __init__(self, *, value: List["_models.DaprSecret"], **kwargs):
+    def __init__(self, *, value: List["_models.DaprSecret"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of secrets used by a Dapr component. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.DaprSecret]
         """
         super().__init__(**kwargs)
         self.value = value
 
@@ -3275,16 +3383,16 @@
     }
 
     def __init__(
         self,
         *,
         allowed_principals: Optional["_models.AllowedPrincipals"] = None,
         allowed_applications: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword allowed_principals: The configuration settings of the Azure Active Directory allowed
          principals.
         :paramtype allowed_principals: ~azure.mgmt.appcontainers.models.AllowedPrincipals
         :keyword allowed_applications: The configuration settings of the Azure Active Directory allowed
          applications.
         :paramtype allowed_applications: list[str]
@@ -3307,15 +3415,15 @@
         "error": {"readonly": True},
     }
 
     _attribute_map = {
         "error": {"key": "error", "type": "DefaultErrorResponseError"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.error = None
 
 
 class DefaultErrorResponseError(_serialization.Model):
     """Error model.
@@ -3345,15 +3453,17 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "details": {"key": "details", "type": "[DefaultErrorResponseErrorDetailsItem]"},
         "innererror": {"key": "innererror", "type": "str"},
     }
 
-    def __init__(self, *, details: Optional[List["_models.DefaultErrorResponseErrorDetailsItem"]] = None, **kwargs):
+    def __init__(
+        self, *, details: Optional[List["_models.DefaultErrorResponseErrorDetailsItem"]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword details: Details or the error.
         :paramtype details: list[~azure.mgmt.appcontainers.models.DefaultErrorResponseErrorDetailsItem]
         """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
@@ -3383,15 +3493,15 @@
 
     _attribute_map = {
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
         self.target = None
 
 
@@ -3411,16 +3521,16 @@
     }
 
     def __init__(
         self,
         *,
         provider_name: Optional[str] = None,
         property_bag: Optional[List["_models.DiagnosticDataProviderMetadataPropertyBagItem"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword provider_name: Name of data provider.
         :paramtype provider_name: str
         :keyword property_bag: Collection of properties.
         :paramtype property_bag:
          list[~azure.mgmt.appcontainers.models.DiagnosticDataProviderMetadataPropertyBagItem]
         """
@@ -3439,15 +3549,15 @@
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "value": {"key": "value", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, value: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, value: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: Property name.
         :paramtype name: str
         :keyword value: Property value.
         :paramtype value: str
         """
         super().__init__(**kwargs)
@@ -3474,16 +3584,16 @@
 
     def __init__(
         self,
         *,
         column_name: Optional[str] = None,
         data_type: Optional[str] = None,
         column_type: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword column_name: Column name.
         :paramtype column_name: str
         :keyword data_type: Data type of the column.
         :paramtype data_type: str
         :keyword column_type: Column type.
         :paramtype column_type: str
@@ -3513,16 +3623,16 @@
 
     def __init__(
         self,
         *,
         table_name: Optional[str] = None,
         columns: Optional[List["_models.DiagnosticDataTableResponseColumn"]] = None,
         rows: Optional[List[JSON]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword table_name: Table name.
         :paramtype table_name: str
         :keyword columns: Columns in the table.
         :paramtype columns: list[~azure.mgmt.appcontainers.models.DiagnosticDataTableResponseColumn]
         :keyword rows: Rows in the table.
         :paramtype rows: list[JSON]
@@ -3556,16 +3666,16 @@
     def __init__(
         self,
         *,
         type: Optional[int] = None,
         title: Optional[str] = None,
         description: Optional[str] = None,
         is_visible: Optional[bool] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword type: Rendering type.
         :paramtype type: int
         :keyword title: Title of the table.
         :paramtype title: str
         :keyword description: Description of the table.
         :paramtype description: str
@@ -3610,15 +3720,15 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "DiagnosticsProperties"},
     }
 
-    def __init__(self, *, properties: Optional["_models.DiagnosticsProperties"] = None, **kwargs):
+    def __init__(self, *, properties: Optional["_models.DiagnosticsProperties"] = None, **kwargs: Any) -> None:
         """
         :keyword properties: Diagnostics resource specific properties.
         :paramtype properties: ~azure.mgmt.appcontainers.models.DiagnosticsProperties
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -3642,15 +3752,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Diagnostics]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.Diagnostics"], **kwargs):
+    def __init__(self, *, value: List["_models.Diagnostics"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of diagnostic data. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.Diagnostics]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -3671,16 +3781,16 @@
     }
 
     def __init__(
         self,
         *,
         table: Optional["_models.DiagnosticDataTableResponseObject"] = None,
         rendering_properties: Optional["_models.DiagnosticRendering"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword table: Table response.
         :paramtype table: ~azure.mgmt.appcontainers.models.DiagnosticDataTableResponseObject
         :keyword rendering_properties: Details of the table response.
         :paramtype rendering_properties: ~azure.mgmt.appcontainers.models.DiagnosticRendering
         """
         super().__init__(**kwargs)
@@ -3736,16 +3846,16 @@
     }
 
     def __init__(
         self,
         *,
         support_topic_list: Optional[List["_models.DiagnosticSupportTopic"]] = None,
         analysis_types: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword support_topic_list: List of support topics.
         :paramtype support_topic_list: list[~azure.mgmt.appcontainers.models.DiagnosticSupportTopic]
         :keyword analysis_types: List of analysis types.
         :paramtype analysis_types: list[str]
         """
         super().__init__(**kwargs)
@@ -3784,16 +3894,16 @@
     def __init__(
         self,
         *,
         metadata: Optional["_models.DiagnosticsDefinition"] = None,
         dataset: Optional[List["_models.DiagnosticsDataApiResponse"]] = None,
         status: Optional["_models.DiagnosticsStatus"] = None,
         data_provider_metadata: Optional["_models.DiagnosticDataProviderMetadata"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword metadata: Metadata of the diagnostics response.
         :paramtype metadata: ~azure.mgmt.appcontainers.models.DiagnosticsDefinition
         :keyword dataset: Set of data collections associated with the response.
         :paramtype dataset: list[~azure.mgmt.appcontainers.models.DiagnosticsDataApiResponse]
         :keyword status: Status of the diagnostics response.
         :paramtype status: ~azure.mgmt.appcontainers.models.DiagnosticsStatus
@@ -3818,15 +3928,15 @@
     """
 
     _attribute_map = {
         "message": {"key": "message", "type": "str"},
         "status_id": {"key": "statusId", "type": "int"},
     }
 
-    def __init__(self, *, message: Optional[str] = None, status_id: Optional[int] = None, **kwargs):
+    def __init__(self, *, message: Optional[str] = None, status_id: Optional[int] = None, **kwargs: Any) -> None:
         """
         :keyword message: Diagnostic message.
         :paramtype message: str
         :keyword status_id: Status.
         :paramtype status_id: int
         """
         super().__init__(**kwargs)
@@ -3851,15 +3961,15 @@
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "pes_id": {"key": "pesId", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.id = None
         self.pes_id = None
 
 
 class EnvironmentAuthToken(TrackedResource):
@@ -3907,52 +4017,26 @@
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "token": {"key": "properties.token", "type": "str"},
         "expires": {"key": "properties.expires", "type": "iso-8601"},
     }
 
-    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.token = None
         self.expires = None
 
 
-class EnvironmentSkuProperties(_serialization.Model):
-    """Managed Environment resource SKU properties.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar name: Name of the Sku. Required. Known values are: "Consumption" and "Premium".
-    :vartype name: str or ~azure.mgmt.appcontainers.models.SkuName
-    """
-
-    _validation = {
-        "name": {"required": True},
-    }
-
-    _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-    }
-
-    def __init__(self, *, name: Union[str, "_models.SkuName"], **kwargs):
-        """
-        :keyword name: Name of the Sku. Required. Known values are: "Consumption" and "Premium".
-        :paramtype name: str or ~azure.mgmt.appcontainers.models.SkuName
-        """
-        super().__init__(**kwargs)
-        self.name = name
-
-
 class EnvironmentVar(_serialization.Model):
     """Container App container environment variable.
 
     :ivar name: Environment variable name.
     :vartype name: str
     :ivar value: Non-secret environment variable value.
     :vartype value: str
@@ -3964,16 +4048,21 @@
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "value": {"key": "value", "type": "str"},
         "secret_ref": {"key": "secretRef", "type": "str"},
     }
 
     def __init__(
-        self, *, name: Optional[str] = None, value: Optional[str] = None, secret_ref: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        name: Optional[str] = None,
+        value: Optional[str] = None,
+        secret_ref: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Environment variable name.
         :paramtype name: str
         :keyword value: Non-secret environment variable value.
         :paramtype value: str
         :keyword secret_ref: Name of the Container App secret from which to pull the environment
          variable value.
@@ -4002,15 +4091,15 @@
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "info": {"key": "info", "type": "object"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.type = None
         self.info = None
 
 
 class ErrorDetail(_serialization.Model):
@@ -4042,36 +4131,37 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "details": {"key": "details", "type": "[ErrorDetail]"},
         "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
         self.target = None
         self.details = None
         self.additional_info = None
 
 
 class ErrorResponse(_serialization.Model):
-    """Common error response for all Azure Resource Manager APIs to return error details for failed operations. (This also follows the OData error response format.).
+    """Common error response for all Azure Resource Manager APIs to return error details for failed
+    operations. (This also follows the OData error response format.).
 
     :ivar error: The error object.
     :vartype error: ~azure.mgmt.appcontainers.models.ErrorDetail
     """
 
     _attribute_map = {
         "error": {"key": "error", "type": "ErrorDetail"},
     }
 
-    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs):
+    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs: Any) -> None:
         """
         :keyword error: The error object.
         :paramtype error: ~azure.mgmt.appcontainers.models.ErrorDetail
         """
         super().__init__(**kwargs)
         self.error = error
 
@@ -4091,16 +4181,16 @@
     }
 
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         type: Optional[Union[str, "_models.ExtendedLocationTypes"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The name of the extended location.
         :paramtype name: str
         :keyword type: The type of the extended location. "CustomLocation"
         :paramtype type: str or ~azure.mgmt.appcontainers.models.ExtendedLocationTypes
         """
         super().__init__(**kwargs)
@@ -4133,16 +4223,16 @@
     def __init__(
         self,
         *,
         enabled: Optional[bool] = None,
         registration: Optional["_models.AppRegistration"] = None,
         graph_api_version: Optional[str] = None,
         login: Optional["_models.LoginScopes"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: :code:`<code>false</code>` if the Facebook provider should not be enabled
          despite the set registration; otherwise, :code:`<code>true</code>`.
         :paramtype enabled: bool
         :keyword registration: The configuration settings of the app registration for the Facebook
          provider.
         :paramtype registration: ~azure.mgmt.appcontainers.models.AppRegistration
@@ -4178,16 +4268,16 @@
 
     def __init__(
         self,
         *,
         convention: Optional[Union[str, "_models.ForwardProxyConvention"]] = None,
         custom_host_header_name: Optional[str] = None,
         custom_proto_header_name: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword convention: The convention used to determine the url of the request made. Known values
          are: "NoProxy", "Standard", and "Custom".
         :paramtype convention: str or ~azure.mgmt.appcontainers.models.ForwardProxyConvention
         :keyword custom_host_header_name: The name of the header containing the host of the request.
         :paramtype custom_host_header_name: str
         :keyword custom_proto_header_name: The name of the header containing the scheme of the request.
@@ -4219,16 +4309,16 @@
 
     def __init__(
         self,
         *,
         enabled: Optional[bool] = None,
         registration: Optional["_models.ClientRegistration"] = None,
         login: Optional["_models.LoginScopes"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: :code:`<code>false</code>` if the GitHub provider should not be enabled
          despite the set registration; otherwise, :code:`<code>true</code>`.
         :paramtype enabled: bool
         :keyword registration: The configuration settings of the app registration for the GitHub
          provider.
         :paramtype registration: ~azure.mgmt.appcontainers.models.ClientRegistration
@@ -4280,16 +4370,16 @@
         azure_credentials: Optional["_models.AzureCredentials"] = None,
         context_path: Optional[str] = None,
         image: Optional[str] = None,
         publish_type: Optional[str] = None,
         os: Optional[str] = None,
         runtime_stack: Optional[str] = None,
         runtime_version: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword registry_info: Registry configurations.
         :paramtype registry_info: ~azure.mgmt.appcontainers.models.RegistryInfo
         :keyword azure_credentials: AzureCredentials configurations.
         :paramtype azure_credentials: ~azure.mgmt.appcontainers.models.AzureCredentials
         :keyword context_path: Context path.
         :paramtype context_path: str
@@ -4312,15 +4402,16 @@
         self.publish_type = publish_type
         self.os = os
         self.runtime_stack = runtime_stack
         self.runtime_version = runtime_version
 
 
 class GlobalValidation(_serialization.Model):
-    """The configuration settings that determines the validation flow of users using ContainerApp Service Authentication/Authorization.
+    """The configuration settings that determines the validation flow of users using ContainerApp
+    Service Authentication/Authorization.
 
     :ivar unauthenticated_client_action: The action to take when an unauthenticated client attempts
      to access the app. Known values are: "RedirectToLoginPage", "AllowAnonymous", "Return401", and
      "Return403".
     :vartype unauthenticated_client_action: str or
      ~azure.mgmt.appcontainers.models.UnauthenticatedClientActionV2
     :ivar redirect_to_provider: The default authentication provider to use when multiple providers
@@ -4342,16 +4433,16 @@
 
     def __init__(
         self,
         *,
         unauthenticated_client_action: Optional[Union[str, "_models.UnauthenticatedClientActionV2"]] = None,
         redirect_to_provider: Optional[str] = None,
         excluded_paths: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword unauthenticated_client_action: The action to take when an unauthenticated client
          attempts to access the app. Known values are: "RedirectToLoginPage", "AllowAnonymous",
          "Return401", and "Return403".
         :paramtype unauthenticated_client_action: str or
          ~azure.mgmt.appcontainers.models.UnauthenticatedClientActionV2
         :keyword redirect_to_provider: The default authentication provider to use when multiple
@@ -4395,16 +4486,16 @@
     def __init__(
         self,
         *,
         enabled: Optional[bool] = None,
         registration: Optional["_models.ClientRegistration"] = None,
         login: Optional["_models.LoginScopes"] = None,
         validation: Optional["_models.AllowedAudiencesValidation"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: :code:`<code>false</code>` if the Google provider should not be enabled
          despite the set registration; otherwise, :code:`<code>true</code>`.
         :paramtype enabled: bool
         :keyword registration: The configuration settings of the app registration for the Google
          provider.
         :paramtype registration: ~azure.mgmt.appcontainers.models.ClientRegistration
@@ -4436,29 +4527,30 @@
     }
 
     def __init__(
         self,
         *,
         metadata: Optional[Dict[str, str]] = None,
         auth: Optional[List["_models.ScaleRuleAuth"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword metadata: Metadata properties to describe http scale rule.
         :paramtype metadata: dict[str, str]
         :keyword auth: Authentication secrets for the custom scale rule.
         :paramtype auth: list[~azure.mgmt.appcontainers.models.ScaleRuleAuth]
         """
         super().__init__(**kwargs)
         self.metadata = metadata
         self.auth = auth
 
 
 class HttpSettings(_serialization.Model):
-    """The configuration settings of the HTTP requests for authentication and authorization requests made against ContainerApp Service Authentication/Authorization.
+    """The configuration settings of the HTTP requests for authentication and authorization requests
+    made against ContainerApp Service Authentication/Authorization.
 
     :ivar require_https: :code:`<code>false</code>` if the authentication/authorization responses
      not having the HTTPS scheme are permissible; otherwise, :code:`<code>true</code>`.
     :vartype require_https: bool
     :ivar routes: The configuration settings of the paths HTTP requests.
     :vartype routes: ~azure.mgmt.appcontainers.models.HttpSettingsRoutes
     :ivar forward_proxy: The configuration settings of a forward proxy used to make the requests.
@@ -4473,16 +4565,16 @@
 
     def __init__(
         self,
         *,
         require_https: Optional[bool] = None,
         routes: Optional["_models.HttpSettingsRoutes"] = None,
         forward_proxy: Optional["_models.ForwardProxy"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword require_https: :code:`<code>false</code>` if the authentication/authorization
          responses not having the HTTPS scheme are permissible; otherwise, :code:`<code>true</code>`.
         :paramtype require_https: bool
         :keyword routes: The configuration settings of the paths HTTP requests.
         :paramtype routes: ~azure.mgmt.appcontainers.models.HttpSettingsRoutes
         :keyword forward_proxy: The configuration settings of a forward proxy used to make the
@@ -4502,25 +4594,26 @@
     :vartype api_prefix: str
     """
 
     _attribute_map = {
         "api_prefix": {"key": "apiPrefix", "type": "str"},
     }
 
-    def __init__(self, *, api_prefix: Optional[str] = None, **kwargs):
+    def __init__(self, *, api_prefix: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword api_prefix: The prefix that should precede all the authentication/authorization paths.
         :paramtype api_prefix: str
         """
         super().__init__(**kwargs)
         self.api_prefix = api_prefix
 
 
 class IdentityProviders(_serialization.Model):
-    """The configuration settings of each of the identity providers used to configure ContainerApp Service Authentication/Authorization.
+    """The configuration settings of each of the identity providers used to configure ContainerApp
+    Service Authentication/Authorization.
 
     :ivar azure_active_directory: The configuration settings of the Azure Active directory
      provider.
     :vartype azure_active_directory: ~azure.mgmt.appcontainers.models.AzureActiveDirectory
     :ivar facebook: The configuration settings of the Facebook provider.
     :vartype facebook: ~azure.mgmt.appcontainers.models.Facebook
     :ivar git_hub: The configuration settings of the GitHub provider.
@@ -4561,16 +4654,16 @@
         facebook: Optional["_models.Facebook"] = None,
         git_hub: Optional["_models.GitHub"] = None,
         google: Optional["_models.Google"] = None,
         twitter: Optional["_models.Twitter"] = None,
         apple: Optional["_models.Apple"] = None,
         azure_static_web_apps: Optional["_models.AzureStaticWebApps"] = None,
         custom_open_id_connect_providers: Optional[Dict[str, "_models.CustomOpenIdConnectProvider"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword azure_active_directory: The configuration settings of the Azure Active directory
          provider.
         :paramtype azure_active_directory: ~azure.mgmt.appcontainers.models.AzureActiveDirectory
         :keyword facebook: The configuration settings of the Facebook provider.
         :paramtype facebook: ~azure.mgmt.appcontainers.models.Facebook
         :keyword git_hub: The configuration settings of the GitHub provider.
@@ -4623,14 +4716,16 @@
     :vartype custom_domains: list[~azure.mgmt.appcontainers.models.CustomDomain]
     :ivar allow_insecure: Bool indicating if HTTP connections to is allowed. If set to false HTTP
      connections are automatically redirected to HTTPS connections.
     :vartype allow_insecure: bool
     :ivar ip_security_restrictions: Rules to restrict incoming IP address.
     :vartype ip_security_restrictions:
      list[~azure.mgmt.appcontainers.models.IpSecurityRestrictionRule]
+    :ivar sticky_sessions: Sticky Sessions for Single Revision Mode.
+    :vartype sticky_sessions: ~azure.mgmt.appcontainers.models.IngressStickySessions
     :ivar client_certificate_mode: Client certificate mode for mTLS authentication. Ignore
      indicates server drops client certificate on forwarding. Accept indicates server forwards
      client certificate but does not require a client certificate. Require indicates server requires
      a client certificate. Known values are: "ignore", "accept", and "require".
     :vartype client_certificate_mode: str or
      ~azure.mgmt.appcontainers.models.IngressClientCertificateMode
     :ivar cors_policy: CORS policy for container app.
@@ -4647,14 +4742,15 @@
         "target_port": {"key": "targetPort", "type": "int"},
         "exposed_port": {"key": "exposedPort", "type": "int"},
         "transport": {"key": "transport", "type": "str"},
         "traffic": {"key": "traffic", "type": "[TrafficWeight]"},
         "custom_domains": {"key": "customDomains", "type": "[CustomDomain]"},
         "allow_insecure": {"key": "allowInsecure", "type": "bool"},
         "ip_security_restrictions": {"key": "ipSecurityRestrictions", "type": "[IpSecurityRestrictionRule]"},
+        "sticky_sessions": {"key": "stickySessions", "type": "IngressStickySessions"},
         "client_certificate_mode": {"key": "clientCertificateMode", "type": "str"},
         "cors_policy": {"key": "corsPolicy", "type": "CorsPolicy"},
     }
 
     def __init__(
         self,
         *,
@@ -4662,18 +4758,19 @@
         target_port: Optional[int] = None,
         exposed_port: Optional[int] = None,
         transport: Union[str, "_models.IngressTransportMethod"] = "auto",
         traffic: Optional[List["_models.TrafficWeight"]] = None,
         custom_domains: Optional[List["_models.CustomDomain"]] = None,
         allow_insecure: bool = False,
         ip_security_restrictions: Optional[List["_models.IpSecurityRestrictionRule"]] = None,
+        sticky_sessions: Optional["_models.IngressStickySessions"] = None,
         client_certificate_mode: Optional[Union[str, "_models.IngressClientCertificateMode"]] = None,
         cors_policy: Optional["_models.CorsPolicy"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword external: Bool indicating if app exposes an external http endpoint.
         :paramtype external: bool
         :keyword target_port: Target Port in containers for traffic from ingress.
         :paramtype target_port: int
         :keyword exposed_port: Exposed Port in containers for TCP traffic from ingress.
         :paramtype exposed_port: int
@@ -4686,14 +4783,16 @@
         :paramtype custom_domains: list[~azure.mgmt.appcontainers.models.CustomDomain]
         :keyword allow_insecure: Bool indicating if HTTP connections to is allowed. If set to false
          HTTP connections are automatically redirected to HTTPS connections.
         :paramtype allow_insecure: bool
         :keyword ip_security_restrictions: Rules to restrict incoming IP address.
         :paramtype ip_security_restrictions:
          list[~azure.mgmt.appcontainers.models.IpSecurityRestrictionRule]
+        :keyword sticky_sessions: Sticky Sessions for Single Revision Mode.
+        :paramtype sticky_sessions: ~azure.mgmt.appcontainers.models.IngressStickySessions
         :keyword client_certificate_mode: Client certificate mode for mTLS authentication. Ignore
          indicates server drops client certificate on forwarding. Accept indicates server forwards
          client certificate but does not require a client certificate. Require indicates server requires
          a client certificate. Known values are: "ignore", "accept", and "require".
         :paramtype client_certificate_mode: str or
          ~azure.mgmt.appcontainers.models.IngressClientCertificateMode
         :keyword cors_policy: CORS policy for container app.
@@ -4705,18 +4804,39 @@
         self.target_port = target_port
         self.exposed_port = exposed_port
         self.transport = transport
         self.traffic = traffic
         self.custom_domains = custom_domains
         self.allow_insecure = allow_insecure
         self.ip_security_restrictions = ip_security_restrictions
+        self.sticky_sessions = sticky_sessions
         self.client_certificate_mode = client_certificate_mode
         self.cors_policy = cors_policy
 
 
+class IngressStickySessions(_serialization.Model):
+    """Sticky Sessions for Single Revision Mode.
+
+    :ivar affinity: Sticky Session Affinity. Known values are: "sticky" and "none".
+    :vartype affinity: str or ~azure.mgmt.appcontainers.models.Affinity
+    """
+
+    _attribute_map = {
+        "affinity": {"key": "affinity", "type": "str"},
+    }
+
+    def __init__(self, *, affinity: Optional[Union[str, "_models.Affinity"]] = None, **kwargs: Any) -> None:
+        """
+        :keyword affinity: Sticky Session Affinity. Known values are: "sticky" and "none".
+        :paramtype affinity: str or ~azure.mgmt.appcontainers.models.Affinity
+        """
+        super().__init__(**kwargs)
+        self.affinity = affinity
+
+
 class InitContainer(BaseContainer):
     """Container App init container definition.
 
     :ivar image: Container image tag.
     :vartype image: str
     :ivar name: Custom container name.
     :vartype name: str
@@ -4748,16 +4868,16 @@
         image: Optional[str] = None,
         name: Optional[str] = None,
         command: Optional[List[str]] = None,
         args: Optional[List[str]] = None,
         env: Optional[List["_models.EnvironmentVar"]] = None,
         resources: Optional["_models.ContainerResources"] = None,
         volume_mounts: Optional[List["_models.VolumeMount"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword image: Container image tag.
         :paramtype image: str
         :keyword name: Custom container name.
         :paramtype name: str
         :keyword command: Container start command.
         :paramtype command: list[str]
@@ -4815,16 +4935,16 @@
     def __init__(
         self,
         *,
         name: str,
         ip_address_range: str,
         action: Union[str, "_models.Action"],
         description: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Name for the IP restriction rule. Required.
         :paramtype name: str
         :keyword description: Describe the IP restriction rule that is being sent to the container-app.
          This is an optional field.
         :paramtype description: str
         :keyword ip_address_range: CIDR notation to match incoming IP address. Required.
@@ -4836,14 +4956,705 @@
         super().__init__(**kwargs)
         self.name = name
         self.description = description
         self.ip_address_range = ip_address_range
         self.action = action
 
 
+class Job(TrackedResource):  # pylint: disable=too-many-instance-attributes
+    """Container App Job.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.appcontainers.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    :ivar identity: Managed identities needed by a container app job to interact with other Azure
+     services to not maintain any secrets or credentials in code.
+    :vartype identity: ~azure.mgmt.appcontainers.models.ManagedServiceIdentity
+    :ivar provisioning_state: Provisioning state of the Container Apps Job. Known values are:
+     "InProgress", "Succeeded", "Failed", "Canceled", and "Deleting".
+    :vartype provisioning_state: str or ~azure.mgmt.appcontainers.models.JobProvisioningState
+    :ivar environment_id: Resource ID of environment.
+    :vartype environment_id: str
+    :ivar workload_profile_name: Workload profile name to pin for container apps job execution.
+    :vartype workload_profile_name: str
+    :ivar configuration: Container Apps Job configuration properties.
+    :vartype configuration: ~azure.mgmt.appcontainers.models.JobConfiguration
+    :ivar template: Container Apps job definition.
+    :vartype template: ~azure.mgmt.appcontainers.models.JobTemplate
+    :ivar outbound_ip_addresses: Outbound IP Addresses of a container apps job.
+    :vartype outbound_ip_addresses: list[str]
+    :ivar event_stream_endpoint: The endpoint of the eventstream of the container apps job.
+    :vartype event_stream_endpoint: str
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+        "provisioning_state": {"readonly": True},
+        "outbound_ip_addresses": {"readonly": True},
+        "event_stream_endpoint": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+        "identity": {"key": "identity", "type": "ManagedServiceIdentity"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "environment_id": {"key": "properties.environmentId", "type": "str"},
+        "workload_profile_name": {"key": "properties.workloadProfileName", "type": "str"},
+        "configuration": {"key": "properties.configuration", "type": "JobConfiguration"},
+        "template": {"key": "properties.template", "type": "JobTemplate"},
+        "outbound_ip_addresses": {"key": "properties.outboundIpAddresses", "type": "[str]"},
+        "event_stream_endpoint": {"key": "properties.eventStreamEndpoint", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location: str,
+        tags: Optional[Dict[str, str]] = None,
+        identity: Optional["_models.ManagedServiceIdentity"] = None,
+        environment_id: Optional[str] = None,
+        workload_profile_name: Optional[str] = None,
+        configuration: Optional["_models.JobConfiguration"] = None,
+        template: Optional["_models.JobTemplate"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        :keyword identity: Managed identities needed by a container app job to interact with other
+         Azure services to not maintain any secrets or credentials in code.
+        :paramtype identity: ~azure.mgmt.appcontainers.models.ManagedServiceIdentity
+        :keyword environment_id: Resource ID of environment.
+        :paramtype environment_id: str
+        :keyword workload_profile_name: Workload profile name to pin for container apps job execution.
+        :paramtype workload_profile_name: str
+        :keyword configuration: Container Apps Job configuration properties.
+        :paramtype configuration: ~azure.mgmt.appcontainers.models.JobConfiguration
+        :keyword template: Container Apps job definition.
+        :paramtype template: ~azure.mgmt.appcontainers.models.JobTemplate
+        """
+        super().__init__(tags=tags, location=location, **kwargs)
+        self.identity = identity
+        self.provisioning_state = None
+        self.environment_id = environment_id
+        self.workload_profile_name = workload_profile_name
+        self.configuration = configuration
+        self.template = template
+        self.outbound_ip_addresses = None
+        self.event_stream_endpoint = None
+
+
+class JobConfiguration(_serialization.Model):
+    """Non versioned Container Apps Job configuration properties.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar secrets: Collection of secrets used by a Container Apps Job.
+    :vartype secrets: list[~azure.mgmt.appcontainers.models.Secret]
+    :ivar trigger_type: Trigger type of the job. Known values are: "Scheduled", "Event", and
+     "Manual".
+    :vartype trigger_type: str or ~azure.mgmt.appcontainers.models.TriggerType
+    :ivar replica_timeout: Maximum number of seconds a replica is allowed to run. Required.
+    :vartype replica_timeout: int
+    :ivar replica_retry_limit: Maximum number of retries before failing the job.
+    :vartype replica_retry_limit: int
+    :ivar manual_trigger_config: Manual trigger configuration for a single execution job.
+     Properties replicaCompletionCount and parallelism would be set to 1 by default.
+    :vartype manual_trigger_config:
+     ~azure.mgmt.appcontainers.models.JobConfigurationManualTriggerConfig
+    :ivar schedule_trigger_config: Cron formatted repeating trigger schedule ("\ * * * * *") for
+     cronjobs. Properties completions and parallelism would be set to 1 by default.
+    :vartype schedule_trigger_config:
+     ~azure.mgmt.appcontainers.models.JobConfigurationScheduleTriggerConfig
+    :ivar registries: Collection of private container registry credentials used by a Container apps
+     job.
+    :vartype registries: list[~azure.mgmt.appcontainers.models.RegistryCredentials]
+    """
+
+    _validation = {
+        "trigger_type": {"required": True},
+        "replica_timeout": {"required": True},
+    }
+
+    _attribute_map = {
+        "secrets": {"key": "secrets", "type": "[Secret]"},
+        "trigger_type": {"key": "triggerType", "type": "str"},
+        "replica_timeout": {"key": "replicaTimeout", "type": "int"},
+        "replica_retry_limit": {"key": "replicaRetryLimit", "type": "int"},
+        "manual_trigger_config": {"key": "manualTriggerConfig", "type": "JobConfigurationManualTriggerConfig"},
+        "schedule_trigger_config": {"key": "scheduleTriggerConfig", "type": "JobConfigurationScheduleTriggerConfig"},
+        "registries": {"key": "registries", "type": "[RegistryCredentials]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        trigger_type: Union[str, "_models.TriggerType"] = "Manual",
+        replica_timeout: int,
+        secrets: Optional[List["_models.Secret"]] = None,
+        replica_retry_limit: Optional[int] = None,
+        manual_trigger_config: Optional["_models.JobConfigurationManualTriggerConfig"] = None,
+        schedule_trigger_config: Optional["_models.JobConfigurationScheduleTriggerConfig"] = None,
+        registries: Optional[List["_models.RegistryCredentials"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword secrets: Collection of secrets used by a Container Apps Job.
+        :paramtype secrets: list[~azure.mgmt.appcontainers.models.Secret]
+        :keyword trigger_type: Trigger type of the job. Known values are: "Scheduled", "Event", and
+         "Manual".
+        :paramtype trigger_type: str or ~azure.mgmt.appcontainers.models.TriggerType
+        :keyword replica_timeout: Maximum number of seconds a replica is allowed to run. Required.
+        :paramtype replica_timeout: int
+        :keyword replica_retry_limit: Maximum number of retries before failing the job.
+        :paramtype replica_retry_limit: int
+        :keyword manual_trigger_config: Manual trigger configuration for a single execution job.
+         Properties replicaCompletionCount and parallelism would be set to 1 by default.
+        :paramtype manual_trigger_config:
+         ~azure.mgmt.appcontainers.models.JobConfigurationManualTriggerConfig
+        :keyword schedule_trigger_config: Cron formatted repeating trigger schedule ("\ * * * * *") for
+         cronjobs. Properties completions and parallelism would be set to 1 by default.
+        :paramtype schedule_trigger_config:
+         ~azure.mgmt.appcontainers.models.JobConfigurationScheduleTriggerConfig
+        :keyword registries: Collection of private container registry credentials used by a Container
+         apps job.
+        :paramtype registries: list[~azure.mgmt.appcontainers.models.RegistryCredentials]
+        """
+        super().__init__(**kwargs)
+        self.secrets = secrets
+        self.trigger_type = trigger_type
+        self.replica_timeout = replica_timeout
+        self.replica_retry_limit = replica_retry_limit
+        self.manual_trigger_config = manual_trigger_config
+        self.schedule_trigger_config = schedule_trigger_config
+        self.registries = registries
+
+
+class JobConfigurationManualTriggerConfig(_serialization.Model):
+    """Manual trigger configuration for a single execution job. Properties replicaCompletionCount and
+    parallelism would be set to 1 by default.
+
+    :ivar replica_completion_count: Minimum number of successful replica completions before overall
+     job completion.
+    :vartype replica_completion_count: int
+    :ivar parallelism: Number of parallel replicas of a job that can run at a given time.
+    :vartype parallelism: int
+    """
+
+    _attribute_map = {
+        "replica_completion_count": {"key": "replicaCompletionCount", "type": "int"},
+        "parallelism": {"key": "parallelism", "type": "int"},
+    }
+
+    def __init__(
+        self, *, replica_completion_count: Optional[int] = None, parallelism: Optional[int] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword replica_completion_count: Minimum number of successful replica completions before
+         overall job completion.
+        :paramtype replica_completion_count: int
+        :keyword parallelism: Number of parallel replicas of a job that can run at a given time.
+        :paramtype parallelism: int
+        """
+        super().__init__(**kwargs)
+        self.replica_completion_count = replica_completion_count
+        self.parallelism = parallelism
+
+
+class JobConfigurationScheduleTriggerConfig(_serialization.Model):
+    """Cron formatted repeating trigger schedule ("\ * * * * *") for cronjobs. Properties completions
+    and parallelism would be set to 1 by default.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar replica_completion_count: Minimum number of successful replica completions before overall
+     job completion.
+    :vartype replica_completion_count: int
+    :ivar cron_expression: Cron formatted repeating schedule ("\ * * * * *") of a Cron Job.
+     Required.
+    :vartype cron_expression: str
+    :ivar parallelism: Number of parallel replicas of a job that can run at a given time.
+    :vartype parallelism: int
+    """
+
+    _validation = {
+        "cron_expression": {"required": True},
+    }
+
+    _attribute_map = {
+        "replica_completion_count": {"key": "replicaCompletionCount", "type": "int"},
+        "cron_expression": {"key": "cronExpression", "type": "str"},
+        "parallelism": {"key": "parallelism", "type": "int"},
+    }
+
+    def __init__(
+        self,
+        *,
+        cron_expression: str,
+        replica_completion_count: Optional[int] = None,
+        parallelism: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword replica_completion_count: Minimum number of successful replica completions before
+         overall job completion.
+        :paramtype replica_completion_count: int
+        :keyword cron_expression: Cron formatted repeating schedule ("\ * * * * *") of a Cron Job.
+         Required.
+        :paramtype cron_expression: str
+        :keyword parallelism: Number of parallel replicas of a job that can run at a given time.
+        :paramtype parallelism: int
+        """
+        super().__init__(**kwargs)
+        self.replica_completion_count = replica_completion_count
+        self.cron_expression = cron_expression
+        self.parallelism = parallelism
+
+
+class JobExecution(_serialization.Model):
+    """Container Apps Jobs execution.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar name: Job execution Name.
+    :vartype name: str
+    :ivar id: Job execution Id.
+    :vartype id: str
+    :ivar type: Job Type.
+    :vartype type: str
+    :ivar status: Current running State of the job. Known values are: "Running", "Processing",
+     "Stopped", "Degraded", "Failed", "Unknown", and "Succeeded".
+    :vartype status: str or ~azure.mgmt.appcontainers.models.JobExecutionRunningState
+    :ivar start_time: Job execution start time.
+    :vartype start_time: ~datetime.datetime
+    :ivar end_time: Job execution start time.
+    :vartype end_time: ~datetime.datetime
+    :ivar template: Job's execution container.
+    :vartype template: ~azure.mgmt.appcontainers.models.JobExecutionTemplate
+    """
+
+    _validation = {
+        "status": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "id": {"key": "id", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "status": {"key": "status", "type": "str"},
+        "start_time": {"key": "startTime", "type": "iso-8601"},
+        "end_time": {"key": "endTime", "type": "iso-8601"},
+        "template": {"key": "template", "type": "JobExecutionTemplate"},
+    }
+
+    def __init__(
+        self,
+        *,
+        name: Optional[str] = None,
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        type: Optional[str] = None,
+        start_time: Optional[datetime.datetime] = None,
+        end_time: Optional[datetime.datetime] = None,
+        template: Optional["_models.JobExecutionTemplate"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword name: Job execution Name.
+        :paramtype name: str
+        :keyword id: Job execution Id.
+        :paramtype id: str
+        :keyword type: Job Type.
+        :paramtype type: str
+        :keyword start_time: Job execution start time.
+        :paramtype start_time: ~datetime.datetime
+        :keyword end_time: Job execution start time.
+        :paramtype end_time: ~datetime.datetime
+        :keyword template: Job's execution container.
+        :paramtype template: ~azure.mgmt.appcontainers.models.JobExecutionTemplate
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.id = id
+        self.type = type
+        self.status = None
+        self.start_time = start_time
+        self.end_time = end_time
+        self.template = template
+
+
+class JobExecutionBase(_serialization.Model):
+    """Container App's Job execution name.
+
+    :ivar name: Job execution name.
+    :vartype name: str
+    :ivar id: Job execution Id.
+    :vartype id: str
+    """
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "id": {"key": "id", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        name: Optional[str] = None,
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword name: Job execution name.
+        :paramtype name: str
+        :keyword id: Job execution Id.
+        :paramtype id: str
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.id = id
+
+
+class JobExecutionContainer(_serialization.Model):
+    """Container Apps Jobs execution container definition.
+
+    :ivar image: Container image tag.
+    :vartype image: str
+    :ivar name: Custom container name.
+    :vartype name: str
+    :ivar command: Container start command.
+    :vartype command: list[str]
+    :ivar args: Container start command arguments.
+    :vartype args: list[str]
+    :ivar env: Container environment variables.
+    :vartype env: list[~azure.mgmt.appcontainers.models.EnvironmentVar]
+    :ivar resources: Container resource requirements.
+    :vartype resources: ~azure.mgmt.appcontainers.models.ContainerResources
+    """
+
+    _attribute_map = {
+        "image": {"key": "image", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "command": {"key": "command", "type": "[str]"},
+        "args": {"key": "args", "type": "[str]"},
+        "env": {"key": "env", "type": "[EnvironmentVar]"},
+        "resources": {"key": "resources", "type": "ContainerResources"},
+    }
+
+    def __init__(
+        self,
+        *,
+        image: Optional[str] = None,
+        name: Optional[str] = None,
+        command: Optional[List[str]] = None,
+        args: Optional[List[str]] = None,
+        env: Optional[List["_models.EnvironmentVar"]] = None,
+        resources: Optional["_models.ContainerResources"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword image: Container image tag.
+        :paramtype image: str
+        :keyword name: Custom container name.
+        :paramtype name: str
+        :keyword command: Container start command.
+        :paramtype command: list[str]
+        :keyword args: Container start command arguments.
+        :paramtype args: list[str]
+        :keyword env: Container environment variables.
+        :paramtype env: list[~azure.mgmt.appcontainers.models.EnvironmentVar]
+        :keyword resources: Container resource requirements.
+        :paramtype resources: ~azure.mgmt.appcontainers.models.ContainerResources
+        """
+        super().__init__(**kwargs)
+        self.image = image
+        self.name = name
+        self.command = command
+        self.args = args
+        self.env = env
+        self.resources = resources
+
+
+class JobExecutionNamesCollection(_serialization.Model):
+    """Container App executions names list.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar value: Collection of resources. Required.
+    :vartype value: list[~azure.mgmt.appcontainers.models.JobExecutionBase]
+    """
+
+    _validation = {
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[JobExecutionBase]"},
+    }
+
+    def __init__(self, *, value: List["_models.JobExecutionBase"], **kwargs: Any) -> None:
+        """
+        :keyword value: Collection of resources. Required.
+        :paramtype value: list[~azure.mgmt.appcontainers.models.JobExecutionBase]
+        """
+        super().__init__(**kwargs)
+        self.value = value
+
+
+class JobExecutionTemplate(_serialization.Model):
+    """Job's execution template, containing container configuration for a job's execution.
+
+    :ivar containers: List of container definitions for the Container Apps Job.
+    :vartype containers: list[~azure.mgmt.appcontainers.models.JobExecutionContainer]
+    :ivar init_containers: List of specialized containers that run before job containers.
+    :vartype init_containers: list[~azure.mgmt.appcontainers.models.JobExecutionContainer]
+    """
+
+    _attribute_map = {
+        "containers": {"key": "containers", "type": "[JobExecutionContainer]"},
+        "init_containers": {"key": "initContainers", "type": "[JobExecutionContainer]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        containers: Optional[List["_models.JobExecutionContainer"]] = None,
+        init_containers: Optional[List["_models.JobExecutionContainer"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword containers: List of container definitions for the Container Apps Job.
+        :paramtype containers: list[~azure.mgmt.appcontainers.models.JobExecutionContainer]
+        :keyword init_containers: List of specialized containers that run before job containers.
+        :paramtype init_containers: list[~azure.mgmt.appcontainers.models.JobExecutionContainer]
+        """
+        super().__init__(**kwargs)
+        self.containers = containers
+        self.init_containers = init_containers
+
+
+class JobPatchProperties(_serialization.Model):
+    """Container Apps Job resource specific properties.
+
+    :ivar identity: Managed identities needed by a container app job to interact with other Azure
+     services to not maintain any secrets or credentials in code.
+    :vartype identity: ~azure.mgmt.appcontainers.models.ManagedServiceIdentity
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar properties:
+    :vartype properties: ~azure.mgmt.appcontainers.models.JobPatchPropertiesProperties
+    """
+
+    _attribute_map = {
+        "identity": {"key": "identity", "type": "ManagedServiceIdentity"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "properties": {"key": "properties", "type": "JobPatchPropertiesProperties"},
+    }
+
+    def __init__(
+        self,
+        *,
+        identity: Optional["_models.ManagedServiceIdentity"] = None,
+        tags: Optional[Dict[str, str]] = None,
+        properties: Optional["_models.JobPatchPropertiesProperties"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword identity: Managed identities needed by a container app job to interact with other
+         Azure services to not maintain any secrets or credentials in code.
+        :paramtype identity: ~azure.mgmt.appcontainers.models.ManagedServiceIdentity
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword properties:
+        :paramtype properties: ~azure.mgmt.appcontainers.models.JobPatchPropertiesProperties
+        """
+        super().__init__(**kwargs)
+        self.identity = identity
+        self.tags = tags
+        self.properties = properties
+
+
+class JobPatchPropertiesProperties(_serialization.Model):
+    """JobPatchPropertiesProperties.
+
+    :ivar environment_id: Resource ID of environment.
+    :vartype environment_id: str
+    :ivar configuration: Container Apps Job configuration properties.
+    :vartype configuration: ~azure.mgmt.appcontainers.models.JobConfiguration
+    :ivar template: Container Apps job definition.
+    :vartype template: ~azure.mgmt.appcontainers.models.JobTemplate
+    :ivar outbound_ip_addresses: Outbound IP Addresses of a container apps job.
+    :vartype outbound_ip_addresses: list[str]
+    :ivar event_stream_endpoint: The endpoint of the eventstream of the container apps job.
+    :vartype event_stream_endpoint: str
+    """
+
+    _attribute_map = {
+        "environment_id": {"key": "environmentId", "type": "str"},
+        "configuration": {"key": "configuration", "type": "JobConfiguration"},
+        "template": {"key": "template", "type": "JobTemplate"},
+        "outbound_ip_addresses": {"key": "outboundIpAddresses", "type": "[str]"},
+        "event_stream_endpoint": {"key": "eventStreamEndpoint", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        environment_id: Optional[str] = None,
+        configuration: Optional["_models.JobConfiguration"] = None,
+        template: Optional["_models.JobTemplate"] = None,
+        outbound_ip_addresses: Optional[List[str]] = None,
+        event_stream_endpoint: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword environment_id: Resource ID of environment.
+        :paramtype environment_id: str
+        :keyword configuration: Container Apps Job configuration properties.
+        :paramtype configuration: ~azure.mgmt.appcontainers.models.JobConfiguration
+        :keyword template: Container Apps job definition.
+        :paramtype template: ~azure.mgmt.appcontainers.models.JobTemplate
+        :keyword outbound_ip_addresses: Outbound IP Addresses of a container apps job.
+        :paramtype outbound_ip_addresses: list[str]
+        :keyword event_stream_endpoint: The endpoint of the eventstream of the container apps job.
+        :paramtype event_stream_endpoint: str
+        """
+        super().__init__(**kwargs)
+        self.environment_id = environment_id
+        self.configuration = configuration
+        self.template = template
+        self.outbound_ip_addresses = outbound_ip_addresses
+        self.event_stream_endpoint = event_stream_endpoint
+
+
+class JobsCollection(_serialization.Model):
+    """Container Apps Jobs collection ARM resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar value: Collection of resources. Required.
+    :vartype value: list[~azure.mgmt.appcontainers.models.Job]
+    :ivar next_link: Link to next page of resources.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "value": {"required": True},
+        "next_link": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[Job]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(self, *, value: List["_models.Job"], **kwargs: Any) -> None:
+        """
+        :keyword value: Collection of resources. Required.
+        :paramtype value: list[~azure.mgmt.appcontainers.models.Job]
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = None
+
+
+class JobSecretsCollection(_serialization.Model):
+    """Container Apps Job Secrets Collection ARM resource.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar value: Collection of resources. Required.
+    :vartype value: list[~azure.mgmt.appcontainers.models.Secret]
+    """
+
+    _validation = {
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[Secret]"},
+    }
+
+    def __init__(self, *, value: List["_models.Secret"], **kwargs: Any) -> None:
+        """
+        :keyword value: Collection of resources. Required.
+        :paramtype value: list[~azure.mgmt.appcontainers.models.Secret]
+        """
+        super().__init__(**kwargs)
+        self.value = value
+
+
+class JobTemplate(_serialization.Model):
+    """Container Apps Job versioned application definition. Defines the desired state of an immutable
+    revision. Any changes to this section Will result in a new revision being created.
+
+    :ivar init_containers: List of specialized containers that run before app containers.
+    :vartype init_containers: list[~azure.mgmt.appcontainers.models.InitContainer]
+    :ivar containers: List of container definitions for the Container App.
+    :vartype containers: list[~azure.mgmt.appcontainers.models.Container]
+    :ivar volumes: List of volume definitions for the Container App.
+    :vartype volumes: list[~azure.mgmt.appcontainers.models.Volume]
+    """
+
+    _attribute_map = {
+        "init_containers": {"key": "initContainers", "type": "[InitContainer]"},
+        "containers": {"key": "containers", "type": "[Container]"},
+        "volumes": {"key": "volumes", "type": "[Volume]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        init_containers: Optional[List["_models.InitContainer"]] = None,
+        containers: Optional[List["_models.Container"]] = None,
+        volumes: Optional[List["_models.Volume"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword init_containers: List of specialized containers that run before app containers.
+        :paramtype init_containers: list[~azure.mgmt.appcontainers.models.InitContainer]
+        :keyword containers: List of container definitions for the Container App.
+        :paramtype containers: list[~azure.mgmt.appcontainers.models.Container]
+        :keyword volumes: List of volume definitions for the Container App.
+        :paramtype volumes: list[~azure.mgmt.appcontainers.models.Volume]
+        """
+        super().__init__(**kwargs)
+        self.init_containers = init_containers
+        self.containers = containers
+        self.volumes = volumes
+
+
 class JwtClaimChecks(_serialization.Model):
     """The configuration settings of the checks that should be made while validating the JWT Claims.
 
     :ivar allowed_groups: The list of the allowed groups.
     :vartype allowed_groups: list[str]
     :ivar allowed_client_applications: The list of the allowed client applications.
     :vartype allowed_client_applications: list[str]
@@ -4855,55 +5666,79 @@
     }
 
     def __init__(
         self,
         *,
         allowed_groups: Optional[List[str]] = None,
         allowed_client_applications: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword allowed_groups: The list of the allowed groups.
         :paramtype allowed_groups: list[str]
         :keyword allowed_client_applications: The list of the allowed client applications.
         :paramtype allowed_client_applications: list[str]
         """
         super().__init__(**kwargs)
         self.allowed_groups = allowed_groups
         self.allowed_client_applications = allowed_client_applications
 
 
+class KedaConfiguration(_serialization.Model):
+    """Configuration properties Keda component.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar version: The version of Keda.
+    :vartype version: str
+    """
+
+    _validation = {
+        "version": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "version": {"key": "version", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.version = None
+
+
 class LogAnalyticsConfiguration(_serialization.Model):
     """Log analytics configuration.
 
     :ivar customer_id: Log analytics customer id.
     :vartype customer_id: str
     :ivar shared_key: Log analytics customer key.
     :vartype shared_key: str
     """
 
     _attribute_map = {
         "customer_id": {"key": "customerId", "type": "str"},
         "shared_key": {"key": "sharedKey", "type": "str"},
     }
 
-    def __init__(self, *, customer_id: Optional[str] = None, shared_key: Optional[str] = None, **kwargs):
+    def __init__(self, *, customer_id: Optional[str] = None, shared_key: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword customer_id: Log analytics customer id.
         :paramtype customer_id: str
         :keyword shared_key: Log analytics customer key.
         :paramtype shared_key: str
         """
         super().__init__(**kwargs)
         self.customer_id = customer_id
         self.shared_key = shared_key
 
 
 class Login(_serialization.Model):
-    """The configuration settings of the login flow of users using ContainerApp Service Authentication/Authorization.
+    """The configuration settings of the login flow of users using ContainerApp Service
+    Authentication/Authorization.
 
     :ivar routes: The routes that specify the endpoints used for login and logout requests.
     :vartype routes: ~azure.mgmt.appcontainers.models.LoginRoutes
     :ivar preserve_url_fragments_for_logins: :code:`<code>true</code>` if the fragments from the
      request are preserved after the login request is made; otherwise, :code:`<code>false</code>`.
     :vartype preserve_url_fragments_for_logins: bool
     :ivar allowed_external_redirect_urls: External URLs that can be redirected to as part of
@@ -4929,16 +5764,16 @@
         self,
         *,
         routes: Optional["_models.LoginRoutes"] = None,
         preserve_url_fragments_for_logins: Optional[bool] = None,
         allowed_external_redirect_urls: Optional[List[str]] = None,
         cookie_expiration: Optional["_models.CookieExpiration"] = None,
         nonce: Optional["_models.Nonce"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword routes: The routes that specify the endpoints used for login and logout requests.
         :paramtype routes: ~azure.mgmt.appcontainers.models.LoginRoutes
         :keyword preserve_url_fragments_for_logins: :code:`<code>true</code>` if the fragments from the
          request are preserved after the login request is made; otherwise, :code:`<code>false</code>`.
         :paramtype preserve_url_fragments_for_logins: bool
         :keyword allowed_external_redirect_urls: External URLs that can be redirected to as part of
@@ -4966,15 +5801,15 @@
     :vartype logout_endpoint: str
     """
 
     _attribute_map = {
         "logout_endpoint": {"key": "logoutEndpoint", "type": "str"},
     }
 
-    def __init__(self, *, logout_endpoint: Optional[str] = None, **kwargs):
+    def __init__(self, *, logout_endpoint: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword logout_endpoint: The endpoint at which a logout request should be made.
         :paramtype logout_endpoint: str
         """
         super().__init__(**kwargs)
         self.logout_endpoint = logout_endpoint
 
@@ -4986,23 +5821,200 @@
     :vartype scopes: list[str]
     """
 
     _attribute_map = {
         "scopes": {"key": "scopes", "type": "[str]"},
     }
 
-    def __init__(self, *, scopes: Optional[List[str]] = None, **kwargs):
+    def __init__(self, *, scopes: Optional[List[str]] = None, **kwargs: Any) -> None:
         """
         :keyword scopes: A list of the scopes that should be requested while authenticating.
         :paramtype scopes: list[str]
         """
         super().__init__(**kwargs)
         self.scopes = scopes
 
 
+class ManagedCertificate(TrackedResource):
+    """Managed certificates used for Custom Domain bindings of Container Apps in a Managed
+    Environment.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.appcontainers.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    :ivar properties: Certificate resource specific properties.
+    :vartype properties: ~azure.mgmt.appcontainers.models.ManagedCertificateProperties
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+        "properties": {"key": "properties", "type": "ManagedCertificateProperties"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location: str,
+        tags: Optional[Dict[str, str]] = None,
+        properties: Optional["_models.ManagedCertificateProperties"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        :keyword properties: Certificate resource specific properties.
+        :paramtype properties: ~azure.mgmt.appcontainers.models.ManagedCertificateProperties
+        """
+        super().__init__(tags=tags, location=location, **kwargs)
+        self.properties = properties
+
+
+class ManagedCertificateCollection(_serialization.Model):
+    """Collection of Managed Certificates.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar value: Collection of resources. Required.
+    :vartype value: list[~azure.mgmt.appcontainers.models.ManagedCertificate]
+    :ivar next_link: Link to next page of resources.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "value": {"required": True},
+        "next_link": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[ManagedCertificate]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(self, *, value: List["_models.ManagedCertificate"], **kwargs: Any) -> None:
+        """
+        :keyword value: Collection of resources. Required.
+        :paramtype value: list[~azure.mgmt.appcontainers.models.ManagedCertificate]
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = None
+
+
+class ManagedCertificatePatch(_serialization.Model):
+    """A managed certificate to update.
+
+    :ivar tags: Application-specific metadata in the form of key-value pairs.
+    :vartype tags: dict[str, str]
+    """
+
+    _attribute_map = {
+        "tags": {"key": "tags", "type": "{str}"},
+    }
+
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword tags: Application-specific metadata in the form of key-value pairs.
+        :paramtype tags: dict[str, str]
+        """
+        super().__init__(**kwargs)
+        self.tags = tags
+
+
+class ManagedCertificateProperties(_serialization.Model):
+    """Certificate resource specific properties.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar provisioning_state: Provisioning state of the certificate. Known values are: "Succeeded",
+     "Failed", "Canceled", "DeleteFailed", and "Pending".
+    :vartype provisioning_state: str or
+     ~azure.mgmt.appcontainers.models.CertificateProvisioningState
+    :ivar subject_name: Subject name of the certificate.
+    :vartype subject_name: str
+    :ivar error: Any error occurred during the certificate provision.
+    :vartype error: str
+    :ivar domain_control_validation: Selected type of domain control validation for managed
+     certificates. Known values are: "CNAME", "HTTP", and "TXT".
+    :vartype domain_control_validation: str or
+     ~azure.mgmt.appcontainers.models.ManagedCertificateDomainControlValidation
+    :ivar validation_token: A TXT token used for DNS TXT domain control validation when issuing
+     this type of managed certificates.
+    :vartype validation_token: str
+    """
+
+    _validation = {
+        "provisioning_state": {"readonly": True},
+        "error": {"readonly": True},
+        "validation_token": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "provisioning_state": {"key": "provisioningState", "type": "str"},
+        "subject_name": {"key": "subjectName", "type": "str"},
+        "error": {"key": "error", "type": "str"},
+        "domain_control_validation": {"key": "domainControlValidation", "type": "str"},
+        "validation_token": {"key": "validationToken", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        subject_name: Optional[str] = None,
+        domain_control_validation: Optional[Union[str, "_models.ManagedCertificateDomainControlValidation"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword subject_name: Subject name of the certificate.
+        :paramtype subject_name: str
+        :keyword domain_control_validation: Selected type of domain control validation for managed
+         certificates. Known values are: "CNAME", "HTTP", and "TXT".
+        :paramtype domain_control_validation: str or
+         ~azure.mgmt.appcontainers.models.ManagedCertificateDomainControlValidation
+        """
+        super().__init__(**kwargs)
+        self.provisioning_state = None
+        self.subject_name = subject_name
+        self.error = None
+        self.domain_control_validation = domain_control_validation
+        self.validation_token = None
+
+
 class ManagedEnvironment(TrackedResource):  # pylint: disable=too-many-instance-attributes
     """An environment for hosting container apps.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -5019,16 +6031,14 @@
     :vartype system_data: ~azure.mgmt.appcontainers.models.SystemData
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
     :ivar kind: Kind of the Environment.
     :vartype kind: str
-    :ivar sku: SKU properties of the Environment.
-    :vartype sku: ~azure.mgmt.appcontainers.models.EnvironmentSkuProperties
     :ivar provisioning_state: Provisioning state of the Environment. Known values are: "Succeeded",
      "Failed", "Canceled", "Waiting", "InitializationInProgress", "InfrastructureSetupInProgress",
      "InfrastructureSetupComplete", "ScheduledForDelete", "UpgradeRequested", and "UpgradeFailed".
     :vartype provisioning_state: str or
      ~azure.mgmt.appcontainers.models.EnvironmentProvisioningState
     :ivar dapr_ai_instrumentation_key: Azure Monitor instrumentation key used by Dapr to export
      Service to Service communication telemetry.
@@ -5053,14 +6063,22 @@
     :ivar custom_domain_configuration: Custom domain configuration for the environment.
     :vartype custom_domain_configuration:
      ~azure.mgmt.appcontainers.models.CustomDomainConfiguration
     :ivar event_stream_endpoint: The endpoint of the eventstream of the Environment.
     :vartype event_stream_endpoint: str
     :ivar workload_profiles: Workload profiles configured for the Managed Environment.
     :vartype workload_profiles: list[~azure.mgmt.appcontainers.models.WorkloadProfile]
+    :ivar keda_configuration: The configuration of Keda component.
+    :vartype keda_configuration: ~azure.mgmt.appcontainers.models.KedaConfiguration
+    :ivar dapr_configuration: The configuration of Dapr component.
+    :vartype dapr_configuration: ~azure.mgmt.appcontainers.models.DaprConfiguration
+    :ivar infrastructure_resource_group: Name of the platform-managed resource group created for
+     the Managed Environment to host infrastructure resources. If a subnet ID is provided, this
+     resource group will be created in the same subscription as the subnet.
+    :vartype infrastructure_resource_group: str
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -5076,15 +6094,14 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "kind": {"key": "kind", "type": "str"},
-        "sku": {"key": "sku", "type": "EnvironmentSkuProperties"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "dapr_ai_instrumentation_key": {"key": "properties.daprAIInstrumentationKey", "type": "str"},
         "dapr_ai_connection_string": {"key": "properties.daprAIConnectionString", "type": "str"},
         "vnet_configuration": {"key": "properties.vnetConfiguration", "type": "VnetConfiguration"},
         "deployment_errors": {"key": "properties.deploymentErrors", "type": "str"},
         "default_domain": {"key": "properties.defaultDomain", "type": "str"},
         "static_ip": {"key": "properties.staticIp", "type": "str"},
@@ -5092,41 +6109,44 @@
         "zone_redundant": {"key": "properties.zoneRedundant", "type": "bool"},
         "custom_domain_configuration": {
             "key": "properties.customDomainConfiguration",
             "type": "CustomDomainConfiguration",
         },
         "event_stream_endpoint": {"key": "properties.eventStreamEndpoint", "type": "str"},
         "workload_profiles": {"key": "properties.workloadProfiles", "type": "[WorkloadProfile]"},
+        "keda_configuration": {"key": "properties.kedaConfiguration", "type": "KedaConfiguration"},
+        "dapr_configuration": {"key": "properties.daprConfiguration", "type": "DaprConfiguration"},
+        "infrastructure_resource_group": {"key": "properties.infrastructureResourceGroup", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
         kind: Optional[str] = None,
-        sku: Optional["_models.EnvironmentSkuProperties"] = None,
         dapr_ai_instrumentation_key: Optional[str] = None,
         dapr_ai_connection_string: Optional[str] = None,
         vnet_configuration: Optional["_models.VnetConfiguration"] = None,
         app_logs_configuration: Optional["_models.AppLogsConfiguration"] = None,
         zone_redundant: Optional[bool] = None,
         custom_domain_configuration: Optional["_models.CustomDomainConfiguration"] = None,
         workload_profiles: Optional[List["_models.WorkloadProfile"]] = None,
-        **kwargs
-    ):
+        keda_configuration: Optional["_models.KedaConfiguration"] = None,
+        dapr_configuration: Optional["_models.DaprConfiguration"] = None,
+        infrastructure_resource_group: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword kind: Kind of the Environment.
         :paramtype kind: str
-        :keyword sku: SKU properties of the Environment.
-        :paramtype sku: ~azure.mgmt.appcontainers.models.EnvironmentSkuProperties
         :keyword dapr_ai_instrumentation_key: Azure Monitor instrumentation key used by Dapr to export
          Service to Service communication telemetry.
         :paramtype dapr_ai_instrumentation_key: str
         :keyword dapr_ai_connection_string: Application Insights connection string used by Dapr to
          export Service to Service communication telemetry.
         :paramtype dapr_ai_connection_string: str
         :keyword vnet_configuration: Vnet configuration for the environment.
@@ -5138,67 +6158,40 @@
         :keyword zone_redundant: Whether or not this Managed Environment is zone-redundant.
         :paramtype zone_redundant: bool
         :keyword custom_domain_configuration: Custom domain configuration for the environment.
         :paramtype custom_domain_configuration:
          ~azure.mgmt.appcontainers.models.CustomDomainConfiguration
         :keyword workload_profiles: Workload profiles configured for the Managed Environment.
         :paramtype workload_profiles: list[~azure.mgmt.appcontainers.models.WorkloadProfile]
+        :keyword keda_configuration: The configuration of Keda component.
+        :paramtype keda_configuration: ~azure.mgmt.appcontainers.models.KedaConfiguration
+        :keyword dapr_configuration: The configuration of Dapr component.
+        :paramtype dapr_configuration: ~azure.mgmt.appcontainers.models.DaprConfiguration
+        :keyword infrastructure_resource_group: Name of the platform-managed resource group created for
+         the Managed Environment to host infrastructure resources. If a subnet ID is provided, this
+         resource group will be created in the same subscription as the subnet.
+        :paramtype infrastructure_resource_group: str
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.kind = kind
-        self.sku = sku
         self.provisioning_state = None
         self.dapr_ai_instrumentation_key = dapr_ai_instrumentation_key
         self.dapr_ai_connection_string = dapr_ai_connection_string
         self.vnet_configuration = vnet_configuration
         self.deployment_errors = None
         self.default_domain = None
         self.static_ip = None
         self.app_logs_configuration = app_logs_configuration
         self.zone_redundant = zone_redundant
         self.custom_domain_configuration = custom_domain_configuration
         self.event_stream_endpoint = None
         self.workload_profiles = workload_profiles
-
-
-class ManagedEnvironmentOutboundSettings(_serialization.Model):
-    """Configuration used to control the Environment Egress outbound traffic.
-
-    :ivar out_bound_type: Outbound type for the cluster. Known values are: "LoadBalancer" and
-     "UserDefinedRouting".
-    :vartype out_bound_type: str or ~azure.mgmt.appcontainers.models.ManagedEnvironmentOutBoundType
-    :ivar virtual_network_appliance_ip: Virtual Appliance IP used as the Egress controller for the
-     Environment.
-    :vartype virtual_network_appliance_ip: str
-    """
-
-    _attribute_map = {
-        "out_bound_type": {"key": "outBoundType", "type": "str"},
-        "virtual_network_appliance_ip": {"key": "virtualNetworkApplianceIp", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        out_bound_type: Optional[Union[str, "_models.ManagedEnvironmentOutBoundType"]] = None,
-        virtual_network_appliance_ip: Optional[str] = None,
-        **kwargs
-    ):
-        """
-        :keyword out_bound_type: Outbound type for the cluster. Known values are: "LoadBalancer" and
-         "UserDefinedRouting".
-        :paramtype out_bound_type: str or
-         ~azure.mgmt.appcontainers.models.ManagedEnvironmentOutBoundType
-        :keyword virtual_network_appliance_ip: Virtual Appliance IP used as the Egress controller for
-         the Environment.
-        :paramtype virtual_network_appliance_ip: str
-        """
-        super().__init__(**kwargs)
-        self.out_bound_type = out_bound_type
-        self.virtual_network_appliance_ip = virtual_network_appliance_ip
+        self.keda_configuration = keda_configuration
+        self.dapr_configuration = dapr_configuration
+        self.infrastructure_resource_group = infrastructure_resource_group
 
 
 class ManagedEnvironmentsCollection(_serialization.Model):
     """Collection of Environments.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -5216,15 +6209,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[ManagedEnvironment]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.ManagedEnvironment"], **kwargs):
+    def __init__(self, *, value: List["_models.ManagedEnvironment"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.ManagedEnvironment]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -5261,15 +6254,17 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "ManagedEnvironmentStorageProperties"},
     }
 
-    def __init__(self, *, properties: Optional["_models.ManagedEnvironmentStorageProperties"] = None, **kwargs):
+    def __init__(
+        self, *, properties: Optional["_models.ManagedEnvironmentStorageProperties"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword properties: Storage properties.
         :paramtype properties: ~azure.mgmt.appcontainers.models.ManagedEnvironmentStorageProperties
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -5281,15 +6276,15 @@
     :vartype azure_file: ~azure.mgmt.appcontainers.models.AzureFileProperties
     """
 
     _attribute_map = {
         "azure_file": {"key": "azureFile", "type": "AzureFileProperties"},
     }
 
-    def __init__(self, *, azure_file: Optional["_models.AzureFileProperties"] = None, **kwargs):
+    def __init__(self, *, azure_file: Optional["_models.AzureFileProperties"] = None, **kwargs: Any) -> None:
         """
         :keyword azure_file: Azure file properties.
         :paramtype azure_file: ~azure.mgmt.appcontainers.models.AzureFileProperties
         """
         super().__init__(**kwargs)
         self.azure_file = azure_file
 
@@ -5307,15 +6302,15 @@
         "value": {"required": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[ManagedEnvironmentStorage]"},
     }
 
-    def __init__(self, *, value: List["_models.ManagedEnvironmentStorage"], **kwargs):
+    def __init__(self, *, value: List["_models.ManagedEnvironmentStorage"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of storage resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.ManagedEnvironmentStorage]
         """
         super().__init__(**kwargs)
         self.value = value
 
@@ -5359,16 +6354,16 @@
     }
 
     def __init__(
         self,
         *,
         type: Union[str, "_models.ManagedServiceIdentityType"],
         user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentity"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword type: Type of managed service identity (where both SystemAssigned and UserAssigned
          types are allowed). Required. Known values are: "None", "SystemAssigned", "UserAssigned", and
          "SystemAssigned,UserAssigned".
         :paramtype type: str or ~azure.mgmt.appcontainers.models.ManagedServiceIdentityType
         :keyword user_assigned_identities: The set of user assigned identities associated with the
          resource. The userAssignedIdentities dictionary keys will be ARM resource ids in the form:
@@ -5397,16 +6392,16 @@
 
     _attribute_map = {
         "validate_nonce": {"key": "validateNonce", "type": "bool"},
         "nonce_expiration_interval": {"key": "nonceExpirationInterval", "type": "str"},
     }
 
     def __init__(
-        self, *, validate_nonce: Optional[bool] = None, nonce_expiration_interval: Optional[str] = None, **kwargs
-    ):
+        self, *, validate_nonce: Optional[bool] = None, nonce_expiration_interval: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword validate_nonce: :code:`<code>false</code>` if the nonce should not be validated while
          completing the login flow; otherwise, :code:`<code>true</code>`.
         :paramtype validate_nonce: bool
         :keyword nonce_expiration_interval: The time after the request is made when the nonce should
          expire.
         :paramtype nonce_expiration_interval: str
@@ -5433,16 +6428,16 @@
     }
 
     def __init__(
         self,
         *,
         method: Optional[Literal["ClientSecretPost"]] = None,
         client_secret_setting_name: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword method: The method that should be used to authenticate the user. Default value is
          "ClientSecretPost".
         :paramtype method: str
         :keyword client_secret_setting_name: The app setting that contains the client secret for the
          custom Open ID Connect provider.
         :paramtype client_secret_setting_name: str
@@ -5480,16 +6475,16 @@
         self,
         *,
         authorization_endpoint: Optional[str] = None,
         token_endpoint: Optional[str] = None,
         issuer: Optional[str] = None,
         certification_uri: Optional[str] = None,
         well_known_open_id_configuration: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword authorization_endpoint: The endpoint to be used to make an authorization request.
         :paramtype authorization_endpoint: str
         :keyword token_endpoint: The endpoint to be used to request a token.
         :paramtype token_endpoint: str
         :keyword issuer: The endpoint that issues the token.
         :paramtype issuer: str
@@ -5518,15 +6513,17 @@
     """
 
     _attribute_map = {
         "name_claim_type": {"key": "nameClaimType", "type": "str"},
         "scopes": {"key": "scopes", "type": "[str]"},
     }
 
-    def __init__(self, *, name_claim_type: Optional[str] = None, scopes: Optional[List[str]] = None, **kwargs):
+    def __init__(
+        self, *, name_claim_type: Optional[str] = None, scopes: Optional[List[str]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword name_claim_type: The name of the claim that contains the users name.
         :paramtype name_claim_type: str
         :keyword scopes: A list of the scopes that should be requested while authenticating.
         :paramtype scopes: list[str]
         """
         super().__init__(**kwargs)
@@ -5554,16 +6551,16 @@
 
     def __init__(
         self,
         *,
         client_id: Optional[str] = None,
         client_credential: Optional["_models.OpenIdConnectClientCredential"] = None,
         open_id_connect_configuration: Optional["_models.OpenIdConnectConfig"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword client_id: The client id of the custom Open ID Connect provider.
         :paramtype client_id: str
         :keyword client_credential: The authentication credentials of the custom Open ID Connect
          provider.
         :paramtype client_credential: ~azure.mgmt.appcontainers.models.OpenIdConnectClientCredential
         :keyword open_id_connect_configuration: The configuration settings of the endpoints used for
@@ -5599,16 +6596,16 @@
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         is_data_action: Optional[bool] = None,
         display: Optional["_models.OperationDisplay"] = None,
         origin: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Name of the operation.
         :paramtype name: str
         :keyword is_data_action: Indicates whether the operation is a data action.
         :paramtype is_data_action: bool
         :keyword display: Display of the operation.
         :paramtype display: ~azure.mgmt.appcontainers.models.OperationDisplay
@@ -5645,16 +6642,16 @@
     def __init__(
         self,
         *,
         provider: Optional[str] = None,
         resource: Optional[str] = None,
         operation: Optional[str] = None,
         description: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword provider: Resource provider of the operation.
         :paramtype provider: str
         :keyword resource: Resource of the operation.
         :paramtype resource: str
         :keyword operation: Localized friendly name for the operation.
         :paramtype operation: str
@@ -5687,16 +6684,16 @@
 
     def __init__(
         self,
         *,
         queue_name: Optional[str] = None,
         queue_length: Optional[int] = None,
         auth: Optional[List["_models.ScaleRuleAuth"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword queue_name: Queue name.
         :paramtype queue_name: str
         :keyword queue_length: Queue length.
         :paramtype queue_length: int
         :keyword auth: Authentication secrets for the queue scale rule.
         :paramtype auth: list[~azure.mgmt.appcontainers.models.ScaleRuleAuth]
@@ -5732,16 +6729,16 @@
     def __init__(
         self,
         *,
         server: Optional[str] = None,
         username: Optional[str] = None,
         password_secret_ref: Optional[str] = None,
         identity: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword server: Container Registry Server.
         :paramtype server: str
         :keyword username: Container Registry Username.
         :paramtype username: str
         :keyword password_secret_ref: The name of the Secret that contains the registry login password.
         :paramtype password_secret_ref: str
@@ -5776,16 +6773,16 @@
 
     def __init__(
         self,
         *,
         registry_url: Optional[str] = None,
         registry_user_name: Optional[str] = None,
         registry_password: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword registry_url: registry server Url.
         :paramtype registry_url: str
         :keyword registry_user_name: registry username.
         :paramtype registry_user_name: str
         :keyword registry_password: registry secret.
         :paramtype registry_password: str
@@ -5831,15 +6828,15 @@
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "created_time": {"key": "properties.createdTime", "type": "iso-8601"},
         "containers": {"key": "properties.containers", "type": "[ReplicaContainer]"},
     }
 
-    def __init__(self, *, containers: Optional[List["_models.ReplicaContainer"]] = None, **kwargs):
+    def __init__(self, *, containers: Optional[List["_models.ReplicaContainer"]] = None, **kwargs: Any) -> None:
         """
         :keyword containers: The containers collection under a replica.
         :paramtype containers: list[~azure.mgmt.appcontainers.models.ReplicaContainer]
         """
         super().__init__(**kwargs)
         self.created_time = None
         self.containers = containers
@@ -5858,15 +6855,15 @@
         "value": {"required": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Replica]"},
     }
 
-    def __init__(self, *, value: List["_models.Replica"], **kwargs):
+    def __init__(self, *, value: List["_models.Replica"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.Replica]
         """
         super().__init__(**kwargs)
         self.value = value
 
@@ -5911,16 +6908,16 @@
         self,
         *,
         name: Optional[str] = None,
         container_id: Optional[str] = None,
         ready: Optional[bool] = None,
         started: Optional[bool] = None,
         restart_count: Optional[int] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The Name of the Container.
         :paramtype name: str
         :keyword container_id: The Id of the Container.
         :paramtype container_id: str
         :keyword ready: The container ready status.
         :paramtype ready: bool
@@ -6013,15 +7010,15 @@
         "replicas": {"key": "properties.replicas", "type": "int"},
         "traffic_weight": {"key": "properties.trafficWeight", "type": "int"},
         "provisioning_error": {"key": "properties.provisioningError", "type": "str"},
         "health_state": {"key": "properties.healthState", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.created_time = None
         self.last_active_time = None
         self.fqdn = None
         self.template = None
         self.active = None
@@ -6051,15 +7048,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Revision]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.Revision"], **kwargs):
+    def __init__(self, *, value: List["_models.Revision"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.Revision]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -6084,16 +7081,16 @@
 
     def __init__(
         self,
         *,
         min_replicas: Optional[int] = None,
         max_replicas: int = 10,
         rules: Optional[List["_models.ScaleRule"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword min_replicas: Optional. Minimum number of container replicas.
         :paramtype min_replicas: int
         :keyword max_replicas: Optional. Maximum number of container replicas. Defaults to 10 if not
          set.
         :paramtype max_replicas: int
         :keyword rules: Scaling rules.
@@ -6132,16 +7129,16 @@
         self,
         *,
         name: Optional[str] = None,
         azure_queue: Optional["_models.QueueScaleRule"] = None,
         custom: Optional["_models.CustomScaleRule"] = None,
         http: Optional["_models.HttpScaleRule"] = None,
         tcp: Optional["_models.TcpScaleRule"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Scale Rule Name.
         :paramtype name: str
         :keyword azure_queue: Azure Queue based scaling.
         :paramtype azure_queue: ~azure.mgmt.appcontainers.models.QueueScaleRule
         :keyword custom: Custom scale rule.
         :paramtype custom: ~azure.mgmt.appcontainers.models.CustomScaleRule
@@ -6168,15 +7165,17 @@
     """
 
     _attribute_map = {
         "secret_ref": {"key": "secretRef", "type": "str"},
         "trigger_parameter": {"key": "triggerParameter", "type": "str"},
     }
 
-    def __init__(self, *, secret_ref: Optional[str] = None, trigger_parameter: Optional[str] = None, **kwargs):
+    def __init__(
+        self, *, secret_ref: Optional[str] = None, trigger_parameter: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword secret_ref: Name of the Container App secret from which to pull the auth params.
         :paramtype secret_ref: str
         :keyword trigger_parameter: Trigger Parameter that uses the secret.
         :paramtype trigger_parameter: str
         """
         super().__init__(**kwargs)
@@ -6187,31 +7186,55 @@
 class Secret(_serialization.Model):
     """Secret definition.
 
     :ivar name: Secret Name.
     :vartype name: str
     :ivar value: Secret Value.
     :vartype value: str
+    :ivar identity: Resource ID of a managed identity to authenticate with Azure Key Vault, or
+     System to use a system-assigned identity.
+    :vartype identity: str
+    :ivar key_vault_url: Azure Key Vault URL pointing to the secret referenced by the container
+     app.
+    :vartype key_vault_url: str
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "value": {"key": "value", "type": "str"},
+        "identity": {"key": "identity", "type": "str"},
+        "key_vault_url": {"key": "keyVaultUrl", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, value: Optional[str] = None, **kwargs):
+    def __init__(
+        self,
+        *,
+        name: Optional[str] = None,
+        value: Optional[str] = None,
+        identity: Optional[str] = None,
+        key_vault_url: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Secret Name.
         :paramtype name: str
         :keyword value: Secret Value.
         :paramtype value: str
+        :keyword identity: Resource ID of a managed identity to authenticate with Azure Key Vault, or
+         System to use a system-assigned identity.
+        :paramtype identity: str
+        :keyword key_vault_url: Azure Key Vault URL pointing to the secret referenced by the container
+         app.
+        :paramtype key_vault_url: str
         """
         super().__init__(**kwargs)
         self.name = name
         self.value = value
+        self.identity = identity
+        self.key_vault_url = key_vault_url
 
 
 class SecretsCollection(_serialization.Model):
     """Container App Secrets Collection ARM resource.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -6223,23 +7246,51 @@
         "value": {"required": True},
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[ContainerAppSecret]"},
     }
 
-    def __init__(self, *, value: List["_models.ContainerAppSecret"], **kwargs):
+    def __init__(self, *, value: List["_models.ContainerAppSecret"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.ContainerAppSecret]
         """
         super().__init__(**kwargs)
         self.value = value
 
 
+class SecretVolumeItem(_serialization.Model):
+    """Secret to be added to volume.
+
+    :ivar secret_ref: Name of the Container App secret from which to pull the secret value.
+    :vartype secret_ref: str
+    :ivar path: Path to project secret to. If no path is provided, path defaults to name of secret
+     listed in secretRef.
+    :vartype path: str
+    """
+
+    _attribute_map = {
+        "secret_ref": {"key": "secretRef", "type": "str"},
+        "path": {"key": "path", "type": "str"},
+    }
+
+    def __init__(self, *, secret_ref: Optional[str] = None, path: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword secret_ref: Name of the Container App secret from which to pull the secret value.
+        :paramtype secret_ref: str
+        :keyword path: Path to project secret to. If no path is provided, path defaults to name of
+         secret listed in secretRef.
+        :paramtype path: str
+        """
+        super().__init__(**kwargs)
+        self.secret_ref = secret_ref
+        self.path = path
+
+
 class SourceControl(ProxyResource):
     """Container App SourceControl.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
@@ -6291,16 +7342,16 @@
 
     def __init__(
         self,
         *,
         repo_url: Optional[str] = None,
         branch: Optional[str] = None,
         github_action_configuration: Optional["_models.GithubActionConfiguration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword repo_url: The repo url which will be integrated to ContainerApp.
         :paramtype repo_url: str
         :keyword branch: The branch which will trigger the auto deployment.
         :paramtype branch: str
         :keyword github_action_configuration: Container App Revision Template with all possible
          settings and the
@@ -6335,15 +7386,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[SourceControl]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.SourceControl"], **kwargs):
+    def __init__(self, *, value: List["_models.SourceControl"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.SourceControl]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -6382,16 +7433,16 @@
         *,
         created_by: Optional[str] = None,
         created_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         last_modified_at: Optional[datetime.datetime] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword created_by: The identity that created the resource.
         :paramtype created_by: str
         :keyword created_by_type: The type of identity that created the resource. Known values are:
          "User", "Application", "ManagedIdentity", and "Key".
         :paramtype created_by_type: str or ~azure.mgmt.appcontainers.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
@@ -6428,16 +7479,16 @@
     }
 
     def __init__(
         self,
         *,
         metadata: Optional[Dict[str, str]] = None,
         auth: Optional[List["_models.ScaleRuleAuth"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword metadata: Metadata properties to describe tcp scale rule.
         :paramtype metadata: dict[str, str]
         :keyword auth: Authentication secrets for the tcp scale rule.
         :paramtype auth: list[~azure.mgmt.appcontainers.models.ScaleRuleAuth]
         """
         super().__init__(**kwargs)
@@ -6446,24 +7497,24 @@
 
 
 class Template(_serialization.Model):
     """Container App versioned application definition.
     Defines the desired state of an immutable revision.
     Any changes to this section Will result in a new revision being created.
 
-        :ivar revision_suffix: User friendly suffix that is appended to the revision name.
-        :vartype revision_suffix: str
-        :ivar init_containers: List of specialized containers that run before app containers.
-        :vartype init_containers: list[~azure.mgmt.appcontainers.models.InitContainer]
-        :ivar containers: List of container definitions for the Container App.
-        :vartype containers: list[~azure.mgmt.appcontainers.models.Container]
-        :ivar scale: Scaling properties for the Container App.
-        :vartype scale: ~azure.mgmt.appcontainers.models.Scale
-        :ivar volumes: List of volume definitions for the Container App.
-        :vartype volumes: list[~azure.mgmt.appcontainers.models.Volume]
+    :ivar revision_suffix: User friendly suffix that is appended to the revision name.
+    :vartype revision_suffix: str
+    :ivar init_containers: List of specialized containers that run before app containers.
+    :vartype init_containers: list[~azure.mgmt.appcontainers.models.InitContainer]
+    :ivar containers: List of container definitions for the Container App.
+    :vartype containers: list[~azure.mgmt.appcontainers.models.Container]
+    :ivar scale: Scaling properties for the Container App.
+    :vartype scale: ~azure.mgmt.appcontainers.models.Scale
+    :ivar volumes: List of volume definitions for the Container App.
+    :vartype volumes: list[~azure.mgmt.appcontainers.models.Volume]
     """
 
     _attribute_map = {
         "revision_suffix": {"key": "revisionSuffix", "type": "str"},
         "init_containers": {"key": "initContainers", "type": "[InitContainer]"},
         "containers": {"key": "containers", "type": "[Container]"},
         "scale": {"key": "scale", "type": "Scale"},
@@ -6474,16 +7525,16 @@
         self,
         *,
         revision_suffix: Optional[str] = None,
         init_containers: Optional[List["_models.InitContainer"]] = None,
         containers: Optional[List["_models.Container"]] = None,
         scale: Optional["_models.Scale"] = None,
         volumes: Optional[List["_models.Volume"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword revision_suffix: User friendly suffix that is appended to the revision name.
         :paramtype revision_suffix: str
         :keyword init_containers: List of specialized containers that run before app containers.
         :paramtype init_containers: list[~azure.mgmt.appcontainers.models.InitContainer]
         :keyword containers: List of container definitions for the Container App.
         :paramtype containers: list[~azure.mgmt.appcontainers.models.Container]
@@ -6523,16 +7574,16 @@
     def __init__(
         self,
         *,
         revision_name: Optional[str] = None,
         weight: Optional[int] = None,
         latest_revision: bool = False,
         label: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword revision_name: Name of a revision.
         :paramtype revision_name: str
         :keyword weight: Traffic weight assigned to a revision.
         :paramtype weight: int
         :keyword latest_revision: Indicates that the traffic weight belongs to a latest stable
          revision.
@@ -6560,16 +7611,20 @@
 
     _attribute_map = {
         "enabled": {"key": "enabled", "type": "bool"},
         "registration": {"key": "registration", "type": "TwitterRegistration"},
     }
 
     def __init__(
-        self, *, enabled: Optional[bool] = None, registration: Optional["_models.TwitterRegistration"] = None, **kwargs
-    ):
+        self,
+        *,
+        enabled: Optional[bool] = None,
+        registration: Optional["_models.TwitterRegistration"] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: :code:`<code>false</code>` if the Twitter provider should not be enabled
          despite the set registration; otherwise, :code:`<code>true</code>`.
         :paramtype enabled: bool
         :keyword registration: The configuration settings of the app registration for the Twitter
          provider.
         :paramtype registration: ~azure.mgmt.appcontainers.models.TwitterRegistration
@@ -6594,16 +7649,16 @@
 
     _attribute_map = {
         "consumer_key": {"key": "consumerKey", "type": "str"},
         "consumer_secret_setting_name": {"key": "consumerSecretSettingName", "type": "str"},
     }
 
     def __init__(
-        self, *, consumer_key: Optional[str] = None, consumer_secret_setting_name: Optional[str] = None, **kwargs
-    ):
+        self, *, consumer_key: Optional[str] = None, consumer_secret_setting_name: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword consumer_key: The OAuth 1.0a consumer key of the Twitter application used for sign-in.
          This setting is required for enabling Twitter Sign-In.
          Twitter Sign-In documentation: https://dev.twitter.com/web/sign-in.
         :paramtype consumer_key: str
         :keyword consumer_secret_setting_name: The app setting name that contains the OAuth 1.0a
          consumer secret of the Twitter
@@ -6632,147 +7687,134 @@
     }
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "client_id": {"key": "clientId", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.principal_id = None
         self.client_id = None
 
 
 class VnetConfiguration(_serialization.Model):
     """Configuration properties for apps environment to join a Virtual Network.
 
     :ivar internal: Boolean indicating the environment only has an internal load balancer. These
-     environments do not have a public static IP resource. They must provide runtimeSubnetId and
-     infrastructureSubnetId if enabling this property.
+     environments do not have a public static IP resource. They must provide infrastructureSubnetId
+     if enabling this property.
     :vartype internal: bool
-    :ivar infrastructure_subnet_id: Resource ID of a subnet for infrastructure components. This
-     subnet must be in the same VNET as the subnet defined in runtimeSubnetId. Must not overlap with
-     any other provided IP ranges.
+    :ivar infrastructure_subnet_id: Resource ID of a subnet for infrastructure components. Must not
+     overlap with any other provided IP ranges.
     :vartype infrastructure_subnet_id: str
-    :ivar runtime_subnet_id: Resource ID of a subnet that Container App containers are injected
-     into. This subnet must be in the same VNET as the subnet defined in infrastructureSubnetId.
-     Must not overlap with any other provided IP ranges.
-    :vartype runtime_subnet_id: str
     :ivar docker_bridge_cidr: CIDR notation IP range assigned to the Docker bridge, network. Must
      not overlap with any other provided IP ranges.
     :vartype docker_bridge_cidr: str
     :ivar platform_reserved_cidr: IP range in CIDR notation that can be reserved for environment
      infrastructure IP addresses. Must not overlap with any other provided IP ranges.
     :vartype platform_reserved_cidr: str
     :ivar platform_reserved_dns_ip: An IP address from the IP range defined by platformReservedCidr
      that will be reserved for the internal DNS server.
     :vartype platform_reserved_dns_ip: str
-    :ivar outbound_settings: Configuration used to control the Environment Egress outbound traffic.
-    :vartype outbound_settings: ~azure.mgmt.appcontainers.models.ManagedEnvironmentOutboundSettings
     """
 
     _attribute_map = {
         "internal": {"key": "internal", "type": "bool"},
         "infrastructure_subnet_id": {"key": "infrastructureSubnetId", "type": "str"},
-        "runtime_subnet_id": {"key": "runtimeSubnetId", "type": "str"},
         "docker_bridge_cidr": {"key": "dockerBridgeCidr", "type": "str"},
         "platform_reserved_cidr": {"key": "platformReservedCidr", "type": "str"},
         "platform_reserved_dns_ip": {"key": "platformReservedDnsIP", "type": "str"},
-        "outbound_settings": {"key": "outboundSettings", "type": "ManagedEnvironmentOutboundSettings"},
     }
 
     def __init__(
         self,
         *,
         internal: Optional[bool] = None,
         infrastructure_subnet_id: Optional[str] = None,
-        runtime_subnet_id: Optional[str] = None,
         docker_bridge_cidr: Optional[str] = None,
         platform_reserved_cidr: Optional[str] = None,
         platform_reserved_dns_ip: Optional[str] = None,
-        outbound_settings: Optional["_models.ManagedEnvironmentOutboundSettings"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword internal: Boolean indicating the environment only has an internal load balancer. These
-         environments do not have a public static IP resource. They must provide runtimeSubnetId and
-         infrastructureSubnetId if enabling this property.
+         environments do not have a public static IP resource. They must provide infrastructureSubnetId
+         if enabling this property.
         :paramtype internal: bool
-        :keyword infrastructure_subnet_id: Resource ID of a subnet for infrastructure components. This
-         subnet must be in the same VNET as the subnet defined in runtimeSubnetId. Must not overlap with
-         any other provided IP ranges.
+        :keyword infrastructure_subnet_id: Resource ID of a subnet for infrastructure components. Must
+         not overlap with any other provided IP ranges.
         :paramtype infrastructure_subnet_id: str
-        :keyword runtime_subnet_id: Resource ID of a subnet that Container App containers are injected
-         into. This subnet must be in the same VNET as the subnet defined in infrastructureSubnetId.
-         Must not overlap with any other provided IP ranges.
-        :paramtype runtime_subnet_id: str
         :keyword docker_bridge_cidr: CIDR notation IP range assigned to the Docker bridge, network.
          Must not overlap with any other provided IP ranges.
         :paramtype docker_bridge_cidr: str
         :keyword platform_reserved_cidr: IP range in CIDR notation that can be reserved for environment
          infrastructure IP addresses. Must not overlap with any other provided IP ranges.
         :paramtype platform_reserved_cidr: str
         :keyword platform_reserved_dns_ip: An IP address from the IP range defined by
          platformReservedCidr that will be reserved for the internal DNS server.
         :paramtype platform_reserved_dns_ip: str
-        :keyword outbound_settings: Configuration used to control the Environment Egress outbound
-         traffic.
-        :paramtype outbound_settings:
-         ~azure.mgmt.appcontainers.models.ManagedEnvironmentOutboundSettings
         """
         super().__init__(**kwargs)
         self.internal = internal
         self.infrastructure_subnet_id = infrastructure_subnet_id
-        self.runtime_subnet_id = runtime_subnet_id
         self.docker_bridge_cidr = docker_bridge_cidr
         self.platform_reserved_cidr = platform_reserved_cidr
         self.platform_reserved_dns_ip = platform_reserved_dns_ip
-        self.outbound_settings = outbound_settings
 
 
 class Volume(_serialization.Model):
     """Volume definitions for the Container App.
 
     :ivar name: Volume name.
     :vartype name: str
     :ivar storage_type: Storage type for the volume. If not provided, use EmptyDir. Known values
-     are: "AzureFile" and "EmptyDir".
+     are: "AzureFile", "EmptyDir", and "Secret".
     :vartype storage_type: str or ~azure.mgmt.appcontainers.models.StorageType
-    :ivar storage_name: Name of storage resource. No need to provide for EmptyDir.
+    :ivar storage_name: Name of storage resource. No need to provide for EmptyDir and Secret.
     :vartype storage_name: str
+    :ivar secrets: List of secrets to be added in volume. If no secrets are provided, all secrets
+     in collection will be added to volume.
+    :vartype secrets: list[~azure.mgmt.appcontainers.models.SecretVolumeItem]
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "storage_type": {"key": "storageType", "type": "str"},
         "storage_name": {"key": "storageName", "type": "str"},
+        "secrets": {"key": "secrets", "type": "[SecretVolumeItem]"},
     }
 
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         storage_type: Optional[Union[str, "_models.StorageType"]] = None,
         storage_name: Optional[str] = None,
-        **kwargs
-    ):
+        secrets: Optional[List["_models.SecretVolumeItem"]] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Volume name.
         :paramtype name: str
         :keyword storage_type: Storage type for the volume. If not provided, use EmptyDir. Known values
-         are: "AzureFile" and "EmptyDir".
+         are: "AzureFile", "EmptyDir", and "Secret".
         :paramtype storage_type: str or ~azure.mgmt.appcontainers.models.StorageType
-        :keyword storage_name: Name of storage resource. No need to provide for EmptyDir.
+        :keyword storage_name: Name of storage resource. No need to provide for EmptyDir and Secret.
         :paramtype storage_name: str
+        :keyword secrets: List of secrets to be added in volume. If no secrets are provided, all
+         secrets in collection will be added to volume.
+        :paramtype secrets: list[~azure.mgmt.appcontainers.models.SecretVolumeItem]
         """
         super().__init__(**kwargs)
         self.name = name
         self.storage_type = storage_type
         self.storage_name = storage_name
+        self.secrets = secrets
 
 
 class VolumeMount(_serialization.Model):
     """Volume mount for the Container App.
 
     :ivar volume_name: This must match the Name of a Volume.
     :vartype volume_name: str
@@ -6782,15 +7824,15 @@
     """
 
     _attribute_map = {
         "volume_name": {"key": "volumeName", "type": "str"},
         "mount_path": {"key": "mountPath", "type": "str"},
     }
 
-    def __init__(self, *, volume_name: Optional[str] = None, mount_path: Optional[str] = None, **kwargs):
+    def __init__(self, *, volume_name: Optional[str] = None, mount_path: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword volume_name: This must match the Name of a Volume.
         :paramtype volume_name: str
         :keyword mount_path: Path within the container at which the volume should be mounted.Must not
          contain ':'.
         :paramtype mount_path: str
         """
@@ -6800,51 +7842,64 @@
 
 
 class WorkloadProfile(_serialization.Model):
     """Workload profile to scope container app execution.
 
     All required parameters must be populated in order to send to Azure.
 
+    :ivar name: Workload profile type for the workloads to run on. Required.
+    :vartype name: str
     :ivar workload_profile_type: Workload profile type for the workloads to run on. Required.
     :vartype workload_profile_type: str
-    :ivar minimum_count: The minimum capacity. Required.
+    :ivar minimum_count: The minimum capacity.
     :vartype minimum_count: int
-    :ivar maximum_count: The maximum capacity. Required.
+    :ivar maximum_count: The maximum capacity.
     :vartype maximum_count: int
     """
 
     _validation = {
+        "name": {"required": True},
         "workload_profile_type": {"required": True},
-        "minimum_count": {"required": True},
-        "maximum_count": {"required": True},
     }
 
     _attribute_map = {
+        "name": {"key": "name", "type": "str"},
         "workload_profile_type": {"key": "workloadProfileType", "type": "str"},
         "minimum_count": {"key": "minimumCount", "type": "int"},
         "maximum_count": {"key": "maximumCount", "type": "int"},
     }
 
-    def __init__(self, *, workload_profile_type: str, minimum_count: int, maximum_count: int, **kwargs):
+    def __init__(
+        self,
+        *,
+        name: str,
+        workload_profile_type: str,
+        minimum_count: Optional[int] = None,
+        maximum_count: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
         """
+        :keyword name: Workload profile type for the workloads to run on. Required.
+        :paramtype name: str
         :keyword workload_profile_type: Workload profile type for the workloads to run on. Required.
         :paramtype workload_profile_type: str
-        :keyword minimum_count: The minimum capacity. Required.
+        :keyword minimum_count: The minimum capacity.
         :paramtype minimum_count: int
-        :keyword maximum_count: The maximum capacity. Required.
+        :keyword maximum_count: The maximum capacity.
         :paramtype maximum_count: int
         """
         super().__init__(**kwargs)
+        self.name = name
         self.workload_profile_type = workload_profile_type
         self.minimum_count = minimum_count
         self.maximum_count = maximum_count
 
 
 class WorkloadProfileStates(ProxyResource):
-    """Collection of all the workload Profile States for a Premium Managed Environment..
+    """Collection of all the workload Profile States for a Managed Environment..
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
     :vartype id: str
     :ivar name: The name of the resource.
@@ -6870,15 +7925,17 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "WorkloadProfileStatesProperties"},
     }
 
-    def __init__(self, *, properties: Optional["_models.WorkloadProfileStatesProperties"] = None, **kwargs):
+    def __init__(
+        self, *, properties: Optional["_models.WorkloadProfileStatesProperties"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword properties: Workload Profile resource specific properties.
         :paramtype properties: ~azure.mgmt.appcontainers.models.WorkloadProfileStatesProperties
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -6902,15 +7959,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[WorkloadProfileStates]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: List["_models.WorkloadProfileStates"], **kwargs):
+    def __init__(self, *, value: List["_models.WorkloadProfileStates"], **kwargs: Any) -> None:
         """
         :keyword value: Collection of resources. Required.
         :paramtype value: list[~azure.mgmt.appcontainers.models.WorkloadProfileStates]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -6935,16 +7992,16 @@
 
     def __init__(
         self,
         *,
         minimum_count: Optional[int] = None,
         maximum_count: Optional[int] = None,
         current_count: Optional[int] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword minimum_count: Minimum count of instances.
         :paramtype minimum_count: int
         :keyword maximum_count: Maximum count of nodes.
         :paramtype maximum_count: int
         :keyword current_count: Current count of nodes.
         :paramtype current_count: int
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/_container_apps_api_client_enums.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/_container_apps_api_client_enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,21 @@
     provided, this is the default.</item></list>.
     """
 
     MULTIPLE = "Multiple"
     SINGLE = "Single"
 
 
+class Affinity(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Sticky Session Affinity."""
+
+    STICKY = "sticky"
+    NONE = "none"
+
+
 class Applicability(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """indicates whether the profile is default for the location."""
 
     LOCATION_DEFAULT = "LocationDefault"
     CUSTOM = "Custom"
 
 
@@ -60,22 +67,14 @@
 class BindingType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Custom Domain binding type."""
 
     DISABLED = "Disabled"
     SNI_ENABLED = "SniEnabled"
 
 
-class Category(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Used to map workload profile types to billing meter."""
-
-    PREMIUM_SKU_GENERAL_PURPOSE = "PremiumSkuGeneralPurpose"
-    PREMIUM_SKU_MEMORY_OPTIMIZED = "PremiumSkuMemoryOptimized"
-    PREMIUM_SKU_COMPUTE_OPTIMIZED = "PremiumSkuComputeOptimized"
-
-
 class CertificateProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Provisioning state of the certificate."""
 
     SUCCEEDED = "Succeeded"
     FAILED = "Failed"
     CANCELED = "Canceled"
     DELETE_FAILED = "DeleteFailed"
@@ -181,30 +180,53 @@
 
     AUTO = "auto"
     HTTP = "http"
     HTTP2 = "http2"
     TCP = "tcp"
 
 
+class JobExecutionRunningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Current running State of the job."""
+
+    RUNNING = "Running"
+    PROCESSING = "Processing"
+    STOPPED = "Stopped"
+    DEGRADED = "Degraded"
+    FAILED = "Failed"
+    UNKNOWN = "Unknown"
+    SUCCEEDED = "Succeeded"
+
+
+class JobProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Provisioning state of the Container Apps Job."""
+
+    IN_PROGRESS = "InProgress"
+    SUCCEEDED = "Succeeded"
+    FAILED = "Failed"
+    CANCELED = "Canceled"
+    DELETING = "Deleting"
+
+
 class LogLevel(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Sets the log level for the Dapr sidecar. Allowed values are debug, info, warn, error. Default
     is info.
     """
 
     INFO = "info"
     DEBUG = "debug"
     WARN = "warn"
     ERROR = "error"
 
 
-class ManagedEnvironmentOutBoundType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Outbound type for the cluster."""
+class ManagedCertificateDomainControlValidation(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Selected type of domain control validation for managed certificates."""
 
-    LOAD_BALANCER = "LoadBalancer"
-    USER_DEFINED_ROUTING = "UserDefinedRouting"
+    CNAME = "CNAME"
+    HTTP = "HTTP"
+    TXT = "TXT"
 
 
 class ManagedServiceIdentityType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Type of managed service identity (where both SystemAssigned and UserAssigned types are
     allowed).
     """
 
@@ -235,37 +257,37 @@
 class Scheme(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Scheme to use for connecting to the host. Defaults to HTTP."""
 
     HTTP = "HTTP"
     HTTPS = "HTTPS"
 
 
-class SkuName(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Name of the Sku."""
-
-    #: Consumption SKU of Managed Environment.
-    CONSUMPTION = "Consumption"
-    #: Premium SKU of Managed Environment.
-    PREMIUM = "Premium"
-
-
 class SourceControlOperationState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Current provisioning State of the operation."""
 
     IN_PROGRESS = "InProgress"
     SUCCEEDED = "Succeeded"
     FAILED = "Failed"
     CANCELED = "Canceled"
 
 
 class StorageType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Storage type for the volume. If not provided, use EmptyDir."""
 
     AZURE_FILE = "AzureFile"
     EMPTY_DIR = "EmptyDir"
+    SECRET = "Secret"
+
+
+class TriggerType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Trigger type of the job."""
+
+    SCHEDULED = "Scheduled"
+    EVENT = "Event"
+    MANUAL = "Manual"
 
 
 class Type(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of probe."""
 
     LIVENESS = "Liveness"
     READINESS = "Readiness"
```

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/_patch.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-appcontainers-2.0.0b2/azure/mgmt/appcontainers/models/__init__.py` & `azure-mgmt-appcontainers-3.0.0b1/azure/mgmt/appcontainers/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from ._models_py3 import ConnectedEnvironmentStorage
 from ._models_py3 import ConnectedEnvironmentStorageProperties
 from ._models_py3 import ConnectedEnvironmentStoragesCollection
 from ._models_py3 import Container
 from ._models_py3 import ContainerApp
 from ._models_py3 import ContainerAppAuthToken
 from ._models_py3 import ContainerAppCollection
+from ._models_py3 import ContainerAppJobExecutions
 from ._models_py3 import ContainerAppProbe
 from ._models_py3 import ContainerAppProbeHttpGet
 from ._models_py3 import ContainerAppProbeHttpGetHttpHeadersItem
 from ._models_py3 import ContainerAppProbeTcpSocket
 from ._models_py3 import ContainerAppSecret
 from ._models_py3 import ContainerResources
 from ._models_py3 import CookieExpiration
@@ -62,14 +63,15 @@
 from ._models_py3 import CustomHostnameAnalysisResultCustomDomainVerificationFailureInfo
 from ._models_py3 import CustomHostnameAnalysisResultCustomDomainVerificationFailureInfoDetailsItem
 from ._models_py3 import CustomOpenIdConnectProvider
 from ._models_py3 import CustomScaleRule
 from ._models_py3 import Dapr
 from ._models_py3 import DaprComponent
 from ._models_py3 import DaprComponentsCollection
+from ._models_py3 import DaprConfiguration
 from ._models_py3 import DaprMetadata
 from ._models_py3 import DaprSecret
 from ._models_py3 import DaprSecretsCollection
 from ._models_py3 import DefaultAuthorizationPolicy
 from ._models_py3 import DefaultErrorResponse
 from ._models_py3 import DefaultErrorResponseError
 from ._models_py3 import DefaultErrorResponseErrorDetailsItem
@@ -82,15 +84,14 @@
 from ._models_py3 import Diagnostics
 from ._models_py3 import DiagnosticsCollection
 from ._models_py3 import DiagnosticsDataApiResponse
 from ._models_py3 import DiagnosticsDefinition
 from ._models_py3 import DiagnosticsProperties
 from ._models_py3 import DiagnosticsStatus
 from ._models_py3 import EnvironmentAuthToken
-from ._models_py3 import EnvironmentSkuProperties
 from ._models_py3 import EnvironmentVar
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorResponse
 from ._models_py3 import ExtendedLocation
 from ._models_py3 import Facebook
 from ._models_py3 import ForwardProxy
@@ -99,23 +100,42 @@
 from ._models_py3 import GlobalValidation
 from ._models_py3 import Google
 from ._models_py3 import HttpScaleRule
 from ._models_py3 import HttpSettings
 from ._models_py3 import HttpSettingsRoutes
 from ._models_py3 import IdentityProviders
 from ._models_py3 import Ingress
+from ._models_py3 import IngressStickySessions
 from ._models_py3 import InitContainer
 from ._models_py3 import IpSecurityRestrictionRule
+from ._models_py3 import Job
+from ._models_py3 import JobConfiguration
+from ._models_py3 import JobConfigurationManualTriggerConfig
+from ._models_py3 import JobConfigurationScheduleTriggerConfig
+from ._models_py3 import JobExecution
+from ._models_py3 import JobExecutionBase
+from ._models_py3 import JobExecutionContainer
+from ._models_py3 import JobExecutionNamesCollection
+from ._models_py3 import JobExecutionTemplate
+from ._models_py3 import JobPatchProperties
+from ._models_py3 import JobPatchPropertiesProperties
+from ._models_py3 import JobSecretsCollection
+from ._models_py3 import JobTemplate
+from ._models_py3 import JobsCollection
 from ._models_py3 import JwtClaimChecks
+from ._models_py3 import KedaConfiguration
 from ._models_py3 import LogAnalyticsConfiguration
 from ._models_py3 import Login
 from ._models_py3 import LoginRoutes
 from ._models_py3 import LoginScopes
+from ._models_py3 import ManagedCertificate
+from ._models_py3 import ManagedCertificateCollection
+from ._models_py3 import ManagedCertificatePatch
+from ._models_py3 import ManagedCertificateProperties
 from ._models_py3 import ManagedEnvironment
-from ._models_py3 import ManagedEnvironmentOutboundSettings
 from ._models_py3 import ManagedEnvironmentStorage
 from ._models_py3 import ManagedEnvironmentStorageProperties
 from ._models_py3 import ManagedEnvironmentStoragesCollection
 from ._models_py3 import ManagedEnvironmentsCollection
 from ._models_py3 import ManagedServiceIdentity
 from ._models_py3 import Nonce
 from ._models_py3 import OpenIdConnectClientCredential
@@ -134,14 +154,15 @@
 from ._models_py3 import Resource
 from ._models_py3 import Revision
 from ._models_py3 import RevisionCollection
 from ._models_py3 import Scale
 from ._models_py3 import ScaleRule
 from ._models_py3 import ScaleRuleAuth
 from ._models_py3 import Secret
+from ._models_py3 import SecretVolumeItem
 from ._models_py3 import SecretsCollection
 from ._models_py3 import SourceControl
 from ._models_py3 import SourceControlCollection
 from ._models_py3 import SystemData
 from ._models_py3 import TcpScaleRule
 from ._models_py3 import Template
 from ._models_py3 import TrackedResource
@@ -156,39 +177,41 @@
 from ._models_py3 import WorkloadProfileStates
 from ._models_py3 import WorkloadProfileStatesCollection
 from ._models_py3 import WorkloadProfileStatesProperties
 
 from ._container_apps_api_client_enums import AccessMode
 from ._container_apps_api_client_enums import Action
 from ._container_apps_api_client_enums import ActiveRevisionsMode
+from ._container_apps_api_client_enums import Affinity
 from ._container_apps_api_client_enums import AppProtocol
 from ._container_apps_api_client_enums import Applicability
 from ._container_apps_api_client_enums import BindingType
-from ._container_apps_api_client_enums import Category
 from ._container_apps_api_client_enums import CertificateProvisioningState
 from ._container_apps_api_client_enums import CheckNameAvailabilityReason
 from ._container_apps_api_client_enums import ConnectedEnvironmentProvisioningState
 from ._container_apps_api_client_enums import ContainerAppProvisioningState
 from ._container_apps_api_client_enums import CookieExpirationConvention
 from ._container_apps_api_client_enums import CreatedByType
 from ._container_apps_api_client_enums import DnsVerificationTestResult
 from ._container_apps_api_client_enums import EnvironmentProvisioningState
 from ._container_apps_api_client_enums import ExtendedLocationTypes
 from ._container_apps_api_client_enums import ForwardProxyConvention
 from ._container_apps_api_client_enums import IngressClientCertificateMode
 from ._container_apps_api_client_enums import IngressTransportMethod
+from ._container_apps_api_client_enums import JobExecutionRunningState
+from ._container_apps_api_client_enums import JobProvisioningState
 from ._container_apps_api_client_enums import LogLevel
-from ._container_apps_api_client_enums import ManagedEnvironmentOutBoundType
+from ._container_apps_api_client_enums import ManagedCertificateDomainControlValidation
 from ._container_apps_api_client_enums import ManagedServiceIdentityType
 from ._container_apps_api_client_enums import RevisionHealthState
 from ._container_apps_api_client_enums import RevisionProvisioningState
 from ._container_apps_api_client_enums import Scheme
-from ._container_apps_api_client_enums import SkuName
 from ._container_apps_api_client_enums import SourceControlOperationState
 from ._container_apps_api_client_enums import StorageType
+from ._container_apps_api_client_enums import TriggerType
 from ._container_apps_api_client_enums import Type
 from ._container_apps_api_client_enums import UnauthenticatedClientActionV2
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
@@ -230,14 +253,15 @@
     "ConnectedEnvironmentStorage",
     "ConnectedEnvironmentStorageProperties",
     "ConnectedEnvironmentStoragesCollection",
     "Container",
     "ContainerApp",
     "ContainerAppAuthToken",
     "ContainerAppCollection",
+    "ContainerAppJobExecutions",
     "ContainerAppProbe",
     "ContainerAppProbeHttpGet",
     "ContainerAppProbeHttpGetHttpHeadersItem",
     "ContainerAppProbeTcpSocket",
     "ContainerAppSecret",
     "ContainerResources",
     "CookieExpiration",
@@ -248,14 +272,15 @@
     "CustomHostnameAnalysisResultCustomDomainVerificationFailureInfo",
     "CustomHostnameAnalysisResultCustomDomainVerificationFailureInfoDetailsItem",
     "CustomOpenIdConnectProvider",
     "CustomScaleRule",
     "Dapr",
     "DaprComponent",
     "DaprComponentsCollection",
+    "DaprConfiguration",
     "DaprMetadata",
     "DaprSecret",
     "DaprSecretsCollection",
     "DefaultAuthorizationPolicy",
     "DefaultErrorResponse",
     "DefaultErrorResponseError",
     "DefaultErrorResponseErrorDetailsItem",
@@ -268,15 +293,14 @@
     "Diagnostics",
     "DiagnosticsCollection",
     "DiagnosticsDataApiResponse",
     "DiagnosticsDefinition",
     "DiagnosticsProperties",
     "DiagnosticsStatus",
     "EnvironmentAuthToken",
-    "EnvironmentSkuProperties",
     "EnvironmentVar",
     "ErrorAdditionalInfo",
     "ErrorDetail",
     "ErrorResponse",
     "ExtendedLocation",
     "Facebook",
     "ForwardProxy",
@@ -285,23 +309,42 @@
     "GlobalValidation",
     "Google",
     "HttpScaleRule",
     "HttpSettings",
     "HttpSettingsRoutes",
     "IdentityProviders",
     "Ingress",
+    "IngressStickySessions",
     "InitContainer",
     "IpSecurityRestrictionRule",
+    "Job",
+    "JobConfiguration",
+    "JobConfigurationManualTriggerConfig",
+    "JobConfigurationScheduleTriggerConfig",
+    "JobExecution",
+    "JobExecutionBase",
+    "JobExecutionContainer",
+    "JobExecutionNamesCollection",
+    "JobExecutionTemplate",
+    "JobPatchProperties",
+    "JobPatchPropertiesProperties",
+    "JobSecretsCollection",
+    "JobTemplate",
+    "JobsCollection",
     "JwtClaimChecks",
+    "KedaConfiguration",
     "LogAnalyticsConfiguration",
     "Login",
     "LoginRoutes",
     "LoginScopes",
+    "ManagedCertificate",
+    "ManagedCertificateCollection",
+    "ManagedCertificatePatch",
+    "ManagedCertificateProperties",
     "ManagedEnvironment",
-    "ManagedEnvironmentOutboundSettings",
     "ManagedEnvironmentStorage",
     "ManagedEnvironmentStorageProperties",
     "ManagedEnvironmentStoragesCollection",
     "ManagedEnvironmentsCollection",
     "ManagedServiceIdentity",
     "Nonce",
     "OpenIdConnectClientCredential",
@@ -320,14 +363,15 @@
     "Resource",
     "Revision",
     "RevisionCollection",
     "Scale",
     "ScaleRule",
     "ScaleRuleAuth",
     "Secret",
+    "SecretVolumeItem",
     "SecretsCollection",
     "SourceControl",
     "SourceControlCollection",
     "SystemData",
     "TcpScaleRule",
     "Template",
     "TrackedResource",
@@ -341,37 +385,39 @@
     "WorkloadProfile",
     "WorkloadProfileStates",
     "WorkloadProfileStatesCollection",
     "WorkloadProfileStatesProperties",
     "AccessMode",
     "Action",
     "ActiveRevisionsMode",
+    "Affinity",
     "AppProtocol",
     "Applicability",
     "BindingType",
-    "Category",
     "CertificateProvisioningState",
     "CheckNameAvailabilityReason",
     "ConnectedEnvironmentProvisioningState",
     "ContainerAppProvisioningState",
     "CookieExpirationConvention",
     "CreatedByType",
     "DnsVerificationTestResult",
     "EnvironmentProvisioningState",
     "ExtendedLocationTypes",
     "ForwardProxyConvention",
     "IngressClientCertificateMode",
     "IngressTransportMethod",
+    "JobExecutionRunningState",
+    "JobProvisioningState",
     "LogLevel",
-    "ManagedEnvironmentOutBoundType",
+    "ManagedCertificateDomainControlValidation",
     "ManagedServiceIdentityType",
     "RevisionHealthState",
     "RevisionProvisioningState",
     "Scheme",
-    "SkuName",
     "SourceControlOperationState",
     "StorageType",
+    "TriggerType",
     "Type",
     "UnauthenticatedClientActionV2",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

