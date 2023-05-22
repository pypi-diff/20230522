# Comparing `tmp/azure-mgmt-devcenter-1.0.0b3.zip` & `tmp/azure-mgmt-devcenter-1.0.0b4.zip`

## zipinfo {}

```diff
@@ -1,83 +1,85 @@
-Zip file size: 195019 bytes, number of entries: 81
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/
--rw-rw-r--  2.0 unx     2861 b- defN 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/PKG-INFO
--rw-rw-r--  2.0 unx      626 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/_meta.json
--rw-rw-r--  2.0 unx     2824 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/setup.py
--rw-rw-r--  2.0 unx      215 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/MANIFEST.in
--rw-rw-r--  2.0 unx     1364 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/README.md
--rw-rw-r--  2.0 unx      604 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/CHANGELOG.md
--rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/LICENSE
--rw-rw-r--  2.0 unx       38 b- defN 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/setup.cfg
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/
--rw-rw-r--  2.0 unx       65 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/
--rw-rw-r--  2.0 unx      913 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/py.typed
--rw-rw-r--  2.0 unx     9162 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_dev_center_mgmt_client.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_patch.py
--rw-rw-r--  2.0 unx     3804 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_configuration.py
--rw-rw-r--  2.0 unx    77450 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_serialization.py
--rw-rw-r--  2.0 unx      488 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_version.py
--rw-rw-r--  2.0 unx     1169 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_vendor.py
--rw-rw-r--  2.0 unx     7850 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/__init__.py
--rw-rw-r--  2.0 unx   170625 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/_models_py3.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/_patch.py
--rw-rw-r--  2.0 unx     3759 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/_dev_center_mgmt_client_enums.py
--rw-rw-r--  2.0 unx     2369 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/__init__.py
--rw-rw-r--  2.0 unx     7445 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_usages_operations.py
--rw-rw-r--  2.0 unx    13616 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_image_versions_operations.py
--rw-rw-r--  2.0 unx    52444 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_catalogs_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_patch.py
--rw-rw-r--  2.0 unx    12927 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_project_allowed_environment_types_operations.py
--rw-rw-r--  2.0 unx    34069 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_project_environment_types_operations.py
--rw-rw-r--  2.0 unx    48220 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_dev_centers_operations.py
--rw-rw-r--  2.0 unx    19219 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_images_operations.py
--rw-rw-r--  2.0 unx    57537 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_dev_box_definitions_operations.py
--rw-rw-r--  2.0 unx    45386 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_attached_networks_operations.py
--rw-rw-r--  2.0 unx     6388 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_operation_statuses_operations.py
--rw-rw-r--  2.0 unx    33939 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_environment_types_operations.py
--rw-rw-r--  2.0 unx    47825 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_projects_operations.py
--rw-rw-r--  2.0 unx     7483 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_skus_operations.py
--rw-rw-r--  2.0 unx    50249 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_schedules_operations.py
--rw-rw-r--  2.0 unx     6707 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_operations.py
--rw-rw-r--  2.0 unx    64919 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_network_connections_operations.py
--rw-rw-r--  2.0 unx    32610 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_galleries_operations.py
--rw-rw-r--  2.0 unx    44608 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_pools_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/
--rw-rw-r--  2.0 unx      860 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/__init__.py
--rw-rw-r--  2.0 unx     9303 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/_dev_center_mgmt_client.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/_patch.py
--rw-rw-r--  2.0 unx     3808 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/_configuration.py
--rw-rw-r--  2.0 unx     2369 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     6277 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_usages_operations.py
--rw-rw-r--  2.0 unx    10246 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_image_versions_operations.py
--rw-rw-r--  2.0 unx    43503 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_catalogs_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     9923 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_project_allowed_environment_types_operations.py
--rw-rw-r--  2.0 unx    25974 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_project_environment_types_operations.py
--rw-rw-r--  2.0 unx    40204 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_dev_centers_operations.py
--rw-rw-r--  2.0 unx    14465 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_images_operations.py
--rw-rw-r--  2.0 unx    46661 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_dev_box_definitions_operations.py
--rw-rw-r--  2.0 unx    35883 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_attached_networks_operations.py
--rw-rw-r--  2.0 unx     5061 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_operation_statuses_operations.py
--rw-rw-r--  2.0 unx    25752 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_environment_types_operations.py
--rw-rw-r--  2.0 unx    39876 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_projects_operations.py
--rw-rw-r--  2.0 unx     6341 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_skus_operations.py
--rw-rw-r--  2.0 unx    41377 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_schedules_operations.py
--rw-rw-r--  2.0 unx     5950 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    52175 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_network_connections_operations.py
--rw-rw-r--  2.0 unx    26668 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_galleries_operations.py
--rw-rw-r--  2.0 unx    37179 b- defN 22-Nov-08 05:57 azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_pools_operations.py
--rw-rw-r--  2.0 unx     2861 b- defN 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx      116 b- defN 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     3433 b- defN 22-Nov-08 05:58 azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/SOURCES.txt
-81 files, 1372585 bytes uncompressed, 177003 bytes compressed:  87.1%
+Zip file size: 201978 bytes, number of entries: 83
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/
+-rw-rw-r--  2.0 unx     2824 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/setup.py
+-rw-rw-r--  2.0 unx       38 b- defN 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/setup.cfg
+-rw-rw-r--  2.0 unx     3576 b- defN 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/PKG-INFO
+-rw-rw-r--  2.0 unx      215 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/MANIFEST.in
+-rw-rw-r--  2.0 unx     1364 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/README.md
+-rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/LICENSE
+-rw-rw-r--  2.0 unx     1319 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/CHANGELOG.md
+-rw-rw-r--  2.0 unx      626 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/_meta.json
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/
+-rw-rw-r--  2.0 unx     9541 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_dev_center_mgmt_client.py
+-rw-rw-r--  2.0 unx      913 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/__init__.py
+-rw-rw-r--  2.0 unx       26 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/py.typed
+-rw-rw-r--  2.0 unx    77450 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_serialization.py
+-rw-rw-r--  2.0 unx      488 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_version.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_patch.py
+-rw-rw-r--  2.0 unx     3804 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_configuration.py
+-rw-rw-r--  2.0 unx     1169 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_vendor.py
+-rw-rw-r--  2.0 unx    34069 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_project_environment_types_operations.py
+-rw-rw-r--  2.0 unx    44608 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_pools_operations.py
+-rw-rw-r--  2.0 unx    19219 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_images_operations.py
+-rw-rw-r--  2.0 unx    47825 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_projects_operations.py
+-rw-rw-r--  2.0 unx    48220 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_dev_centers_operations.py
+-rw-rw-r--  2.0 unx     2489 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/__init__.py
+-rw-rw-r--  2.0 unx    32610 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_galleries_operations.py
+-rw-rw-r--  2.0 unx    52444 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_catalogs_operations.py
+-rw-rw-r--  2.0 unx     9112 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx    67905 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_network_connections_operations.py
+-rw-rw-r--  2.0 unx     6707 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_operations.py
+-rw-rw-r--  2.0 unx    50249 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_schedules_operations.py
+-rw-rw-r--  2.0 unx     7483 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_skus_operations.py
+-rw-rw-r--  2.0 unx    33939 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_environment_types_operations.py
+-rw-rw-r--  2.0 unx    57537 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_dev_box_definitions_operations.py
+-rw-rw-r--  2.0 unx    13616 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_image_versions_operations.py
+-rw-rw-r--  2.0 unx     7445 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_usages_operations.py
+-rw-rw-r--  2.0 unx    45386 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_attached_networks_operations.py
+-rw-rw-r--  2.0 unx     6388 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_operation_statuses_operations.py
+-rw-rw-r--  2.0 unx    12927 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_project_allowed_environment_types_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_patch.py
+-rw-rw-r--  2.0 unx     4767 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/_dev_center_mgmt_client_enums.py
+-rw-rw-r--  2.0 unx     8368 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/__init__.py
+-rw-rw-r--  2.0 unx   184970 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/_models_py3.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/_patch.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/
+-rw-rw-r--  2.0 unx     9686 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/_dev_center_mgmt_client.py
+-rw-rw-r--  2.0 unx      860 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/_patch.py
+-rw-rw-r--  2.0 unx     3808 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/_configuration.py
+-rw-rw-r--  2.0 unx    25974 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_project_environment_types_operations.py
+-rw-rw-r--  2.0 unx    37179 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_pools_operations.py
+-rw-rw-r--  2.0 unx    14465 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_images_operations.py
+-rw-rw-r--  2.0 unx    39876 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_projects_operations.py
+-rw-rw-r--  2.0 unx    40204 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_dev_centers_operations.py
+-rw-rw-r--  2.0 unx     2489 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    26668 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_galleries_operations.py
+-rw-rw-r--  2.0 unx    43503 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_catalogs_operations.py
+-rw-rw-r--  2.0 unx     7822 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx    55255 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_network_connections_operations.py
+-rw-rw-r--  2.0 unx     5950 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    41377 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_schedules_operations.py
+-rw-rw-r--  2.0 unx     6341 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_skus_operations.py
+-rw-rw-r--  2.0 unx    25752 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_environment_types_operations.py
+-rw-rw-r--  2.0 unx    46661 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_dev_box_definitions_operations.py
+-rw-rw-r--  2.0 unx    10246 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_image_versions_operations.py
+-rw-rw-r--  2.0 unx     6277 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_usages_operations.py
+-rw-rw-r--  2.0 unx    35883 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_attached_networks_operations.py
+-rw-rw-r--  2.0 unx     5061 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_operation_statuses_operations.py
+-rw-rw-r--  2.0 unx     9923 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_project_allowed_environment_types_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-24 05:31 azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      116 b- defN 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     3576 b- defN 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx     3579 b- defN 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-24 05:32 azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/dependency_links.txt
+83 files, 1414749 bytes uncompressed, 183406 bytes compressed:  87.0%
```

## zipnote {}

