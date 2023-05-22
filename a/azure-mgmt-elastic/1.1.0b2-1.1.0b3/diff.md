# Comparing `tmp/azure-mgmt-elastic-1.1.0b2.zip` & `tmp/azure-mgmt-elastic-1.1.0b3.zip`

## zipinfo {}

```diff
@@ -1,87 +1,89 @@
-Zip file size: 164022 bytes, number of entries: 85
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/
--rw-rw-r--  2.0 unx     1136 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/CHANGELOG.md
--rw-rw-r--  2.0 unx     2130 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/README.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/setup.cfg
--rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/setup.py
--rw-rw-r--  2.0 unx     1074 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/LICENSE
--rw-rw-r--  2.0 unx      622 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/_meta.json
--rw-rw-r--  2.0 unx     4155 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/PKG-INFO
--rw-rw-r--  2.0 unx      213 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/MANIFEST.in
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/
--rw-rw-r--  2.0 unx       65 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/
--rw-rw-r--  2.0 unx     1302 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_patch.py
--rw-rw-r--  2.0 unx    78824 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_serialization.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_microsoft_elastic.py
--rw-rw-r--  2.0 unx     3815 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_configuration.py
--rw-rw-r--  2.0 unx      887 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/py.typed
--rw-rw-r--  2.0 unx      488 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_version.py
--rw-rw-r--  2.0 unx     9932 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py
--rw-rw-r--  2.0 unx     6790 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_traffic_filters_operations.py
--rw-rw-r--  2.0 unx     6879 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py
--rw-rw-r--  2.0 unx    14489 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitor_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_patch.py
--rw-rw-r--  2.0 unx    10264 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py
--rw-rw-r--  2.0 unx     6729 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_ingestion_operations.py
--rw-rw-r--  2.0 unx     9887 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
--rw-rw-r--  2.0 unx     8167 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_host_operations.py
--rw-rw-r--  2.0 unx     6748 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
--rw-rw-r--  2.0 unx    11094 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py
--rw-rw-r--  2.0 unx    28858 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_tag_rules_operations.py
--rw-rw-r--  2.0 unx     6671 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py
--rw-rw-r--  2.0 unx     6675 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_upgradable_versions_operations.py
--rw-rw-r--  2.0 unx    44918 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitors_operations.py
--rw-rw-r--  2.0 unx    10290 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_collection_operations.py
--rw-rw-r--  2.0 unx     2757 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/__init__.py
--rw-rw-r--  2.0 unx    11048 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_external_user_operations.py
--rw-rw-r--  2.0 unx    10467 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_organizations_operations.py
--rw-rw-r--  2.0 unx     6738 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_deployment_info_operations.py
--rw-rw-r--  2.0 unx     6924 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_operations.py
--rw-rw-r--  2.0 unx     8249 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitored_resources_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_patch.py
--rw-rw-r--  2.0 unx     2605 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_microsoft_elastic_enums.py
--rw-rw-r--  2.0 unx     4461 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/__init__.py
--rw-rw-r--  2.0 unx    60730 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_models_py3.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_patch.py
--rw-rw-r--  2.0 unx    10496 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_microsoft_elastic.py
--rw-rw-r--  2.0 unx     3863 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_configuration.py
--rw-rw-r--  2.0 unx      834 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/__init__.py
--rw-rw-r--  2.0 unx     8470 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py
--rw-rw-r--  2.0 unx     5219 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py
--rw-rw-r--  2.0 unx     5316 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py
--rw-rw-r--  2.0 unx    13036 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitor_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     8716 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py
--rw-rw-r--  2.0 unx     5340 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py
--rw-rw-r--  2.0 unx     8425 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
--rw-rw-r--  2.0 unx     6814 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_host_operations.py
--rw-rw-r--  2.0 unx     5374 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
--rw-rw-r--  2.0 unx     9253 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py
--rw-rw-r--  2.0 unx    23116 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py
--rw-rw-r--  2.0 unx     5292 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py
--rw-rw-r--  2.0 unx     5289 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py
--rw-rw-r--  2.0 unx    37307 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitors_operations.py
--rw-rw-r--  2.0 unx     8679 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py
--rw-rw-r--  2.0 unx     2757 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     9429 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_external_user_operations.py
--rw-rw-r--  2.0 unx     8978 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_organizations_operations.py
--rw-rw-r--  2.0 unx     5344 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py
--rw-rw-r--  2.0 unx     6177 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_operations.py
--rw-rw-r--  2.0 unx     6910 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/top_level.txt
--rw-rw-r--  2.0 unx      124 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/requires.txt
--rw-rw-r--  2.0 unx     3704 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     4155 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/PKG-INFO
-85 files, 632117 bytes uncompressed, 145300 bytes compressed:  77.0%
+Zip file size: 164892 bytes, number of entries: 87
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure/
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/setup.cfg
+-rw-rw-r--  2.0 unx     1074 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/LICENSE
+-rw-rw-r--  2.0 unx     2130 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/README.md
+-rw-rw-r--  2.0 unx      622 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/_meta.json
+-rw-rw-r--  2.0 unx     2828 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/setup.py
+-rw-rw-r--  2.0 unx     1611 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/CHANGELOG.md
+-rw-rw-r--  2.0 unx     4630 b- defN 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/PKG-INFO
+-rw-rw-r--  2.0 unx      213 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/MANIFEST.in
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx     3832 b- defN 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx     4630 b- defN 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx      124 b- defN 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/requires.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/
+-rw-rw-r--  2.0 unx      887 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_patch.py
+-rw-rw-r--  2.0 unx    10611 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_microsoft_elastic.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/py.typed
+-rw-rw-r--  2.0 unx    78836 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_serialization.py
+-rw-rw-r--  2.0 unx     3558 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_configuration.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_vendor.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_version.py
+-rw-rw-r--  2.0 unx     2858 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/__init__.py
+-rw-rw-r--  2.0 unx     6353 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx    14123 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_monitor_operations.py
+-rw-rw-r--  2.0 unx     6561 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx     9197 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_organizations_operations.py
+-rw-rw-r--  2.0 unx     7849 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_vm_host_operations.py
+-rw-rw-r--  2.0 unx     6430 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx    28228 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_tag_rules_operations.py
+-rw-rw-r--  2.0 unx     6606 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_operations.py
+-rw-rw-r--  2.0 unx     6420 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_deployment_info_operations.py
+-rw-rw-r--  2.0 unx     7931 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_monitored_resources_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_patch.py
+-rw-rw-r--  2.0 unx     6411 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_vm_ingestion_operations.py
+-rw-rw-r--  2.0 unx    10730 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_external_user_operations.py
+-rw-rw-r--  2.0 unx     7297 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_elastic_versions_operations.py
+-rw-rw-r--  2.0 unx     9566 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx    10728 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py
+-rw-rw-r--  2.0 unx    44064 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_monitors_operations.py
+-rw-rw-r--  2.0 unx     6472 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx     9972 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_vm_collection_operations.py
+-rw-rw-r--  2.0 unx     9898 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py
+-rw-rw-r--  2.0 unx     6357 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_upgradable_versions_operations.py
+-rw-rw-r--  2.0 unx     9521 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx    63855 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/_models_py3.py
+-rw-rw-r--  2.0 unx     4811 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/_patch.py
+-rw-rw-r--  2.0 unx     2605 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/_microsoft_elastic_enums.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:12 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/
+-rw-rw-r--  2.0 unx      834 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/_patch.py
+-rw-rw-r--  2.0 unx    10827 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/_microsoft_elastic.py
+-rw-rw-r--  2.0 unx     3606 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/_configuration.py
+-rw-rw-r--  2.0 unx     2858 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     5014 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx    12710 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_monitor_operations.py
+-rw-rw-r--  2.0 unx     5038 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx     7948 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_organizations_operations.py
+-rw-rw-r--  2.0 unx     6536 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_vm_host_operations.py
+-rw-rw-r--  2.0 unx     5096 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx    22646 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py
+-rw-rw-r--  2.0 unx     5899 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx     5066 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py
+-rw-rw-r--  2.0 unx     6632 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     5062 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py
+-rw-rw-r--  2.0 unx     9151 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_external_user_operations.py
+-rw-rw-r--  2.0 unx     6248 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_elastic_versions_operations.py
+-rw-rw-r--  2.0 unx     8144 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx     8927 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py
+-rw-rw-r--  2.0 unx    36693 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_monitors_operations.py
+-rw-rw-r--  2.0 unx     4941 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx     8401 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py
+-rw-rw-r--  2.0 unx     8390 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py
+-rw-rw-r--  2.0 unx     5011 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py
+-rw-rw-r--  2.0 unx     8099 b- defN 23-May-22 09:11 azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
+87 files, 635568 bytes uncompressed, 145658 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -1,256 +1,262 @@
-Filename: azure-mgmt-elastic-1.1.0b2/
+Filename: azure-mgmt-elastic-1.1.0b3/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/
+Filename: azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/
+Filename: azure-mgmt-elastic-1.1.0b3/azure/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/CHANGELOG.md
+Filename: azure-mgmt-elastic-1.1.0b3/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/README.md
+Filename: azure-mgmt-elastic-1.1.0b3/LICENSE
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/setup.cfg
+Filename: azure-mgmt-elastic-1.1.0b3/README.md
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/setup.py
+Filename: azure-mgmt-elastic-1.1.0b3/_meta.json
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/LICENSE
+Filename: azure-mgmt-elastic-1.1.0b3/setup.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/_meta.json
+Filename: azure-mgmt-elastic-1.1.0b3/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/PKG-INFO
+Filename: azure-mgmt-elastic-1.1.0b3/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/MANIFEST.in
+Filename: azure-mgmt-elastic-1.1.0b3/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/
+Filename: azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/
+Filename: azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/
+Filename: azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/
+Filename: azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_vendor.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_serialization.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_microsoft_elastic.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_configuration.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/py.typed
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_version.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_microsoft_elastic.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/py.typed
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitor_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_version.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_ingestion_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_host_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_monitor_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_organizations_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_tag_rules_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_vm_host_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_upgradable_versions_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_tag_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitors_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_collection_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_deployment_info_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_monitored_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_external_user_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_organizations_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_vm_ingestion_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_deployment_info_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_external_user_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_elastic_versions_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitored_resources_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_microsoft_elastic_enums.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_monitors_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_models_py3.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_vm_collection_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_upgradable_versions_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_microsoft_elastic.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_configuration.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/_microsoft_elastic_enums.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitor_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/_microsoft_elastic.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_host_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_monitor_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_organizations_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_vm_host_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitors_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_external_user_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_organizations_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_external_user_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_elastic_versions_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/not-zip-safe
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/top_level.txt
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/requires.txt
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_monitors_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/SOURCES.txt
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/dependency_links.txt
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/PKG-INFO
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py
+Comment: 
+
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py
+Comment: 
+
+Filename: azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-elastic-1.1.0b2/README.md` & `azure-mgmt-elastic-1.1.0b3/README.md`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/setup.py` & `azure-mgmt-elastic-1.1.0b3/setup.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/LICENSE` & `azure-mgmt-elastic-1.1.0b3/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/_meta.json` & `azure-mgmt-elastic-1.1.0b3/_meta.json`

 * *Files 23% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/elastic/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.4.8 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'1f449b5a17448f05ce1cd914f8ed75a0b568d130'",*

 * * "'use'": "{insert: […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/elastic/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.3 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "969fd0c2634fbcc1975d7abe3749330a5145a97c",
+    "autorest_command": "autorest specification/elastic/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.8 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "1f449b5a17448f05ce1cd914f8ed75a0b568d130",
     "readme": "specification/elastic/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.4.3",
+        "@autorest/python@6.4.8",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/PKG-INFO` & `azure-mgmt-elastic-1.1.0b3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-elastic
-Version: 1.1.0b2
+Version: 1.1.0b3
 Summary: Microsoft Azure Elastic Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -85,14 +85,28 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-elastic%2FREADME.png)
 
 
 # Release History
 
+## 1.1.0b3 (2023-05-22)
+
+### Features Added
+
+  - Added operation group ElasticVersionsOperations
+  - Model MonitorProperties has a new parameter generate_api_key
+  - Model UserApiKeyResponse has a new parameter properties
+
+### Breaking Changes
+
+  - Model ElasticMonitorResource no longer has parameter generate_api_key
+  - Model UserApiKeyResponse no longer has parameter api_key
+  - Operation OrganizationsOperations.get_api_key no longer has parameter resource_group_name
+
 ## 1.1.0b2 (2023-04-20)
 
 ### Features Added
 
   - Added operation group OrganizationsOperations
   - Model DeploymentInfoResponse has a new parameter deployment_url
   - Model DeploymentInfoResponse has a new parameter marketplace_saas_info
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_vendor.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_patch.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_serialization.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,15 +625,15 @@
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
@@ -1267,15 +1267,15 @@
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
 
@@ -1291,15 +1291,15 @@
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
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_microsoft_elastic.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_microsoft_elastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     AllTrafficFiltersOperations,
     AssociateTrafficFilterOperations,
     CreateAndAssociateIPFilterOperations,
     CreateAndAssociatePLFilterOperations,
     DeploymentInfoOperations,
     DetachAndDeleteTrafficFilterOperations,
     DetachTrafficFilterOperations,
+    ElasticVersionsOperations,
     ExternalUserOperations,
     ListAssociatedTrafficFiltersOperations,
     MonitorOperations,
     MonitoredResourcesOperations,
     MonitorsOperations,
     Operations,
     OrganizationsOperations,
@@ -46,14 +47,16 @@
 class MicrosoftElastic:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """MicrosoftElastic.
 
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.elastic.operations.Operations
     :ivar monitors: MonitorsOperations operations
     :vartype monitors: azure.mgmt.elastic.operations.MonitorsOperations
+    :ivar elastic_versions: ElasticVersionsOperations operations
+    :vartype elastic_versions: azure.mgmt.elastic.operations.ElasticVersionsOperations
     :ivar monitored_resources: MonitoredResourcesOperations operations
     :vartype monitored_resources: azure.mgmt.elastic.operations.MonitoredResourcesOperations
     :ivar deployment_info: DeploymentInfoOperations operations
     :vartype deployment_info: azure.mgmt.elastic.operations.DeploymentInfoOperations
     :ivar external_user: ExternalUserOperations operations
     :vartype external_user: azure.mgmt.elastic.operations.ExternalUserOperations
     :ivar tag_rules: TagRulesOperations operations
@@ -117,14 +120,17 @@
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.monitors = MonitorsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.elastic_versions = ElasticVersionsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.monitored_resources = MonitoredResourcesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.deployment_info = DeploymentInfoOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external_user = ExternalUserOperations(self._client, self._config, self._serialize, self._deserialize)
         self.tag_rules = TagRulesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.vm_host = VMHostOperations(self._client, self._config, self._serialize, self._deserialize)
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_configuration.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,52 +2,46 @@
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
-from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
-
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class MicrosoftElasticConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for MicrosoftElastic.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The Azure subscription ID. This is a GUID-formatted string (e.g.
      00000000-0000-0000-0000-000000000000). Required.
     :type subscription_id: str
     :keyword api_version: Api Version. Default value is "2023-02-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(MicrosoftElasticConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop("api_version", "2023-02-01-preview")
+        api_version: str = kwargs.pop("api_version", "2023-02-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -59,15 +53,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = ARMChallengeAuthenticationPolicy(
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/__init__.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py`

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
 from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,18 +25,14 @@
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
 
 
@@ -48,17 +43,15 @@
     *,
     ruleset_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter",
     )  # pylint: disable=line-too-long
