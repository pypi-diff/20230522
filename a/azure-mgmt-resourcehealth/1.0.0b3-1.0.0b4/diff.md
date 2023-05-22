# Comparing `tmp/azure-mgmt-resourcehealth-1.0.0b3.zip` & `tmp/azure-mgmt-resourcehealth-1.0.0b4.zip`

## zipinfo {}

```diff
@@ -1,98 +1,141 @@
-Zip file size: 136649 bytes, number of entries: 96
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/
--rw-rw-r--  2.0 unx     2835 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/setup.py
--rw-rw-r--  2.0 unx     1095 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/CHANGELOG.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/setup.cfg
--rw-rw-r--  2.0 unx     1074 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/LICENSE
--rw-rw-r--  2.0 unx      220 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/MANIFEST.in
--rw-rw-r--  2.0 unx      636 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/_meta.json
--rw-rw-r--  2.0 unx     2152 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/README.md
--rw-rw-r--  2.0 unx     4151 b- defN 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/top_level.txt
--rw-rw-r--  2.0 unx     4384 b- defN 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx      116 b- defN 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     4151 b- defN 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/PKG-INFO
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/
--rw-rw-r--  2.0 unx       65 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/aio/
--rw-rw-r--  2.0 unx     3292 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_configuration.py
--rw-rw-r--  2.0 unx      347 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_version.py
--rw-rw-r--  2.0 unx    10216 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_microsoft_resource_health.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/py.typed
--rw-rw-r--  2.0 unx      394 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/models.py
--rw-rw-r--  2.0 unx    78842 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_serialization.py
--rw-rw-r--  2.0 unx      725 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/
--rw-rw-r--  2.0 unx     3860 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_patch.py
--rw-rw-r--  2.0 unx      488 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_version.py
--rw-rw-r--  2.0 unx     5247 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_microsoft_resource_health.py
--rw-rw-r--  2.0 unx     1302 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_vendor.py
--rw-rw-r--  2.0 unx      909 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/__init__.py
--rw-rw-r--  2.0 unx    26312 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_availability_statuses_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_patch.py
--rw-rw-r--  2.0 unx    10288 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_emerging_issues_operations.py
--rw-rw-r--  2.0 unx    10016 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_metadata_operations.py
--rw-rw-r--  2.0 unx     5271 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_operations.py
--rw-rw-r--  2.0 unx    15050 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_events_operations.py
--rw-rw-r--  2.0 unx     1127 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/_patch.py
--rw-rw-r--  2.0 unx     2800 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/_microsoft_resource_health_enums.py
--rw-rw-r--  2.0 unx    71291 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/_models_py3.py
--rw-rw-r--  2.0 unx     4071 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/
--rw-rw-r--  2.0 unx     3908 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/_patch.py
--rw-rw-r--  2.0 unx     5394 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/_microsoft_resource_health.py
--rw-rw-r--  2.0 unx      856 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/__init__.py
--rw-rw-r--  2.0 unx    21142 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_availability_statuses_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     8652 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_emerging_issues_operations.py
--rw-rw-r--  2.0 unx     8435 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_metadata_operations.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    12435 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_events_operations.py
--rw-rw-r--  2.0 unx     1127 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/
--rw-rw-r--  2.0 unx     3860 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_patch.py
--rw-rw-r--  2.0 unx      488 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_version.py
--rw-rw-r--  2.0 unx     5141 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_microsoft_resource_health.py
--rw-rw-r--  2.0 unx     1302 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_vendor.py
--rw-rw-r--  2.0 unx      909 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/__init__.py
--rw-rw-r--  2.0 unx    25693 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_availability_statuses_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_patch.py
--rw-rw-r--  2.0 unx     8516 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_resources_operations.py
--rw-rw-r--  2.0 unx    13209 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_availability_statuses_operations.py
--rw-rw-r--  2.0 unx     5271 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_operations.py
--rw-rw-r--  2.0 unx     1107 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/_patch.py
--rw-rw-r--  2.0 unx      937 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/_microsoft_resource_health_enums.py
--rw-rw-r--  2.0 unx    24521 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/_models_py3.py
--rw-rw-r--  2.0 unx     1881 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 08:22 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/
--rw-rw-r--  2.0 unx     3908 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/_patch.py
--rw-rw-r--  2.0 unx     5284 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/_microsoft_resource_health.py
--rw-rw-r--  2.0 unx      856 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/__init__.py
--rw-rw-r--  2.0 unx    20523 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_availability_statuses_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     7268 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_resources_operations.py
--rw-rw-r--  2.0 unx    10755 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_availability_statuses_operations.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_operations.py
--rw-rw-r--  2.0 unx     1107 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     3356 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/aio/_configuration.py
--rw-rw-r--  2.0 unx    10389 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/aio/_microsoft_resource_health.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Feb-16 08:21 azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/aio/__init__.py
-96 files, 507414 bytes uncompressed, 113031 bytes compressed:  77.7%
+Zip file size: 222916 bytes, number of entries: 139
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/
+-rw-rw-r--  2.0 unx     6361 b- defN 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/setup.cfg
+-rw-rw-r--  2.0 unx      220 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/MANIFEST.in
+-rw-rw-r--  2.0 unx     1074 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/LICENSE
+-rw-rw-r--  2.0 unx     2183 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/README.md
+-rw-rw-r--  2.0 unx      638 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/_meta.json
+-rw-rw-r--  2.0 unx     2843 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/setup.py
+-rw-rw-r--  2.0 unx     3274 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/CHANGELOG.md
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/aio/
+-rw-rw-r--  2.0 unx      729 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/__init__.py
+-rw-rw-r--  2.0 unx      360 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/models.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/py.typed
+-rw-rw-r--  2.0 unx    14412 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_resource_health_mgmt_client.py
+-rw-rw-r--  2.0 unx     3185 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_configuration.py
+-rw-rw-r--  2.0 unx      347 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_version.py
+-rw-rw-r--  2.0 unx    78854 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_serialization.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/
+-rw-rw-r--  2.0 unx      913 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/__init__.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_vendor.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_patch.py
+-rw-rw-r--  2.0 unx     5164 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_resource_health_mgmt_client.py
+-rw-rw-r--  2.0 unx     3614 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_version.py
+-rw-rw-r--  2.0 unx     1885 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/__init__.py
+-rw-rw-r--  2.0 unx    26491 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx      937 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/_resource_health_mgmt_client_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/_patch.py
+-rw-rw-r--  2.0 unx     1107 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/__init__.py
+-rw-rw-r--  2.0 unx    25436 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx    12964 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_patch.py
+-rw-rw-r--  2.0 unx     8281 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_resources_operations.py
+-rw-rw-r--  2.0 unx     5032 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/
+-rw-rw-r--  2.0 unx      860 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/_patch.py
+-rw-rw-r--  2.0 unx     5312 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/_resource_health_mgmt_client.py
+-rw-rw-r--  2.0 unx     3662 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx     1107 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    20338 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx    10546 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     7051 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_resources_operations.py
+-rw-rw-r--  2.0 unx     4284 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/
+-rw-rw-r--  2.0 unx      913 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/__init__.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_vendor.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_patch.py
+-rw-rw-r--  2.0 unx     5270 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_resource_health_mgmt_client.py
+-rw-rw-r--  2.0 unx     3614 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_version.py
+-rw-rw-r--  2.0 unx     4095 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/__init__.py
+-rw-rw-r--  2.0 unx    74217 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx     2800 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/_resource_health_mgmt_client_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/_patch.py
+-rw-rw-r--  2.0 unx     1127 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/__init__.py
+-rw-rw-r--  2.0 unx     9771 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_metadata_operations.py
+-rw-rw-r--  2.0 unx    14809 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_events_operations.py
+-rw-rw-r--  2.0 unx    26055 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_patch.py
+-rw-rw-r--  2.0 unx     5032 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_operations.py
+-rw-rw-r--  2.0 unx    10043 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_emerging_issues_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/
+-rw-rw-r--  2.0 unx      860 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/_patch.py
+-rw-rw-r--  2.0 unx     5422 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/_resource_health_mgmt_client.py
+-rw-rw-r--  2.0 unx     3662 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx     1127 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     8226 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_metadata_operations.py
+-rw-rw-r--  2.0 unx    12230 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_events_operations.py
+-rw-rw-r--  2.0 unx    20957 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     4284 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx     8443 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_emerging_issues_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/
+-rw-rw-r--  2.0 unx      913 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/__init__.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_vendor.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_patch.py
+-rw-rw-r--  2.0 unx     7034 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_resource_health_mgmt_client.py
+-rw-rw-r--  2.0 unx     3499 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_version.py
+-rw-rw-r--  2.0 unx     4821 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/__init__.py
+-rw-rw-r--  2.0 unx    92319 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx     3262 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/_resource_health_mgmt_client_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/_patch.py
+-rw-rw-r--  2.0 unx     1691 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/__init__.py
+-rw-rw-r--  2.0 unx    19094 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_event_operations.py
+-rw-rw-r--  2.0 unx     9771 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_metadata_operations.py
+-rw-rw-r--  2.0 unx    21891 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_impacted_resources_operations.py
+-rw-rw-r--  2.0 unx    19085 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_events_operations.py
+-rw-rw-r--  2.0 unx    25289 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx    12964 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_child_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx    13852 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_security_advisory_impacted_resources_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_patch.py
+-rw-rw-r--  2.0 unx     8281 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_child_resources_operations.py
+-rw-rw-r--  2.0 unx     5032 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_operations.py
+-rw-rw-r--  2.0 unx    10082 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_emerging_issues_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/
+-rw-rw-r--  2.0 unx      860 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/_patch.py
+-rw-rw-r--  2.0 unx     7206 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/_resource_health_mgmt_client.py
+-rw-rw-r--  2.0 unx     3547 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx     1691 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    14142 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_event_operations.py
+-rw-rw-r--  2.0 unx     8226 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_metadata_operations.py
+-rw-rw-r--  2.0 unx    16947 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_impacted_resources_operations.py
+-rw-rw-r--  2.0 unx    15768 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_events_operations.py
+-rw-rw-r--  2.0 unx    20112 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx    10546 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_child_availability_statuses_operations.py
+-rw-rw-r--  2.0 unx    11374 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_security_advisory_impacted_resources_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     7051 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_child_resources_operations.py
+-rw-rw-r--  2.0 unx     4284 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx     8483 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_emerging_issues_operations.py
+-rw-rw-r--  2.0 unx      574 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/aio/__init__.py
+-rw-rw-r--  2.0 unx    14676 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/aio/_resource_health_mgmt_client.py
+-rw-rw-r--  2.0 unx     3249 b- defN 23-May-22 09:06 azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/aio/_configuration.py
+-rw-rw-r--  2.0 unx     6361 b- defN 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     7106 b- defN 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx      124 b- defN 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-22 09:08 azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/dependency_links.txt
+139 files, 919310 bytes uncompressed, 187284 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -1,289 +1,418 @@
-Filename: azure-mgmt-resourcehealth-1.0.0b3/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/setup.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/CHANGELOG.md
+Filename: azure-mgmt-resourcehealth-1.0.0b4/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/setup.cfg
+Filename: azure-mgmt-resourcehealth-1.0.0b4/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/LICENSE
+Filename: azure-mgmt-resourcehealth-1.0.0b4/LICENSE
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/MANIFEST.in
+Filename: azure-mgmt-resourcehealth-1.0.0b4/README.md
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/_meta.json
+Filename: azure-mgmt-resourcehealth-1.0.0b4/_meta.json
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/README.md
+Filename: azure-mgmt-resourcehealth-1.0.0b4/setup.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/PKG-INFO
+Filename: azure-mgmt-resourcehealth-1.0.0b4/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/top_level.txt
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/SOURCES.txt
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/requires.txt
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/dependency_links.txt
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/not-zip-safe
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/PKG-INFO
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/aio/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/models.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/py.typed
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_resource_health_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/aio/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_configuration.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_version.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_version.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_microsoft_resource_health.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/py.typed
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/models.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_serialization.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_resource_health_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_configuration.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_version.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_version.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_microsoft_resource_health.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/_resource_health_mgmt_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_vendor.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_availability_statuses_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_availability_statuses_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_availability_statuses_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_emerging_issues_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_metadata_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_events_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/_microsoft_resource_health_enums.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/_resource_health_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/_models_py3.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_availability_statuses_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/_configuration.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_availability_statuses_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/_microsoft_resource_health.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_availability_statuses_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_emerging_issues_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_metadata_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_events_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_resource_health_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_version.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_configuration.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/_resource_health_mgmt_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_version.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_microsoft_resource_health.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_vendor.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_metadata_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_events_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_availability_statuses_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_availability_statuses_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_resources_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_availability_statuses_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_emerging_issues_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/_microsoft_resource_health_enums.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/_resource_health_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/_models_py3.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_metadata_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/_configuration.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_events_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_availability_statuses_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/_microsoft_resource_health.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_availability_statuses_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_emerging_issues_operations.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_patch.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_resources_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_availability_statuses_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_operations.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/aio/_configuration.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_patch.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/aio/_microsoft_resource_health.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_resource_health_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/aio/__init__.py
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_configuration.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/_version.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/__init__.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/_models_py3.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/_resource_health_mgmt_client_enums.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/models/_patch.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_event_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_metadata_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_impacted_resources_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_events_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_availability_statuses_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_child_availability_statuses_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_security_advisory_impacted_resources_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_patch.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_child_resources_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_emerging_issues_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/__init__.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/_patch.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/_resource_health_mgmt_client.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/_configuration.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_event_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_metadata_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_impacted_resources_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_events_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_availability_statuses_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_child_availability_statuses_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_security_advisory_impacted_resources_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_patch.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_child_resources_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_emerging_issues_operations.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/aio/__init__.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/aio/_resource_health_mgmt_client.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/aio/_configuration.py
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/PKG-INFO
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/not-zip-safe
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/requires.txt
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/setup.py` & `azure-mgmt-resourcehealth-1.0.0b4/setup.py`

 * *Files 2% similar despite different names*

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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/LICENSE` & `azure-mgmt-resourcehealth-1.0.0b4/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/_meta.json` & `azure-mgmt-resourcehealth-1.0.0b4/_meta.json`

 * *Files 26% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/resourcehealth/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.4.12 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'1fea23ac36b111293dc3efc30f725e9ebb790f7f'",*

 * * "'use'": " […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/resourcehealth/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.0 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "51d4c24a011e300b9713179e0515fef35bf3f678",
+    "autorest_command": "autorest specification/resourcehealth/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.12 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "1fea23ac36b111293dc3efc30f725e9ebb790f7f",
     "readme": "specification/resourcehealth/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.4.0",
+        "@autorest/python@6.4.12",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/README.md` & `azure-mgmt-resourcehealth-1.0.0b4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,25 +32,26 @@
 
 In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
 
 With above configuration, client can be authenticated by following code:
 
 ```python
 from azure.identity import DefaultAzureCredential