```diff
@@ -1,244 +1,250 @@
-Filename: azure-mgmt-devcenter-1.0.0b3/
+Filename: azure-mgmt-devcenter-1.0.0b4/
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/
+Filename: azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/PKG-INFO
+Filename: azure-mgmt-devcenter-1.0.0b4/setup.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/_meta.json
+Filename: azure-mgmt-devcenter-1.0.0b4/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/setup.py
+Filename: azure-mgmt-devcenter-1.0.0b4/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/MANIFEST.in
+Filename: azure-mgmt-devcenter-1.0.0b4/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/README.md
+Filename: azure-mgmt-devcenter-1.0.0b4/README.md
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/CHANGELOG.md
+Filename: azure-mgmt-devcenter-1.0.0b4/LICENSE
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/LICENSE
+Filename: azure-mgmt-devcenter-1.0.0b4/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/setup.cfg
+Filename: azure-mgmt-devcenter-1.0.0b4/_meta.json
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/__init__.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/__init__.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/__init__.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_dev_center_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/py.typed
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/__init__.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_dev_center_mgmt_client.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/py.typed
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_patch.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_configuration.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_version.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_serialization.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_patch.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_version.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_vendor.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/__init__.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_project_environment_types_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/_models_py3.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/_patch.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_images_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/_dev_center_mgmt_client_enums.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_projects_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/__init__.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_dev_centers_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_usages_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_image_versions_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_galleries_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_catalogs_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_catalogs_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_patch.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_project_allowed_environment_types_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_network_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_project_environment_types_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_dev_centers_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_schedules_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_images_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_skus_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_dev_box_definitions_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_environment_types_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_attached_networks_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_dev_box_definitions_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_operation_statuses_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_image_versions_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_environment_types_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_usages_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_projects_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_attached_networks_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_skus_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_operation_statuses_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_schedules_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_project_allowed_environment_types_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_network_connections_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/_dev_center_mgmt_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_galleries_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_pools_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/__init__.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/_dev_center_mgmt_client.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/_dev_center_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/_patch.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/_configuration.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/__init__.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_usages_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_project_environment_types_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_image_versions_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_catalogs_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_images_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_patch.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_projects_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_project_allowed_environment_types_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_dev_centers_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_project_environment_types_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_dev_centers_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_galleries_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_images_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_catalogs_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_dev_box_definitions_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_attached_networks_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_network_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_operation_statuses_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_environment_types_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_schedules_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_projects_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_skus_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_skus_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_environment_types_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_schedules_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_dev_box_definitions_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_image_versions_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_network_connections_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_usages_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_galleries_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_attached_networks_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_pools_operations.py
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_operation_statuses_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/PKG-INFO
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_project_allowed_environment_types_operations.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/requires.txt
+Filename: azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/top_level.txt
+Filename: azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/dependency_links.txt
+Filename: azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/not-zip-safe
+Filename: azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/SOURCES.txt
+Filename: azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/PKG-INFO` & `azure-mgmt-devcenter-1.0.0b4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-devcenter
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Microsoft Azure Devcenter Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -49,14 +49,31 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-devcenter%2FREADME.png)
 
 
 # Release History
 
+## 1.0.0b4 (2022-11-24)
+
+### Features Added
+
+  - Added operation group CheckNameAvailabilityOperations
+  - Model DevBoxDefinition has a new parameter hibernate_support
+  - Model DevBoxDefinitionProperties has a new parameter hibernate_support
+  - Model DevBoxDefinitionUpdate has a new parameter hibernate_support
+  - Model DevBoxDefinitionUpdateProperties has a new parameter hibernate_support
+  - Model DevCenter has a new parameter dev_center_uri
+  - Model Project has a new parameter dev_center_uri
+  - Model ProjectProperties has a new parameter dev_center_uri
+
+### Breaking Changes
+
+  - Renamed operation NetworkConnectionsOperations.run_health_checks to NetworkConnectionsOperations.begin_run_health_checks
+
 ## 1.0.0b3 (2022-11-08)
 
 ### Features Added
 
   - Model Catalog has a new parameter sync_state
   - Model CatalogProperties has a new parameter sync_state
   - Model OperationStatus has a new parameter operations
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/_meta.json` & `azure-mgmt-devcenter-1.0.0b4/_meta.json`

 * *Files 7% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'commit'": "'b1780623ffb2d4c719c2a62878930d317522290d'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
     "autorest_command": "autorest specification/devcenter/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.2.1 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "4903b1ed79e30f689d7c469cfa06734cfcd106d6",