@@ -110,17 +103,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_associate_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
@@ -179,17 +170,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._associate_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py`

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
 
 
@@ -46,23 +41,21 @@
     *,
     ruleset_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
@@ -75,22 +68,22 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class TrafficFiltersOperations:
+class DetachAndDeleteTrafficFilterOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.MicrosoftElastic`'s
-        :attr:`traffic_filters` attribute.
+        :attr:`detach_and_delete_traffic_filter` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
@@ -98,17 +91,17 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
     ) -> None:
-        """Delete traffic filter from the account.
+        """Detach and Delete traffic filter from the given deployment.
 
-        Delete traffic filter from the account.
+        Detach and Delete traffic filter from the given deployment.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :param ruleset_id: Ruleset Id of the filter. Default value is None.
@@ -125,17 +118,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
@@ -161,9 +152,9 @@
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py`

 * *Files 9% similar despite different names*

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
@@ -24,127 +23,105 @@
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
 
 
-def build_delete_request(
-    resource_group_name: str,
-    monitor_name: str,
-    subscription_id: str,
-    *,
-    ruleset_id: Optional[str] = None,
-    **kwargs: Any
-) -> HttpRequest:
+def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-    if ruleset_id is not None:
-        _params["rulesetId"] = _SERIALIZER.query("ruleset_id", ruleset_id, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class DetachAndDeleteTrafficFilterOperations:
+class ListAssociatedTrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.MicrosoftElastic`'s
-        :attr:`detach_and_delete_traffic_filter` attribute.
+        :attr:`list_associated_traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def delete(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
-    ) -> None:
-        """Detach and Delete traffic filter from the given deployment.
+    def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.ElasticTrafficFilterResponse:
+        """Get the list of all associated traffic filters for the given deployment.
 
-        Detach and Delete traffic filter from the given deployment.
+        Get the list of all associated traffic filters for the given deployment.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param ruleset_id: Ruleset Id of the filter. Default value is None.
-        :type ruleset_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
+        :return: ElasticTrafficFilterResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.elastic.models.ElasticTrafficFilterResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[None] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
-            ruleset_id=ruleset_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
+            template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
         _stream = False
@@ -157,13 +134,17 @@
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        deserialized = self._deserialize("ElasticTrafficFilterResponse", pipeline_response)
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter"
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitor_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_monitor_operations.py`

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
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,34 +25,28 @@
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
 
 
 def build_upgrade_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade",