-from azure.mgmt.resourcehealth import MicrosoftResourceHealth
+from azure.mgmt.resourcehealth import ResourceHealthMgmtClient
 import os
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
-client = MicrosoftResourceHealth(credential=DefaultAzureCredential(), subscription_id=sub_id)
+client = ResourceHealthMgmtClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Resource Health Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Resource Health Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure_mgmt_resourcehealth.egg-info/SOURCES.txt` & `azure-mgmt-resourcehealth-1.0.0b4/azure_mgmt_resourcehealth.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -4,75 +4,113 @@
 README.md
 _meta.json
 setup.py
 azure/__init__.py
 azure/mgmt/__init__.py
 azure/mgmt/resourcehealth/__init__.py
 azure/mgmt/resourcehealth/_configuration.py
-azure/mgmt/resourcehealth/_microsoft_resource_health.py
+azure/mgmt/resourcehealth/_resource_health_mgmt_client.py
 azure/mgmt/resourcehealth/_serialization.py
 azure/mgmt/resourcehealth/_version.py
 azure/mgmt/resourcehealth/models.py
 azure/mgmt/resourcehealth/py.typed
 azure/mgmt/resourcehealth/aio/__init__.py
 azure/mgmt/resourcehealth/aio/_configuration.py
-azure/mgmt/resourcehealth/aio/_microsoft_resource_health.py
+azure/mgmt/resourcehealth/aio/_resource_health_mgmt_client.py
 azure/mgmt/resourcehealth/v2015_01_01/__init__.py
 azure/mgmt/resourcehealth/v2015_01_01/_configuration.py
-azure/mgmt/resourcehealth/v2015_01_01/_microsoft_resource_health.py
 azure/mgmt/resourcehealth/v2015_01_01/_patch.py
+azure/mgmt/resourcehealth/v2015_01_01/_resource_health_mgmt_client.py
 azure/mgmt/resourcehealth/v2015_01_01/_vendor.py
 azure/mgmt/resourcehealth/v2015_01_01/_version.py
 azure/mgmt/resourcehealth/v2015_01_01/aio/__init__.py
 azure/mgmt/resourcehealth/v2015_01_01/aio/_configuration.py
-azure/mgmt/resourcehealth/v2015_01_01/aio/_microsoft_resource_health.py
 azure/mgmt/resourcehealth/v2015_01_01/aio/_patch.py
+azure/mgmt/resourcehealth/v2015_01_01/aio/_resource_health_mgmt_client.py
 azure/mgmt/resourcehealth/v2015_01_01/aio/operations/__init__.py
 azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_availability_statuses_operations.py
 azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_availability_statuses_operations.py
 azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_resources_operations.py
 azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_operations.py
 azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_patch.py
 azure/mgmt/resourcehealth/v2015_01_01/models/__init__.py
-azure/mgmt/resourcehealth/v2015_01_01/models/_microsoft_resource_health_enums.py
 azure/mgmt/resourcehealth/v2015_01_01/models/_models_py3.py
 azure/mgmt/resourcehealth/v2015_01_01/models/_patch.py
+azure/mgmt/resourcehealth/v2015_01_01/models/_resource_health_mgmt_client_enums.py
 azure/mgmt/resourcehealth/v2015_01_01/operations/__init__.py
 azure/mgmt/resourcehealth/v2015_01_01/operations/_availability_statuses_operations.py
 azure/mgmt/resourcehealth/v2015_01_01/operations/_child_availability_statuses_operations.py
 azure/mgmt/resourcehealth/v2015_01_01/operations/_child_resources_operations.py
 azure/mgmt/resourcehealth/v2015_01_01/operations/_operations.py
 azure/mgmt/resourcehealth/v2015_01_01/operations/_patch.py
 azure/mgmt/resourcehealth/v2018_07_01/__init__.py
 azure/mgmt/resourcehealth/v2018_07_01/_configuration.py
-azure/mgmt/resourcehealth/v2018_07_01/_microsoft_resource_health.py
 azure/mgmt/resourcehealth/v2018_07_01/_patch.py
+azure/mgmt/resourcehealth/v2018_07_01/_resource_health_mgmt_client.py
 azure/mgmt/resourcehealth/v2018_07_01/_vendor.py
 azure/mgmt/resourcehealth/v2018_07_01/_version.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/__init__.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/_configuration.py
-azure/mgmt/resourcehealth/v2018_07_01/aio/_microsoft_resource_health.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/_patch.py
+azure/mgmt/resourcehealth/v2018_07_01/aio/_resource_health_mgmt_client.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/operations/__init__.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_availability_statuses_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_emerging_issues_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_events_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_metadata_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_patch.py
 azure/mgmt/resourcehealth/v2018_07_01/models/__init__.py
-azure/mgmt/resourcehealth/v2018_07_01/models/_microsoft_resource_health_enums.py
 azure/mgmt/resourcehealth/v2018_07_01/models/_models_py3.py
 azure/mgmt/resourcehealth/v2018_07_01/models/_patch.py
+azure/mgmt/resourcehealth/v2018_07_01/models/_resource_health_mgmt_client_enums.py
 azure/mgmt/resourcehealth/v2018_07_01/operations/__init__.py
 azure/mgmt/resourcehealth/v2018_07_01/operations/_availability_statuses_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/operations/_emerging_issues_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/operations/_events_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/operations/_metadata_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/operations/_operations.py
 azure/mgmt/resourcehealth/v2018_07_01/operations/_patch.py