+    "commit": "b1780623ffb2d4c719c2a62878930d317522290d",
     "readme": "specification/devcenter/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
         "@autorest/python@6.2.1",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/setup.py` & `azure-mgmt-devcenter-1.0.0b4/setup.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/README.md` & `azure-mgmt-devcenter-1.0.0b4/README.md`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/LICENSE` & `azure-mgmt-devcenter-1.0.0b4/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/__init__.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_dev_center_mgmt_client.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_dev_center_mgmt_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from . import models
 from ._configuration import DevCenterMgmtClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     AttachedNetworksOperations,
     CatalogsOperations,
+    CheckNameAvailabilityOperations,
     DevBoxDefinitionsOperations,
     DevCentersOperations,
     EnvironmentTypesOperations,
     GalleriesOperations,
     ImageVersionsOperations,
     ImagesOperations,
     NetworkConnectionsOperations,
@@ -70,29 +71,32 @@
     :vartype dev_box_definitions: azure.mgmt.devcenter.operations.DevBoxDefinitionsOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.devcenter.operations.Operations
     :ivar operation_statuses: OperationStatusesOperations operations
     :vartype operation_statuses: azure.mgmt.devcenter.operations.OperationStatusesOperations
     :ivar usages: UsagesOperations operations
     :vartype usages: azure.mgmt.devcenter.operations.UsagesOperations
+    :ivar check_name_availability: CheckNameAvailabilityOperations operations
+    :vartype check_name_availability:
+     azure.mgmt.devcenter.operations.CheckNameAvailabilityOperations
     :ivar skus: SkusOperations operations
     :vartype skus: azure.mgmt.devcenter.operations.SkusOperations
     :ivar pools: PoolsOperations operations
     :vartype pools: azure.mgmt.devcenter.operations.PoolsOperations
     :ivar schedules: SchedulesOperations operations
     :vartype schedules: azure.mgmt.devcenter.operations.SchedulesOperations
     :ivar network_connections: NetworkConnectionsOperations operations
     :vartype network_connections: azure.mgmt.devcenter.operations.NetworkConnectionsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-10-12-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-11-11-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -133,14 +137,17 @@
             self._client, self._config, self._serialize, self._deserialize
         )
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.operation_statuses = OperationStatusesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.usages = UsagesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.check_name_availability = CheckNameAvailabilityOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.pools = PoolsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.schedules = SchedulesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.network_connections = NetworkConnectionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_patch.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_configuration.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-10-12-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-11-11-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(DevCenterMgmtClientConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-10-12-preview")  # type: Literal["2022-10-12-preview"]
+        api_version = kwargs.pop("api_version", "2022-11-11-preview")  # type: Literal["2022-11-11-preview"]
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_serialization.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/_vendor.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/__init__.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from ._models_py3 import AttachedNetworkListResult
 from ._models_py3 import Capability
 from ._models_py3 import Catalog
 from ._models_py3 import CatalogListResult
 from ._models_py3 import CatalogProperties
 from ._models_py3 import CatalogUpdate
 from ._models_py3 import CatalogUpdateProperties
+from ._models_py3 import CheckNameAvailabilityRequest
+from ._models_py3 import CheckNameAvailabilityResponse
 from ._models_py3 import CloudErrorBody
 from ._models_py3 import DevBoxDefinition
 from ._models_py3 import DevBoxDefinitionListResult
 from ._models_py3 import DevBoxDefinitionProperties
 from ._models_py3 import DevBoxDefinitionUpdate
 from ._models_py3 import DevBoxDefinitionUpdateProperties
 from ._models_py3 import DevCenter
@@ -28,14 +30,15 @@
 from ._models_py3 import DevCenterUpdate
 from ._models_py3 import EnvironmentRole
 from ._models_py3 import EnvironmentType
 from ._models_py3 import EnvironmentTypeListResult
 from ._models_py3 import EnvironmentTypeUpdate
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDetail
+from ._models_py3 import ErrorResponse
 from ._models_py3 import Gallery
 from ._models_py3 import GalleryListResult
 from ._models_py3 import GitCatalog
 from ._models_py3 import HealthCheck
 from ._models_py3 import HealthCheckStatusDetails
 from ._models_py3 import HealthCheckStatusDetailsListResult
 from ._models_py3 import Image
@@ -89,23 +92,26 @@
 from ._models_py3 import Usage
 from ._models_py3 import UsageName
 from ._models_py3 import UserAssignedIdentity
 from ._models_py3 import UserRoleAssignmentValue
 
 from ._dev_center_mgmt_client_enums import ActionType
 from ._dev_center_mgmt_client_enums import CatalogSyncState
+from ._dev_center_mgmt_client_enums import CheckNameAvailabilityReason
 from ._dev_center_mgmt_client_enums import CreatedByType
 from ._dev_center_mgmt_client_enums import DomainJoinType
 from ._dev_center_mgmt_client_enums import EnableStatus
 from ._dev_center_mgmt_client_enums import HealthCheckStatus
+from ._dev_center_mgmt_client_enums import HibernateSupport
 from ._dev_center_mgmt_client_enums import ImageValidationStatus
 from ._dev_center_mgmt_client_enums import LicenseType
 from ._dev_center_mgmt_client_enums import LocalAdminStatus
 from ._dev_center_mgmt_client_enums import ManagedServiceIdentityType
 from ._dev_center_mgmt_client_enums import Origin
+from ._dev_center_mgmt_client_enums import ProvisioningState
 from ._dev_center_mgmt_client_enums import ScheduledFrequency
 from ._dev_center_mgmt_client_enums import ScheduledType
 from ._dev_center_mgmt_client_enums import SkuTier
 from ._dev_center_mgmt_client_enums import UsageUnit
 from ._patch import __all__ as _patch_all
 from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
@@ -117,14 +123,16 @@
     "AttachedNetworkListResult",
     "Capability",
     "Catalog",
     "CatalogListResult",
     "CatalogProperties",
     "CatalogUpdate",
     "CatalogUpdateProperties",
+    "CheckNameAvailabilityRequest",
+    "CheckNameAvailabilityResponse",
     "CloudErrorBody",
     "DevBoxDefinition",
     "DevBoxDefinitionListResult",
     "DevBoxDefinitionProperties",
     "DevBoxDefinitionUpdate",
     "DevBoxDefinitionUpdateProperties",
     "DevCenter",
@@ -133,14 +141,15 @@
     "DevCenterUpdate",
     "EnvironmentRole",
     "EnvironmentType",
     "EnvironmentTypeListResult",
     "EnvironmentTypeUpdate",
     "ErrorAdditionalInfo",
     "ErrorDetail",
+    "ErrorResponse",
     "Gallery",
     "GalleryListResult",
     "GitCatalog",
     "HealthCheck",
     "HealthCheckStatusDetails",
     "HealthCheckStatusDetailsListResult",
     "Image",
@@ -193,23 +202,26 @@
     "TrackedResourceUpdate",
     "Usage",
     "UsageName",
     "UserAssignedIdentity",
     "UserRoleAssignmentValue",
     "ActionType",
     "CatalogSyncState",
+    "CheckNameAvailabilityReason",
     "CreatedByType",
     "DomainJoinType",
     "EnableStatus",
     "HealthCheckStatus",
+    "HibernateSupport",
     "ImageValidationStatus",
     "LicenseType",
     "LocalAdminStatus",
     "ManagedServiceIdentityType",
     "Origin",
+    "ProvisioningState",
     "ScheduledFrequency",
     "ScheduledType",
     "SkuTier",
     "UsageUnit",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/_models_py3.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/_models_py3.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,19 @@
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.devcenter.models.SystemData
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -140,16 +143,19 @@
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.devcenter.models.SystemData
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     :ivar network_connection_id: The resource ID of the NetworkConnection you want to attach.
     :vartype network_connection_id: str
     :ivar network_connection_location: The geo-location where the NetworkConnection resource
      specified in 'networkConnectionResourceId' property lives.
     :vartype network_connection_location: str
     :ivar health_check_status: Health check status values. Known values are: "Pending", "Running",
      "Passed", "Failed", "Warning", and "Unknown".
@@ -267,16 +273,19 @@
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.devcenter.models.SystemData
     :ivar git_hub: Properties for a GitHub catalog type.
     :vartype git_hub: ~azure.mgmt.devcenter.models.GitCatalog
     :ivar ado_git: Properties for an Azure DevOps catalog type.
     :vartype ado_git: ~azure.mgmt.devcenter.models.GitCatalog
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     :ivar sync_state: The synchronization state of the catalog. Known values are: "Succeeded",
      "InProgress", "Failed", and "Canceled".
     :vartype sync_state: str or ~azure.mgmt.devcenter.models.CatalogSyncState
     :ivar last_sync_time: When the catalog was last synced.
     :vartype last_sync_time: ~datetime.datetime
     """
 
@@ -388,16 +397,19 @@
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar git_hub: Properties for a GitHub catalog type.
     :vartype git_hub: ~azure.mgmt.devcenter.models.GitCatalog
     :ivar ado_git: Properties for an Azure DevOps catalog type.
     :vartype ado_git: ~azure.mgmt.devcenter.models.GitCatalog
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     :ivar sync_state: The synchronization state of the catalog. Known values are: "Succeeded",
      "InProgress", "Failed", and "Canceled".
     :vartype sync_state: str or ~azure.mgmt.devcenter.models.CatalogSyncState
     :ivar last_sync_time: When the catalog was last synced.
     :vartype last_sync_time: ~datetime.datetime
     """
 
@@ -469,14 +481,81 @@
         """
         super().__init__(**kwargs)
         self.tags = tags
         self.git_hub = git_hub
         self.ado_git = ado_git
 
 
+class CheckNameAvailabilityRequest(_serialization.Model):
+    """The check availability request body.
+
+    :ivar name: The name of the resource for which availability needs to be checked.
+    :vartype name: str
+    :ivar type: The resource type.
+    :vartype type: str
+    """
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+    }
+
+    def __init__(self, *, name: Optional[str] = None, type: Optional[str] = None, **kwargs):
+        """
+        :keyword name: The name of the resource for which availability needs to be checked.
+        :paramtype name: str
+        :keyword type: The resource type.
+        :paramtype type: str
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.type = type
+
+
+class CheckNameAvailabilityResponse(_serialization.Model):
+    """The check availability result.
+
+    :ivar name_available: Indicates if the resource name is available.
+    :vartype name_available: bool
+    :ivar reason: The reason why the given name is not available. Known values are: "Invalid" and
+     "AlreadyExists".
+    :vartype reason: str or ~azure.mgmt.devcenter.models.CheckNameAvailabilityReason
+    :ivar message: Detailed reason why the given name is available.
+    :vartype message: str
+    """
+
+    _attribute_map = {
+        "name_available": {"key": "nameAvailable", "type": "bool"},
+        "reason": {"key": "reason", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        name_available: Optional[bool] = None,
+        reason: Optional[Union[str, "_models.CheckNameAvailabilityReason"]] = None,
+        message: Optional[str] = None,
+        **kwargs
+    ):
+        """
+        :keyword name_available: Indicates if the resource name is available.
+        :paramtype name_available: bool
+        :keyword reason: The reason why the given name is not available. Known values are: "Invalid"
+         and "AlreadyExists".
+        :paramtype reason: str or ~azure.mgmt.devcenter.models.CheckNameAvailabilityReason
+        :keyword message: Detailed reason why the given name is available.
+        :paramtype message: str
+        """
+        super().__init__(**kwargs)
+        self.name_available = name_available
+        self.reason = reason
+        self.message = message
+
+
 class CloudErrorBody(_serialization.Model):
     """An error response from the DevCenter service.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar code: An identifier for the error. Codes are invariant and are intended to be consumed
      programmatically. Required.
@@ -610,16 +689,23 @@
     :ivar image_reference: Image reference information.
     :vartype image_reference: ~azure.mgmt.devcenter.models.ImageReference
     :ivar sku: The SKU for Dev Boxes created using this definition.
     :vartype sku: ~azure.mgmt.devcenter.models.Sku
     :ivar os_storage_type: The storage type used for the Operating System disk of Dev Boxes created
      using this definition.
     :vartype os_storage_type: str
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar hibernate_support: Indicates whether Dev Boxes created with this definition are capable
+     of hibernation. Not all images are capable of supporting hibernation. To find out more see
+     https://aka.ms/devbox/hibernate. Known values are: "Disabled" and "Enabled".
+    :vartype hibernate_support: str or ~azure.mgmt.devcenter.models.HibernateSupport
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     :ivar image_validation_status: Validation status of the configured image. Known values are:
      "Unknown", "Pending", "Succeeded", "Failed", and "TimedOut".
     :vartype image_validation_status: str or ~azure.mgmt.devcenter.models.ImageValidationStatus
     :ivar image_validation_error_details: Details for image validator error. Populated when the
      image validation is not successful.
     :vartype image_validation_error_details:
      ~azure.mgmt.devcenter.models.ImageValidationErrorDetails
@@ -646,14 +732,15 @@
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "image_reference": {"key": "properties.imageReference", "type": "ImageReference"},
         "sku": {"key": "properties.sku", "type": "Sku"},
         "os_storage_type": {"key": "properties.osStorageType", "type": "str"},
+        "hibernate_support": {"key": "properties.hibernateSupport", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "image_validation_status": {"key": "properties.imageValidationStatus", "type": "str"},
         "image_validation_error_details": {
             "key": "properties.imageValidationErrorDetails",
             "type": "ImageValidationErrorDetails",
         },
         "active_image_reference": {"key": "properties.activeImageReference", "type": "ImageReference"},
@@ -663,33 +750,39 @@
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
         image_reference: Optional["_models.ImageReference"] = None,
         sku: Optional["_models.Sku"] = None,
         os_storage_type: Optional[str] = None,
+        hibernate_support: Optional[Union[str, "_models.HibernateSupport"]] = None,
         **kwargs
     ):
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword image_reference: Image reference information.
         :paramtype image_reference: ~azure.mgmt.devcenter.models.ImageReference
         :keyword sku: The SKU for Dev Boxes created using this definition.
         :paramtype sku: ~azure.mgmt.devcenter.models.Sku
         :keyword os_storage_type: The storage type used for the Operating System disk of Dev Boxes
          created using this definition.
         :paramtype os_storage_type: str
+        :keyword hibernate_support: Indicates whether Dev Boxes created with this definition are
+         capable of hibernation. Not all images are capable of supporting hibernation. To find out more
+         see https://aka.ms/devbox/hibernate. Known values are: "Disabled" and "Enabled".
+        :paramtype hibernate_support: str or ~azure.mgmt.devcenter.models.HibernateSupport
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.image_reference = image_reference
         self.sku = sku
         self.os_storage_type = os_storage_type
+        self.hibernate_support = hibernate_support
         self.provisioning_state = None
         self.image_validation_status = None
         self.image_validation_error_details = None
         self.active_image_reference = None
 
 
 class DevBoxDefinitionListResult(_serialization.Model):
@@ -726,59 +819,77 @@
     :ivar image_reference: Image reference information.
     :vartype image_reference: ~azure.mgmt.devcenter.models.ImageReference
     :ivar sku: The SKU for Dev Boxes created using this definition.
     :vartype sku: ~azure.mgmt.devcenter.models.Sku
     :ivar os_storage_type: The storage type used for the Operating System disk of Dev Boxes created
      using this definition.
     :vartype os_storage_type: str
+    :ivar hibernate_support: Indicates whether Dev Boxes created with this definition are capable
+     of hibernation. Not all images are capable of supporting hibernation. To find out more see
+     https://aka.ms/devbox/hibernate. Known values are: "Disabled" and "Enabled".
+    :vartype hibernate_support: str or ~azure.mgmt.devcenter.models.HibernateSupport
     """
 
     _attribute_map = {
         "image_reference": {"key": "imageReference", "type": "ImageReference"},
         "sku": {"key": "sku", "type": "Sku"},
         "os_storage_type": {"key": "osStorageType", "type": "str"},
+        "hibernate_support": {"key": "hibernateSupport", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         image_reference: Optional["_models.ImageReference"] = None,
         sku: Optional["_models.Sku"] = None,
         os_storage_type: Optional[str] = None,
+        hibernate_support: Optional[Union[str, "_models.HibernateSupport"]] = None,
         **kwargs
     ):
         """
         :keyword image_reference: Image reference information.
         :paramtype image_reference: ~azure.mgmt.devcenter.models.ImageReference
         :keyword sku: The SKU for Dev Boxes created using this definition.
         :paramtype sku: ~azure.mgmt.devcenter.models.Sku
         :keyword os_storage_type: The storage type used for the Operating System disk of Dev Boxes
          created using this definition.
         :paramtype os_storage_type: str
+        :keyword hibernate_support: Indicates whether Dev Boxes created with this definition are
+         capable of hibernation. Not all images are capable of supporting hibernation. To find out more
+         see https://aka.ms/devbox/hibernate. Known values are: "Disabled" and "Enabled".
+        :paramtype hibernate_support: str or ~azure.mgmt.devcenter.models.HibernateSupport
         """
         super().__init__(**kwargs)
         self.image_reference = image_reference
         self.sku = sku
         self.os_storage_type = os_storage_type
+        self.hibernate_support = hibernate_support
 
 
 class DevBoxDefinitionProperties(DevBoxDefinitionUpdateProperties):
     """Properties of a Dev Box definition.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar image_reference: Image reference information.
     :vartype image_reference: ~azure.mgmt.devcenter.models.ImageReference
     :ivar sku: The SKU for Dev Boxes created using this definition.
     :vartype sku: ~azure.mgmt.devcenter.models.Sku
     :ivar os_storage_type: The storage type used for the Operating System disk of Dev Boxes created
      using this definition.
     :vartype os_storage_type: str
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar hibernate_support: Indicates whether Dev Boxes created with this definition are capable
+     of hibernation. Not all images are capable of supporting hibernation. To find out more see
+     https://aka.ms/devbox/hibernate. Known values are: "Disabled" and "Enabled".
+    :vartype hibernate_support: str or ~azure.mgmt.devcenter.models.HibernateSupport
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     :ivar image_validation_status: Validation status of the configured image. Known values are:
      "Unknown", "Pending", "Succeeded", "Failed", and "TimedOut".
     :vartype image_validation_status: str or ~azure.mgmt.devcenter.models.ImageValidationStatus
     :ivar image_validation_error_details: Details for image validator error. Populated when the
      image validation is not successful.
     :vartype image_validation_error_details:
      ~azure.mgmt.devcenter.models.ImageValidationErrorDetails
@@ -794,38 +905,50 @@
         "active_image_reference": {"readonly": True},
     }
 
     _attribute_map = {
         "image_reference": {"key": "imageReference", "type": "ImageReference"},
         "sku": {"key": "sku", "type": "Sku"},
         "os_storage_type": {"key": "osStorageType", "type": "str"},
+        "hibernate_support": {"key": "hibernateSupport", "type": "str"},
         "provisioning_state": {"key": "provisioningState", "type": "str"},
         "image_validation_status": {"key": "imageValidationStatus", "type": "str"},
         "image_validation_error_details": {"key": "imageValidationErrorDetails", "type": "ImageValidationErrorDetails"},
         "active_image_reference": {"key": "activeImageReference", "type": "ImageReference"},
     }
 
     def __init__(
         self,
         *,
         image_reference: Optional["_models.ImageReference"] = None,
         sku: Optional["_models.Sku"] = None,
         os_storage_type: Optional[str] = None,
+        hibernate_support: Optional[Union[str, "_models.HibernateSupport"]] = None,
         **kwargs
     ):
         """
         :keyword image_reference: Image reference information.
         :paramtype image_reference: ~azure.mgmt.devcenter.models.ImageReference
         :keyword sku: The SKU for Dev Boxes created using this definition.
         :paramtype sku: ~azure.mgmt.devcenter.models.Sku
         :keyword os_storage_type: The storage type used for the Operating System disk of Dev Boxes
          created using this definition.
         :paramtype os_storage_type: str
+        :keyword hibernate_support: Indicates whether Dev Boxes created with this definition are
+         capable of hibernation. Not all images are capable of supporting hibernation. To find out more
+         see https://aka.ms/devbox/hibernate. Known values are: "Disabled" and "Enabled".
+        :paramtype hibernate_support: str or ~azure.mgmt.devcenter.models.HibernateSupport
         """
-        super().__init__(image_reference=image_reference, sku=sku, os_storage_type=os_storage_type, **kwargs)
+        super().__init__(
+            image_reference=image_reference,
+            sku=sku,
+            os_storage_type=os_storage_type,
+            hibernate_support=hibernate_support,
+            **kwargs
+        )
         self.provisioning_state = None
         self.image_validation_status = None
         self.image_validation_error_details = None
         self.active_image_reference = None
 
 
 class TrackedResourceUpdate(_serialization.Model):
@@ -864,51 +987,62 @@
     :ivar image_reference: Image reference information.
     :vartype image_reference: ~azure.mgmt.devcenter.models.ImageReference
     :ivar sku: The SKU for Dev Boxes created using this definition.
     :vartype sku: ~azure.mgmt.devcenter.models.Sku
     :ivar os_storage_type: The storage type used for the Operating System disk of Dev Boxes created
      using this definition.
     :vartype os_storage_type: str
+    :ivar hibernate_support: Indicates whether Dev Boxes created with this definition are capable
+     of hibernation. Not all images are capable of supporting hibernation. To find out more see
+     https://aka.ms/devbox/hibernate. Known values are: "Disabled" and "Enabled".
+    :vartype hibernate_support: str or ~azure.mgmt.devcenter.models.HibernateSupport
     """
 
     _attribute_map = {
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "image_reference": {"key": "properties.imageReference", "type": "ImageReference"},
         "sku": {"key": "properties.sku", "type": "Sku"},
         "os_storage_type": {"key": "properties.osStorageType", "type": "str"},
+        "hibernate_support": {"key": "properties.hibernateSupport", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         tags: Optional[Dict[str, str]] = None,
         location: Optional[str] = None,
         image_reference: Optional["_models.ImageReference"] = None,
         sku: Optional["_models.Sku"] = None,
         os_storage_type: Optional[str] = None,
+        hibernate_support: Optional[Union[str, "_models.HibernateSupport"]] = None,
         **kwargs
     ):
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives.
         :paramtype location: str
         :keyword image_reference: Image reference information.
         :paramtype image_reference: ~azure.mgmt.devcenter.models.ImageReference
         :keyword sku: The SKU for Dev Boxes created using this definition.
         :paramtype sku: ~azure.mgmt.devcenter.models.Sku
         :keyword os_storage_type: The storage type used for the Operating System disk of Dev Boxes
          created using this definition.
         :paramtype os_storage_type: str
+        :keyword hibernate_support: Indicates whether Dev Boxes created with this definition are
+         capable of hibernation. Not all images are capable of supporting hibernation. To find out more
+         see https://aka.ms/devbox/hibernate. Known values are: "Disabled" and "Enabled".
+        :paramtype hibernate_support: str or ~azure.mgmt.devcenter.models.HibernateSupport
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.image_reference = image_reference
         self.sku = sku
         self.os_storage_type = os_storage_type
+        self.hibernate_support = hibernate_support
 
 
 class DevCenter(TrackedResource):
     """Represents a devcenter resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -927,36 +1061,43 @@
     :vartype system_data: ~azure.mgmt.devcenter.models.SystemData
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
     :ivar identity: Managed identity properties.
     :vartype identity: ~azure.mgmt.devcenter.models.ManagedServiceIdentity
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
+    :ivar dev_center_uri: The URI of the resource.
+    :vartype dev_center_uri: str
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
         "location": {"required": True},
         "provisioning_state": {"readonly": True},
+        "dev_center_uri": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "identity": {"key": "identity", "type": "ManagedServiceIdentity"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "dev_center_uri": {"key": "properties.devCenterUri", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
@@ -970,14 +1111,15 @@
         :paramtype location: str
         :keyword identity: Managed identity properties.
         :paramtype identity: ~azure.mgmt.devcenter.models.ManagedServiceIdentity
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.identity = identity
         self.provisioning_state = None
+        self.dev_center_uri = None
 
 
 class DevCenterListResult(_serialization.Model):
     """Result of the list devcenters operation.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -1234,16 +1376,19 @@
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.devcenter.models.SystemData
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -1384,14 +1529,34 @@
         self.code = None
         self.message = None
         self.target = None
         self.details = None
         self.additional_info = None
 
 
+class ErrorResponse(_serialization.Model):
+    """Common error response for all Azure Resource Manager APIs to return error details for failed operations. (This also follows the OData error response format.).
+
+    :ivar error: The error object.
+    :vartype error: ~azure.mgmt.devcenter.models.ErrorDetail
+    """
+
+    _attribute_map = {
+        "error": {"key": "error", "type": "ErrorDetail"},
+    }
+
+    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs):
+        """
+        :keyword error: The error object.
+        :paramtype error: ~azure.mgmt.devcenter.models.ErrorDetail
+        """
+        super().__init__(**kwargs)
+        self.error = error
+
+
 class Gallery(Resource):
     """Represents a gallery.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
@@ -1400,16 +1565,19 @@
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.devcenter.models.SystemData
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     :ivar gallery_resource_id: The resource ID of the backing Azure Compute Gallery.
     :vartype gallery_resource_id: str
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
@@ -1708,16 +1876,19 @@
     :vartype offer: str
     :ivar sku: The SKU name for the image.
     :vartype sku: str
     :ivar recommended_machine_configuration: The recommended machine configuration to use with the
      image.
     :vartype recommended_machine_configuration:
      ~azure.mgmt.devcenter.models.RecommendedMachineConfiguration
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -1890,16 +2061,19 @@
     :ivar published_date: The datetime that the backing image version was published.
     :vartype published_date: ~datetime.datetime
     :ivar exclude_from_latest: If the version should be excluded from being treated as the latest
      version.
     :vartype exclude_from_latest: bool
     :ivar os_disk_image_size_in_gb: The size of the OS disk image, in GB.
     :vartype os_disk_image_size_in_gb: int
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -2081,16 +2255,19 @@
     :vartype organization_unit: str
     :ivar domain_username: The username of an Active Directory account (user or service account)
      that has permissions to create computer objects in Active Directory. Required format:
      admin@contoso.com.
     :vartype domain_username: str
     :ivar domain_password: The password for the account used to join domain.
     :vartype domain_password: str
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     :ivar health_check_status: Overall health status of the network connection. Health checks are
      run on creation, update, and periodically to validate the network connection. Known values are:
      "Pending", "Running", "Passed", "Failed", "Warning", and "Unknown".
     :vartype health_check_status: str or ~azure.mgmt.devcenter.models.HealthCheckStatus
     :ivar networking_resource_group_name: The name for resource group where NICs will be placed.
     :vartype networking_resource_group_name: str
     :ivar domain_join_type: AAD Join type. Known values are: "HybridAzureADJoin" and "AzureADJoin".
@@ -2343,16 +2520,19 @@
     :vartype organization_unit: str
     :ivar domain_username: The username of an Active Directory account (user or service account)
      that has permissions to create computer objects in Active Directory. Required format:
      admin@contoso.com.
     :vartype domain_username: str
     :ivar domain_password: The password for the account used to join domain.
     :vartype domain_password: str
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     :ivar health_check_status: Overall health status of the network connection. Health checks are
      run on creation, update, and periodically to validate the network connection. Known values are:
      "Pending", "Running", "Passed", "Failed", "Warning", and "Unknown".
     :vartype health_check_status: str or ~azure.mgmt.devcenter.models.HealthCheckStatus
     :ivar networking_resource_group_name: The name for resource group where NICs will be placed.
     :vartype networking_resource_group_name: str
     :ivar domain_join_type: AAD Join type. Required. Known values are: "HybridAzureADJoin" and
@@ -2747,16 +2927,19 @@
     :vartype network_connection_name: str
     :ivar license_type: Specifies the license type indicating the caller has already acquired
      licenses for the Dev Boxes that will be created. "Windows_Client"
     :vartype license_type: str or ~azure.mgmt.devcenter.models.LicenseType
     :ivar local_administrator: Indicates whether owners of Dev Boxes in this pool are added as
      local administrators on the Dev Box. Known values are: "Disabled" and "Enabled".
     :vartype local_administrator: str or ~azure.mgmt.devcenter.models.LocalAdminStatus
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -2902,16 +3085,19 @@
     :vartype network_connection_name: str
     :ivar license_type: Specifies the license type indicating the caller has already acquired
      licenses for the Dev Boxes that will be created. "Windows_Client"
     :vartype license_type: str or ~azure.mgmt.devcenter.models.LicenseType
     :ivar local_administrator: Indicates whether owners of Dev Boxes in this pool are added as
      local administrators on the Dev Box. Known values are: "Disabled" and "Enabled".
     :vartype local_administrator: str or ~azure.mgmt.devcenter.models.LocalAdminStatus
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "provisioning_state": {"readonly": True},
     }
 
     _attribute_map = {
@@ -3037,37 +3223,44 @@
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
     :ivar dev_center_id: Resource Id of an associated DevCenter.
     :vartype dev_center_id: str
     :ivar description: Description of the project.
     :vartype description: str
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
+    :ivar dev_center_uri: The URI of the resource.
+    :vartype dev_center_uri: str
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
         "location": {"required": True},
         "provisioning_state": {"readonly": True},
+        "dev_center_uri": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "dev_center_id": {"key": "properties.devCenterId", "type": "str"},
         "description": {"key": "properties.description", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "dev_center_uri": {"key": "properties.devCenterUri", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
@@ -3085,14 +3278,15 @@
         :keyword description: Description of the project.
         :paramtype description: str
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.dev_center_id = dev_center_id
         self.description = description
         self.provisioning_state = None
+        self.dev_center_uri = None
 
 
 class ProjectEnvironmentType(Resource):  # pylint: disable=too-many-instance-attributes
     """Represents an environment type.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -3122,16 +3316,19 @@
     :ivar creator_role_assignment: The role definition assigned to the environment creator on
      backing resources.
     :vartype creator_role_assignment:
      ~azure.mgmt.devcenter.models.ProjectEnvironmentTypeUpdatePropertiesCreatorRoleAssignment
     :ivar user_role_assignments: Role Assignments created on environment backing resources. This is
      a mapping from a user object ID to an object of role definition IDs.
     :vartype user_role_assignments: dict[str, ~azure.mgmt.devcenter.models.UserRoleAssignmentValue]
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -3303,16 +3500,19 @@
     :ivar creator_role_assignment: The role definition assigned to the environment creator on
      backing resources.
     :vartype creator_role_assignment:
      ~azure.mgmt.devcenter.models.ProjectEnvironmentTypeUpdatePropertiesCreatorRoleAssignment
     :ivar user_role_assignments: Role Assignments created on environment backing resources. This is
      a mapping from a user object ID to an object of role definition IDs.
     :vartype user_role_assignments: dict[str, ~azure.mgmt.devcenter.models.UserRoleAssignmentValue]
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "provisioning_state": {"readonly": True},
     }
 
     _attribute_map = {
@@ -3514,37 +3714,45 @@
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar dev_center_id: Resource Id of an associated DevCenter.
     :vartype dev_center_id: str
     :ivar description: Description of the project.
     :vartype description: str
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
+    :ivar dev_center_uri: The URI of the resource.
+    :vartype dev_center_uri: str
     """
 
     _validation = {
         "provisioning_state": {"readonly": True},
+        "dev_center_uri": {"readonly": True},
     }
 
     _attribute_map = {
         "dev_center_id": {"key": "devCenterId", "type": "str"},
         "description": {"key": "description", "type": "str"},
         "provisioning_state": {"key": "provisioningState", "type": "str"},
+        "dev_center_uri": {"key": "devCenterUri", "type": "str"},
     }
 
     def __init__(self, *, dev_center_id: Optional[str] = None, description: Optional[str] = None, **kwargs):
         """
         :keyword dev_center_id: Resource Id of an associated DevCenter.
         :paramtype dev_center_id: str
         :keyword description: Description of the project.
         :paramtype description: str
         """
         super().__init__(dev_center_id=dev_center_id, description=description, **kwargs)
         self.provisioning_state = None
+        self.dev_center_uri = None
 
 
 class ProjectUpdate(TrackedResourceUpdate):
     """The project properties for partial update. Properties not provided in the update request will not be changed.
 
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
@@ -3666,16 +3874,19 @@
     :ivar time: The target time to trigger the action. The format is HH:MM.
     :vartype time: str
     :ivar time_zone: The IANA timezone id at which the schedule should execute.
     :vartype time_zone: str
     :ivar state: Indicates whether or not this scheduled task is enabled. Known values are:
      "Enabled" and "Disabled".
     :vartype state: str or ~azure.mgmt.devcenter.models.EnableStatus
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -3822,16 +4033,19 @@
     :ivar time: The target time to trigger the action. The format is HH:MM.
     :vartype time: str
     :ivar time_zone: The IANA timezone id at which the schedule should execute.
     :vartype time_zone: str
     :ivar state: Indicates whether or not this scheduled task is enabled. Known values are:
      "Enabled" and "Disabled".
     :vartype state: str or ~azure.mgmt.devcenter.models.EnableStatus
-    :ivar provisioning_state: The provisioning state of the resource.
-    :vartype provisioning_state: str
+    :ivar provisioning_state: The provisioning state of the resource. Known values are:
+     "NotSpecified", "Accepted", "Running", "Creating", "Created", "Updating", "Updated",
+     "Deleting", "Deleted", "Succeeded", "Failed", "Canceled", "MovingResources",
+     "TransientFailure", "RolloutInProgress", and "StorageProvisioningFailed".
+    :vartype provisioning_state: str or ~azure.mgmt.devcenter.models.ProvisioningState
     """
 
     _validation = {
         "provisioning_state": {"readonly": True},
     }
 
     _attribute_map = {
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/models/_patch.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/__init__.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from ._environment_types_operations import EnvironmentTypesOperations
 from ._project_allowed_environment_types_operations import ProjectAllowedEnvironmentTypesOperations
 from ._project_environment_types_operations import ProjectEnvironmentTypesOperations
 from ._dev_box_definitions_operations import DevBoxDefinitionsOperations
 from ._operations import Operations
 from ._operation_statuses_operations import OperationStatusesOperations
 from ._usages_operations import UsagesOperations
+from ._check_name_availability_operations import CheckNameAvailabilityOperations
 from ._skus_operations import SkusOperations
 from ._pools_operations import PoolsOperations
 from ._schedules_operations import SchedulesOperations
 from ._network_connections_operations import NetworkConnectionsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
@@ -40,14 +41,15 @@
     "EnvironmentTypesOperations",
     "ProjectAllowedEnvironmentTypesOperations",
     "ProjectEnvironmentTypesOperations",
     "DevBoxDefinitionsOperations",
     "Operations",
     "OperationStatusesOperations",
     "UsagesOperations",
+    "CheckNameAvailabilityOperations",
     "SkusOperations",
     "PoolsOperations",
     "SchedulesOperations",
     "NetworkConnectionsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_usages_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_usages_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
 
 def build_list_by_location_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.DevCenter/locations/{location}/usages"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -101,15 +101,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ListUsagesResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_image_versions_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_image_versions_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/galleries/{galleryName}/images/{imageName}/versions",
     )  # pylint: disable=line-too-long
@@ -92,16 +92,16 @@
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/galleries/{galleryName}/images/{imageName}/versions/{versionName}",
     )  # pylint: disable=line-too-long
@@ -167,15 +167,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ImageVersionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -279,15 +279,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ImageVersion]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             gallery_name=gallery_name,
             image_name=image_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_catalogs_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_catalogs_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 def build_list_by_dev_center_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/catalogs",
     )  # pylint: disable=line-too-long
@@ -83,16 +83,16 @@
 def build_get_request(
     resource_group_name: str, dev_center_name: str, catalog_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/catalogs/{catalogName}",
     )  # pylint: disable=line-too-long
@@ -119,16 +119,16 @@
 def build_create_or_update_request(
     resource_group_name: str, dev_center_name: str, catalog_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/catalogs/{catalogName}",
@@ -158,16 +158,16 @@
 def build_update_request(
     resource_group_name: str, dev_center_name: str, catalog_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/catalogs/{catalogName}",
@@ -197,16 +197,16 @@
 def build_delete_request(
     resource_group_name: str, dev_center_name: str, catalog_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/catalogs/{catalogName}",
     )  # pylint: disable=line-too-long
@@ -233,16 +233,16 @@
 def build_sync_request(
     resource_group_name: str, dev_center_name: str, catalog_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/catalogs/{catalogName}/sync",
     )  # pylint: disable=line-too-long
@@ -305,15 +305,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.CatalogListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -404,15 +404,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Catalog]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             catalog_name=catalog_name,
             subscription_id=self._config.subscription_id,
@@ -460,15 +460,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Catalog]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -623,15 +623,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Catalog]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(  # type: ignore
@@ -690,15 +690,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Catalog]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -855,15 +855,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Catalog]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(  # type: ignore
@@ -917,15 +917,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             catalog_name=catalog_name,
             subscription_id=self._config.subscription_id,
@@ -978,15 +978,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1035,15 +1035,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_sync_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             catalog_name=catalog_name,
             subscription_id=self._config.subscription_id,
@@ -1096,15 +1096,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._sync_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_patch.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_project_allowed_environment_types_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_project_allowed_environment_types_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 def build_list_request(
     resource_group_name: str, project_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/allowedEnvironmentTypes",
     )  # pylint: disable=line-too-long
@@ -81,16 +81,16 @@
 def build_get_request(
     resource_group_name: str, project_name: str, environment_type_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/allowedEnvironmentTypes/{environmentTypeName}",
     )  # pylint: disable=line-too-long
@@ -154,15 +154,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AllowedEnvironmentTypeListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -255,15 +255,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AllowedEnvironmentType]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_project_environment_types_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_project_environment_types_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 def build_list_request(
     resource_group_name: str, project_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/environmentTypes",
     )  # pylint: disable=line-too-long
@@ -81,16 +81,16 @@
 def build_get_request(
     resource_group_name: str, project_name: str, environment_type_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/environmentTypes/{environmentTypeName}",
     )  # pylint: disable=line-too-long
@@ -117,16 +117,16 @@
 def build_create_or_update_request(
     resource_group_name: str, project_name: str, environment_type_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/environmentTypes/{environmentTypeName}",
@@ -156,16 +156,16 @@
 def build_update_request(
     resource_group_name: str, project_name: str, environment_type_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/environmentTypes/{environmentTypeName}",
@@ -195,16 +195,16 @@
 def build_delete_request(
     resource_group_name: str, project_name: str, environment_type_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/environmentTypes/{environmentTypeName}",
     )  # pylint: disable=line-too-long
@@ -268,15 +268,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectEnvironmentTypeListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -369,15 +369,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectEnvironmentType]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
@@ -508,15 +508,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectEnvironmentType]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -659,15 +659,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectEnvironmentType]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -737,15 +737,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_dev_centers_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_dev_centers_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 def build_list_by_subscription_request(
     subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.DevCenter/devcenters")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -76,16 +76,16 @@
 def build_list_by_resource_group_request(
     resource_group_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters",
     )  # pylint: disable=line-too-long
@@ -112,16 +112,16 @@
 def build_get_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}",
     )  # pylint: disable=line-too-long
@@ -147,16 +147,16 @@
 def build_create_or_update_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}",
@@ -185,16 +185,16 @@
 def build_update_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}",
@@ -223,16 +223,16 @@
 def build_delete_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}",
     )  # pylint: disable=line-too-long
@@ -287,15 +287,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenterListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -377,15 +377,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenterListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -473,15 +473,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenter]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -523,15 +523,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenter]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -676,15 +676,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenter]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(  # type: ignore
@@ -737,15 +737,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.DevCenter]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -888,15 +888,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenter]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(  # type: ignore
@@ -949,15 +949,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -1005,15 +1005,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_images_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_images_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 def build_list_by_dev_center_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/images",
     )  # pylint: disable=line-too-long
@@ -87,16 +87,16 @@
     top: Optional[int] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/galleries/{galleryName}/images",
     )  # pylint: disable=line-too-long
@@ -130,16 +130,16 @@
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/galleries/{galleryName}/images/{imageName}",
     )  # pylint: disable=line-too-long
@@ -203,15 +203,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ImageListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -304,15 +304,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ImageListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -408,15 +408,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Image]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             gallery_name=gallery_name,
             image_name=image_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_dev_box_definitions_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_dev_box_definitions_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 def build_list_by_dev_center_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/devboxdefinitions",
     )  # pylint: disable=line-too-long
@@ -83,16 +83,16 @@
 def build_get_request(
     resource_group_name: str, dev_center_name: str, dev_box_definition_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/devboxdefinitions/{devBoxDefinitionName}",
     )  # pylint: disable=line-too-long
@@ -119,16 +119,16 @@
 def build_create_or_update_request(
     resource_group_name: str, dev_center_name: str, dev_box_definition_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/devboxdefinitions/{devBoxDefinitionName}",
@@ -158,16 +158,16 @@
 def build_update_request(
     resource_group_name: str, dev_center_name: str, dev_box_definition_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/devboxdefinitions/{devBoxDefinitionName}",
@@ -197,16 +197,16 @@
 def build_delete_request(
     resource_group_name: str, dev_center_name: str, dev_box_definition_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/devboxdefinitions/{devBoxDefinitionName}",
     )  # pylint: disable=line-too-long
@@ -233,16 +233,16 @@
 def build_list_by_project_request(
     resource_group_name: str, project_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/devboxdefinitions",
     )  # pylint: disable=line-too-long
@@ -270,16 +270,16 @@
 def build_get_by_project_request(
     resource_group_name: str, project_name: str, dev_box_definition_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/devboxdefinitions/{devBoxDefinitionName}",
     )  # pylint: disable=line-too-long
@@ -342,15 +342,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinitionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -443,15 +443,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             dev_box_definition_name=dev_box_definition_name,
             subscription_id=self._config.subscription_id,
@@ -499,15 +499,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -669,15 +669,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(  # type: ignore
@@ -736,15 +736,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.DevBoxDefinition]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -904,15 +904,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(  # type: ignore
@@ -966,15 +966,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             dev_box_definition_name=dev_box_definition_name,
             subscription_id=self._config.subscription_id,
@@ -1027,15 +1027,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1092,15 +1092,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinitionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1193,15 +1193,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
 
         request = build_get_by_project_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             dev_box_definition_name=dev_box_definition_name,
             subscription_id=self._config.subscription_id,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_attached_networks_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_attached_networks_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 def build_list_by_project_request(
     resource_group_name: str, project_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/attachednetworks",
     )  # pylint: disable=line-too-long
@@ -87,16 +87,16 @@
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/attachednetworks/{attachedNetworkConnectionName}",
     )  # pylint: disable=line-too-long
@@ -125,16 +125,16 @@
 def build_list_by_dev_center_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/attachednetworks",
     )  # pylint: disable=line-too-long
@@ -166,16 +166,16 @@
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/attachednetworks/{attachedNetworkConnectionName}",
     )  # pylint: disable=line-too-long
@@ -208,16 +208,16 @@
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/attachednetworks/{attachedNetworkConnectionName}",
@@ -253,16 +253,16 @@
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/attachednetworks/{attachedNetworkConnectionName}",
     )  # pylint: disable=line-too-long
@@ -328,15 +328,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -429,15 +429,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkConnection]
 
         request = build_get_by_project_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             attached_network_connection_name=attached_network_connection_name,
             subscription_id=self._config.subscription_id,
@@ -489,15 +489,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -590,15 +590,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkConnection]
 
         request = build_get_by_dev_center_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             attached_network_connection_name=attached_network_connection_name,
             subscription_id=self._config.subscription_id,
@@ -646,15 +646,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkConnection]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -813,15 +813,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkConnection]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(  # type: ignore
@@ -875,15 +875,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             attached_network_connection_name=attached_network_connection_name,
             subscription_id=self._config.subscription_id,
@@ -936,15 +936,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_operation_statuses_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_operation_statuses_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 
 def build_get_request(location: str, operation_id: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.DevCenter/locations/{location}/operationStatuses/{operationId}",
     )  # pylint: disable=line-too-long
@@ -113,15 +113,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.OperationStatus]
 
         request = build_get_request(
             location=location,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_environment_types_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_environment_types_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 def build_list_by_dev_center_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/environmentTypes",
     )  # pylint: disable=line-too-long
@@ -81,16 +81,16 @@
 def build_get_request(
     resource_group_name: str, dev_center_name: str, environment_type_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/environmentTypes/{environmentTypeName}",
     )  # pylint: disable=line-too-long
@@ -117,16 +117,16 @@
 def build_create_or_update_request(
     resource_group_name: str, dev_center_name: str, environment_type_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/environmentTypes/{environmentTypeName}",
@@ -156,16 +156,16 @@
 def build_update_request(
     resource_group_name: str, dev_center_name: str, environment_type_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/environmentTypes/{environmentTypeName}",
@@ -195,16 +195,16 @@
 def build_delete_request(
     resource_group_name: str, dev_center_name: str, environment_type_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/environmentTypes/{environmentTypeName}",
     )  # pylint: disable=line-too-long
@@ -267,15 +267,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.EnvironmentTypeListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -368,15 +368,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.EnvironmentType]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
@@ -506,15 +506,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.EnvironmentType]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -657,15 +657,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.EnvironmentType]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -735,15 +735,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_projects_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_projects_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 def build_list_by_subscription_request(
     subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.DevCenter/projects")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -76,16 +76,16 @@
 def build_list_by_resource_group_request(
     resource_group_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects",
     )  # pylint: disable=line-too-long
@@ -110,16 +110,16 @@
 
 
 def build_get_request(resource_group_name: str, project_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}",
     )  # pylint: disable=line-too-long
@@ -145,16 +145,16 @@
 def build_create_or_update_request(
     resource_group_name: str, project_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}",
@@ -183,16 +183,16 @@
 def build_update_request(
     resource_group_name: str, project_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}",
@@ -221,16 +221,16 @@
 def build_delete_request(
     resource_group_name: str, project_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}",
     )  # pylint: disable=line-too-long
@@ -285,15 +285,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -375,15 +375,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -471,15 +471,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Project]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -521,15 +521,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Project]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -674,15 +674,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Project]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(  # type: ignore
@@ -735,15 +735,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Project]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -886,15 +886,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Project]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(  # type: ignore
@@ -947,15 +947,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -1003,15 +1003,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_skus_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_skus_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 def build_list_by_subscription_request(
     subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.DevCenter/skus")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -103,15 +103,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.SkuListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_schedules_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_schedules_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     top: Optional[int] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools/{poolName}/schedules",
     )  # pylint: disable=line-too-long
@@ -97,16 +97,16 @@
     top: Optional[int] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools/{poolName}/schedules/{scheduleName}",
     )  # pylint: disable=line-too-long
@@ -145,16 +145,16 @@
     top: Optional[int] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools/{poolName}/schedules/{scheduleName}",
@@ -196,16 +196,16 @@
     top: Optional[int] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools/{poolName}/schedules/{scheduleName}",
@@ -247,16 +247,16 @@
     top: Optional[int] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools/{poolName}/schedules/{scheduleName}",
     )  # pylint: disable=line-too-long
@@ -326,15 +326,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ScheduleListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -439,15 +439,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Schedule]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             pool_name=pool_name,
             schedule_name=schedule_name,
@@ -499,15 +499,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Schedule]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -689,15 +689,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Schedule]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(  # type: ignore
@@ -760,15 +760,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Schedule]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -948,15 +948,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Schedule]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(  # type: ignore
@@ -1018,15 +1018,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             pool_name=pool_name,
             schedule_name=schedule_name,
@@ -1092,15 +1092,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.DevCenter/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -91,15 +91,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.OperationListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_network_connections_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_network_connections_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 def build_list_by_subscription_request(
     subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.DevCenter/networkConnections"
     )
     path_format_arguments = {
@@ -78,16 +78,16 @@
 def build_list_by_resource_group_request(
     resource_group_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections",
     )  # pylint: disable=line-too-long
@@ -114,16 +114,16 @@
 def build_get_request(
     resource_group_name: str, network_connection_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}",
     )  # pylint: disable=line-too-long
@@ -149,16 +149,16 @@
 def build_create_or_update_request(
     resource_group_name: str, network_connection_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}",
@@ -187,16 +187,16 @@
 def build_update_request(
     resource_group_name: str, network_connection_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}",
@@ -225,16 +225,16 @@
 def build_delete_request(
     resource_group_name: str, network_connection_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}",
     )  # pylint: disable=line-too-long
@@ -265,16 +265,16 @@
     top: Optional[int] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/healthChecks",
     )  # pylint: disable=line-too-long
@@ -302,16 +302,16 @@
 def build_get_health_details_request(
     resource_group_name: str, network_connection_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/healthChecks/latest",
     )  # pylint: disable=line-too-long
@@ -337,16 +337,16 @@
 def build_run_health_checks_request(
     resource_group_name: str, network_connection_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/runHealthChecks",
     )  # pylint: disable=line-too-long
@@ -401,15 +401,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnectionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -491,15 +491,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnectionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -588,15 +588,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnection]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             network_connection_name=network_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -642,15 +642,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnection]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -805,15 +805,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnection]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(  # type: ignore
@@ -870,15 +870,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.NetworkConnection]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -1031,15 +1031,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnection]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(  # type: ignore
@@ -1092,15 +1092,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             network_connection_name=network_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -1149,15 +1149,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1215,15 +1215,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.HealthCheckStatusDetailsListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1315,15 +1315,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.HealthCheckStatusDetails]
 
         request = build_get_health_details_request(
             resource_group_name=resource_group_name,
             network_connection_name=network_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -1349,67 +1349,122 @@
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get_health_details.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/healthChecks/latest"}  # type: ignore
 
-    @distributed_trace
-    def run_health_checks(  # pylint: disable=inconsistent-return-statements
+    def _run_health_checks_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, network_connection_name: str, **kwargs: Any
     ) -> None:
-        """Triggers a new health check run. The execution and health check result can be tracked via the
-        network Connection health check details.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param network_connection_name: Name of the Network Connection that can be applied to a Pool.
-         Required.
-        :type network_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_run_health_checks_request(
             resource_group_name=resource_group_name,
             network_connection_name=network_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.run_health_checks.metadata["url"],
+            template_url=self._run_health_checks_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)  # type: ignore
 
         pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    run_health_checks.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/runHealthChecks"}  # type: ignore
+    _run_health_checks_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/runHealthChecks"}  # type: ignore
+
+    @distributed_trace
+    def begin_run_health_checks(
+        self, resource_group_name: str, network_connection_name: str, **kwargs: Any
+    ) -> LROPoller[None]:
+        """Triggers a new health check run. The execution and health check result can be tracked via the
+        network Connection health check details.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param network_connection_name: Name of the Network Connection that can be applied to a Pool.
+         Required.
+        :type network_connection_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-11-11-preview"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        if cont_token is None:
+            raw_result = self._run_health_checks_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                network_connection_name=network_connection_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})
+
+        if polling is True:
+            polling_method = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )  # type: PollingMethod
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
+    begin_run_health_checks.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/runHealthChecks"}  # type: ignore
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_galleries_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_galleries_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 def build_list_by_dev_center_request(
     resource_group_name: str, dev_center_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/galleries",
     )  # pylint: disable=line-too-long
@@ -83,16 +83,16 @@
 def build_get_request(
     resource_group_name: str, dev_center_name: str, gallery_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/galleries/{galleryName}",
     )  # pylint: disable=line-too-long
@@ -119,16 +119,16 @@
 def build_create_or_update_request(
     resource_group_name: str, dev_center_name: str, gallery_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/galleries/{galleryName}",
@@ -158,16 +158,16 @@
 def build_delete_request(
     resource_group_name: str, dev_center_name: str, gallery_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/devcenters/{devCenterName}/galleries/{galleryName}",
     )  # pylint: disable=line-too-long
@@ -230,15 +230,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.GalleryListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -329,15 +329,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Gallery]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             gallery_name=gallery_name,
             subscription_id=self._config.subscription_id,
@@ -385,15 +385,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Gallery]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -548,15 +548,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Gallery]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(  # type: ignore
@@ -610,15 +610,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             gallery_name=gallery_name,
             subscription_id=self._config.subscription_id,
@@ -671,15 +671,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/operations/_pools_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/operations/_pools_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 def build_list_by_project_request(
     resource_group_name: str, project_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools",
     )  # pylint: disable=line-too-long
@@ -83,16 +83,16 @@
 def build_get_request(
     resource_group_name: str, project_name: str, pool_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools/{poolName}",
     )  # pylint: disable=line-too-long
@@ -119,16 +119,16 @@
 def build_create_or_update_request(
     resource_group_name: str, project_name: str, pool_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools/{poolName}",
@@ -158,16 +158,16 @@
 def build_update_request(
     resource_group_name: str, project_name: str, pool_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools/{poolName}",
@@ -197,16 +197,16 @@
 def build_delete_request(
     resource_group_name: str, project_name: str, pool_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-10-12-preview")
-    )  # type: Literal["2022-10-12-preview"]
+        "api_version", _params.pop("api-version", "2022-11-11-preview")
+    )  # type: Literal["2022-11-11-preview"]
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/projects/{projectName}/pools/{poolName}",
     )  # pylint: disable=line-too-long
@@ -269,15 +269,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.PoolListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -368,15 +368,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Pool]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             pool_name=pool_name,
             subscription_id=self._config.subscription_id,
@@ -419,15 +419,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Pool]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -581,15 +581,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Pool]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(  # type: ignore
@@ -648,15 +648,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Pool]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -813,15 +813,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Pool]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(  # type: ignore
@@ -875,15 +875,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             pool_name=pool_name,
             subscription_id=self._config.subscription_id,
@@ -936,15 +936,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/__init__.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/_dev_center_mgmt_client.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/_dev_center_mgmt_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from .. import models
 from .._serialization import Deserializer, Serializer
 from ._configuration import DevCenterMgmtClientConfiguration
 from .operations import (
     AttachedNetworksOperations,
     CatalogsOperations,
+    CheckNameAvailabilityOperations,
     DevBoxDefinitionsOperations,
     DevCentersOperations,
     EnvironmentTypesOperations,
     GalleriesOperations,
     ImageVersionsOperations,
     ImagesOperations,
     NetworkConnectionsOperations,
@@ -70,29 +71,32 @@
     :vartype dev_box_definitions: azure.mgmt.devcenter.aio.operations.DevBoxDefinitionsOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.devcenter.aio.operations.Operations
     :ivar operation_statuses: OperationStatusesOperations operations
     :vartype operation_statuses: azure.mgmt.devcenter.aio.operations.OperationStatusesOperations
     :ivar usages: UsagesOperations operations
     :vartype usages: azure.mgmt.devcenter.aio.operations.UsagesOperations
+    :ivar check_name_availability: CheckNameAvailabilityOperations operations
+    :vartype check_name_availability:
+     azure.mgmt.devcenter.aio.operations.CheckNameAvailabilityOperations
     :ivar skus: SkusOperations operations
     :vartype skus: azure.mgmt.devcenter.aio.operations.SkusOperations
     :ivar pools: PoolsOperations operations
     :vartype pools: azure.mgmt.devcenter.aio.operations.PoolsOperations
     :ivar schedules: SchedulesOperations operations
     :vartype schedules: azure.mgmt.devcenter.aio.operations.SchedulesOperations
     :ivar network_connections: NetworkConnectionsOperations operations
     :vartype network_connections: azure.mgmt.devcenter.aio.operations.NetworkConnectionsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-10-12-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-11-11-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -133,14 +137,17 @@
             self._client, self._config, self._serialize, self._deserialize
         )
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.operation_statuses = OperationStatusesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.usages = UsagesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.check_name_availability = CheckNameAvailabilityOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.pools = PoolsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.schedules = SchedulesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.network_connections = NetworkConnectionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/_patch.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/_configuration.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-10-12-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-11-11-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(DevCenterMgmtClientConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-10-12-preview")  # type: Literal["2022-10-12-preview"]
+        api_version = kwargs.pop("api_version", "2022-11-11-preview")  # type: Literal["2022-11-11-preview"]
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/__init__.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from ._environment_types_operations import EnvironmentTypesOperations
 from ._project_allowed_environment_types_operations import ProjectAllowedEnvironmentTypesOperations
 from ._project_environment_types_operations import ProjectEnvironmentTypesOperations
 from ._dev_box_definitions_operations import DevBoxDefinitionsOperations
 from ._operations import Operations
 from ._operation_statuses_operations import OperationStatusesOperations
 from ._usages_operations import UsagesOperations
+from ._check_name_availability_operations import CheckNameAvailabilityOperations
 from ._skus_operations import SkusOperations
 from ._pools_operations import PoolsOperations
 from ._schedules_operations import SchedulesOperations
 from ._network_connections_operations import NetworkConnectionsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
@@ -40,14 +41,15 @@
     "EnvironmentTypesOperations",
     "ProjectAllowedEnvironmentTypesOperations",
     "ProjectEnvironmentTypesOperations",
     "DevBoxDefinitionsOperations",
     "Operations",
     "OperationStatusesOperations",
     "UsagesOperations",
+    "CheckNameAvailabilityOperations",
     "SkusOperations",
     "PoolsOperations",
     "SchedulesOperations",
     "NetworkConnectionsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_usages_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_usages_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ListUsagesResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_image_versions_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_image_versions_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ImageVersionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -191,15 +191,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ImageVersion]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             gallery_name=gallery_name,
             image_name=image_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_catalogs_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_catalogs_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.CatalogListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -188,15 +188,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Catalog]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             catalog_name=catalog_name,
             subscription_id=self._config.subscription_id,
@@ -244,15 +244,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Catalog]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -410,15 +410,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Catalog]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(  # type: ignore
@@ -478,15 +478,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Catalog]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -646,15 +646,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Catalog]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(  # type: ignore
@@ -709,15 +709,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             catalog_name=catalog_name,
             subscription_id=self._config.subscription_id,
@@ -770,15 +770,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -828,15 +828,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_sync_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             catalog_name=catalog_name,
             subscription_id=self._config.subscription_id,
@@ -889,15 +889,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._sync_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_patch.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_project_allowed_environment_types_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_project_allowed_environment_types_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AllowedEnvironmentTypeListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -181,15 +181,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AllowedEnvironmentType]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_project_environment_types_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_project_environment_types_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectEnvironmentTypeListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -187,15 +187,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectEnvironmentType]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
@@ -326,15 +326,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectEnvironmentType]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -477,15 +477,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectEnvironmentType]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -555,15 +555,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_dev_centers_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_dev_centers_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenterListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -170,15 +170,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenterListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -266,15 +266,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenter]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -316,15 +316,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenter]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -472,15 +472,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenter]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(  # type: ignore
@@ -534,15 +534,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.DevCenter]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -688,15 +688,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevCenter]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(  # type: ignore
@@ -750,15 +750,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -806,15 +806,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_images_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_images_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ImageListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -183,15 +183,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ImageListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -287,15 +287,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Image]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             gallery_name=gallery_name,
             image_name=image_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_dev_box_definitions_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_dev_box_definitions_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinitionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -189,15 +189,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             dev_box_definition_name=dev_box_definition_name,
             subscription_id=self._config.subscription_id,
@@ -245,15 +245,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -415,15 +415,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(  # type: ignore
@@ -483,15 +483,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.DevBoxDefinition]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -651,15 +651,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(  # type: ignore
@@ -714,15 +714,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             dev_box_definition_name=dev_box_definition_name,
             subscription_id=self._config.subscription_id,
@@ -775,15 +775,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -841,15 +841,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinitionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -942,15 +942,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.DevBoxDefinition]
 
         request = build_get_by_project_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             dev_box_definition_name=dev_box_definition_name,
             subscription_id=self._config.subscription_id,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_attached_networks_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_attached_networks_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -190,15 +190,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkConnection]
 
         request = build_get_by_project_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             attached_network_connection_name=attached_network_connection_name,
             subscription_id=self._config.subscription_id,
@@ -251,15 +251,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -352,15 +352,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkConnection]
 
         request = build_get_by_dev_center_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             attached_network_connection_name=attached_network_connection_name,
             subscription_id=self._config.subscription_id,
@@ -408,15 +408,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkConnection]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -578,15 +578,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.AttachedNetworkConnection]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(  # type: ignore
@@ -641,15 +641,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             attached_network_connection_name=attached_network_connection_name,
             subscription_id=self._config.subscription_id,
@@ -702,15 +702,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_operation_statuses_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_operation_statuses_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.OperationStatus]
 
         request = build_get_request(
             location=location,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_environment_types_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_environment_types_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.EnvironmentTypeListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -185,15 +185,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.EnvironmentType]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
@@ -323,15 +323,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.EnvironmentType]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -474,15 +474,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.EnvironmentType]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -552,15 +552,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             environment_type_name=environment_type_name,
             subscription_id=self._config.subscription_id,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_projects_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_projects_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -170,15 +170,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProjectListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -266,15 +266,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Project]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -316,15 +316,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Project]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -472,15 +472,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Project]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(  # type: ignore
@@ -534,15 +534,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Project]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -688,15 +688,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Project]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(  # type: ignore
@@ -750,15 +750,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -806,15 +806,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_skus_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_skus_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.SkuListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_schedules_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_schedules_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.ScheduleListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -201,15 +201,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Schedule]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             pool_name=pool_name,
             schedule_name=schedule_name,
@@ -261,15 +261,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Schedule]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -454,15 +454,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Schedule]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(  # type: ignore
@@ -526,15 +526,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Schedule]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -717,15 +717,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Schedule]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(  # type: ignore
@@ -788,15 +788,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             pool_name=pool_name,
             schedule_name=schedule_name,
@@ -862,15 +862,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.OperationListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_network_connections_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_network_connections_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnectionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -175,15 +175,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnectionListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -274,15 +274,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnection]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             network_connection_name=network_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -328,15 +328,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnection]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -491,15 +491,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnection]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(  # type: ignore
@@ -557,15 +557,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.NetworkConnection]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -718,15 +718,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.NetworkConnection]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(  # type: ignore
@@ -780,15 +780,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             network_connection_name=network_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -839,15 +839,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -907,15 +907,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.HealthCheckStatusDetailsListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1007,15 +1007,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.HealthCheckStatusDetails]
 
         request = build_get_health_details_request(
             resource_group_name=resource_group_name,
             network_connection_name=network_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -1041,67 +1041,123 @@
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get_health_details.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/healthChecks/latest"}  # type: ignore
 
-    @distributed_trace_async
-    async def run_health_checks(  # pylint: disable=inconsistent-return-statements
+    async def _run_health_checks_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, network_connection_name: str, **kwargs: Any
     ) -> None:
-        """Triggers a new health check run. The execution and health check result can be tracked via the
-        network Connection health check details.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param network_connection_name: Name of the Network Connection that can be applied to a Pool.
-         Required.
-        :type network_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_run_health_checks_request(
             resource_group_name=resource_group_name,
             network_connection_name=network_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.run_health_checks.metadata["url"],
+            template_url=self._run_health_checks_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)  # type: ignore
 
         pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    run_health_checks.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/runHealthChecks"}  # type: ignore
+    _run_health_checks_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/runHealthChecks"}  # type: ignore
+
+    @distributed_trace_async
+    async def begin_run_health_checks(
+        self, resource_group_name: str, network_connection_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[None]:
+        """Triggers a new health check run. The execution and health check result can be tracked via the
+        network Connection health check details.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param network_connection_name: Name of the Network Connection that can be applied to a Pool.
+         Required.
+        :type network_connection_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-11-11-preview"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        if cont_token is None:
+            raw_result = await self._run_health_checks_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                network_connection_name=network_connection_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})
+
+        if polling is True:
+            polling_method = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )  # type: AsyncPollingMethod
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
+    begin_run_health_checks.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevCenter/networkConnections/{networkConnectionName}/runHealthChecks"}  # type: ignore
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_galleries_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_galleries_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.GalleryListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -186,15 +186,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Gallery]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             gallery_name=gallery_name,
             subscription_id=self._config.subscription_id,
@@ -242,15 +242,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Gallery]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -408,15 +408,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Gallery]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(  # type: ignore
@@ -471,15 +471,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             dev_center_name=dev_center_name,
             gallery_name=gallery_name,
             subscription_id=self._config.subscription_id,
@@ -532,15 +532,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure/mgmt/devcenter/aio/operations/_pools_operations.py` & `azure-mgmt-devcenter-1.0.0b4/azure/mgmt/devcenter/aio/operations/_pools_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.PoolListResult]
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -185,15 +185,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Pool]
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             pool_name=pool_name,
             subscription_id=self._config.subscription_id,
@@ -236,15 +236,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Pool]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -398,15 +398,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Pool]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(  # type: ignore
@@ -466,15 +466,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Pool]]
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -631,15 +631,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
         cls = kwargs.pop("cls", None)  # type: ClsType[_models.Pool]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(  # type: ignore
@@ -694,15 +694,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             project_name=project_name,
             pool_name=pool_name,
             subscription_id=self._config.subscription_id,
@@ -755,15 +755,15 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-10-12-preview"]
+        )  # type: Literal["2022-11-11-preview"]
         cls = kwargs.pop("cls", None)  # type: ClsType[None]
         polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/PKG-INFO` & `azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-devcenter
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Microsoft Azure Devcenter Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -49,14 +49,31 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-devcenter%2FREADME.png)
 
 
 # Release History
 
+## 1.0.0b4 (2022-11-24)
+
+### Features Added
+
+  - Added operation group CheckNameAvailabilityOperations
+  - Model DevBoxDefinition has a new parameter hibernate_support
+  - Model DevBoxDefinitionProperties has a new parameter hibernate_support
+  - Model DevBoxDefinitionUpdate has a new parameter hibernate_support
+  - Model DevBoxDefinitionUpdateProperties has a new parameter hibernate_support
+  - Model DevCenter has a new parameter dev_center_uri
+  - Model Project has a new parameter dev_center_uri
+  - Model ProjectProperties has a new parameter dev_center_uri
+
+### Breaking Changes
+
+  - Renamed operation NetworkConnectionsOperations.run_health_checks to NetworkConnectionsOperations.begin_run_health_checks
+
 ## 1.0.0b3 (2022-11-08)
 
 ### Features Added
 
   - Model Catalog has a new parameter sync_state
   - Model CatalogProperties has a new parameter sync_state
   - Model OperationStatus has a new parameter operations
```