@@ -110,17 +103,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -275,17 +266,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._upgrade_initial(  # type: ignore
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_patch.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py`

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
 from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,18 +25,14 @@
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
 
 
@@ -49,17 +44,15 @@
     ips: Optional[str] = None,
     name: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter",
     )  # pylint: disable=line-too-long
@@ -118,17 +111,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ips=ips,
@@ -195,17 +186,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_ingestion_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_vm_ingestion_operations.py`

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
@@ -24,34 +23,28 @@
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
 
 
 def build_details_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmIngestionDetails",
     )  # pylint: disable=line-too-long
@@ -114,17 +107,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.VMIngestionDetailsResponse] = kwargs.pop("cls", None)
 
         request = build_details_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py`

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
 from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,18 +25,14 @@
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
 
 
@@ -48,17 +43,15 @@
     *,
     ruleset_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter",
     )  # pylint: disable=line-too-long
@@ -110,17 +103,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
@@ -179,17 +170,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._update_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_host_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_vm_host_operations.py`

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
@@ -26,32 +25,26 @@
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
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listVMHost",
     )  # pylint: disable=line-too-long
@@ -106,17 +99,15 @@
         :return: An iterator like instance of either VMResources or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.VMResources]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.VMHostListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py`

 * *Files 8% similar despite different names*

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
@@ -24,38 +23,32 @@
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
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
@@ -66,38 +59,38 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class ListAssociatedTrafficFiltersOperations:
+class AllTrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.MicrosoftElastic`'s
-        :attr:`list_associated_traffic_filters` attribute.
+        :attr:`all_traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.ElasticTrafficFilterResponse:
-        """Get the list of all associated traffic filters for the given deployment.
+        """Get the list of all traffic filters for the account.
 
-        Get the list of all associated traffic filters for the given deployment.
+        Get the list of all traffic filters for the account.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -112,17 +105,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -151,9 +142,9 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py`

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
 from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,18 +25,14 @@
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
 
 
@@ -50,17 +45,15 @@
     private_endpoint_guid: Optional[str] = None,
     private_endpoint_name: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter",
     )  # pylint: disable=line-too-long
@@ -122,17 +115,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             name=name,
@@ -203,17 +194,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_tag_rules_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_tag_rules_operations.py`

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
@@ -28,32 +27,26 @@
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
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules",
     )  # pylint: disable=line-too-long
@@ -76,17 +69,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, monitor_name: str, rule_set_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}",
@@ -113,17 +104,15 @@
 
 def build_get_request(
     resource_group_name: str, monitor_name: str, rule_set_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}",
     )  # pylint: disable=line-too-long
@@ -147,17 +136,15 @@
 
 def build_delete_request(
     resource_group_name: str, monitor_name: str, rule_set_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}",
     )  # pylint: disable=line-too-long
@@ -215,17 +202,15 @@
         :return: An iterator like instance of either MonitoringTagRules or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.MonitoringTagRules]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MonitoringTagRulesListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -400,17 +385,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.MonitoringTagRules] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -489,17 +472,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MonitoringTagRules] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             rule_set_name=rule_set_name,
             subscription_id=self._config.subscription_id,
@@ -546,17 +527,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             rule_set_name=rule_set_name,
             subscription_id=self._config.subscription_id,
@@ -615,17 +594,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
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

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_traffic_filters_operations.py`

 * *Files 9% similar despite different names*

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
@@ -24,113 +23,119 @@
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
 
 
-def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_delete_request(
+    resource_group_name: str,
+    monitor_name: str,
+    subscription_id: str,
+    *,
+    ruleset_id: Optional[str] = None,
+    **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+    if ruleset_id is not None:
+        _params["rulesetId"] = _SERIALIZER.query("ruleset_id", ruleset_id, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class AllTrafficFiltersOperations:
+class TrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.MicrosoftElastic`'s
-        :attr:`all_traffic_filters` attribute.
+        :attr:`traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.ElasticTrafficFilterResponse:
-        """Get the list of all traffic filters for the account.
+    def delete(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """Delete traffic filter from the account.
 
-        Get the list of all traffic filters for the account.
+        Delete traffic filter from the account.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
+        :param ruleset_id: Ruleset Id of the filter. Default value is None.
+        :type ruleset_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ElasticTrafficFilterResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.elastic.models.ElasticTrafficFilterResponse
+        :return: None or the result of cls(response)
+        :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_list_request(
+        request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
+            ruleset_id=ruleset_id,
             api_version=api_version,
-            template_url=self.list.metadata["url"],
+            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
         _stream = False
@@ -143,17 +148,13 @@
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("ElasticTrafficFilterResponse", pipeline_response)
-
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, None, {})
 
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters"
+    delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_upgradable_versions_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_upgradable_versions_operations.py`

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
@@ -24,34 +23,28 @@
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
 
 
 def build_details_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listUpgradableVersions",
     )  # pylint: disable=line-too-long
@@ -114,17 +107,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.UpgradableVersionsList] = kwargs.pop("cls", None)
 
         request = build_details_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitors_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_monitors_operations.py`

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
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,32 +27,26 @@
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
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Elastic/monitors")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
@@ -69,17 +62,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors",
     )  # pylint: disable=line-too-long
@@ -99,17 +90,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}",
     )  # pylint: disable=line-too-long