+azure/mgmt/resourcehealth/v2022_10_01/__init__.py
+azure/mgmt/resourcehealth/v2022_10_01/_configuration.py
+azure/mgmt/resourcehealth/v2022_10_01/_patch.py
+azure/mgmt/resourcehealth/v2022_10_01/_resource_health_mgmt_client.py
+azure/mgmt/resourcehealth/v2022_10_01/_vendor.py
+azure/mgmt/resourcehealth/v2022_10_01/_version.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/__init__.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/_configuration.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/_patch.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/_resource_health_mgmt_client.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/__init__.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_availability_statuses_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_child_availability_statuses_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_child_resources_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_emerging_issues_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_event_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_events_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_impacted_resources_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_metadata_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_patch.py
+azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_security_advisory_impacted_resources_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/models/__init__.py
+azure/mgmt/resourcehealth/v2022_10_01/models/_models_py3.py
+azure/mgmt/resourcehealth/v2022_10_01/models/_patch.py
+azure/mgmt/resourcehealth/v2022_10_01/models/_resource_health_mgmt_client_enums.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/__init__.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_availability_statuses_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_child_availability_statuses_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_child_resources_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_emerging_issues_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_event_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_events_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_impacted_resources_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_metadata_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_operations.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_patch.py
+azure/mgmt/resourcehealth/v2022_10_01/operations/_security_advisory_impacted_resources_operations.py
 azure_mgmt_resourcehealth.egg-info/PKG-INFO
 azure_mgmt_resourcehealth.egg-info/SOURCES.txt
 azure_mgmt_resourcehealth.egg-info/dependency_links.txt
 azure_mgmt_resourcehealth.egg-info/not-zip-safe
 azure_mgmt_resourcehealth.egg-info/requires.txt
 azure_mgmt_resourcehealth.egg-info/top_level.txt
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_configuration.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/aio/_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,60 +8,60 @@
 # Changes may cause incorrect behavior and will be lost if the code is
 # regenerated.
 # --------------------------------------------------------------------------
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
+from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
-class MicrosoftResourceHealthConfiguration(Configuration):
-    """Configuration for MicrosoftResourceHealth.
+class ResourceHealthMgmtClientConfiguration(Configuration):
+    """Configuration for ResourceHealthMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call. Required.
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     """
 
     def __init__(
         self,
-        credential: "TokenCredential",
+        credential: "AsyncTokenCredential",
         subscription_id: str,
         **kwargs: Any
-    ):
+    ) -> None:
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
-        super(MicrosoftResourceHealthConfiguration, self).__init__(**kwargs)
+        super(ResourceHealthMgmtClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'azure-mgmt-resourcehealth/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs: Any
-    ):
+    ) -> None:
         self.user_agent_policy = kwargs.get('user_agent_policy') or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get('headers_policy') or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get('proxy_policy') or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get('logging_policy') or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get('http_logging_policy') or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get('retry_policy') or policies.RetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get('retry_policy') or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get('custom_hook_policy') or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get('redirect_policy') or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get('redirect_policy') or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get('authentication_policy')
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = ARMChallengeAuthenticationPolicy(self.credential, *self.credential_scopes, **kwargs)
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(self.credential, *self.credential_scopes, **kwargs)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_microsoft_resource_health.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_resource_health_mgmt_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,201 +11,266 @@
 
 from typing import Any, Optional, TYPE_CHECKING
 
 from azure.mgmt.core import ARMPipelineClient
 from azure.profiles import KnownProfiles, ProfileDefinition
 from azure.profiles.multiapiclient import MultiApiClientMixin
 
-from ._configuration import MicrosoftResourceHealthConfiguration
+from ._configuration import ResourceHealthMgmtClientConfiguration
 from ._serialization import Deserializer, Serializer
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 class _SDKClient(object):
     def __init__(self, *args, **kwargs):
         """This is a fake class to support current implemetation of MultiApiClientMixin."
         Will be removed in final version of multiapi azure-core based client
         """
         pass
 
-class MicrosoftResourceHealth(MultiApiClientMixin, _SDKClient):
+class ResourceHealthMgmtClient(MultiApiClientMixin, _SDKClient):
     """The Resource Health Client.
 
     This ready contains multiple API versions, to help you deal with all of the Azure clouds
     (Azure Stack, Azure Government, Azure China, etc.).
     By default, it uses the latest API version available on public Azure.
     For production, you should stick to a particular api-version and/or profile.
     The profile sets a mapping between an operation group and its API version.
     The api-version parameter sets the default API version if the operation
     group is not described in the profile.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param api_version: API version to use if no profile is provided, or if missing in profile.
     :type api_version: str
     :param base_url: Service URL
     :type base_url: str
     :param profile: A profile definition, from KnownProfiles to dict.
     :type profile: azure.profiles.KnownProfiles
     """
 
-    DEFAULT_API_VERSION = '2018-07-01'
-    _PROFILE_TAG = "azure.mgmt.resourcehealth.MicrosoftResourceHealth"
+    DEFAULT_API_VERSION = '2022-10-01'
+    _PROFILE_TAG = "azure.mgmt.resourcehealth.ResourceHealthMgmtClient"
     LATEST_PROFILE = ProfileDefinition({
         _PROFILE_TAG: {
             None: DEFAULT_API_VERSION,
-            'child_availability_statuses': '2015-01-01',
-            'child_resources': '2015-01-01',
         }},
         _PROFILE_TAG + " latest"
     )
 
     def __init__(
         self,
         credential: "TokenCredential",
         subscription_id: str,
         api_version: Optional[str]=None,
         base_url: str = "https://management.azure.com",
         profile: KnownProfiles=KnownProfiles.default,
         **kwargs: Any
     ):
-        self._config = MicrosoftResourceHealthConfiguration(credential, subscription_id, **kwargs)
+        self._config = ResourceHealthMgmtClientConfiguration(credential, subscription_id, **kwargs)
         self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
-        super(MicrosoftResourceHealth, self).__init__(
+        super(ResourceHealthMgmtClient, self).__init__(
             api_version=api_version,
             profile=profile
         )
 
     @classmethod
     def _models_dict(cls, api_version):
         return {k: v for k, v in cls.models(api_version).__dict__.items() if isinstance(v, type)}
 
     @classmethod
     def models(cls, api_version=DEFAULT_API_VERSION):
         """Module depends on the API version:
 
            * 2015-01-01: :mod:`v2015_01_01.models<azure.mgmt.resourcehealth.v2015_01_01.models>`
            * 2018-07-01: :mod:`v2018_07_01.models<azure.mgmt.resourcehealth.v2018_07_01.models>`
+           * 2022-10-01: :mod:`v2022_10_01.models<azure.mgmt.resourcehealth.v2022_10_01.models>`
         """
         if api_version == '2015-01-01':
             from .v2015_01_01 import models
             return models
         elif api_version == '2018-07-01':
             from .v2018_07_01 import models
             return models
+        elif api_version == '2022-10-01':
+            from .v2022_10_01 import models
+            return models
         raise ValueError("API version {} is not available".format(api_version))
 
     @property
     def availability_statuses(self):
         """Instance depends on the API version:
 
            * 2015-01-01: :class:`AvailabilityStatusesOperations<azure.mgmt.resourcehealth.v2015_01_01.operations.AvailabilityStatusesOperations>`
            * 2018-07-01: :class:`AvailabilityStatusesOperations<azure.mgmt.resourcehealth.v2018_07_01.operations.AvailabilityStatusesOperations>`
+           * 2022-10-01: :class:`AvailabilityStatusesOperations<azure.mgmt.resourcehealth.v2022_10_01.operations.AvailabilityStatusesOperations>`
         """
         api_version = self._get_api_version('availability_statuses')
         if api_version == '2015-01-01':
             from .v2015_01_01.operations import AvailabilityStatusesOperations as OperationClass
         elif api_version == '2018-07-01':
             from .v2018_07_01.operations import AvailabilityStatusesOperations as OperationClass
+        elif api_version == '2022-10-01':
+            from .v2022_10_01.operations import AvailabilityStatusesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'availability_statuses'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def child_availability_statuses(self):
         """Instance depends on the API version:
 
            * 2015-01-01: :class:`ChildAvailabilityStatusesOperations<azure.mgmt.resourcehealth.v2015_01_01.operations.ChildAvailabilityStatusesOperations>`
+           * 2022-10-01: :class:`ChildAvailabilityStatusesOperations<azure.mgmt.resourcehealth.v2022_10_01.operations.ChildAvailabilityStatusesOperations>`
         """
         api_version = self._get_api_version('child_availability_statuses')
         if api_version == '2015-01-01':
             from .v2015_01_01.operations import ChildAvailabilityStatusesOperations as OperationClass
+        elif api_version == '2022-10-01':
+            from .v2022_10_01.operations import ChildAvailabilityStatusesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'child_availability_statuses'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def child_resources(self):
         """Instance depends on the API version:
 
            * 2015-01-01: :class:`ChildResourcesOperations<azure.mgmt.resourcehealth.v2015_01_01.operations.ChildResourcesOperations>`
+           * 2022-10-01: :class:`ChildResourcesOperations<azure.mgmt.resourcehealth.v2022_10_01.operations.ChildResourcesOperations>`
         """
         api_version = self._get_api_version('child_resources')
         if api_version == '2015-01-01':
             from .v2015_01_01.operations import ChildResourcesOperations as OperationClass
+        elif api_version == '2022-10-01':
+            from .v2022_10_01.operations import ChildResourcesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'child_resources'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def emerging_issues(self):
         """Instance depends on the API version:
 
            * 2018-07-01: :class:`EmergingIssuesOperations<azure.mgmt.resourcehealth.v2018_07_01.operations.EmergingIssuesOperations>`
+           * 2022-10-01: :class:`EmergingIssuesOperations<azure.mgmt.resourcehealth.v2022_10_01.operations.EmergingIssuesOperations>`
         """
         api_version = self._get_api_version('emerging_issues')
         if api_version == '2018-07-01':
             from .v2018_07_01.operations import EmergingIssuesOperations as OperationClass
+        elif api_version == '2022-10-01':
+            from .v2022_10_01.operations import EmergingIssuesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'emerging_issues'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
+    def event(self):
+        """Instance depends on the API version:
+
+           * 2022-10-01: :class:`EventOperations<azure.mgmt.resourcehealth.v2022_10_01.operations.EventOperations>`
+        """
+        api_version = self._get_api_version('event')
+        if api_version == '2022-10-01':
+            from .v2022_10_01.operations import EventOperations as OperationClass
+        else:
+            raise ValueError("API version {} does not have operation group 'event'".format(api_version))
+        self._config.api_version = api_version
+        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
+
+    @property
     def events(self):
         """Instance depends on the API version:
 
            * 2018-07-01: :class:`EventsOperations<azure.mgmt.resourcehealth.v2018_07_01.operations.EventsOperations>`