## Comparing `azure-mgmt-devcenter-1.0.0b3/azure_mgmt_devcenter.egg-info/SOURCES.txt` & `azure-mgmt-devcenter-1.0.0b4/azure_mgmt_devcenter.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 azure/mgmt/devcenter/aio/__init__.py
 azure/mgmt/devcenter/aio/_configuration.py
 azure/mgmt/devcenter/aio/_dev_center_mgmt_client.py
 azure/mgmt/devcenter/aio/_patch.py
 azure/mgmt/devcenter/aio/operations/__init__.py
 azure/mgmt/devcenter/aio/operations/_attached_networks_operations.py
 azure/mgmt/devcenter/aio/operations/_catalogs_operations.py
+azure/mgmt/devcenter/aio/operations/_check_name_availability_operations.py
 azure/mgmt/devcenter/aio/operations/_dev_box_definitions_operations.py
 azure/mgmt/devcenter/aio/operations/_dev_centers_operations.py
 azure/mgmt/devcenter/aio/operations/_environment_types_operations.py
 azure/mgmt/devcenter/aio/operations/_galleries_operations.py
 azure/mgmt/devcenter/aio/operations/_image_versions_operations.py
 azure/mgmt/devcenter/aio/operations/_images_operations.py
 azure/mgmt/devcenter/aio/operations/_network_connections_operations.py
@@ -41,14 +42,15 @@
 azure/mgmt/devcenter/models/__init__.py
 azure/mgmt/devcenter/models/_dev_center_mgmt_client_enums.py
 azure/mgmt/devcenter/models/_models_py3.py
 azure/mgmt/devcenter/models/_patch.py
 azure/mgmt/devcenter/operations/__init__.py
 azure/mgmt/devcenter/operations/_attached_networks_operations.py
 azure/mgmt/devcenter/operations/_catalogs_operations.py
+azure/mgmt/devcenter/operations/_check_name_availability_operations.py
 azure/mgmt/devcenter/operations/_dev_box_definitions_operations.py
 azure/mgmt/devcenter/operations/_dev_centers_operations.py
 azure/mgmt/devcenter/operations/_environment_types_operations.py
 azure/mgmt/devcenter/operations/_galleries_operations.py
 azure/mgmt/devcenter/operations/_image_versions_operations.py
 azure/mgmt/devcenter/operations/_images_operations.py
 azure/mgmt/devcenter/operations/_network_connections_operations.py
```