@@ -132,17 +121,15 @@
 
 def build_create_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}",
@@ -168,17 +155,15 @@
 
 def build_update_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}",
@@ -204,17 +189,15 @@
 
 def build_delete_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}",
     )  # pylint: disable=line-too-long
@@ -265,17 +248,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ElasticMonitorResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -358,17 +339,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ElasticMonitorResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -461,17 +440,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -521,17 +498,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -697,17 +672,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_initial(
@@ -845,17 +818,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -916,17 +887,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -980,17 +949,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
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

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_collection_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_vm_collection_operations.py`

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
@@ -24,34 +23,28 @@
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
 
 
 def build_update_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmCollectionUpdate",
@@ -189,17 +182,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/__init__.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import Operations
 from ._monitors_operations import MonitorsOperations
+from ._elastic_versions_operations import ElasticVersionsOperations
 from ._monitored_resources_operations import MonitoredResourcesOperations
 from ._deployment_info_operations import DeploymentInfoOperations
 from ._external_user_operations import ExternalUserOperations
 from ._tag_rules_operations import TagRulesOperations
 from ._vm_host_operations import VMHostOperations
 from ._vm_ingestion_operations import VMIngestionOperations
 from ._vm_collection_operations import VMCollectionOperations
@@ -30,14 +31,15 @@
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "MonitorsOperations",
+    "ElasticVersionsOperations",
     "MonitoredResourcesOperations",
     "DeploymentInfoOperations",
     "ExternalUserOperations",
     "TagRulesOperations",
     "VMHostOperations",
     "VMIngestionOperations",
     "VMCollectionOperations",
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_external_user_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_external_user_operations.py`

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
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,34 +23,28 @@
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
 
 
 def build_create_or_update_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createOrUpdateExternalUser",
@@ -195,17 +188,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ExternalUserCreationResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_organizations_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_organizations_operations.py`

 * *Files 18% similar despite different names*

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
@@ -24,43 +23,35 @@
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
 
 
-def build_get_api_key_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_get_api_key_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/getOrganizationApiKey",
-    )  # pylint: disable=line-too-long
+        "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Elastic/getOrganizationApiKey"
+    )
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -89,85 +80,66 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @overload
     def get_api_key(
-        self,
-        resource_group_name: str,
-        body: Optional[_models.UserEmailId] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
+        self, body: Optional[_models.UserEmailId] = None, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.UserApiKeyResponse:
         """Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
         Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
-        :param resource_group_name: The name of the resource group to which the Elastic resource
-         belongs. Required.
-        :type resource_group_name: str
         :param body: Email Id parameter of the User Organization, of which the API Key must be
          returned. Default value is None.
         :type body: ~azure.mgmt.elastic.models.UserEmailId
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: UserApiKeyResponse or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.UserApiKeyResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def get_api_key(
-        self,
-        resource_group_name: str,
-        body: Optional[IO] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.UserApiKeyResponse:
         """Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
         Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
-        :param resource_group_name: The name of the resource group to which the Elastic resource
-         belongs. Required.
-        :type resource_group_name: str
         :param body: Email Id parameter of the User Organization, of which the API Key must be
          returned. Default value is None.
         :type body: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: UserApiKeyResponse or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.UserApiKeyResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def get_api_key(
-        self, resource_group_name: str, body: Optional[Union[_models.UserEmailId, IO]] = None, **kwargs: Any
+        self, body: Optional[Union[_models.UserEmailId, IO]] = None, **kwargs: Any
     ) -> _models.UserApiKeyResponse:
         """Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
         Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
-        :param resource_group_name: The name of the resource group to which the Elastic resource
-         belongs. Required.
-        :type resource_group_name: str
         :param body: Email Id parameter of the User Organization, of which the API Key must be
          returned. Is either a UserEmailId type or a IO type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.UserEmailId or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -182,17 +154,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.UserApiKeyResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -200,15 +170,14 @@
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UserEmailId")
             else:
                 _json = None
 
         request = build_get_api_key_request(
-            resource_group_name=resource_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             template_url=self.get_api_key.metadata["url"],
             headers=_headers,
@@ -234,10 +203,8 @@
         deserialized = self._deserialize("UserApiKeyResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get_api_key.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/getOrganizationApiKey"
-    }
+    get_api_key.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Elastic/getOrganizationApiKey"}
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_deployment_info_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_deployment_info_operations.py`

 * *Files 8% similar despite different names*

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
@@ -24,32 +23,26 @@
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
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listDeploymentInfo",
     )  # pylint: disable=line-too-long
@@ -114,17 +107,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DeploymentInfoResponse] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_operations.py`

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
@@ -26,32 +25,26 @@
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
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Elastic/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -91,17 +84,15 @@
         :return: An iterator like instance of either OperationResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.OperationResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitored_resources_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/operations/_monitored_resources_operations.py`

 * *Files 9% similar despite different names*

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
@@ -26,32 +25,26 @@
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
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-02-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listMonitoredResources",
     )  # pylint: disable=line-too-long
@@ -106,17 +99,15 @@
         :return: An iterator like instance of either MonitoredResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.MonitoredResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MonitoredResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_patch.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_microsoft_elastic_enums.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/_microsoft_elastic_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/__init__.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from ._models_py3 import ElasticMonitorResourceListResponse
 from ._models_py3 import ElasticMonitorResourceUpdateParameters
 from ._models_py3 import ElasticMonitorUpgrade
 from ._models_py3 import ElasticProperties
 from ._models_py3 import ElasticTrafficFilter
 from ._models_py3 import ElasticTrafficFilterResponse
 from ._models_py3 import ElasticTrafficFilterRule
+from ._models_py3 import ElasticVersionListFormat
+from ._models_py3 import ElasticVersionListProperties
+from ._models_py3 import ElasticVersionsListResponse
 from ._models_py3 import ErrorResponseBody
 from ._models_py3 import ExternalUserCreationResponse
 from ._models_py3 import ExternalUserInfo
 from ._models_py3 import FilteringTag
 from ._models_py3 import IdentityProperties
 from ._models_py3 import LogRules
 from ._models_py3 import MarketplaceSaaSInfo
@@ -36,14 +39,15 @@
 from ._models_py3 import OperationListResult
 from ._models_py3 import OperationResult
 from ._models_py3 import ResourceProviderDefaultErrorResponse
 from ._models_py3 import ResourceSku
 from ._models_py3 import SystemData
 from ._models_py3 import UpgradableVersionsList
 from ._models_py3 import UserApiKeyResponse
+from ._models_py3 import UserApiKeyResponseProperties
 from ._models_py3 import UserEmailId
 from ._models_py3 import UserInfo
 from ._models_py3 import VMCollectionUpdate
 from ._models_py3 import VMHostListResponse
 from ._models_py3 import VMIngestionDetailsResponse
 from ._models_py3 import VMResources
 
@@ -70,14 +74,17 @@
     "ElasticMonitorResourceListResponse",
     "ElasticMonitorResourceUpdateParameters",
     "ElasticMonitorUpgrade",
     "ElasticProperties",
     "ElasticTrafficFilter",
     "ElasticTrafficFilterResponse",
     "ElasticTrafficFilterRule",
+    "ElasticVersionListFormat",
+    "ElasticVersionListProperties",
+    "ElasticVersionsListResponse",
     "ErrorResponseBody",
     "ExternalUserCreationResponse",
     "ExternalUserInfo",
     "FilteringTag",
     "IdentityProperties",
     "LogRules",
     "MarketplaceSaaSInfo",
@@ -92,14 +99,15 @@
     "OperationListResult",
     "OperationResult",
     "ResourceProviderDefaultErrorResponse",
     "ResourceSku",
     "SystemData",
     "UpgradableVersionsList",
     "UserApiKeyResponse",