+           * 2022-10-01: :class:`EventsOperations<azure.mgmt.resourcehealth.v2022_10_01.operations.EventsOperations>`
         """
         api_version = self._get_api_version('events')
         if api_version == '2018-07-01':
             from .v2018_07_01.operations import EventsOperations as OperationClass
+        elif api_version == '2022-10-01':
+            from .v2022_10_01.operations import EventsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'events'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
+    def impacted_resources(self):
+        """Instance depends on the API version:
+
+           * 2022-10-01: :class:`ImpactedResourcesOperations<azure.mgmt.resourcehealth.v2022_10_01.operations.ImpactedResourcesOperations>`
+        """
+        api_version = self._get_api_version('impacted_resources')
+        if api_version == '2022-10-01':
+            from .v2022_10_01.operations import ImpactedResourcesOperations as OperationClass
+        else:
+            raise ValueError("API version {} does not have operation group 'impacted_resources'".format(api_version))
+        self._config.api_version = api_version
+        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
+
+    @property
     def metadata(self):
         """Instance depends on the API version:
 
            * 2018-07-01: :class:`MetadataOperations<azure.mgmt.resourcehealth.v2018_07_01.operations.MetadataOperations>`
+           * 2022-10-01: :class:`MetadataOperations<azure.mgmt.resourcehealth.v2022_10_01.operations.MetadataOperations>`
         """
         api_version = self._get_api_version('metadata')
         if api_version == '2018-07-01':
             from .v2018_07_01.operations import MetadataOperations as OperationClass
+        elif api_version == '2022-10-01':
+            from .v2022_10_01.operations import MetadataOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'metadata'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def operations(self):
         """Instance depends on the API version:
 
            * 2015-01-01: :class:`Operations<azure.mgmt.resourcehealth.v2015_01_01.operations.Operations>`
            * 2018-07-01: :class:`Operations<azure.mgmt.resourcehealth.v2018_07_01.operations.Operations>`
+           * 2022-10-01: :class:`Operations<azure.mgmt.resourcehealth.v2022_10_01.operations.Operations>`
         """
         api_version = self._get_api_version('operations')
         if api_version == '2015-01-01':
             from .v2015_01_01.operations import Operations as OperationClass
         elif api_version == '2018-07-01':
             from .v2018_07_01.operations import Operations as OperationClass
+        elif api_version == '2022-10-01':
+            from .v2022_10_01.operations import Operations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'operations'".format(api_version))
         self._config.api_version = api_version
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
+    @property
+    def security_advisory_impacted_resources(self):
+        """Instance depends on the API version:
+
+           * 2022-10-01: :class:`SecurityAdvisoryImpactedResourcesOperations<azure.mgmt.resourcehealth.v2022_10_01.operations.SecurityAdvisoryImpactedResourcesOperations>`
+        """
+        api_version = self._get_api_version('security_advisory_impacted_resources')
+        if api_version == '2022-10-01':
+            from .v2022_10_01.operations import SecurityAdvisoryImpactedResourcesOperations as OperationClass
+        else:
+            raise ValueError("API version {} does not have operation group 'security_advisory_impacted_resources'".format(api_version))
+        self._config.api_version = api_version
+        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
+
     def close(self):
         self._client.close()
     def __enter__(self):
         self._client.__enter__()
         return self
     def __exit__(self, *exc_details):
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/_serialization.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
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
@@ -1269,15 +1269,15 @@
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
 
@@ -1293,15 +1293,15 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/__init__.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._microsoft_resource_health import MicrosoftResourceHealth
-__all__ = ['MicrosoftResourceHealth']
+from ._resource_health_mgmt_client import ResourceHealthMgmtClient
+__all__ = ['ResourceHealthMgmtClient']
 
 try:
     from ._patch import patch_sdk  # type: ignore
     patch_sdk()
 except ImportError:
     pass
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_configuration.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,29 @@
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
 
 
-class MicrosoftResourceHealthConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
-    """Configuration for MicrosoftResourceHealth.
+class ResourceHealthMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for ResourceHealthMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
@@ -38,16 +32,16 @@
     :type subscription_id: str
     :keyword api_version: Api Version. Default value is "2018-07-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(MicrosoftResourceHealthConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", "2018-07-01")
+        super(ResourceHealthMgmtClientConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2018-07-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_microsoft_resource_health.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_resource_health_mgmt_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 from typing import Any, TYPE_CHECKING
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
 from . import models as _models
 from .._serialization import Deserializer, Serializer
-from ._configuration import MicrosoftResourceHealthConfiguration
+from ._configuration import ResourceHealthMgmtClientConfiguration
 from .operations import (
     AvailabilityStatusesOperations,
     EmergingIssuesOperations,
     EventsOperations,
     MetadataOperations,
     Operations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class MicrosoftResourceHealth:  # pylint: disable=client-accepts-api-version-keyword
+class ResourceHealthMgmtClient:  # pylint: disable=client-accepts-api-version-keyword
     """The Resource Health Client.
 
     :ivar events: EventsOperations operations
     :vartype events: azure.mgmt.resourcehealth.v2018_07_01.operations.EventsOperations
     :ivar availability_statuses: AvailabilityStatusesOperations operations
     :vartype availability_statuses:
      azure.mgmt.resourcehealth.v2018_07_01.operations.AvailabilityStatusesOperations
@@ -58,18 +58,18 @@
     def __init__(
         self,
         credential: "TokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
-        self._config = MicrosoftResourceHealthConfiguration(
+        self._config = ResourceHealthMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.events = EventsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.availability_statuses = AvailabilityStatusesOperations(
@@ -100,13 +100,13 @@
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
     def close(self) -> None:
         self._client.close()
 
-    def __enter__(self) -> "MicrosoftResourceHealth":
+    def __enter__(self) -> "ResourceHealthMgmtClient":
         self._client.__enter__()
         return self
 
     def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/_vendor.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_availability_statuses_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_availability_statuses_operations.py`

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
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_subscription_id_request(
     subscription_id: str, *, filter: Optional[str] = None, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.ResourceHealth/availabilityStatuses"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -80,15 +75,15 @@
     filter: Optional[str] = None,
     expand: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ResourceHealth/availabilityStatuses",
     )  # pylint: disable=line-too-long
@@ -114,15 +109,15 @@
 
 def build_get_by_resource_request(
     resource_uri: str, *, filter: Optional[str] = None, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{resourceUri}/providers/Microsoft.ResourceHealth/availabilityStatuses/current")
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -144,15 +139,15 @@
 
 def build_list_request(
     resource_uri: str, *, filter: Optional[str] = None, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{resourceUri}/providers/Microsoft.ResourceHealth/availabilityStatuses")
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -174,15 +169,15 @@
 
 class AvailabilityStatusesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2018_07_01.ResourceHealthMgmtClient`'s
         :attr:`availability_statuses` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -211,15 +206,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -265,16 +260,17 @@
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
@@ -309,15 +305,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -364,16 +360,17 @@
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
@@ -420,31 +417,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.AvailabilityStatus] = kwargs.pop("cls", None)
 
         request = build_get_by_resource_request(
             resource_uri=resource_uri,
             filter=filter,
             expand=expand,
             api_version=api_version,
             template_url=self.get_by_resource.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -486,15 +484,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -540,16 +538,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_emerging_issues_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_emerging_issues_operations.py`

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
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar, Union
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,58 +25,54 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_get_request(issue_name: Union[str, _models.Enum8], **kwargs: Any) -> HttpRequest:
+def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.ResourceHealth/emergingIssues/{issueName}")
-    path_format_arguments = {
-        "issueName": _SERIALIZER.url("issue_name", issue_name, "str"),
-    }
-
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url = kwargs.pop("template_url", "/providers/Microsoft.ResourceHealth/emergingIssues")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_request(**kwargs: Any) -> HttpRequest:
+def build_get_request(issue_name: Union[str, _models.IssueNameParameter], **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.ResourceHealth/emergingIssues")
+    _url = kwargs.pop("template_url", "/providers/Microsoft.ResourceHealth/emergingIssues/{issueName}")
+    path_format_arguments = {
+        "issueName": _SERIALIZER.url("issue_name", issue_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -86,97 +81,42 @@
 
 class EmergingIssuesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2022_10_01.ResourceHealthMgmtClient`'s
         :attr:`emerging_issues` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def get(self, issue_name: Union[str, _models.Enum8], **kwargs: Any) -> _models.EmergingIssuesGetResult:
-        """Gets Azure services' emerging issues.
-
-        :param issue_name: The name of the emerging issue. "default" Required.
-        :type issue_name: str or ~azure.mgmt.resourcehealth.v2018_07_01.models.Enum8
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: EmergingIssuesGetResult or the result of cls(response)
-        :rtype: ~azure.mgmt.resourcehealth.v2018_07_01.models.EmergingIssuesGetResult
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
-        cls: ClsType[_models.EmergingIssuesGetResult] = kwargs.pop("cls", None)
-
-        request = build_get_request(
-            issue_name=issue_name,
-            api_version=api_version,
-            template_url=self.get.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("EmergingIssuesGetResult", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
-    get.metadata = {"url": "/providers/Microsoft.ResourceHealth/emergingIssues/{issueName}"}
-
-    @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.EmergingIssuesGetResult"]:
         """Lists Azure services' emerging issues.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EmergingIssuesGetResult or the result of
          cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.EmergingIssuesGetResult]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2022_10_01.models.EmergingIssuesGetResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
         cls: ClsType[_models.EmergingIssueListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -219,22 +159,79 @@
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
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     list.metadata = {"url": "/providers/Microsoft.ResourceHealth/emergingIssues"}
+
+    @distributed_trace
+    def get(self, issue_name: Union[str, _models.IssueNameParameter], **kwargs: Any) -> _models.EmergingIssuesGetResult:
+        """Gets Azure services' emerging issues.
+
+        :param issue_name: The name of the emerging issue. "default" Required.
+        :type issue_name: str or ~azure.mgmt.resourcehealth.v2022_10_01.models.IssueNameParameter
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: EmergingIssuesGetResult or the result of cls(response)
+        :rtype: ~azure.mgmt.resourcehealth.v2022_10_01.models.EmergingIssuesGetResult
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
+        cls: ClsType[_models.EmergingIssuesGetResult] = kwargs.pop("cls", None)
+
+        request = build_get_request(
+            issue_name=issue_name,
+            api_version=api_version,
+            template_url=self.get.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("EmergingIssuesGetResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    get.metadata = {"url": "/providers/Microsoft.ResourceHealth/emergingIssues/{issueName}"}
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_metadata_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_metadata_operations.py`

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
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
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
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.ResourceHealth/metadata")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -60,15 +55,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_entity_request(name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.ResourceHealth/metadata/{name}")
     path_format_arguments = {
         "name": _SERIALIZER.url("name", name, "str"),
     }
@@ -86,15 +81,15 @@
 
 class MetadataOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2018_07_01.ResourceHealthMgmtClient`'s
         :attr:`metadata` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -112,15 +107,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.MetadataEntity]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.MetadataEntityListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -163,16 +158,17 @@
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
@@ -201,29 +197,30 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.MetadataEntity] = kwargs.pop("cls", None)
 
         request = build_get_entity_request(
             name=name,
             api_version=api_version,
             template_url=self.get_entity.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_operations.py`

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
 from ..._serialization import Serializer
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
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.ResourceHealth/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -60,15 +55,15 @@
 
 class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2015_01_01.ResourceHealthMgmtClient`'s
         :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -79,42 +74,43 @@
 
     @distributed_trace
     def list(self, **kwargs: Any) -> _models.OperationListResult:
         """Lists available operations for the resourcehealth resource provider.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: OperationListResult or the result of cls(response)
-        :rtype: ~azure.mgmt.resourcehealth.v2018_07_01.models.OperationListResult
+        :rtype: ~azure.mgmt.resourcehealth.v2015_01_01.models.OperationListResult
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
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         request = build_list_request(
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/_events_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_events_operations.py`

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
 from ..._serialization import Serializer
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
     query_start_time: Optional[str] = None,
     view: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.ResourceHealth/events")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
@@ -80,15 +75,15 @@
 
 def build_list_by_single_resource_request(
     resource_uri: str, *, filter: Optional[str] = None, view: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{resourceUri}/providers/Microsoft.ResourceHealth/events")
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -110,15 +105,15 @@
 
 class EventsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2018_07_01.ResourceHealthMgmtClient`'s
         :attr:`events` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -153,15 +148,15 @@
         :return: An iterator like instance of either Event or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.Event]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.Events] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -208,16 +203,17 @@
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
@@ -255,15 +251,15 @@
         :return: An iterator like instance of either Event or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.Event]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.Events] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -309,16 +305,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/operations/__init__.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/_microsoft_resource_health_enums.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/_resource_health_mgmt_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/_models_py3.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,24 @@
     :vartype summary: str
     :ivar detailed_status: Details of the availability status.
     :vartype detailed_status: str
     :ivar reason_type: When the resource's availabilityState is Unavailable, it describes where the
      health impacting event was originated. Examples are planned, unplanned, user initiated or an
      outage etc.
     :vartype reason_type: str
+    :ivar context: When an event is created, it can either be triggered by a customer or the
+     platform of the resource and this field will illustrate that. This field is connected to the
+     category field in this object.
+    :vartype context: str
+    :ivar category: When a context field is set to Platform, this field will reflect if the event
+     was planned or unplanned. If the context field does not have a value of Platform, then this
+     field will be ignored.
+    :vartype category: str
+    :ivar article_id: The Article Id.
+    :vartype article_id: str
     :ivar root_cause_attribution_time: When the resource's availabilityState is Unavailable, it
      provides the Timestamp for when the health impacting event was received.
     :vartype root_cause_attribution_time: ~datetime.datetime
     :ivar health_event_type: In case of an availability impacting event, it describes when the
      health impacting event was originated. Examples are Lifecycle, Downtime, Fault Analysis etc.
     :vartype health_event_type: str
     :ivar health_event_cause: In case of an availability impacting event, it describes where the
@@ -171,14 +181,17 @@
     """
 
     _attribute_map = {
         "availability_state": {"key": "availabilityState", "type": "str"},
         "summary": {"key": "summary", "type": "str"},
         "detailed_status": {"key": "detailedStatus", "type": "str"},
         "reason_type": {"key": "reasonType", "type": "str"},
+        "context": {"key": "context", "type": "str"},
+        "category": {"key": "category", "type": "str"},
+        "article_id": {"key": "articleId", "type": "str"},
         "root_cause_attribution_time": {"key": "rootCauseAttributionTime", "type": "iso-8601"},
         "health_event_type": {"key": "healthEventType", "type": "str"},
         "health_event_cause": {"key": "healthEventCause", "type": "str"},
         "health_event_category": {"key": "healthEventCategory", "type": "str"},
         "health_event_id": {"key": "healthEventId", "type": "str"},
         "resolution_eta": {"key": "resolutionETA", "type": "iso-8601"},
         "occurred_time": {"key": "occurredTime", "type": "iso-8601"},
@@ -192,14 +205,17 @@
     def __init__(
         self,
         *,
         availability_state: Optional[Union[str, "_models.AvailabilityStateValues"]] = None,
         summary: Optional[str] = None,
         detailed_status: Optional[str] = None,
         reason_type: Optional[str] = None,
+        context: Optional[str] = None,
+        category: Optional[str] = None,
+        article_id: Optional[str] = None,
         root_cause_attribution_time: Optional[datetime.datetime] = None,
         health_event_type: Optional[str] = None,
         health_event_cause: Optional[str] = None,
         health_event_category: Optional[str] = None,
         health_event_id: Optional[str] = None,
         resolution_eta: Optional[datetime.datetime] = None,
         occurred_time: Optional[datetime.datetime] = None,
@@ -220,14 +236,24 @@
         :paramtype summary: str
         :keyword detailed_status: Details of the availability status.
         :paramtype detailed_status: str
         :keyword reason_type: When the resource's availabilityState is Unavailable, it describes where
          the health impacting event was originated. Examples are planned, unplanned, user initiated or
          an outage etc.
         :paramtype reason_type: str
+        :keyword context: When an event is created, it can either be triggered by a customer or the
+         platform of the resource and this field will illustrate that. This field is connected to the
+         category field in this object.
+        :paramtype context: str
+        :keyword category: When a context field is set to Platform, this field will reflect if the
+         event was planned or unplanned. If the context field does not have a value of Platform, then
+         this field will be ignored.
+        :paramtype category: str
+        :keyword article_id: The Article Id.
+        :paramtype article_id: str
         :keyword root_cause_attribution_time: When the resource's availabilityState is Unavailable, it
          provides the Timestamp for when the health impacting event was received.
         :paramtype root_cause_attribution_time: ~datetime.datetime
         :keyword health_event_type: In case of an availability impacting event, it describes when the
          health impacting event was originated. Examples are Lifecycle, Downtime, Fault Analysis etc.
         :paramtype health_event_type: str
         :keyword health_event_cause: In case of an availability impacting event, it describes where the
@@ -264,14 +290,17 @@
          list[~azure.mgmt.resourcehealth.v2018_07_01.models.ServiceImpactingEvent]
         """
         super().__init__(**kwargs)
         self.availability_state = availability_state
         self.summary = summary
         self.detailed_status = detailed_status
         self.reason_type = reason_type
+        self.context = context
+        self.category = category
+        self.article_id = article_id
         self.root_cause_attribution_time = root_cause_attribution_time
         self.health_event_type = health_event_type
         self.health_event_cause = health_event_cause
         self.health_event_category = health_event_category
         self.health_event_id = health_event_id
         self.resolution_eta = resolution_eta
         self.occurred_time = occurred_time
@@ -551,14 +580,16 @@
     :ivar header: Header text of event.
     :vartype header: str
     :ivar level: Level of insight. Known values are: "Critical" and "Warning".
     :vartype level: str or ~azure.mgmt.resourcehealth.v2018_07_01.models.LevelValues
     :ivar event_level: Level of event. Known values are: "Critical", "Error", "Warning", and
      "Informational".
     :vartype event_level: str or ~azure.mgmt.resourcehealth.v2018_07_01.models.EventLevelValues
+    :ivar reason: The reason for the Incident.
+    :vartype reason: str
     :ivar article: Article of event.
     :vartype article: ~azure.mgmt.resourcehealth.v2018_07_01.models.EventPropertiesArticle
     :ivar links: Useful links of event.
     :vartype links: list[~azure.mgmt.resourcehealth.v2018_07_01.models.Link]
     :ivar impact_start_time: It provides the Timestamp for when the health impacting event started.
     :vartype impact_start_time: ~datetime.datetime
     :ivar impact_mitigation_time: It provides the Timestamp for when the health impacting event
@@ -610,14 +641,15 @@
         "event_source": {"key": "properties.eventSource", "type": "str"},
         "status": {"key": "properties.status", "type": "str"},
         "title": {"key": "properties.title", "type": "str"},
         "summary": {"key": "properties.summary", "type": "str"},
         "header": {"key": "properties.header", "type": "str"},
         "level": {"key": "properties.level", "type": "str"},
         "event_level": {"key": "properties.eventLevel", "type": "str"},
+        "reason": {"key": "properties.reason", "type": "str"},
         "article": {"key": "properties.article", "type": "EventPropertiesArticle"},
         "links": {"key": "properties.links", "type": "[Link]"},
         "impact_start_time": {"key": "properties.impactStartTime", "type": "iso-8601"},
         "impact_mitigation_time": {"key": "properties.impactMitigationTime", "type": "iso-8601"},
         "impact": {"key": "properties.impact", "type": "[Impact]"},
         "recommended_actions": {"key": "properties.recommendedActions", "type": "EventPropertiesRecommendedActions"},
         "faqs": {"key": "properties.faqs", "type": "[Faq]"},
@@ -638,14 +670,15 @@
         event_source: Optional[Union[str, "_models.EventSourceValues"]] = None,
         status: Optional[Union[str, "_models.EventStatusValues"]] = None,
         title: Optional[str] = None,
         summary: Optional[str] = None,
         header: Optional[str] = None,
         level: Optional[Union[str, "_models.LevelValues"]] = None,
         event_level: Optional[Union[str, "_models.EventLevelValues"]] = None,
+        reason: Optional[str] = None,
         article: Optional["_models.EventPropertiesArticle"] = None,
         links: Optional[List["_models.Link"]] = None,
         impact_start_time: Optional[datetime.datetime] = None,
         impact_mitigation_time: Optional[datetime.datetime] = None,
         impact: Optional[List["_models.Impact"]] = None,
         recommended_actions: Optional["_models.EventPropertiesRecommendedActions"] = None,
         faqs: Optional[List["_models.Faq"]] = None,
@@ -674,14 +707,16 @@
         :keyword header: Header text of event.
         :paramtype header: str
         :keyword level: Level of insight. Known values are: "Critical" and "Warning".
         :paramtype level: str or ~azure.mgmt.resourcehealth.v2018_07_01.models.LevelValues
         :keyword event_level: Level of event. Known values are: "Critical", "Error", "Warning", and
          "Informational".
         :paramtype event_level: str or ~azure.mgmt.resourcehealth.v2018_07_01.models.EventLevelValues
+        :keyword reason: The reason for the Incident.
+        :paramtype reason: str
         :keyword article: Article of event.
         :paramtype article: ~azure.mgmt.resourcehealth.v2018_07_01.models.EventPropertiesArticle
         :keyword links: Useful links of event.
         :paramtype links: list[~azure.mgmt.resourcehealth.v2018_07_01.models.Link]
         :keyword impact_start_time: It provides the Timestamp for when the health impacting event
          started.
         :paramtype impact_start_time: ~datetime.datetime
@@ -724,14 +759,15 @@
         self.event_source = event_source
         self.status = status
         self.title = title
         self.summary = summary
         self.header = header
         self.level = level
         self.event_level = event_level
+        self.reason = reason
         self.article = article
         self.links = links
         self.impact_start_time = impact_start_time
         self.impact_mitigation_time = impact_mitigation_time
         self.impact = impact
         self.recommended_actions = recommended_actions
         self.faqs = faqs
@@ -746,27 +782,46 @@
 
 
 class EventPropertiesArticle(_serialization.Model):
     """Article of event.
 
     :ivar article_content: Article content of event.
     :vartype article_content: str
+    :ivar article_id: Article Id.
+    :vartype article_id: str
+    :ivar parameters: It provides a map of parameter name and value.
+    :vartype parameters: JSON
     """
 
     _attribute_map = {
         "article_content": {"key": "articleContent", "type": "str"},
+        "article_id": {"key": "articleId", "type": "str"},
+        "parameters": {"key": "parameters", "type": "object"},
     }
 
-    def __init__(self, *, article_content: Optional[str] = None, **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *,
+        article_content: Optional[str] = None,
+        article_id: Optional[str] = None,
+        parameters: Optional[JSON] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword article_content: Article content of event.
         :paramtype article_content: str
+        :keyword article_id: Article Id.
+        :paramtype article_id: str
+        :keyword parameters: It provides a map of parameter name and value.
+        :paramtype parameters: JSON
         """
         super().__init__(**kwargs)
         self.article_content = article_content
+        self.article_id = article_id
+        self.parameters = parameters
 
 
 class EventPropertiesRecommendedActions(_serialization.Model):
     """Recommended actions of event.
 
     :ivar message: Recommended action title for the service health event.
     :vartype message: str
@@ -1344,44 +1399,51 @@
 class RecommendedAction(_serialization.Model):
     """Lists actions the user can take based on the current availabilityState of the resource.
 
     :ivar action: Recommended action.
     :vartype action: str
     :ivar action_url: Link to the action.
     :vartype action_url: str
+    :ivar action_url_comment: the comment for the Action.
+    :vartype action_url_comment: str
     :ivar action_url_text: Substring of action, it describes which text should host the action url.
     :vartype action_url_text: str
     """
 
     _attribute_map = {
         "action": {"key": "action", "type": "str"},
         "action_url": {"key": "actionUrl", "type": "str"},
+        "action_url_comment": {"key": "_ActionUrl\\.Comment", "type": "str"},
         "action_url_text": {"key": "actionUrlText", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         action: Optional[str] = None,
         action_url: Optional[str] = None,
+        action_url_comment: Optional[str] = None,
         action_url_text: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword action: Recommended action.
         :paramtype action: str
         :keyword action_url: Link to the action.
         :paramtype action_url: str
+        :keyword action_url_comment: the comment for the Action.
+        :paramtype action_url_comment: str
         :keyword action_url_text: Substring of action, it describes which text should host the action
          url.
         :paramtype action_url_text: str
         """
         super().__init__(**kwargs)
         self.action = action
         self.action_url = action_url
+        self.action_url_comment = action_url_comment
         self.action_url_text = action_url_text
 
 
 class ServiceImpactingEvent(_serialization.Model):
     """Lists the service impacting events that may be affecting the health of the resource.
 
     :ivar event_start_time: Timestamp for when the event started.
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/models/__init__.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,26 +36,26 @@
 from ._models_py3 import ServiceImpactingEvent
 from ._models_py3 import ServiceImpactingEventIncidentProperties
 from ._models_py3 import ServiceImpactingEventStatus
 from ._models_py3 import StatusActiveEvent
 from ._models_py3 import StatusBanner
 from ._models_py3 import Update
 
-from ._microsoft_resource_health_enums import AvailabilityStateValues
-from ._microsoft_resource_health_enums import Enum8
-from ._microsoft_resource_health_enums import EventLevelValues
-from ._microsoft_resource_health_enums import EventSourceValues
-from ._microsoft_resource_health_enums import EventStatusValues
-from ._microsoft_resource_health_enums import EventTypeValues
-from ._microsoft_resource_health_enums import LevelValues
-from ._microsoft_resource_health_enums import LinkTypeValues
-from ._microsoft_resource_health_enums import ReasonChronicityTypes
-from ._microsoft_resource_health_enums import Scenario
-from ._microsoft_resource_health_enums import SeverityValues
-from ._microsoft_resource_health_enums import StageValues
+from ._resource_health_mgmt_client_enums import AvailabilityStateValues
+from ._resource_health_mgmt_client_enums import Enum8
+from ._resource_health_mgmt_client_enums import EventLevelValues
+from ._resource_health_mgmt_client_enums import EventSourceValues
+from ._resource_health_mgmt_client_enums import EventStatusValues
+from ._resource_health_mgmt_client_enums import EventTypeValues
+from ._resource_health_mgmt_client_enums import LevelValues
+from ._resource_health_mgmt_client_enums import LinkTypeValues
+from ._resource_health_mgmt_client_enums import ReasonChronicityTypes
+from ._resource_health_mgmt_client_enums import Scenario
+from ._resource_health_mgmt_client_enums import SeverityValues
+from ._resource_health_mgmt_client_enums import StageValues
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AvailabilityStatus",
     "AvailabilityStatusListResult",
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/_configuration.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/_configuration.py`

 * *Files 9% similar despite different names*

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
 
 
-class MicrosoftResourceHealthConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
-    """Configuration for MicrosoftResourceHealth.
+class ResourceHealthMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for ResourceHealthMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
      subscription. The subscription ID forms part of the URI for every service call. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2018-07-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2015-01-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(MicrosoftResourceHealthConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", "2018-07-01")
+        super(ResourceHealthMgmtClientConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2015-01-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/_microsoft_resource_health.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/_resource_health_mgmt_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
 from .. import models as _models
 from ..._serialization import Deserializer, Serializer
-from ._configuration import MicrosoftResourceHealthConfiguration
+from ._configuration import ResourceHealthMgmtClientConfiguration
 from .operations import (
     AvailabilityStatusesOperations,
     EmergingIssuesOperations,
     EventsOperations,
     MetadataOperations,
     Operations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class MicrosoftResourceHealth:  # pylint: disable=client-accepts-api-version-keyword
+class ResourceHealthMgmtClient:  # pylint: disable=client-accepts-api-version-keyword
     """The Resource Health Client.
 
     :ivar events: EventsOperations operations
     :vartype events: azure.mgmt.resourcehealth.v2018_07_01.aio.operations.EventsOperations
     :ivar availability_statuses: AvailabilityStatusesOperations operations
     :vartype availability_statuses:
      azure.mgmt.resourcehealth.v2018_07_01.aio.operations.AvailabilityStatusesOperations
@@ -58,18 +58,18 @@
     def __init__(
         self,
         credential: "AsyncTokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
-        self._config = MicrosoftResourceHealthConfiguration(
+        self._config = ResourceHealthMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.events = EventsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.availability_statuses = AvailabilityStatusesOperations(
@@ -100,13 +100,13 @@
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
     async def close(self) -> None:
         await self._client.close()
 
-    async def __aenter__(self) -> "MicrosoftResourceHealth":
+    async def __aenter__(self) -> "ResourceHealthMgmtClient":
         await self._client.__aenter__()
         return self
 
     async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/__init__.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._microsoft_resource_health import MicrosoftResourceHealth
+from ._resource_health_mgmt_client import ResourceHealthMgmtClient
+from ._version import VERSION
+
+__version__ = VERSION
 
 try:
     from ._patch import __all__ as _patch_all
     from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "MicrosoftResourceHealth",
+    "ResourceHealthMgmtClient",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_availability_statuses_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_availability_statuses_operations.py`

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
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -32,29 +31,25 @@
 from ...operations._availability_statuses_operations import (
     build_get_by_resource_request,
     build_list_by_resource_group_request,
     build_list_by_subscription_id_request,
     build_list_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class AvailabilityStatusesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.aio.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2018_07_01.aio.ResourceHealthMgmtClient`'s
         :attr:`availability_statuses` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -83,15 +78,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -137,16 +132,17 @@
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
@@ -181,15 +177,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -236,16 +232,17 @@
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
@@ -292,31 +289,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.AvailabilityStatus] = kwargs.pop("cls", None)
 
         request = build_get_by_resource_request(
             resource_uri=resource_uri,
             filter=filter,
             expand=expand,
             api_version=api_version,
             template_url=self.get_by_resource.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -358,15 +356,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -412,16 +410,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_emerging_issues_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_emerging_issues_operations.py`

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
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar, Union
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -27,29 +26,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._emerging_issues_operations import build_get_request, build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class EmergingIssuesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.aio.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2018_07_01.aio.ResourceHealthMgmtClient`'s
         :attr:`emerging_issues` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -76,29 +71,30 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.EmergingIssuesGetResult] = kwargs.pop("cls", None)
 
         request = build_get_request(
             issue_name=issue_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -123,15 +119,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.EmergingIssuesGetResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.EmergingIssueListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -174,16 +170,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_metadata_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_metadata_operations.py`

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
@@ -27,29 +26,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._metadata_operations import build_get_entity_request, build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class MetadataOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.aio.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2022_10_01.aio.ResourceHealthMgmtClient`'s
         :attr:`metadata` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -61,21 +56,21 @@
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.MetadataEntity"]:
         """Gets the list of metadata entities.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either MetadataEntity or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.MetadataEntity]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2022_10_01.models.MetadataEntity]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
         cls: ClsType[_models.MetadataEntityListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -118,16 +113,17 @@
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
@@ -142,43 +138,44 @@
     async def get_entity(self, name: str, **kwargs: Any) -> _models.MetadataEntity:
         """Gets the list of metadata entities.
 
         :param name: Name of metadata entity. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MetadataEntity or the result of cls(response)
-        :rtype: ~azure.mgmt.resourcehealth.v2018_07_01.models.MetadataEntity
+        :rtype: ~azure.mgmt.resourcehealth.v2022_10_01.models.MetadataEntity
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
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
         cls: ClsType[_models.MetadataEntity] = kwargs.pop("cls", None)
 
         request = build_get_entity_request(
             name=name,
             api_version=api_version,
             template_url=self.get_entity.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/aio/operations/_operations.py`

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
@@ -24,29 +23,25 @@
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
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.aio.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2022_10_01.aio.ResourceHealthMgmtClient`'s
         :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -57,42 +52,43 @@
 
     @distributed_trace_async
     async def list(self, **kwargs: Any) -> _models.OperationListResult:
         """Lists available operations for the resourcehealth resource provider.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: OperationListResult or the result of cls(response)
-        :rtype: ~azure.mgmt.resourcehealth.v2018_07_01.models.OperationListResult
+        :rtype: ~azure.mgmt.resourcehealth.v2022_10_01.models.OperationListResult
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
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         request = build_list_request(
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_events_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_events_operations.py`

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
@@ -29,29 +28,25 @@
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._events_operations import (
     build_list_by_single_resource_request,
     build_list_by_subscription_id_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class EventsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2018_07_01.aio.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2018_07_01.aio.ResourceHealthMgmtClient`'s
         :attr:`events` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -87,15 +82,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.Event]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.Events] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -142,16 +137,17 @@
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
@@ -190,15 +186,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2018_07_01.models.Event]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.Events] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -244,16 +240,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/__init__.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_configuration.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/_configuration.py`

 * *Files 16% similar despite different names*

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
 
 
-class MicrosoftResourceHealthConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
-    """Configuration for MicrosoftResourceHealth.
+class ResourceHealthMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for ResourceHealthMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
      subscription. The subscription ID forms part of the URI for every service call. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2015-01-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2018-07-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(MicrosoftResourceHealthConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", "2015-01-01")
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+        super(ResourceHealthMgmtClientConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2018-07-01")
 
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_microsoft_resource_health.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_resource_health_mgmt_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from typing import Any, TYPE_CHECKING
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
 from . import models as _models
 from .._serialization import Deserializer, Serializer
-from ._configuration import MicrosoftResourceHealthConfiguration
+from ._configuration import ResourceHealthMgmtClientConfiguration
 from .operations import (
     AvailabilityStatusesOperations,
     ChildAvailabilityStatusesOperations,
     ChildResourcesOperations,
     Operations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class MicrosoftResourceHealth:  # pylint: disable=client-accepts-api-version-keyword
+class ResourceHealthMgmtClient:  # pylint: disable=client-accepts-api-version-keyword
     """The Resource Health Client.
 
     :ivar availability_statuses: AvailabilityStatusesOperations operations
     :vartype availability_statuses:
      azure.mgmt.resourcehealth.v2015_01_01.operations.AvailabilityStatusesOperations
     :ivar child_availability_statuses: ChildAvailabilityStatusesOperations operations
     :vartype child_availability_statuses:
@@ -56,18 +56,18 @@
     def __init__(
         self,
         credential: "TokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
-        self._config = MicrosoftResourceHealthConfiguration(
+        self._config = ResourceHealthMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.availability_statuses = AvailabilityStatusesOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -99,13 +99,13 @@
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
     def close(self) -> None:
         self._client.close()
 
-    def __enter__(self) -> "MicrosoftResourceHealth":
+    def __enter__(self) -> "ResourceHealthMgmtClient":
         self._client.__enter__()
         return self
 
     def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/_vendor.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_availability_statuses_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_availability_statuses_operations.py`

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
@@ -26,32 +25,28 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_subscription_id_request(
     subscription_id: str, *, filter: Optional[str] = None, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.ResourceHealth/availabilityStatuses"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -80,15 +75,15 @@
     filter: Optional[str] = None,
     expand: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ResourceHealth/availabilityStatuses",
     )  # pylint: disable=line-too-long
@@ -114,15 +109,15 @@
 
 def build_get_by_resource_request(
     resource_uri: str, *, filter: Optional[str] = None, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{resourceUri}/providers/Microsoft.ResourceHealth/availabilityStatuses/current")
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -144,15 +139,15 @@
 
 def build_list_request(
     resource_uri: str, *, filter: Optional[str] = None, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{resourceUri}/providers/Microsoft.ResourceHealth/availabilityStatuses")
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -174,15 +169,15 @@
 
 class AvailabilityStatusesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2015_01_01.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2015_01_01.ResourceHealthMgmtClient`'s
         :attr:`availability_statuses` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -210,15 +205,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -264,16 +259,17 @@
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
@@ -307,15 +303,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -362,16 +358,17 @@
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
@@ -416,31 +413,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatus] = kwargs.pop("cls", None)
 
         request = build_get_by_resource_request(
             resource_uri=resource_uri,
             filter=filter,
             expand=expand,
             api_version=api_version,
             template_url=self.get_by_resource.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -481,15 +479,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -535,16 +533,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_resources_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2022_10_01/operations/_child_resources_operations.py`

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
 from ..._serialization import Serializer
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
     resource_uri: str, *, filter: Optional[str] = None, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{resourceUri}/providers/Microsoft.ResourceHealth/childResources")
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -73,15 +68,15 @@
 
 class ChildResourcesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2015_01_01.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2022_10_01.ResourceHealthMgmtClient`'s
         :attr:`child_resources` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -108,21 +103,21 @@
         :type filter: str
         :param expand: Setting $expand=recommendedactions in url query expands the recommendedactions
          in the response. Default value is None.
         :type expand: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either AvailabilityStatus or the result of cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2022_10_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-10-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -168,16 +163,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_availability_statuses_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/_child_availability_statuses_operations.py`

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
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_by_resource_request(
     resource_uri: str, *, filter: Optional[str] = None, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/{resourceUri}/providers/Microsoft.ResourceHealth/childAvailabilityStatuses/current"
     )
     path_format_arguments = {
@@ -75,15 +70,15 @@
 
 def build_list_request(
     resource_uri: str, *, filter: Optional[str] = None, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{resourceUri}/providers/Microsoft.ResourceHealth/childAvailabilityStatuses")
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -105,15 +100,15 @@
 
 class ChildAvailabilityStatusesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2015_01_01.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2015_01_01.ResourceHealthMgmtClient`'s
         :attr:`child_availability_statuses` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -152,31 +147,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatus] = kwargs.pop("cls", None)
 
         request = build_get_by_resource_request(
             resource_uri=resource_uri,
             filter=filter,
             expand=expand,
             api_version=api_version,
             template_url=self.get_by_resource.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -217,15 +213,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -271,16 +267,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_operations.py`

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
 from ..._serialization import Serializer
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
 
-    api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.ResourceHealth/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -60,15 +55,15 @@
 
 class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2015_01_01.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2018_07_01.ResourceHealthMgmtClient`'s
         :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -79,42 +74,43 @@
 
     @distributed_trace
     def list(self, **kwargs: Any) -> _models.OperationListResult:
         """Lists available operations for the resourcehealth resource provider.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: OperationListResult or the result of cls(response)
-        :rtype: ~azure.mgmt.resourcehealth.v2015_01_01.models.OperationListResult
+        :rtype: ~azure.mgmt.resourcehealth.v2018_07_01.models.OperationListResult
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
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-07-01"))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         request = build_list_request(
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/operations/__init__.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/_microsoft_resource_health_enums.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/_resource_health_mgmt_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/_models_py3.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/_models_py3.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,14 +118,24 @@
     :vartype summary: str
     :ivar detailed_status: Details of the availability status.
     :vartype detailed_status: str
     :ivar reason_type: When the resource's availabilityState is Unavailable, it describes where the
      health impacting event was originated. Examples are planned, unplanned, user initiated or an
      outage etc.
     :vartype reason_type: str
+    :ivar context: When an event is created, it can either be triggered by a customer or the
+     platform of the resource and this field will illustrate that. This field is connected to the
+     category field in this object.
+    :vartype context: str
+    :ivar category: When a context field is set to Platform, this field will reflect if the event
+     was planned or unplanned. If the context field does not have a value of Platform, then this
+     field will be ignored.
+    :vartype category: str
+    :ivar article_id: The Article Id.
+    :vartype article_id: str
     :ivar root_cause_attribution_time: When the resource's availabilityState is Unavailable, it
      provides the Timestamp for when the health impacting event was received.
     :vartype root_cause_attribution_time: ~datetime.datetime
     :ivar resolution_eta: When the resource's availabilityState is Unavailable and the reasonType
      is not User Initiated, it provides the date and time for when the issue is expected to be
      resolved.
     :vartype resolution_eta: ~datetime.datetime
@@ -154,14 +164,17 @@
     """
 
     _attribute_map = {
         "availability_state": {"key": "availabilityState", "type": "str"},
         "summary": {"key": "summary", "type": "str"},
         "detailed_status": {"key": "detailedStatus", "type": "str"},
         "reason_type": {"key": "reasonType", "type": "str"},
+        "context": {"key": "context", "type": "str"},
+        "category": {"key": "category", "type": "str"},
+        "article_id": {"key": "articleId", "type": "str"},
         "root_cause_attribution_time": {"key": "rootCauseAttributionTime", "type": "iso-8601"},
         "resolution_eta": {"key": "resolutionETA", "type": "iso-8601"},
         "occured_time": {"key": "occuredTime", "type": "iso-8601"},
         "reason_chronicity": {"key": "reasonChronicity", "type": "str"},
         "reported_time": {"key": "reportedTime", "type": "iso-8601"},
         "is_arm_resource": {"key": "isArmResource", "type": "bool"},
         "recently_resolved_state": {
@@ -175,14 +188,17 @@
     def __init__(
         self,
         *,
         availability_state: Optional[Union[str, "_models.AvailabilityStateValues"]] = None,
         summary: Optional[str] = None,
         detailed_status: Optional[str] = None,
         reason_type: Optional[str] = None,
+        context: Optional[str] = None,
+        category: Optional[str] = None,
+        article_id: Optional[str] = None,
         root_cause_attribution_time: Optional[datetime.datetime] = None,
         resolution_eta: Optional[datetime.datetime] = None,
         occured_time: Optional[datetime.datetime] = None,
         reason_chronicity: Optional[Union[str, "_models.ReasonChronicityTypes"]] = None,
         reported_time: Optional[datetime.datetime] = None,
         is_arm_resource: Optional[bool] = None,
         recently_resolved_state: Optional["_models.AvailabilityStatusPropertiesRecentlyResolvedState"] = None,
@@ -199,14 +215,24 @@
         :paramtype summary: str
         :keyword detailed_status: Details of the availability status.
         :paramtype detailed_status: str
         :keyword reason_type: When the resource's availabilityState is Unavailable, it describes where
          the health impacting event was originated. Examples are planned, unplanned, user initiated or
          an outage etc.
         :paramtype reason_type: str
+        :keyword context: When an event is created, it can either be triggered by a customer or the
+         platform of the resource and this field will illustrate that. This field is connected to the
+         category field in this object.
+        :paramtype context: str
+        :keyword category: When a context field is set to Platform, this field will reflect if the
+         event was planned or unplanned. If the context field does not have a value of Platform, then
+         this field will be ignored.
+        :paramtype category: str
+        :keyword article_id: The Article Id.
+        :paramtype article_id: str
         :keyword root_cause_attribution_time: When the resource's availabilityState is Unavailable, it
          provides the Timestamp for when the health impacting event was received.
         :paramtype root_cause_attribution_time: ~datetime.datetime
         :keyword resolution_eta: When the resource's availabilityState is Unavailable and the
          reasonType is not User Initiated, it provides the date and time for when the issue is expected
          to be resolved.
         :paramtype resolution_eta: ~datetime.datetime
@@ -234,14 +260,17 @@
          list[~azure.mgmt.resourcehealth.v2015_01_01.models.ServiceImpactingEvent]
         """
         super().__init__(**kwargs)
         self.availability_state = availability_state
         self.summary = summary
         self.detailed_status = detailed_status
         self.reason_type = reason_type
+        self.context = context
+        self.category = category
+        self.article_id = article_id
         self.root_cause_attribution_time = root_cause_attribution_time
         self.resolution_eta = resolution_eta
         self.occured_time = occured_time
         self.reason_chronicity = reason_chronicity
         self.reported_time = reported_time
         self.is_arm_resource = is_arm_resource
         self.recently_resolved_state = recently_resolved_state
@@ -428,44 +457,51 @@
 class RecommendedAction(_serialization.Model):
     """Lists actions the user can take based on the current availabilityState of the resource.
 
     :ivar action: Recommended action.
     :vartype action: str
     :ivar action_url: Link to the action.
     :vartype action_url: str
+    :ivar action_url_comment: the comment for the Action.
+    :vartype action_url_comment: str
     :ivar action_url_text: Substring of action, it describes which text should host the action url.
     :vartype action_url_text: str
     """
 
     _attribute_map = {
         "action": {"key": "action", "type": "str"},
         "action_url": {"key": "actionUrl", "type": "str"},
+        "action_url_comment": {"key": "_ActionUrl\\.Comment", "type": "str"},
         "action_url_text": {"key": "actionUrlText", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         action: Optional[str] = None,
         action_url: Optional[str] = None,
+        action_url_comment: Optional[str] = None,
         action_url_text: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword action: Recommended action.
         :paramtype action: str
         :keyword action_url: Link to the action.
         :paramtype action_url: str
+        :keyword action_url_comment: the comment for the Action.
+        :paramtype action_url_comment: str
         :keyword action_url_text: Substring of action, it describes which text should host the action
          url.
         :paramtype action_url_text: str
         """
         super().__init__(**kwargs)
         self.action = action
         self.action_url = action_url
+        self.action_url_comment = action_url_comment
         self.action_url_text = action_url_text
 
 
 class ServiceImpactingEvent(_serialization.Model):
     """Lists the service impacting events that may be affecting the health of the resource.
 
     :ivar event_start_time: Timestamp for when the event started.
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/models/__init__.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from ._models_py3 import OperationDisplay
 from ._models_py3 import OperationListResult
 from ._models_py3 import RecommendedAction
 from ._models_py3 import ServiceImpactingEvent
 from ._models_py3 import ServiceImpactingEventIncidentProperties
 from ._models_py3 import ServiceImpactingEventStatus
 
-from ._microsoft_resource_health_enums import AvailabilityStateValues
-from ._microsoft_resource_health_enums import ReasonChronicityTypes
+from ._resource_health_mgmt_client_enums import AvailabilityStateValues
+from ._resource_health_mgmt_client_enums import ReasonChronicityTypes
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AvailabilityStatus",
     "AvailabilityStatusListResult",
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/_configuration.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/_configuration.py`

 * *Files 12% similar despite different names*

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
 
 
-class MicrosoftResourceHealthConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
-    """Configuration for MicrosoftResourceHealth.
+class ResourceHealthMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for ResourceHealthMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
      subscription. The subscription ID forms part of the URI for every service call. Required.
     :type subscription_id: str
     :keyword api_version: Api Version. Default value is "2015-01-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(MicrosoftResourceHealthConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", "2015-01-01")
+    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+        super(ResourceHealthMgmtClientConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2015-01-01")
 
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/_microsoft_resource_health.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/_resource_health_mgmt_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
 from .. import models as _models
 from ..._serialization import Deserializer, Serializer
-from ._configuration import MicrosoftResourceHealthConfiguration
+from ._configuration import ResourceHealthMgmtClientConfiguration
 from .operations import (
     AvailabilityStatusesOperations,
     ChildAvailabilityStatusesOperations,
     ChildResourcesOperations,
     Operations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class MicrosoftResourceHealth:  # pylint: disable=client-accepts-api-version-keyword
+class ResourceHealthMgmtClient:  # pylint: disable=client-accepts-api-version-keyword
     """The Resource Health Client.
 
     :ivar availability_statuses: AvailabilityStatusesOperations operations
     :vartype availability_statuses:
      azure.mgmt.resourcehealth.v2015_01_01.aio.operations.AvailabilityStatusesOperations
     :ivar child_availability_statuses: ChildAvailabilityStatusesOperations operations
     :vartype child_availability_statuses:
@@ -56,18 +56,18 @@
     def __init__(
         self,
         credential: "AsyncTokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
-        self._config = MicrosoftResourceHealthConfiguration(
+        self._config = ResourceHealthMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.availability_statuses = AvailabilityStatusesOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -99,13 +99,13 @@
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
     async def close(self) -> None:
         await self._client.close()
 
-    async def __aenter__(self) -> "MicrosoftResourceHealth":
+    async def __aenter__(self) -> "ResourceHealthMgmtClient":
         await self._client.__aenter__()
         return self
 
     async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/__init__.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._microsoft_resource_health import MicrosoftResourceHealth
+from ._resource_health_mgmt_client import ResourceHealthMgmtClient
+from ._version import VERSION
+
+__version__ = VERSION
 
 try:
     from ._patch import __all__ as _patch_all
     from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "MicrosoftResourceHealth",
+    "ResourceHealthMgmtClient",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_availability_statuses_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_availability_statuses_operations.py`

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
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -32,29 +31,25 @@
 from ...operations._availability_statuses_operations import (
     build_get_by_resource_request,
     build_list_by_resource_group_request,
     build_list_by_subscription_id_request,
     build_list_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class AvailabilityStatusesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2015_01_01.aio.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2015_01_01.aio.ResourceHealthMgmtClient`'s
         :attr:`availability_statuses` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -82,15 +77,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -136,16 +131,17 @@
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
@@ -179,15 +175,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -234,16 +230,17 @@
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
@@ -288,31 +285,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatus] = kwargs.pop("cls", None)
 
         request = build_get_by_resource_request(
             resource_uri=resource_uri,
             filter=filter,
             expand=expand,
             api_version=api_version,
             template_url=self.get_by_resource.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -353,15 +351,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -407,16 +405,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_patch.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2018_07_01/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_resources_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_resources_operations.py`

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
@@ -26,29 +25,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._child_resources_operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ChildResourcesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2015_01_01.aio.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2015_01_01.aio.ResourceHealthMgmtClient`'s
         :attr:`child_resources` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -81,15 +76,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -135,16 +130,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_availability_statuses_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_child_availability_statuses_operations.py`

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
@@ -27,29 +26,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._child_availability_statuses_operations import build_get_by_resource_request, build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ChildAvailabilityStatusesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2015_01_01.aio.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2015_01_01.aio.ResourceHealthMgmtClient`'s
         :attr:`child_availability_statuses` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -88,31 +83,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatus] = kwargs.pop("cls", None)
 
         request = build_get_by_resource_request(
             resource_uri=resource_uri,
             filter=filter,
             expand=expand,
             api_version=api_version,
             template_url=self.get_by_resource.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -153,15 +149,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.resourcehealth.v2015_01_01.models.AvailabilityStatus]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.AvailabilityStatusListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -207,16 +203,17 @@
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

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_operations.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/_operations.py`

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
@@ -24,29 +23,25 @@
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
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.resourcehealth.v2015_01_01.aio.MicrosoftResourceHealth`'s
+        :class:`~azure.mgmt.resourcehealth.v2015_01_01.aio.ResourceHealthMgmtClient`'s
         :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -71,28 +66,29 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2015-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2015-01-01"))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         request = build_list_request(
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
```

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/__init__.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/v2015_01_01/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-resourcehealth-1.0.0b3/azure/mgmt/resourcehealth/aio/_configuration.py` & `azure-mgmt-resourcehealth-1.0.0b4/azure/mgmt/resourcehealth/_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,60 +8,60 @@
 # Changes may cause incorrect behavior and will be lost if the code is
 # regenerated.
 # --------------------------------------------------------------------------
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
+from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
-class MicrosoftResourceHealthConfiguration(Configuration):
-    """Configuration for MicrosoftResourceHealth.
+class ResourceHealthMgmtClientConfiguration(Configuration):
+    """Configuration for ResourceHealthMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call. Required.
+    :type credential: ~azure.core.credentials.TokenCredential
+    :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     """
 
     def __init__(
         self,
-        credential: "AsyncTokenCredential",
+        credential: "TokenCredential",
         subscription_id: str,
         **kwargs: Any
-    ) -> None:
+    ):
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
-        super(MicrosoftResourceHealthConfiguration, self).__init__(**kwargs)
+        super(ResourceHealthMgmtClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'azure-mgmt-resourcehealth/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs: Any
-    ) -> None:
+    ):
         self.user_agent_policy = kwargs.get('user_agent_policy') or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get('headers_policy') or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get('proxy_policy') or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get('logging_policy') or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get('http_logging_policy') or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get('retry_policy') or policies.AsyncRetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get('retry_policy') or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get('custom_hook_policy') or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get('redirect_policy') or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get('redirect_policy') or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get('authentication_policy')
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(self.credential, *self.credential_scopes, **kwargs)
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(self.credential, *self.credential_scopes, **kwargs)
```