+    "UserApiKeyResponseProperties",
     "UserEmailId",
     "UserInfo",
     "VMCollectionUpdate",
     "VMHostListResponse",
     "VMIngestionDetailsResponse",
     "VMResources",
     "CreatedByType",
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_models_py3.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/models/_models_py3.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,41 +228,37 @@
     :vartype type: str
     :ivar sku: SKU of the monitor resource.
     :vartype sku: ~azure.mgmt.elastic.models.ResourceSku
     :ivar properties: Properties of the monitor resource.
     :vartype properties: ~azure.mgmt.elastic.models.MonitorProperties
     :ivar identity: Identity properties of the monitor resource.
     :vartype identity: ~azure.mgmt.elastic.models.IdentityProperties
-    :ivar generate_api_key: Flag to determine if User API Key has to be generated and shared.
-    :vartype generate_api_key: bool
     :ivar tags: The tags of the monitor resource.
     :vartype tags: dict[str, str]
     :ivar location: The location of the monitor resource. Required.
     :vartype location: str
     :ivar system_data: The system metadata relating to this resource.
     :vartype system_data: ~azure.mgmt.elastic.models.SystemData
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
-        "generate_api_key": {"readonly": True},
         "location": {"required": True},
         "system_data": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "sku": {"key": "sku", "type": "ResourceSku"},
         "properties": {"key": "properties", "type": "MonitorProperties"},
         "identity": {"key": "identity", "type": "IdentityProperties"},
-        "generate_api_key": {"key": "generateApiKey", "type": "bool"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
     def __init__(
         self,
@@ -289,15 +285,14 @@
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.sku = sku
         self.properties = properties
         self.identity = identity
-        self.generate_api_key = None
         self.tags = tags
         self.location = location
         self.system_data = None
 
 
 class ElasticMonitorResourceListResponse(_serialization.Model):
     """Response of a list operation.
@@ -539,14 +534,86 @@
         self.source = source
         self.description = description
         self.azure_endpoint_guid = azure_endpoint_guid
         self.azure_endpoint_name = azure_endpoint_name
         self.id = id
 
 
+class ElasticVersionListFormat(_serialization.Model):
+    """Elastic Version List Format.
+
+    :ivar properties: Elastic Version Properties.
+    :vartype properties: ~azure.mgmt.elastic.models.ElasticVersionListProperties
+    """
+
+    _attribute_map = {
+        "properties": {"key": "properties", "type": "ElasticVersionListProperties"},
+    }
+
+    def __init__(self, *, properties: Optional["_models.ElasticVersionListProperties"] = None, **kwargs: Any) -> None:
+        """
+        :keyword properties: Elastic Version Properties.
+        :paramtype properties: ~azure.mgmt.elastic.models.ElasticVersionListProperties
+        """
+        super().__init__(**kwargs)
+        self.properties = properties
+
+
+class ElasticVersionListProperties(_serialization.Model):
+    """Elastic Version Properties.
+
+    :ivar version: Available elastic version of the given region.
+    :vartype version: str
+    """
+
+    _attribute_map = {
+        "version": {"key": "version", "type": "str"},
+    }
+
+    def __init__(self, *, version: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword version: Available elastic version of the given region.
+        :paramtype version: str
+        """
+        super().__init__(**kwargs)
+        self.version = version
+
+
+class ElasticVersionsListResponse(_serialization.Model):
+    """List of elastic versions available in a region.
+
+    :ivar value: Results of a list operation.
+    :vartype value: list[~azure.mgmt.elastic.models.ElasticVersionListFormat]
+    :ivar next_link: Link to the next set of results, if any.
+    :vartype next_link: str
+    """
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[ElasticVersionListFormat]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        value: Optional[List["_models.ElasticVersionListFormat"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword value: Results of a list operation.
+        :paramtype value: list[~azure.mgmt.elastic.models.ElasticVersionListFormat]
+        :keyword next_link: Link to the next set of results, if any.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = next_link
+
+
 class ErrorResponseBody(_serialization.Model):
     """Error response body.
 
     :ivar code: Error code.
     :vartype code: str
     :ivar message: Error message.
     :vartype message: str
@@ -795,20 +862,20 @@
         self.send_activity_logs = send_activity_logs
         self.filtering_tags = filtering_tags
 
 
 class MarketplaceSaaSInfo(_serialization.Model):
     """Marketplace SAAS Info of the resource.
 
-    :ivar marketplace_subscription: Marketplace Subscription Id.
+    :ivar marketplace_subscription: Marketplace Subscription.
     :vartype marketplace_subscription:
      ~azure.mgmt.elastic.models.MarketplaceSaaSInfoMarketplaceSubscription
-    :ivar marketplace_name: Subscription Details: Marketplace SAAS Name.
+    :ivar marketplace_name: Marketplace Subscription Details: SAAS Name.
     :vartype marketplace_name: str
-    :ivar marketplace_resource_id: Subscription Details: Marketplace Resource URI.
+    :ivar marketplace_resource_id: Marketplace Subscription Details: Resource URI.
     :vartype marketplace_resource_id: str
     """
 
     _attribute_map = {
         "marketplace_subscription": {
             "key": "marketplaceSubscription",
             "type": "MarketplaceSaaSInfoMarketplaceSubscription",
@@ -822,30 +889,30 @@
         *,
         marketplace_subscription: Optional["_models.MarketplaceSaaSInfoMarketplaceSubscription"] = None,
         marketplace_name: Optional[str] = None,
         marketplace_resource_id: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
-        :keyword marketplace_subscription: Marketplace Subscription Id.
+        :keyword marketplace_subscription: Marketplace Subscription.
         :paramtype marketplace_subscription:
          ~azure.mgmt.elastic.models.MarketplaceSaaSInfoMarketplaceSubscription
-        :keyword marketplace_name: Subscription Details: Marketplace SAAS Name.
+        :keyword marketplace_name: Marketplace Subscription Details: SAAS Name.
         :paramtype marketplace_name: str
-        :keyword marketplace_resource_id: Subscription Details: Marketplace Resource URI.
+        :keyword marketplace_resource_id: Marketplace Subscription Details: Resource URI.
         :paramtype marketplace_resource_id: str
         """
         super().__init__(**kwargs)
         self.marketplace_subscription = marketplace_subscription
         self.marketplace_name = marketplace_name
         self.marketplace_resource_id = marketplace_resource_id
 
 
 class MarketplaceSaaSInfoMarketplaceSubscription(_serialization.Model):
-    """Marketplace Subscription Id.
+    """Marketplace Subscription.
 
     :ivar id: Marketplace Subscription Id. This is a GUID-formatted string.
     :vartype id: str
     """
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
@@ -1066,14 +1133,16 @@
     :vartype user_info: ~azure.mgmt.elastic.models.UserInfo
     :ivar version: Version of elastic of the monitor resource.
     :vartype version: str
     :ivar liftr_resource_category: Known values are: "Unknown" and "MonitorLogs".
     :vartype liftr_resource_category: str or ~azure.mgmt.elastic.models.LiftrResourceCategories
     :ivar liftr_resource_preference: The priority of the resource.
     :vartype liftr_resource_preference: int
+    :ivar generate_api_key: Flag to determine if User API Key has to be generated and shared.
+    :vartype generate_api_key: bool
     """
 
     _validation = {
         "liftr_resource_category": {"readonly": True},
         "liftr_resource_preference": {"readonly": True},
     }
 
@@ -1081,24 +1150,26 @@
         "provisioning_state": {"key": "provisioningState", "type": "str"},
         "monitoring_status": {"key": "monitoringStatus", "type": "str"},
         "elastic_properties": {"key": "elasticProperties", "type": "ElasticProperties"},
         "user_info": {"key": "userInfo", "type": "UserInfo"},
         "version": {"key": "version", "type": "str"},
         "liftr_resource_category": {"key": "liftrResourceCategory", "type": "str"},
         "liftr_resource_preference": {"key": "liftrResourcePreference", "type": "int"},
+        "generate_api_key": {"key": "generateApiKey", "type": "bool"},
     }
 
     def __init__(
         self,
         *,
         provisioning_state: Optional[Union[str, "_models.ProvisioningState"]] = None,
         monitoring_status: Optional[Union[str, "_models.MonitoringStatus"]] = None,
         elastic_properties: Optional["_models.ElasticProperties"] = None,
         user_info: Optional["_models.UserInfo"] = None,
         version: Optional[str] = None,
+        generate_api_key: Optional[bool] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword provisioning_state: Provisioning state of the monitor resource. Known values are:
          "Accepted", "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted",
          and "NotSpecified".
         :paramtype provisioning_state: str or ~azure.mgmt.elastic.models.ProvisioningState
@@ -1107,23 +1178,26 @@
         :paramtype monitoring_status: str or ~azure.mgmt.elastic.models.MonitoringStatus
         :keyword elastic_properties: Elastic cloud properties.
         :paramtype elastic_properties: ~azure.mgmt.elastic.models.ElasticProperties
         :keyword user_info: User information.
         :paramtype user_info: ~azure.mgmt.elastic.models.UserInfo
         :keyword version: Version of elastic of the monitor resource.
         :paramtype version: str
+        :keyword generate_api_key: Flag to determine if User API Key has to be generated and shared.
+        :paramtype generate_api_key: bool
         """
         super().__init__(**kwargs)
         self.provisioning_state = provisioning_state
         self.monitoring_status = monitoring_status
         self.elastic_properties = elastic_properties
         self.user_info = user_info
         self.version = version
         self.liftr_resource_category = None
         self.liftr_resource_preference = None
+        self.generate_api_key = generate_api_key
 
 
 class OperationDisplay(_serialization.Model):
     """The object that represents the operation.
 
     :ivar provider: Service provider, i.e., Microsoft.Elastic.
     :vartype provider: str
@@ -1383,27 +1457,47 @@
         self.upgradable_versions = upgradable_versions
 
 
 class UserApiKeyResponse(_serialization.Model):
     """The User Api Key created for the Organization associated with the User Email Id that was passed
     in the request.
 
-    :ivar api_key: The User Api Key Generated based on ReturnApiKey flag. This is applicable for
+    :ivar properties:
+    :vartype properties: ~azure.mgmt.elastic.models.UserApiKeyResponseProperties
+    """
+
+    _attribute_map = {
+        "properties": {"key": "properties", "type": "UserApiKeyResponseProperties"},
+    }
+
+    def __init__(self, *, properties: Optional["_models.UserApiKeyResponseProperties"] = None, **kwargs: Any) -> None:
+        """
+        :keyword properties:
+        :paramtype properties: ~azure.mgmt.elastic.models.UserApiKeyResponseProperties
+        """
+        super().__init__(**kwargs)
+        self.properties = properties
+
+
+class UserApiKeyResponseProperties(_serialization.Model):
+    """UserApiKeyResponseProperties.
+
+    :ivar api_key: The User Api Key Generated based on GenerateApiKey flag. This is applicable for
      non-Portal clients only.
     :vartype api_key: str
     """
 
     _attribute_map = {
         "api_key": {"key": "apiKey", "type": "str"},
     }
 
     def __init__(self, *, api_key: Optional[str] = None, **kwargs: Any) -> None:
         """
-        :keyword api_key: The User Api Key Generated based on ReturnApiKey flag. This is applicable for
-         non-Portal clients only.
+        :keyword api_key: The User Api Key Generated based on GenerateApiKey flag. This is applicable
+         for non-Portal clients only.
         :paramtype api_key: str
         """
         super().__init__(**kwargs)
         self.api_key = api_key
 
 
 class UserEmailId(_serialization.Model):
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_patch.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_microsoft_elastic.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/_microsoft_elastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     AllTrafficFiltersOperations,
     AssociateTrafficFilterOperations,
     CreateAndAssociateIPFilterOperations,
     CreateAndAssociatePLFilterOperations,
     DeploymentInfoOperations,
     DetachAndDeleteTrafficFilterOperations,
     DetachTrafficFilterOperations,
+    ElasticVersionsOperations,
     ExternalUserOperations,
     ListAssociatedTrafficFiltersOperations,
     MonitorOperations,
     MonitoredResourcesOperations,
     MonitorsOperations,
     Operations,
     OrganizationsOperations,
@@ -46,14 +47,16 @@
 class MicrosoftElastic:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """MicrosoftElastic.
 
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.elastic.aio.operations.Operations
     :ivar monitors: MonitorsOperations operations
     :vartype monitors: azure.mgmt.elastic.aio.operations.MonitorsOperations
+    :ivar elastic_versions: ElasticVersionsOperations operations
+    :vartype elastic_versions: azure.mgmt.elastic.aio.operations.ElasticVersionsOperations
     :ivar monitored_resources: MonitoredResourcesOperations operations
     :vartype monitored_resources: azure.mgmt.elastic.aio.operations.MonitoredResourcesOperations
     :ivar deployment_info: DeploymentInfoOperations operations
     :vartype deployment_info: azure.mgmt.elastic.aio.operations.DeploymentInfoOperations
     :ivar external_user: ExternalUserOperations operations
     :vartype external_user: azure.mgmt.elastic.aio.operations.ExternalUserOperations
     :ivar tag_rules: TagRulesOperations operations
@@ -117,14 +120,17 @@
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.monitors = MonitorsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.elastic_versions = ElasticVersionsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.monitored_resources = MonitoredResourcesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.deployment_info = DeploymentInfoOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external_user = ExternalUserOperations(self._client, self._config, self._serialize, self._deserialize)
         self.tag_rules = TagRulesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.vm_host = VMHostOperations(self._client, self._config, self._serialize, self._deserialize)
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_configuration.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/_configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,52 +2,46 @@
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
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
-
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class MicrosoftElasticConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for MicrosoftElastic.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The Azure subscription ID. This is a GUID-formatted string (e.g.
      00000000-0000-0000-0000-000000000000). Required.
     :type subscription_id: str
     :keyword api_version: Api Version. Default value is "2023-02-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(MicrosoftElasticConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop("api_version", "2023-02-01-preview")
+        api_version: str = kwargs.pop("api_version", "2023-02-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -59,15 +53,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/__init__.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py`

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
 from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,18 +25,14 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._associate_traffic_filter_operations import build_associate_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class AssociateTrafficFilterOperations:
     """
     .. warning::
@@ -67,17 +62,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_associate_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
@@ -136,17 +129,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._associate_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py`

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
@@ -22,32 +21,28 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._traffic_filters_operations import build_delete_request
+from ...operations._detach_and_delete_traffic_filter_operations import build_delete_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class TrafficFiltersOperations:
+class DetachAndDeleteTrafficFilterOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`traffic_filters` attribute.
+        :attr:`detach_and_delete_traffic_filter` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
@@ -55,17 +50,17 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
     async def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
     ) -> None:
-        """Delete traffic filter from the account.
+        """Detach and Delete traffic filter from the given deployment.
 
-        Delete traffic filter from the account.
+        Detach and Delete traffic filter from the given deployment.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :param ruleset_id: Ruleset Id of the filter. Default value is None.
@@ -82,17 +77,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
@@ -118,9 +111,9 @@
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py`

 * *Files 8% similar despite different names*

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
@@ -22,32 +21,28 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._detach_and_delete_traffic_filter_operations import build_delete_request
+from ...operations._traffic_filters_operations import build_delete_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class DetachAndDeleteTrafficFilterOperations:
+class TrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`detach_and_delete_traffic_filter` attribute.
+        :attr:`traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
@@ -55,17 +50,17 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
     async def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
     ) -> None:
-        """Detach and Delete traffic filter from the given deployment.
+        """Delete traffic filter from the account.
 
-        Detach and Delete traffic filter from the given deployment.
+        Delete traffic filter from the account.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :param ruleset_id: Ruleset Id of the filter. Default value is None.
@@ -82,17 +77,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
@@ -118,9 +111,9 @@
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitor_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_monitor_operations.py`

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
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,18 +25,14 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._monitor_operations import build_upgrade_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class MonitorOperations:
     """
     .. warning::
@@ -71,17 +66,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -236,17 +229,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._upgrade_initial(  # type: ignore
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_patch.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py`

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
 from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,18 +25,14 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._create_and_associate_ip_filter_operations import build_create_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class CreateAndAssociateIPFilterOperations:
     """
     .. warning::
@@ -72,17 +67,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ips=ips,
@@ -149,17 +142,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py`

 * *Files 12% similar despite different names*

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
@@ -22,83 +21,77 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._vm_ingestion_operations import build_details_request
+from ...operations._all_traffic_filters_operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class VMIngestionOperations:
+class AllTrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`vm_ingestion` attribute.
+        :attr:`all_traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
-    async def details(
+    async def list(
         self, resource_group_name: str, monitor_name: str, **kwargs: Any
-    ) -> _models.VMIngestionDetailsResponse:
-        """List the vm ingestion details that will be monitored by the Elastic monitor resource.
+    ) -> _models.ElasticTrafficFilterResponse:
+        """Get the list of all traffic filters for the account.
 
-        List the vm ingestion details that will be monitored by the Elastic monitor resource.
+        Get the list of all traffic filters for the account.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: VMIngestionDetailsResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.elastic.models.VMIngestionDetailsResponse
+        :return: ElasticTrafficFilterResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.elastic.models.ElasticTrafficFilterResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.VMIngestionDetailsResponse] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
 
-        request = build_details_request(
+        request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.details.metadata["url"],
+            template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
         _stream = False
@@ -111,17 +104,17 @@
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("VMIngestionDetailsResponse", pipeline_response)
+        deserialized = self._deserialize("ElasticTrafficFilterResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    details.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmIngestionDetails"
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py`

 * *Files 11% similar despite different names*

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
 from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,18 +25,14 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._detach_traffic_filter_operations import build_update_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DetachTrafficFilterOperations:
     """
     .. warning::
@@ -67,17 +62,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
@@ -136,17 +129,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._update_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_host_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_vm_host_operations.py`

 * *Files 9% similar despite different names*

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
 from ...operations._vm_host_operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class VMHostOperations:
     """
     .. warning::
@@ -72,17 +67,15 @@
         :return: An iterator like instance of either VMResources or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.VMResources]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.VMHostListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py`

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
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._list_associated_traffic_filters_operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ListAssociatedTrafficFiltersOperations:
     """
     .. warning::
@@ -80,17 +75,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py`

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
 from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,18 +25,14 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._create_and_associate_pl_filter_operations import build_create_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class CreateAndAssociatePLFilterOperations:
     """
     .. warning::
@@ -73,17 +68,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             name=name,
@@ -154,17 +147,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py`

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
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -34,18 +33,14 @@
 from ...operations._tag_rules_operations import (
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
 
 
 class TagRulesOperations:
     """
     .. warning::
@@ -82,17 +77,15 @@
         :return: An iterator like instance of either MonitoringTagRules or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.MonitoringTagRules]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MonitoringTagRulesListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -267,17 +260,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.MonitoringTagRules] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -356,17 +347,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MonitoringTagRules] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             rule_set_name=rule_set_name,
             subscription_id=self._config.subscription_id,
@@ -413,17 +402,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             rule_set_name=rule_set_name,
             subscription_id=self._config.subscription_id,
@@ -482,17 +469,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
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

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py`

 * *Files 14% similar despite different names*

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
@@ -22,83 +21,77 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._all_traffic_filters_operations import build_list_request
+from ...operations._upgradable_versions_operations import build_details_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class AllTrafficFiltersOperations:
+class UpgradableVersionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`all_traffic_filters` attribute.
+        :attr:`upgradable_versions` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
-    async def list(
+    async def details(
         self, resource_group_name: str, monitor_name: str, **kwargs: Any
-    ) -> _models.ElasticTrafficFilterResponse:
-        """Get the list of all traffic filters for the account.
+    ) -> _models.UpgradableVersionsList:
+        """List of upgradable versions for a given monitor resource.
 
-        Get the list of all traffic filters for the account.
+        List of upgradable versions for a given monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ElasticTrafficFilterResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.elastic.models.ElasticTrafficFilterResponse
+        :return: UpgradableVersionsList or the result of cls(response)
+        :rtype: ~azure.mgmt.elastic.models.UpgradableVersionsList
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.UpgradableVersionsList] = kwargs.pop("cls", None)
 
-        request = build_list_request(
+        request = build_details_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.list.metadata["url"],
+            template_url=self.details.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
         _stream = False
@@ -111,17 +104,17 @@
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("ElasticTrafficFilterResponse", pipeline_response)
+        deserialized = self._deserialize("UpgradableVersionsList", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters"
+    details.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listUpgradableVersions"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py`

 * *Files 20% similar despite different names*

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
@@ -22,83 +21,77 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._upgradable_versions_operations import build_details_request
+from ...operations._deployment_info_operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class UpgradableVersionsOperations:
+class DeploymentInfoOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`upgradable_versions` attribute.
+        :attr:`deployment_info` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
-    async def details(
-        self, resource_group_name: str, monitor_name: str, **kwargs: Any
-    ) -> _models.UpgradableVersionsList:
-        """List of upgradable versions for a given monitor resource.
+    async def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.DeploymentInfoResponse:
+        """Fetch information regarding Elastic cloud deployment corresponding to the Elastic monitor
+        resource.
 
-        List of upgradable versions for a given monitor resource.
+        Fetch information regarding Elastic cloud deployment corresponding to the Elastic monitor
+        resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: UpgradableVersionsList or the result of cls(response)
-        :rtype: ~azure.mgmt.elastic.models.UpgradableVersionsList
+        :return: DeploymentInfoResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.elastic.models.DeploymentInfoResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.UpgradableVersionsList] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.DeploymentInfoResponse] = kwargs.pop("cls", None)
 
-        request = build_details_request(
+        request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.details.metadata["url"],
+            template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
         _stream = False
@@ -111,17 +104,17 @@
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("UpgradableVersionsList", pipeline_response)
+        deserialized = self._deserialize("DeploymentInfoResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    details.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listUpgradableVersions"
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listDeploymentInfo"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitors_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_monitors_operations.py`

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
@@ -36,18 +35,14 @@
     build_delete_request,
     build_get_request,
     build_list_by_resource_group_request,
     build_list_request,
     build_update_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class MonitorsOperations:
     """
     .. warning::
@@ -79,17 +74,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ElasticMonitorResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -173,17 +166,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ElasticMonitorResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -276,17 +267,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -336,17 +325,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -512,17 +499,15 @@
          of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_initial(
@@ -661,17 +646,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -732,17 +715,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -796,17 +777,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
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

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py`

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
@@ -24,18 +23,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._vm_collection_operations import build_update_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class VMCollectionOperations:
     """
     .. warning::
@@ -150,17 +145,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/__init__.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import Operations
 from ._monitors_operations import MonitorsOperations
+from ._elastic_versions_operations import ElasticVersionsOperations
 from ._monitored_resources_operations import MonitoredResourcesOperations
 from ._deployment_info_operations import DeploymentInfoOperations
 from ._external_user_operations import ExternalUserOperations
 from ._tag_rules_operations import TagRulesOperations
 from ._vm_host_operations import VMHostOperations
 from ._vm_ingestion_operations import VMIngestionOperations
 from ._vm_collection_operations import VMCollectionOperations
@@ -30,14 +31,15 @@
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "MonitorsOperations",
+    "ElasticVersionsOperations",
     "MonitoredResourcesOperations",
     "DeploymentInfoOperations",
     "ExternalUserOperations",
     "TagRulesOperations",
     "VMHostOperations",
     "VMIngestionOperations",
     "VMCollectionOperations",
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_external_user_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_external_user_operations.py`

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
 from ...operations._external_user_operations import build_create_or_update_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ExternalUserOperations:
     """
     .. warning::
@@ -156,17 +151,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ExternalUserCreationResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_organizations_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_organizations_operations.py`

 * *Files 8% similar despite different names*

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
 from ...operations._organizations_operations import build_get_api_key_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class OrganizationsOperations:
     """
     .. warning::
@@ -53,85 +48,66 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @overload
     async def get_api_key(
-        self,
-        resource_group_name: str,
-        body: Optional[_models.UserEmailId] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
+        self, body: Optional[_models.UserEmailId] = None, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.UserApiKeyResponse:
         """Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
         Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
-        :param resource_group_name: The name of the resource group to which the Elastic resource
-         belongs. Required.
-        :type resource_group_name: str
         :param body: Email Id parameter of the User Organization, of which the API Key must be
          returned. Default value is None.
         :type body: ~azure.mgmt.elastic.models.UserEmailId
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: UserApiKeyResponse or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.UserApiKeyResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def get_api_key(
-        self,
-        resource_group_name: str,
-        body: Optional[IO] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.UserApiKeyResponse:
         """Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
         Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
-        :param resource_group_name: The name of the resource group to which the Elastic resource
-         belongs. Required.
-        :type resource_group_name: str
         :param body: Email Id parameter of the User Organization, of which the API Key must be
          returned. Default value is None.
         :type body: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: UserApiKeyResponse or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.UserApiKeyResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def get_api_key(
-        self, resource_group_name: str, body: Optional[Union[_models.UserEmailId, IO]] = None, **kwargs: Any
+        self, body: Optional[Union[_models.UserEmailId, IO]] = None, **kwargs: Any
     ) -> _models.UserApiKeyResponse:
         """Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
         Fetch User API Key from internal database, if it was generated and stored while creating the
         Elasticsearch Organization.
 
-        :param resource_group_name: The name of the resource group to which the Elastic resource
-         belongs. Required.
-        :type resource_group_name: str
         :param body: Email Id parameter of the User Organization, of which the API Key must be
          returned. Is either a UserEmailId type or a IO type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.UserEmailId or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -146,17 +122,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.UserApiKeyResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
@@ -164,15 +138,14 @@
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UserEmailId")
             else:
                 _json = None
 
         request = build_get_api_key_request(
-            resource_group_name=resource_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             template_url=self.get_api_key.metadata["url"],
             headers=_headers,
@@ -198,10 +171,8 @@
         deserialized = self._deserialize("UserApiKeyResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get_api_key.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/getOrganizationApiKey"
-    }
+    get_api_key.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Elastic/getOrganizationApiKey"}
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py`

 * *Files 20% similar despite different names*

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
@@ -22,83 +21,77 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._deployment_info_operations import build_list_request
+from ...operations._vm_ingestion_operations import build_details_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class DeploymentInfoOperations:
+class VMIngestionOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`deployment_info` attribute.
+        :attr:`vm_ingestion` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
-    async def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.DeploymentInfoResponse:
-        """Fetch information regarding Elastic cloud deployment corresponding to the Elastic monitor
-        resource.
+    async def details(
+        self, resource_group_name: str, monitor_name: str, **kwargs: Any
+    ) -> _models.VMIngestionDetailsResponse:
+        """List the vm ingestion details that will be monitored by the Elastic monitor resource.
 
-        Fetch information regarding Elastic cloud deployment corresponding to the Elastic monitor
-        resource.
+        List the vm ingestion details that will be monitored by the Elastic monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: DeploymentInfoResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.elastic.models.DeploymentInfoResponse
+        :return: VMIngestionDetailsResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.elastic.models.VMIngestionDetailsResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.DeploymentInfoResponse] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.VMIngestionDetailsResponse] = kwargs.pop("cls", None)
 
-        request = build_list_request(
+        request = build_details_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.list.metadata["url"],
+            template_url=self.details.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
         _stream = False
@@ -111,17 +104,17 @@
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("DeploymentInfoResponse", pipeline_response)
+        deserialized = self._deserialize("VMIngestionDetailsResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listDeploymentInfo"
+    details.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmIngestionDetails"
     }
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_operations.py`

 * *Files 9% similar despite different names*

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
@@ -67,17 +62,15 @@
         :return: An iterator like instance of either OperationResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.OperationResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py` & `azure-mgmt-elastic-1.1.0b3/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py`

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
 from ...operations._monitored_resources_operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class MonitoredResourcesOperations:
     """
     .. warning::
@@ -74,17 +69,15 @@
         :return: An iterator like instance of either MonitoredResource or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.MonitoredResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MonitoredResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/SOURCES.txt` & `azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py
 azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py
 azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py
 azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py
 azure/mgmt/elastic/aio/operations/_deployment_info_operations.py
 azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py
 azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
+azure/mgmt/elastic/aio/operations/_elastic_versions_operations.py
 azure/mgmt/elastic/aio/operations/_external_user_operations.py
 azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
 azure/mgmt/elastic/aio/operations/_monitor_operations.py
 azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
 azure/mgmt/elastic/aio/operations/_monitors_operations.py
 azure/mgmt/elastic/aio/operations/_operations.py
 azure/mgmt/elastic/aio/operations/_organizations_operations.py
@@ -48,14 +49,15 @@
 azure/mgmt/elastic/operations/_all_traffic_filters_operations.py
 azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py
 azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py
 azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py
 azure/mgmt/elastic/operations/_deployment_info_operations.py
 azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py
 azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
+azure/mgmt/elastic/operations/_elastic_versions_operations.py
 azure/mgmt/elastic/operations/_external_user_operations.py
 azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
 azure/mgmt/elastic/operations/_monitor_operations.py
 azure/mgmt/elastic/operations/_monitored_resources_operations.py
 azure/mgmt/elastic/operations/_monitors_operations.py
 azure/mgmt/elastic/operations/_operations.py
 azure/mgmt/elastic/operations/_organizations_operations.py
```

## Comparing `azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/PKG-INFO` & `azure-mgmt-elastic-1.1.0b3/azure_mgmt_elastic.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-elastic
-Version: 1.1.0b2
+Version: 1.1.0b3
 Summary: Microsoft Azure Elastic Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -85,14 +85,28 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-elastic%2FREADME.png)
 
 
 # Release History
 
+## 1.1.0b3 (2023-05-22)
+
+### Features Added
+
+  - Added operation group ElasticVersionsOperations
+  - Model MonitorProperties has a new parameter generate_api_key
+  - Model UserApiKeyResponse has a new parameter properties
+
+### Breaking Changes
+
+  - Model ElasticMonitorResource no longer has parameter generate_api_key
+  - Model UserApiKeyResponse no longer has parameter api_key
+  - Operation OrganizationsOperations.get_api_key no longer has parameter resource_group_name
+
 ## 1.1.0b2 (2023-04-20)
 
 ### Features Added
 
   - Added operation group OrganizationsOperations
   - Model DeploymentInfoResponse has a new parameter deployment_url
   - Model DeploymentInfoResponse has a new parameter marketplace_saas_info
```

