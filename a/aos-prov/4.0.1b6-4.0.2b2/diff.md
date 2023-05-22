# Comparing `tmp/aos_prov-4.0.1b6-py3-none-any.whl.zip` & `tmp/aos_prov-4.0.2b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,64 +1,61 @@
-Zip file size: 74356 bytes, number of entries: 62
--rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/__init__.py
--rw-rw-rw-  2.0 fat     2619 b- defN 23-Jan-20 13:00 aos_prov/actions.py
--rw-rw-rw-  2.0 fat     7077 b- defN 23-Jan-20 10:38 aos_prov/main.py
--rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/commands/__init__.py
--rw-rw-rw-  2.0 fat     7452 b- defN 22-Dec-20 13:47 aos_prov/commands/command_provision.py
--rw-rw-rw-  2.0 fat     5021 b- defN 23-Jan-19 15:42 aos_prov/commands/command_vm.py
--rw-rw-rw-  2.0 fat     2406 b- defN 22-Dec-15 18:20 aos_prov/commands/command_vm_libvirt.py
--rw-rw-rw-  2.0 fat     5398 b- defN 23-Jan-20 15:27 aos_prov/commands/command_vm_multi_node.py
--rw-rw-rw-  2.0 fat     3864 b- defN 23-Jan-19 17:23 aos_prov/commands/download.py
--rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/__init__.py
--rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/cloud/__init__.py
--rw-rw-rw-  2.0 fat     8856 b- defN 22-Dec-15 18:20 aos_prov/communication/cloud/cloud_api.py
--rw-rw-rw-  2.0 fat       93 b- defN 22-Feb-07 18:56 aos_prov/communication/unit/__init__.py
--rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/__init__.py
--rw-rw-rw-  2.0 fat     5403 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/unit_communacation.py
--rw-rw-rw-  2.0 fat     5467 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v0/unit_communication.py
--rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/generated/__init__.py
--rw-rw-rw-  2.0 fat    29503 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py
--rw-rw-rw-  2.0 fat    20612 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py
--rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/__init__.py
--rw-rw-rw-  2.0 fat     6942 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/unit_communacation_v1.py
--rw-rw-rw-  2.0 fat     6926 b- defN 23-Jan-19 17:23 aos_prov/communication/unit/v1/unit_communication_v1.py
--rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/__init__.py
--rw-rw-rw-  2.0 fat     5568 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py
--rw-rw-rw-  2.0 fat      163 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py
--rw-rw-rw-  2.0 fat    31801 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py
--rw-rw-rw-  2.0 fat    20208 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py
--rw-rw-rw-  2.0 fat     9306 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py
--rw-rw-rw-  2.0 fat     8101 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/__init__.py
--rw-rw-rw-  2.0 fat     7346 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/unit_communacation_v2.py
--rw-rw-rw-  2.0 fat     7266 b- defN 23-Jan-19 17:23 aos_prov/communication/unit/v2/unit_communication_v2.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/__init__.py
--rw-rw-rw-  2.0 fat     5568 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
--rw-rw-rw-  2.0 fat      163 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
--rw-rw-rw-  2.0 fat    25101 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
--rw-rw-rw-  2.0 fat    16786 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
--rw-rw-rw-  2.0 fat    17715 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
--rw-rw-rw-  2.0 fat    13170 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/__init__.py
--rw-rw-rw-  2.0 fat    11042 b- defN 23-Jan-19 17:23 aos_prov/communication/unit/v4/unit_communication_v4.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/__init__.py
--rw-rw-rw-  2.0 fat    18732 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/iamanager_pb2.py
--rw-rw-rw-  2.0 fat    34140 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
--rw-rw-rw-  2.0 fat     2750 b- defN 22-Feb-07 18:56 aos_prov/files/1rootCA.crt
--rw-rw-rw-  2.0 fat     2767 b- defN 22-Oct-13 13:59 aos_prov/files/vm.xml
--rw-rw-rw-  2.0 fat      771 b- defN 22-Oct-13 13:59 aos_prov/utils/__init__.py
--rw-rw-rw-  2.0 fat     1614 b- defN 23-Jan-20 10:38 aos_prov/utils/common.py
--rw-rw-rw-  2.0 fat     2679 b- defN 22-Dec-02 13:22 aos_prov/utils/config.py
--rw-rw-rw-  2.0 fat      537 b- defN 22-Oct-13 13:59 aos_prov/utils/errors.py
--rw-rw-rw-  2.0 fat     1229 b- defN 22-Dec-02 13:22 aos_prov/utils/unit_certificate.py
--rw-rw-rw-  2.0 fat     7725 b- defN 23-Jan-19 08:01 aos_prov/utils/user_credentials.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 test/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 test/utils/__init__.py
--rw-rw-rw-  2.0 fat      665 b- defN 22-Dec-02 13:22 test/utils/test_config.py
--rw-rw-rw-  2.0 fat      656 b- defN 22-Dec-02 13:22 test/utils/test_unit_certificate.py
--rw-rw-rw-  2.0 fat      456 b- defN 22-Oct-13 13:59 test/utils/test_user_credentials.py
--rw-rw-rw-  2.0 fat     2279 b- defN 23-Jan-20 15:27 aos_prov-4.0.1b6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-20 15:27 aos_prov-4.0.1b6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       49 b- defN 23-Jan-20 15:27 aos_prov-4.0.1b6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jan-20 15:27 aos_prov-4.0.1b6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     6207 b- defN 23-Jan-20 15:27 aos_prov-4.0.1b6.dist-info/RECORD
-62 files, 381049 bytes uncompressed, 64092 bytes compressed:  83.2%
+Zip file size: 68479 bytes, number of entries: 59
+-rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/__init__.py
+-rw-rw-r--  2.0 unx     2842 b- defN 23-Apr-04 10:59 aos_prov/actions.py
+-rw-rw-r--  2.0 unx     7271 b- defN 23-May-22 11:54 aos_prov/main.py
+-rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/commands/__init__.py
+-rw-rw-r--  2.0 unx     7501 b- defN 23-Apr-04 10:59 aos_prov/commands/command_provision.py
+-rw-rw-r--  2.0 unx     4883 b- defN 23-Jan-19 09:24 aos_prov/commands/command_vm.py
+-rw-rw-r--  2.0 unx     2326 b- defN 22-Dec-16 09:22 aos_prov/commands/command_vm_libvirt.py
+-rw-rw-r--  2.0 unx     9689 b- defN 23-Apr-04 10:59 aos_prov/commands/command_vm_multi_node_manage.py
+-rw-rw-r--  2.0 unx     3799 b- defN 23-Apr-04 10:59 aos_prov/commands/download.py
+-rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/__init__.py
+-rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/cloud/__init__.py
+-rw-rw-r--  2.0 unx     8552 b- defN 23-Apr-04 10:59 aos_prov/communication/cloud/cloud_api.py
+-rw-rw-r--  2.0 unx       89 b- defN 22-Apr-10 14:06 aos_prov/communication/unit/__init__.py
+-rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/__init__.py
+-rw-rw-r--  2.0 unx     5222 b- defN 23-Apr-04 10:59 aos_prov/communication/unit/v0/unit_communication.py
+-rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/generated/__init__.py
+-rw-rw-r--  2.0 unx    28704 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py
+-rw-rw-r--  2.0 unx    20182 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py
+-rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/__init__.py
+-rw-rw-r--  2.0 unx     6382 b- defN 23-Apr-04 10:59 aos_prov/communication/unit/v1/unit_communication_v1.py
+-rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/__init__.py
+-rw-rw-r--  2.0 unx     5409 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py
+-rw-rw-r--  2.0 unx      159 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py
+-rw-rw-r--  2.0 unx    31002 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py
+-rw-rw-r--  2.0 unx    19810 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py
+-rw-rw-r--  2.0 unx     9075 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py
+-rw-rw-r--  2.0 unx     7934 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/__init__.py
+-rw-rw-r--  2.0 unx     6713 b- defN 23-Apr-04 10:59 aos_prov/communication/unit/v2/unit_communication_v2.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/__init__.py
+-rw-rw-r--  2.0 unx     5409 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
+-rw-rw-r--  2.0 unx      159 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
+-rw-rw-r--  2.0 unx    24470 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
+-rw-rw-r--  2.0 unx    16454 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
+-rw-rw-r--  2.0 unx    17266 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
+-rw-rw-r--  2.0 unx    12904 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/__init__.py
+-rw-rw-r--  2.0 unx     9592 b- defN 23-Apr-04 10:59 aos_prov/communication/unit/v4/unit_communication_v4.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/__init__.py
+-rw-rw-r--  2.0 unx    18433 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/iamanager_pb2.py
+-rw-rw-r--  2.0 unx    33405 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
+-rw-rw-r--  2.0 unx     2705 b- defN 22-Apr-10 14:06 aos_prov/files/1rootCA.crt
+-rw-rw-r--  2.0 unx     2690 b- defN 22-Nov-13 13:27 aos_prov/files/vm.xml
+-rw-rw-r--  2.0 unx      748 b- defN 22-Nov-13 13:27 aos_prov/utils/__init__.py
+-rw-rw-r--  2.0 unx     1649 b- defN 23-Apr-04 10:59 aos_prov/utils/common.py
+-rw-rw-r--  2.0 unx     2591 b- defN 22-Dec-01 17:44 aos_prov/utils/config.py
+-rw-rw-r--  2.0 unx      501 b- defN 22-Nov-13 13:27 aos_prov/utils/errors.py
+-rw-rw-r--  2.0 unx     1176 b- defN 22-Dec-01 17:44 aos_prov/utils/unit_certificate.py
+-rw-rw-r--  2.0 unx     7475 b- defN 23-Apr-04 10:59 aos_prov/utils/user_credentials.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 test/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 test/utils/__init__.py
+-rw-rw-r--  2.0 unx      642 b- defN 22-Dec-01 17:44 test/utils/test_config.py
+-rw-rw-r--  2.0 unx      632 b- defN 22-Dec-01 17:44 test/utils/test_unit_certificate.py
+-rw-rw-r--  2.0 unx      439 b- defN 22-Nov-13 13:27 test/utils/test_user_credentials.py
+-rw-rw-r--  2.0 unx     2484 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5880 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/RECORD
+59 files, 356114 bytes uncompressed, 58753 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -15,15 +15,15 @@
 
 Filename: aos_prov/commands/command_vm.py
 Comment: 
 
 Filename: aos_prov/commands/command_vm_libvirt.py
 Comment: 
 
-Filename: aos_prov/commands/command_vm_multi_node.py
+Filename: aos_prov/commands/command_vm_multi_node_manage.py
 Comment: 
 
 Filename: aos_prov/commands/download.py
 Comment: 
 
 Filename: aos_prov/communication/__init__.py
 Comment: 
@@ -36,17 +36,14 @@
 
 Filename: aos_prov/communication/unit/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v0/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v0/unit_communacation.py
-Comment: 
-
 Filename: aos_prov/communication/unit/v0/unit_communication.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v0/generated/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py
@@ -54,17 +51,14 @@
 
 Filename: aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v1/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v1/unit_communacation_v1.py
-Comment: 
-
 Filename: aos_prov/communication/unit/v1/unit_communication_v1.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v1/generated/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py
@@ -84,17 +78,14 @@
 
 Filename: aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v2/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/unit_communacation_v2.py
-Comment: 
-
 Filename: aos_prov/communication/unit/v2/unit_communication_v2.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v2/generated/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
@@ -165,23 +156,23 @@
 
 Filename: test/utils/test_unit_certificate.py
 Comment: 
 
 Filename: test/utils/test_user_credentials.py
 Comment: 
 
-Filename: aos_prov-4.0.1b6.dist-info/METADATA
+Filename: aos_prov-4.0.2b2.dist-info/METADATA
 Comment: 
 
-Filename: aos_prov-4.0.1b6.dist-info/WHEEL
+Filename: aos_prov-4.0.2b2.dist-info/WHEEL
 Comment: 
 
-Filename: aos_prov-4.0.1b6.dist-info/entry_points.txt
+Filename: aos_prov-4.0.2b2.dist-info/entry_points.txt
 Comment: 
 
-Filename: aos_prov-4.0.1b6.dist-info/top_level.txt
+Filename: aos_prov-4.0.2b2.dist-info/top_level.txt
 Comment: 
 
-Filename: aos_prov-4.0.1b6.dist-info/RECORD
+Filename: aos_prov-4.0.2b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aos_prov/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
```

## aos_prov/actions.py

```diff
@@ -1,65 +1,83 @@
 #
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
 #
-import os
-import platform
-import subprocess
+"""aos-prov supported actions module."""
 import time
-import zipfile
-from pathlib import Path
 
 from aos_prov.commands.command_provision import run_provision
+from aos_prov.commands.command_vm_multi_node_manage import new_vm, start_vms
 from aos_prov.commands.download import download_and_save_multinode
 from aos_prov.communication.cloud.cloud_api import CloudAPI
-from aos_prov.utils.common import DOWNLOADS_PATH
+from aos_prov.utils.common import DOWNLOADS_PATH, print_message
 from aos_prov.utils.user_credentials import UserCredentials
 
 
-def create_new_unit(vm_name: str, uc: UserCredentials, disk_location: str, do_provision=False):
+def provision_unit(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1) -> None:
+    """
+    Rub provisioning process for the unit.
+
+    Args:
+        unit_address (str): address:port of the unit.
+        cloud_api (CloudAPI): instance of CloudAPI with user info.
+        reconnect_times (int): Number of connections retries.
+    """
+    run_provision(unit_address, cloud_api, reconnect_times)
+
+
+def create_new_unit(
+    vm_name: str,
+    uc: UserCredentials,
+    disk_location: str,
+    do_provision=False,
+    nodes_count=2,
+    headless=False
+) -> []:
+    """
+    Create a new VirtualBox multi-node Unit.
+
+    Args:
+        vm_name (str): Name of the group of units.
+        uc (UserCredentials): UserCredentials instance.
+        disk_location (str): Full path to the folder with nodes images.
+        do_provision (Boolean): Provision unit after creation or not.
+        nodes_count (int): Count of nodes to create. Supported 1 or 2 nodes.
+        headless (bool): Start VM in headless mode if True
+    Returns:
+        [provisioning_port, node0_ssh_port, node1_ssh_port]: Forwarded ports.
+    """
     cloud_api = CloudAPI(uc)
-    cloud_api.check_cloud_access()
-    if platform.system() == 'Linux':
-        from aos_prov.commands.command_vm_multi_node import new_vm, start_vms
-        vm_port = new_vm(vm_name, disk_location)
-        start_vms([f'/AosUnits/{vm_name}'])
-    elif platform.system() == 'Darwin':
-        from aos_prov.commands.command_vm_multi_node import new_vm, start_vms
-        vm_port = new_vm(vm_name, disk_location)
-        start_vms([f'/AosUnits/{vm_name}'])
-    elif platform.system() == 'Windows':
-        from aos_prov.commands.command_vm_multi_node import new_vm, start_vms
-        vm_port = new_vm(vm_name, disk_location)
-        start_vms([f'/AosUnits/{vm_name}'])
+
+    if do_provision:
+        cloud_api.check_cloud_access()
+
+    provisioning_port, node0_ssh_port, node1_ssh_port = new_vm(vm_name, disk_location, nodes_count)
+
     if do_provision:
+        start_vms(f'/AosUnits/{vm_name}', headless=headless)
         time.sleep(10)
-        run_provision(f'127.0.0.1:{vm_port}', cloud_api, reconnect_times=20)
+        run_provision(f'127.0.0.1:{provisioning_port}', cloud_api, reconnect_times=40)
 
+    return [provisioning_port, node0_ssh_port, node1_ssh_port]
 
-def download_image(download_url: str, force: bool = False):
-    download_and_save_multinode(download_url, DOWNLOADS_PATH, force)
-    print('Download finished. You may find Unit images in: ' + str(DOWNLOADS_PATH.resolve()))
 
+def start_vm(name: str, headless=False) -> None:
+    """Start all VMs in the group.
+
+    Args:
+        name (str): Name of the group to start without root AosUnits group.
+        headless (bool): Start VM in headless mode if True.
+    """
+    start_vms(f'/AosUnits/{name}', check_virtualbox=True, headless=headless)
 
-def install_vbox_sdk():
-    file = download_vbox_sdk()
 
-    with zipfile.ZipFile(file, 'r') as zip_ref:
-        zip_ref.extractall(DOWNLOADS_PATH)
+def download_image(download_url: str, force: bool = False) -> None:
+    """
+    Download unit image.
 
-    envs = os.environ.copy()
-    if platform.system() == 'Windows':
-        command = ['python', 'vboxapisetup.py', 'install', '--user']
-    elif platform.system() == 'Linux':
-        'VBOX_INSTALL_PATH=$(which virtualbox)'
-        command = ['python3', 'vboxapisetup.py', 'install', '--user', '--prefix=']
-    elif platform.system() == 'Darwin':
-        'VBOX_INSTALL_PATH=/Applications/VirtualBox.app/Contents/MacOS'
-        command = ['python3', 'vboxapisetup.py', 'install', '--user', '--prefix=']
-    else:
-        command = 'VBOX_INSTALL_PATH=$(which virtualbox) python3 vboxapisetup.py install --user --prefix='
-    return_code = subprocess.run(command, shell=True, env=envs, cwd=str(Path(DOWNLOADS_PATH / 'sdk' / 'installer')))
-    if return_code.returncode == 0:
-        return
-    else:
-        print('Error installing VirtualBox SDK')
+    Args:
+        download_url (str): URL to download from.
+        force (bool): If set downloaded image will overwrite existing one.
+    """
+    download_and_save_multinode(download_url, DOWNLOADS_PATH, force)
+    print_message(f'Download finished. You may find Unit images in: [b]{str(DOWNLOADS_PATH.resolve())}[/b]')
```

## aos_prov/main.py

```diff
@@ -1,25 +1,21 @@
 #
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
 #
 
 import argparse
 import logging
 import sys
 from pathlib import Path
 
-from colorama import Fore, Style, init
-
-from aos_prov.actions import create_new_unit
-from aos_prov.actions import download_image
-from aos_prov.commands.command_provision import run_provision
+from aos_prov.actions import create_new_unit, download_image, provision_unit, start_vm
 from aos_prov.communication.cloud.cloud_api import DEFAULT_REGISTER_PORT, CloudAPI
 from aos_prov.utils import DEFAULT_USER_CERT_PATH, DEFAULT_USER_KEY_PATH
-from aos_prov.utils.common import DISK_IMAGE_DOWNLOAD_URL, AOS_DISKS_PATH
+from aos_prov.utils.common import DISK_IMAGE_DOWNLOAD_URL, AOS_DISKS_PATH, print_error
 from aos_prov.utils.errors import CloudAccessError, BoardError, DeviceRegisterError, OnBoardingError
 from aos_prov.utils.user_credentials import UserCredentials
 
 try:
     from importlib.metadata import version  # noqa: WPS433
 except ImportError:
     import importlib_metadata as version  # noqa: WPS433
@@ -61,69 +57,77 @@
         default=DEFAULT_USER_KEY_PATH,
         help=f'User key file. Default: {DEFAULT_USER_KEY_PATH}')
 
     parser.add_argument(
         '-p',
         _ARGUMENT_USER_PKCS12,
         required=False,
-        help='Path to user certificate in pkcs12 format',
+        help='Path to user certificate in pkcs12 format.',
         dest='pkcs',
         default=_DEFAULT_USER_CERTIFICATE,
     )
 
     parser.add_argument(
-        '--register-host',
-        help='Overwrite cloud address. By default it is taken from user certificate'
-    )
-
-    parser.add_argument(
         '--register-port',
         default=DEFAULT_REGISTER_PORT,
         help=f'Cloud port. Default: {DEFAULT_REGISTER_PORT}'
     )
 
     parser.add_argument(
-        '-w'
+        '-w',
         '--wait-unit',
-        action='store_true',
-        help=f'Wait for unit.',
-        dest='wait_unit'
+        action='store',
+        metavar='N',
+        help=f'Wait for unit to respond for the first time in minutes. Default value 0 means try once',
+        dest='wait_unit',
+        default=0,
+        type=int
     )
 
     parser.set_defaults(which=None)
 
     sub_parser = parser.add_subparsers(title='Commands')
 
     new_vm_command = sub_parser.add_parser(
         _COMMAND_NEW_VM,
         help='Create new Oracle VM'
     )
     new_vm_command.set_defaults(which=_COMMAND_NEW_VM)
 
     new_vm_command.add_argument(
+        '-N',
         '--name',
         required=True,
         help='Name of the VM'
     )
 
     new_vm_command.add_argument(
+        '-D',
         '--disk',
         required=False,
-        help=f'Full path to the disk',
+        help='Full path to the AosCore-powered disk.',
         default=AOS_DISKS_PATH
     )
 
     start_vm_command = sub_parser.add_parser(
         _COMMAND_START_VM,
         help='Start the VM'
     )
     start_vm_command.add_argument(
+        '-N',
         '--name',
         required=True,
-        help='Name of the VM'
+        help='Name of the VirtualBox group where VMs are located.'
+    )
+
+    start_vm_command.add_argument(
+        '-H',
+        '--headless',
+        action='store_true',
+        help='Start VMs in headless mode.'
     )
     start_vm_command.set_defaults(which=_COMMAND_START_VM)
 
     create_unit_command = sub_parser.add_parser(
         _COMMAND_UNIT_CREATE,
         help='Create and provision new VirtualBox-based unit'
     )
@@ -134,29 +138,36 @@
         required=True,
         help='Name of the VM'
     )
 
     create_unit_command.add_argument(
         '--disk',
         required=False,
-        help='Full path to the disk',
+        help='Full path to the AosCore-powered disk.',
         default=AOS_DISKS_PATH
     )
 
     create_unit_command.add_argument(
+        '-H',
+        '--headless',
+        action='store_true',
+        help='Start created VMs in headless mode.'
+    )
+
+    create_unit_command.add_argument(
         '-p',
         _ARGUMENT_USER_PKCS12,
         required=False,
         help='Path to user certificate in pkcs12 format',
         dest='pkcs',
         default=_DEFAULT_USER_CERTIFICATE,
     )
 
     parser.add_argument(
-        '-v',
+        '-V',
         '--version',
         action='version',
         version=f"%(prog)s {version('aos-prov')}")
 
     download_command = sub_parser.add_parser(_COMMAND_DOWNLOAD, help='Download image')
     download_command.set_defaults(which=_COMMAND_DOWNLOAD)
     download_command.add_argument(
@@ -181,57 +192,62 @@
         (args.cert != DEFAULT_USER_CERT_PATH or args.key != DEFAULT_USER_KEY_PATH):
         args.pkcs = None
     return UserCredentials(cert_file_path=args.cert, key_file_path=args.key, pkcs12=args.pkcs)
 
 
 def main():
     """The main entry point."""
-    init()
     status = 0
     args = _parse_args()
-    print(args)
+
     try:
         if args.which is None:
             uc = _parse_user_creds(args)
             cloud_api = CloudAPI(uc, args.register_port)
             cloud_api.check_cloud_access()
-            wait = 1
-            if args.wait_unit:
-                wait = 20
-            run_provision(args.unit, cloud_api, wait)
+
+            if args.wait_unit == 0:
+                wait = 1
+            else:
+                wait = args.wait_unit // 5
+
+            provision_unit(args.unit, cloud_api, wait)
+
         if args.which == _COMMAND_DOWNLOAD:
             url = DISK_IMAGE_DOWNLOAD_URL
             if args.download_address:
                 url = args.download_address
             download_image(url, args.force)
+
         if args.which == _COMMAND_NEW_VM:
             uc = _parse_user_creds(args)
             create_new_unit(args.name, uc, args.disk)
+
         if args.which == _COMMAND_START_VM:
-            from aos_prov.commands.command_vm import start_vm
-            start_vm(args.name)
+            start_vm(args.name, args.headless)
+
         if args.which == _COMMAND_UNIT_CREATE:
             uc = _parse_user_creds(args)
-            create_new_unit(args.name, uc, args.disk, do_provision=True)
+            create_new_unit(args.name, uc, args.disk, do_provision=True, headless=args.headless)
+
     except CloudAccessError as e:
-        logger.error('\nUnable to provision the board with error:\n%s', str(e))
+        print_error(f"Failed during communication with the AosCloud with error: {str(e)}")
         status = 1
     except DeviceRegisterError as e:
-        print(f"{Fore.RED}FAILED with error: {str(e)} {Style.RESET_ALL}")
-        logger.error('Failed: %s', str(e))
+        print_error(f"FAILED with error: {str(e)}")
         status = 1
     except BoardError as e:
-        logger.error(f'{Fore.RED}Failed during communication with device with error: \n {str(e)}{Style.RESET_ALL}', )
+        print_error(f'Failed during communication with device with error: \n {str(e)}')
         status = 1
     except OnBoardingError as e:
-        print(f"{Fore.RED}Failed to execute the command! {Style.RESET_ALL}")
-        print(f"{Fore.RED}Error: {Style.RESET_ALL}" + str(e))
+        print_error('Failed to execute the command!')
+        print_error(f'Error: {str(e)} ')
         status = 1
     except (AssertionError, KeyboardInterrupt):
-        sys.stdout.write('Exiting ...\n')
+        print_error('Stopped by keyboard...')
         status = 1
 
     sys.exit(status)
 
 
 if __name__ == '__main__':
     main()
```

## aos_prov/commands/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
```

## aos_prov/commands/command_provision.py

```diff
@@ -1,183 +1,189 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-"""Provision unit."""
-
-import time
-
-from colorama import Fore, Style
-from aos_prov.communication.cloud.cloud_api import CloudAPI
-from aos_prov.communication.unit.v0.unit_communication import UnitCommunication
-from aos_prov.communication.unit.v1.unit_communication_v1 import UnitCommunicationV1
-from aos_prov.communication.unit.v2.unit_communication_v2 import UnitCommunicationV2
-from aos_prov.communication.unit.v4.unit_communication_v4 import UnitCommunicationV4
-from aos_prov.utils.config import Config
-from aos_prov.utils.errors import GrpcUnimplemented, BoardError
-from aos_prov.utils.common import generate_random_password, console
-
-COMMAND_TO_DECRYPT = 'diskencryption'
-
-
-def run_provision(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1):
-    """
-    Provision Unit. This function will try to provision starting from the newest to the oldest.
-
-    Args:
-         unit_address (str): Address of the Unit
-         cloud_api (CloudAPI): URL to download
-         reconnect_times (int): URL to download
-
-    Raises:
-        AosProvError: If provision fails.
-    """
-    config = Config()
-    uc = UnitCommunicationV4(unit_address)
-    model_name = ''
-    for retry in range(reconnect_times):
-        try:
-            console.print('Starting provisioning using protocol v4')
-            config.system_id, model_name = uc.get_system_info()
-            config.protocol_version = uc.get_protocol_version()
-            break
-        except GrpcUnimplemented:
-            try:
-                console.print('v4 is not supported. Starting provisioning using protocol v2')
-                uc = UnitCommunicationV2(unit_address)
-                if uc.get_protocol_version() == 3:
-                    uc.need_set_users = False
-                config.system_id, model_name = uc.get_system_info()
-                config.protocol_version = uc.get_protocol_version()
-                break
-            except GrpcUnimplemented:
-                try:
-                    print('v2 is not supported. Using protocol v1')
-                    uc = UnitCommunicationV1(unit_address)
-                    config.system_id, model_name = uc.get_system_info()
-                    config.protocol_version = uc.get_protocol_version()
-                    break
-                except GrpcUnimplemented:
-                    print('v1 is not supported. Using protocol v0')
-                    uc = UnitCommunication(unit_address)
-                    config.system_id, model_name = uc.get_system_info()
-                    config.protocol_version = uc.get_protocol_version()
-                    break
-        except BoardError as be:
-            if retry + 1 < reconnect_times:
-                time.sleep(5)
-            else:
-                raise be
-
-    if config.system_id is None:
-        raise BoardError('Cannot read system_id')
-
-    config.set_model(model_name)
-    cloud_api.check_unit_is_not_provisioned(config.system_id)
-    if config.protocol_version >= 4:  # support of multi domains
-        config.node_ids = uc.get_all_node_ids()
-        for node_id in config.node_ids:
-            config.supported_cert_types = uc.get_cert_types(node_id)
-
-            password = generate_random_password()
-
-            for cert_type in config.supported_cert_types:
-                uc.clear(cert_type, node_id)
-
-            for cert_type in config.supported_cert_types:
-                uc.set_cert_owner(cert_type, password, node_id)
-
-            if COMMAND_TO_DECRYPT in config.supported_cert_types:
-                config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
-                uc.encrypt_disk(password, node_id)
-                uc.wait_for_connection()
-
-            for cert_type in config.supported_cert_types:
-                config.unit_certificates.append(uc.create_keys(cert_type, password, node_id))
-    else:
-        config.supported_cert_types = uc.get_cert_types()
-
-        password = generate_random_password()
-
-        for cert_type in config.supported_cert_types:
-            uc.clear(cert_type)
-
-        for cert_type in config.supported_cert_types:
-            uc.set_cert_owner(cert_type, password)
-
-        if COMMAND_TO_DECRYPT in config.supported_cert_types:
-            config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
-            uc.encrypt_disk(password)
-            uc.wait_for_connection()
-
-        for cert_type in config.supported_cert_types:
-            config.unit_certificates.append(uc.create_keys(cert_type, password))
-
-    register_payload = {
-        'hardware_id': config.system_id,
-        'system_uid': config.system_id,
-        'board_model_name': config.model_name,
-        'board_model_version': config.model_version,
-        'provisioning_software': "aos-provisioning:{version}".format(version=3.1),
-        'additional_csrs': []
-    }
-
-    if cloud_api.use_model_name_param():
-        register_payload['model_name'] = config.model_name
-        register_payload['model_version'] = config.model_version
-    else:
-        register_payload['board_model_name'] = config.model_name
-        register_payload['board_model_version'] = config.model_version
-
-    for cert in config.unit_certificates:
-        if cert.cert_type == 'online':
-            register_payload['online_public_csr'] = cert.csr
-            if cert.node_id:
-                register_payload['online_public_node_id'] = cert.node_id
-        elif cert.cert_type == 'offline':
-            register_payload['offline_public_csr'] = cert.csr
-            if cert.node_id:
-                register_payload['offline_public_node_id'] = cert.node_id
-        else:
-            register_payload['additional_csrs'].append({
-                'cert_type': cert.cert_type,
-                'csr': cert.csr,
-                'node_id': cert.node_id,
-            })
-
-    response = cloud_api.register_device(register_payload)
-    system_uid = response.get('system_uid')
-    additional_certs = response.get('additional_certs', [])
-    for cert in config.unit_certificates:
-        if cert.cert_type == 'online':
-            cert.certificate = response.get('online_certificate')
-        elif cert.cert_type == 'offline':
-            cert.certificate = response.get('offline_certificate')
-        else:
-            for ac in additional_certs:
-                if ac['cert_type'] == cert.cert_type:
-                    if ac.get('node_id'):
-                        if ac.get('node_id') == cert.node_id:
-                            cert.certificate = ac['cert']
-                            break
-                    else:
-                        cert.certificate = ac['cert']
-                        cert.node_id = ac.get('node_id')
-                        break
-
-    for cert in config.unit_certificates:
-        uc.apply_certificate(cert)
-
-    claims = response.get('claim')
-
-    if claims:
-        if not hasattr(uc, 'need_set_users'):
-            uc.set_users([claims])
-        elif uc.need_set_users:
-            uc.set_users([claims])
-
-    uc.finish_provisioning()
-
-    print(f'{Fore.GREEN}Finished successfully!{Style.RESET_ALL}')
-    link = cloud_api.get_unit_link_by_system_uid(system_uid)
-    if link:
-        print(f'You may find your unit on the cloud here: {Fore.GREEN}{link}{Style.RESET_ALL}')
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+"""Provision unit."""
+
+import time
+
+from aos_prov.communication.cloud.cloud_api import CloudAPI
+from aos_prov.communication.unit.v0.unit_communication import UnitCommunication
+from aos_prov.communication.unit.v1.unit_communication_v1 import UnitCommunicationV1
+from aos_prov.communication.unit.v2.unit_communication_v2 import UnitCommunicationV2
+from aos_prov.communication.unit.v4.unit_communication_v4 import UnitCommunicationV4
+from aos_prov.utils.common import generate_random_password, print_message
+from aos_prov.utils.config import Config
+from aos_prov.utils.errors import GrpcUnimplemented, BoardError
+
+COMMAND_TO_DECRYPT = 'diskencryption'
+
+
+def run_provision(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1):
+    """
+    Provision Unit. This function will try to provision starting from the newest to the oldest.
+
+    Args:
+         unit_address (str): Address of the Unit
+         cloud_api (CloudAPI): URL to download
+         reconnect_times (int): URL to download
+
+    Raises:
+        AosProvError: If provision fails.
+    """
+    config = Config()
+    uc = UnitCommunicationV4(unit_address)
+    model_name = ''
+    for retry in range(reconnect_times):
+        try:
+            print_message('Starting provisioning using protocol v4....')
+            config.system_id, model_name = uc.get_system_info()
+            config.protocol_version = uc.get_protocol_version()
+            break
+        except GrpcUnimplemented:
+            try:
+                print_message('v4 is not supported. Starting provisioning using protocol v2...')
+                uc = UnitCommunicationV2(unit_address)
+                if uc.get_protocol_version() == 3:
+                    uc.need_set_users = False
+                config.system_id, model_name = uc.get_system_info()
+                config.protocol_version = uc.get_protocol_version()
+                break
+            except GrpcUnimplemented:
+                try:
+                    print_message('v2 is not supported. Using protocol v1')
+                    uc = UnitCommunicationV1(unit_address)
+                    config.system_id, model_name = uc.get_system_info()
+                    config.protocol_version = uc.get_protocol_version()
+                    break
+                except GrpcUnimplemented:
+                    print_message('v1 is not supported. Using protocol v0')
+                    uc = UnitCommunication(unit_address)
+                    config.system_id, model_name = uc.get_system_info()
+                    config.protocol_version = uc.get_protocol_version()
+                    break
+        except BoardError as be:
+            print_message('[yellow]Connection failed')
+            if retry + 1 < reconnect_times:
+                time.sleep(5)
+            else:
+                raise be
+
+    if config.system_id is None:
+        raise BoardError('Cannot read system_id')
+
+    config.set_model(model_name)
+    cloud_api.check_unit_is_not_provisioned(config.system_id)
+    if config.protocol_version >= 4:  # support of multi domains
+        config.node_ids = uc.get_all_node_ids()
+        for node_id in config.node_ids:
+            config.supported_cert_types = uc.get_cert_types(node_id)
+            need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
+
+            password = generate_random_password()
+
+            for cert_type in config.supported_cert_types:
+                uc.clear(cert_type, node_id)
+
+            for cert_type in config.supported_cert_types:
+                uc.set_cert_owner(cert_type, password, node_id)
+
+            if need_disk_encryption:
+                uc.encrypt_disk(password, node_id)
+                config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
+                if config.protocol_version < 4:
+                    uc.wait_for_connection()
+
+
+            for cert_type in config.supported_cert_types:
+                config.unit_certificates.append(uc.create_keys(cert_type, password, node_id))
+    else:
+        config.supported_cert_types = uc.get_cert_types()
+        need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
+
+        password = generate_random_password()
+
+        for cert_type in config.supported_cert_types:
+            uc.clear(cert_type)
+
+        for cert_type in config.supported_cert_types:
+            uc.set_cert_owner(cert_type, password)
+
+        if need_disk_encryption:
+            uc.encrypt_disk(password)
+            config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
+            if config.protocol_version < 4:
+                uc.wait_for_connection()
+
+        for cert_type in config.supported_cert_types:
+            config.unit_certificates.append(uc.create_keys(cert_type, password))
+
+    register_payload = {
+        'hardware_id': config.system_id,
+        'system_uid': config.system_id,
+        'board_model_name': config.model_name,
+        'board_model_version': config.model_version,
+        'provisioning_software': "aos-provisioning:{version}".format(version=3.1),
+        'additional_csrs': []
+    }
+
+    if cloud_api.use_model_name_param():
+        register_payload['model_name'] = config.model_name
+        register_payload['model_version'] = config.model_version
+    else:
+        register_payload['board_model_name'] = config.model_name
+        register_payload['board_model_version'] = config.model_version
+
+    for cert in config.unit_certificates:
+        if cert.cert_type == 'online':
+            register_payload['online_public_csr'] = cert.csr
+            if cert.node_id:
+                register_payload['online_public_node_id'] = cert.node_id
+        elif cert.cert_type == 'offline':
+            register_payload['offline_public_csr'] = cert.csr
+            if cert.node_id:
+                register_payload['offline_public_node_id'] = cert.node_id
+        else:
+            register_payload['additional_csrs'].append({
+                'cert_type': cert.cert_type,
+                'csr': cert.csr,
+                'node_id': cert.node_id,
+            })
+
+    response = cloud_api.register_device(register_payload)
+    system_uid = response.get('system_uid')
+    additional_certs = response.get('additional_certs', [])
+    for cert in config.unit_certificates:
+        if cert.cert_type == 'online':
+            cert.certificate = response.get('online_certificate')
+        elif cert.cert_type == 'offline':
+            cert.certificate = response.get('offline_certificate')
+        else:
+            for ac in additional_certs:
+                if ac['cert_type'] == cert.cert_type:
+                    if ac.get('node_id'):
+                        if ac.get('node_id') == cert.node_id:
+                            cert.certificate = ac['cert']
+                            break
+                    else:
+                        cert.certificate = ac['cert']
+                        cert.node_id = ac.get('node_id')
+                        break
+
+    for cert in config.unit_certificates:
+        uc.apply_certificate(cert)
+
+    claims = response.get('claim')
+
+    if claims:
+        if not hasattr(uc, 'need_set_users'):
+            uc.set_users([claims])
+        elif uc.need_set_users:
+            uc.set_users([claims])
+
+    uc.finish_provisioning()
+
+    print_message('[green]Finished successfully!')
+    link = cloud_api.get_unit_link_by_system_uid(system_uid)
+
+    if link:
+        print_message(f'You may find your unit on the cloud here: [green]{link}')
```

## aos_prov/commands/command_vm.py

 * *Ordering differences only*

```diff
@@ -1,138 +1,138 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
-import platform
-import socket
-import sys
-from pathlib import Path
-from random import randint
-from shutil import copyfile
-
-if platform.system() == 'Linux':
-    sys.path.append('/usr/lib/virtualbox')
-    sys.path.append('/usr/lib/virtualbox/sdk/bindings/xpcom/python/')
-elif platform.system() == 'Darwin':
-    sys.path.append('/Applications/VirtualBox.app/Contents/MacOS')
-    sys.path.append('/Applications/VirtualBox.app/Contents/MacOS/sdk/bindings/xpcom/python/')
-
-
-from aos_prov.actions import download_image
-from aos_prov.utils.common import DISK_IMAGE_DOWNLOAD_URL, AOS_DISK_PATH
-from aos_prov.utils.errors import OnBoardingError, AosProvError
-
-try:
-    import virtualbox
-    from virtualbox.library import StorageBus, StorageControllerType, IMachine, \
-        DeviceType, AccessMode, NATProtocol, FirmwareType
-except Exception:
-    pass
-
-
-def __create_storage_controller(machine: IMachine):
-    storage_controller = machine.add_storage_controller('IDE', StorageBus.ide)
-    storage_controller.controller_type = StorageControllerType.piix4
-    storage_controller.use_host_io_cache = True
-
-
-def __attach_disk(machine: IMachine, location):
-    medium = machine.parent.open_medium(
-        location,
-        DeviceType.hard_disk,
-        AccessMode.read_write,
-        True
-    )
-    machine.attach_device('IDE', 0, 0, DeviceType.hard_disk, medium)
-
-
-def __check_disk_exist(disk_location: str):
-    disk = Path(disk_location)
-    if not disk.is_file():
-        raise OnBoardingError("Disk file not found")
-
-
-def new_vm(vm_name: str, disk_location: str):
-    print('Creating new virtual machine...')
-
-    disk_location_path = Path(disk_location)
-
-    if not disk_location_path.is_file():
-        if disk_location_path == AOS_DISK_PATH:
-            download_image(DISK_IMAGE_DOWNLOAD_URL)
-        else:
-            raise AosProvError('Disk image ' + disk_location + ' not found or not a file')
-
-    vbox = virtualbox.VirtualBox()
-    try:
-        machine = vbox.create_machine('', vm_name, ['/AosUnits'], 'Linux_64', '')
-    except virtualbox.library_base.VBoxError:
-        raise Exception('Such VM exist')
-    machine.vram_size = 32
-    machine.memory_size = 256
-    machine.cpu_count = 1
-    machine.firmware_type = FirmwareType.efi
-    machine.bios_settings.ioapic_enabled = platform.system() != 'Windows'
-    __create_storage_controller(machine)
-    vbox.register_machine(machine)
-
-    machine_folder = vbox.system_properties.default_machine_folder
-    machine_config_file_name = vbox.compose_machine_filename(vm_name, '/AosUnits', '', machine_folder)
-    vm_dir = Path(machine_config_file_name).parent
-    disk_image = str(Path(vm_dir / 'aos-disk.vmdk').absolute())
-    copyfile(disk_location, disk_image)
-
-    with machine.create_session() as session:
-        __attach_disk(session.machine, location=disk_image)
-        session.machine.save_settings()
-
-    return forward_provisioning_ports(vm_name, vm_name + 'PortForward')
-
-
-def start_vm(vm_name: str):
-    print('Starting virtual machine...')
-    vbox = virtualbox.VirtualBox()
-    machine = vbox.find_machine(vm_name)
-    session = virtualbox.Session()
-    vm = machine.launch_vm_process(session, "gui", [])
-    vm.wait_for_completion(timeout=-1)
-
-
-def forward_provisioning_ports(vm_name: str, redirect_name: str = 'provisioningPortForward', forward_to_port=None):
-    if forward_to_port is None:
-        forward_to_port = randint(8090, 8999)
-        while _is_port_in_use(forward_to_port):
-            forward_to_port = randint(8090, 8999)
-
-    print(f'...will forward provisioning port {8089} to {forward_to_port}')
-    vbox = virtualbox.VirtualBox()
-    machine = vbox.find_machine(vm_name)
-    session = virtualbox.Session()
-    try:
-        machine.lock_machine(session, virtualbox.library.LockType.write)
-        mutable_machine = session.machine
-        adapter = mutable_machine.get_network_adapter(0)
-        adapter.nat_engine.add_redirect(redirect_name, NATProtocol(1), '', forward_to_port, '0.0.0.0', 8089)
-        session.machine.save_settings()
-    finally:
-        session.unlock_machine()
-    return forward_to_port
-
-
-def delete_provisioning_ports(vm_name: str, redirect_name: str = 'provisioningPortForward'):
-    vbox = virtualbox.VirtualBox()
-    machine = vbox.find_machine(vm_name)
-    session = virtualbox.Session()
-    try:
-        machine.lock_machine(session, virtualbox.library.LockType.write)
-        mutable_machine = session.machine
-        adapter = mutable_machine.get_network_adapter(0)
-        adapter.nat_engine.remove_redirect(redirect_name)
-        session.machine.save_settings()
-        session.unlock_machine()
-    except Exception:
-        pass
-
-
-def _is_port_in_use(port):
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        return s.connect_ex(('localhost', port)) == 0
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+import platform
+import socket
+import sys
+from pathlib import Path
+from random import randint
+from shutil import copyfile
+
+if platform.system() == 'Linux':
+    sys.path.append('/usr/lib/virtualbox')
+    sys.path.append('/usr/lib/virtualbox/sdk/bindings/xpcom/python/')
+elif platform.system() == 'Darwin':
+    sys.path.append('/Applications/VirtualBox.app/Contents/MacOS')
+    sys.path.append('/Applications/VirtualBox.app/Contents/MacOS/sdk/bindings/xpcom/python/')
+
+
+from aos_prov.actions import download_image
+from aos_prov.utils.common import DISK_IMAGE_DOWNLOAD_URL, AOS_DISK_PATH
+from aos_prov.utils.errors import OnBoardingError, AosProvError
+
+try:
+    import virtualbox
+    from virtualbox.library import StorageBus, StorageControllerType, IMachine, \
+        DeviceType, AccessMode, NATProtocol, FirmwareType
+except Exception:
+    pass
+
+
+def __create_storage_controller(machine: IMachine):
+    storage_controller = machine.add_storage_controller('IDE', StorageBus.ide)
+    storage_controller.controller_type = StorageControllerType.piix4
+    storage_controller.use_host_io_cache = True
+
+
+def __attach_disk(machine: IMachine, location):
+    medium = machine.parent.open_medium(
+        location,
+        DeviceType.hard_disk,
+        AccessMode.read_write,
+        True
+    )
+    machine.attach_device('IDE', 0, 0, DeviceType.hard_disk, medium)
+
+
+def __check_disk_exist(disk_location: str):
+    disk = Path(disk_location)
+    if not disk.is_file():
+        raise OnBoardingError("Disk file not found")
+
+
+def new_vm(vm_name: str, disk_location: str):
+    print('Creating new virtual machine...')
+
+    disk_location_path = Path(disk_location)
+
+    if not disk_location_path.is_file():
+        if disk_location_path == AOS_DISK_PATH:
+            download_image(DISK_IMAGE_DOWNLOAD_URL)
+        else:
+            raise AosProvError('Disk image ' + disk_location + ' not found or not a file')
+
+    vbox = virtualbox.VirtualBox()
+    try:
+        machine = vbox.create_machine('', vm_name, ['/AosUnits'], 'Linux_64', '')
+    except virtualbox.library_base.VBoxError:
+        raise Exception('Such VM exist')
+    machine.vram_size = 32
+    machine.memory_size = 256
+    machine.cpu_count = 1
+    machine.firmware_type = FirmwareType.efi
+    machine.bios_settings.ioapic_enabled = platform.system() != 'Windows'
+    __create_storage_controller(machine)
+    vbox.register_machine(machine)
+
+    machine_folder = vbox.system_properties.default_machine_folder
+    machine_config_file_name = vbox.compose_machine_filename(vm_name, '/AosUnits', '', machine_folder)
+    vm_dir = Path(machine_config_file_name).parent
+    disk_image = str(Path(vm_dir / 'aos-disk.vmdk').absolute())
+    copyfile(disk_location, disk_image)
+
+    with machine.create_session() as session:
+        __attach_disk(session.machine, location=disk_image)
+        session.machine.save_settings()
+
+    return forward_provisioning_ports(vm_name, vm_name + 'PortForward')
+
+
+def start_vm(vm_name: str):
+    print('Starting virtual machine...')
+    vbox = virtualbox.VirtualBox()
+    machine = vbox.find_machine(vm_name)
+    session = virtualbox.Session()
+    vm = machine.launch_vm_process(session, "gui", [])
+    vm.wait_for_completion(timeout=-1)
+
+
+def forward_provisioning_ports(vm_name: str, redirect_name: str = 'provisioningPortForward', forward_to_port=None):
+    if forward_to_port is None:
+        forward_to_port = randint(8090, 8999)
+        while _is_port_in_use(forward_to_port):
+            forward_to_port = randint(8090, 8999)
+
+    print(f'...will forward provisioning port {8089} to {forward_to_port}')
+    vbox = virtualbox.VirtualBox()
+    machine = vbox.find_machine(vm_name)
+    session = virtualbox.Session()
+    try:
+        machine.lock_machine(session, virtualbox.library.LockType.write)
+        mutable_machine = session.machine
+        adapter = mutable_machine.get_network_adapter(0)
+        adapter.nat_engine.add_redirect(redirect_name, NATProtocol(1), '', forward_to_port, '0.0.0.0', 8089)
+        session.machine.save_settings()
+    finally:
+        session.unlock_machine()
+    return forward_to_port
+
+
+def delete_provisioning_ports(vm_name: str, redirect_name: str = 'provisioningPortForward'):
+    vbox = virtualbox.VirtualBox()
+    machine = vbox.find_machine(vm_name)
+    session = virtualbox.Session()
+    try:
+        machine.lock_machine(session, virtualbox.library.LockType.write)
+        mutable_machine = session.machine
+        adapter = mutable_machine.get_network_adapter(0)
+        adapter.nat_engine.remove_redirect(redirect_name)
+        session.machine.save_settings()
+        session.unlock_machine()
+    except Exception:
+        pass
+
+
+def _is_port_in_use(port):
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        return s.connect_ex(('localhost', port)) == 0
```

## aos_prov/commands/command_vm_libvirt.py

 * *Ordering differences only*

```diff
@@ -1,80 +1,80 @@
-import libvirt
-import os
-import random
-import socket
-import sys
-import uuid
-from pathlib import Path
-from shutil import copyfile
-
-if sys.version_info > (3, 9):
-    from importlib import resources as pkg_resources  # noqa: WPS433, WPS440
-else:
-    import importlib_resources as pkg_resources  # noqa: WPS433, WPS440
-
-from aos_prov.command_download import download_image
-
-__FILES_DIR = 'aos_prov'
-__VM_FILENAME = 'files/vm.xml'
-
-_DOWNLOADS_PATH = Path.home() / '.aos' / 'downloads'
-_VIRT_UNITS_PATH = Path.home() / '.aos' / 'virtual-units'
-
-_IMG_FILE_NAME = 'aos-disk.vmdk'
-
-
-def random_mac():
-    mac = [0x00, 0x16, 0x3e, random.randint(0x00, 0x7f), random.randint(0x00, 0xff), random.randint(0x00, 0xff)]
-    return ':'.join(map(lambda x: "%02x" % x, mac))
-
-
-def _is_port_in_use(port):
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        return s.connect_ex(('localhost', port)) == 0
-
-
-def create_libvirt_vm(name: str, forward_to_port=None):
-    vm_config = pkg_resources.files(__FILES_DIR) / __VM_FILENAME
-    with pkg_resources.as_file(vm_config) as config:
-        with open(config, 'r') as f:
-            xml_config = f.read()
-
-    new_uuid = str(uuid.uuid4())
-    mac_address = random_mac()
-    new_vm_path = str(_VIRT_UNITS_PATH / name / _IMG_FILE_NAME)
-    if not Path(_DOWNLOADS_PATH / _IMG_FILE_NAME).exists():
-        download_image()
-    Path(_VIRT_UNITS_PATH / name).mkdir(parents=True, exist_ok=False)
-
-    copyfile(str(_DOWNLOADS_PATH / _IMG_FILE_NAME), new_vm_path)
-
-    if forward_to_port is None:
-        forward_to_port = random.randint(8090, 8999)
-        while _is_port_in_use(forward_to_port):
-            forward_to_port = random.randint(8090, 8999)
-
-    xml_config = xml_config.format(
-        vm_name=name,
-        uuid=new_uuid,
-        disk_path=new_vm_path,
-        mac_address=mac_address,
-        port_forward=forward_to_port
-    )
-
-    try:
-        conn = libvirt.open("qemu:///system")
-    except libvirt.libvirtError as e:
-        print(repr(e), file=sys.stderr)
-        exit(1)
-
-    try:
-        dom = conn.defineXMLFlags(xml_config, 0)
-    except libvirt.libvirtError as e:
-        print(repr(e), file=sys.stderr)
-        exit(1)
-
-    if dom.create() < 0:
-        print('Can not boot guest domain.', file=sys.stderr)
-        exit(1)
-
-    return new_uuid, forward_to_port
+import libvirt
+import os
+import random
+import socket
+import sys
+import uuid
+from pathlib import Path
+from shutil import copyfile
+
+if sys.version_info > (3, 9):
+    from importlib import resources as pkg_resources  # noqa: WPS433, WPS440
+else:
+    import importlib_resources as pkg_resources  # noqa: WPS433, WPS440
+
+from aos_prov.command_download import download_image
+
+__FILES_DIR = 'aos_prov'
+__VM_FILENAME = 'files/vm.xml'
+
+_DOWNLOADS_PATH = Path.home() / '.aos' / 'downloads'
+_VIRT_UNITS_PATH = Path.home() / '.aos' / 'virtual-units'
+
+_IMG_FILE_NAME = 'aos-disk.vmdk'
+
+
+def random_mac():
+    mac = [0x00, 0x16, 0x3e, random.randint(0x00, 0x7f), random.randint(0x00, 0xff), random.randint(0x00, 0xff)]
+    return ':'.join(map(lambda x: "%02x" % x, mac))
+
+
+def _is_port_in_use(port):
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        return s.connect_ex(('localhost', port)) == 0
+
+
+def create_libvirt_vm(name: str, forward_to_port=None):
+    vm_config = pkg_resources.files(__FILES_DIR) / __VM_FILENAME
+    with pkg_resources.as_file(vm_config) as config:
+        with open(config, 'r') as f:
+            xml_config = f.read()
+
+    new_uuid = str(uuid.uuid4())
+    mac_address = random_mac()
+    new_vm_path = str(_VIRT_UNITS_PATH / name / _IMG_FILE_NAME)
+    if not Path(_DOWNLOADS_PATH / _IMG_FILE_NAME).exists():
+        download_image()
+    Path(_VIRT_UNITS_PATH / name).mkdir(parents=True, exist_ok=False)
+
+    copyfile(str(_DOWNLOADS_PATH / _IMG_FILE_NAME), new_vm_path)
+
+    if forward_to_port is None:
+        forward_to_port = random.randint(8090, 8999)
+        while _is_port_in_use(forward_to_port):
+            forward_to_port = random.randint(8090, 8999)
+
+    xml_config = xml_config.format(
+        vm_name=name,
+        uuid=new_uuid,
+        disk_path=new_vm_path,
+        mac_address=mac_address,
+        port_forward=forward_to_port
+    )
+
+    try:
+        conn = libvirt.open("qemu:///system")
+    except libvirt.libvirtError as e:
+        print(repr(e), file=sys.stderr)
+        exit(1)
+
+    try:
+        dom = conn.defineXMLFlags(xml_config, 0)
+    except libvirt.libvirtError as e:
+        print(repr(e), file=sys.stderr)
+        exit(1)
+
+    if dom.create() < 0:
+        print('Can not boot guest domain.', file=sys.stderr)
+        exit(1)
+
+    return new_uuid, forward_to_port
```

## aos_prov/commands/download.py

```diff
@@ -1,117 +1,116 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-"""Download and save files command."""
-import gzip
-from pathlib import Path
-
-import requests
-from rich.progress import Progress
-
-import tarfile
-from aos_prov.utils.common import DOWNLOADS_PATH
-from aos_prov.utils.errors import AosProvError
-
-
-_SAVE_CHUNK = 8192
-
-
-def _create_downloads_directory():
-    Path(DOWNLOADS_PATH).mkdir(parents=True, exist_ok=True)
-
-
-def _is_gz_file(filepath):
-    with open(filepath, 'rb') as test_f:
-        return test_f.read(2) == b'\x1f\x8b'
-
-
-def download_and_save_multinode(download_url: str, save_path: Path, force_overwrite: bool = False) -> None:
-    """Download and save multinide images.
-
-    Args:
-         download_url (str): URL to download
-         save_path (Path): Save destination url
-         force_overwrite (bool): Force to overwrite files
-
-    Raises:
-        AosProvError: If files exists and force_overwrite is false.
-    """
-    _create_downloads_directory()
-
-    node_files = [save_path / 'aos-node0.vmdk', save_path / 'aos-node1.vmdk']
-
-    for node_file in node_files:
-        if force_overwrite:
-            node_file.unlink(True)
-        elif node_file.exists():
-            raise AosProvError(f'Destination file {node_file} already exist. Delete it or download with -f key')
-
-    download_file_name = save_path / 'downloaded-multi-node-images.tar.gz'
-
-    with open(download_file_name, 'wb') as save_context:
-        response = requests.get(download_url, stream=True)
-        total_length = response.headers.get('content-length')
-
-        if total_length is None:  # no content length header
-            save_context.write(response.content)
-            return
-
-        with Progress() as progress:
-            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
-            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
-                progress.update(task_id, advance=len(received_data))
-                save_context.write(received_data)
-
-    with tarfile.open(download_file_name) as archive:
-        archive.extractall(save_path)
-
-    download_file_name.unlink()
-
-
-def download_and_save_file(
-    download_url: str,
-    save_path: Path,
-    force_overwrite: bool = False,
-    untargz: bool = False
-) -> None:
-    """Download and save file.
-
-    Args:
-         download_url (str): URL to download
-         save_path (Path): URL to download
-         force_overwrite (bool): URL to download
-
-    Raises:
-        AosProvError: If file exists and force_overwrite is false.
-    """
-    _create_downloads_directory()
-
-    if save_path.exists() and not force_overwrite:
-        raise AosProvError('Destination file already exist.')
-
-    with open(save_path, 'wb') as save_context:
-        response = requests.get(download_url, stream=True)
-        total_length = response.headers.get('content-length')
-
-        if total_length is None:  # no content length header
-            save_context.write(response.content)
-            return
-
-        with Progress() as progress:
-            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
-            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
-                progress.update(task_id, advance=len(received_data))
-                save_context.write(received_data)
-
-    if untargz:
-        with tarfile.open(save_path) as archive:
-            archive.extractall(save_path)
-
-    elif _is_gz_file(save_path):
-        with gzip.open(save_path, 'rb') as f:
-            with open(DOWNLOADS_PATH / 'tmp_unpacked', 'wb') as tmp_file:
-                tmp_file.write(f.read())
-
-        Path(save_path).unlink()
-        Path(DOWNLOADS_PATH / 'tmp_unpacked').rename(save_path)
+#
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
+#
+"""Download and save files command."""
+import gzip
+import tarfile
+from pathlib import Path
+
+import requests
+from rich.progress import Progress
+
+from aos_prov.utils.common import DOWNLOADS_PATH, NODE0_IMAGE_FILENAME, NODE1_IMAGE_FILENAME
+from aos_prov.utils.errors import AosProvError
+
+_SAVE_CHUNK = 8192
+
+
+def _create_downloads_directory():
+    Path(DOWNLOADS_PATH).mkdir(parents=True, exist_ok=True)
+
+
+def _is_gz_file(filepath):
+    with open(filepath, 'rb') as test_f:
+        return test_f.read(2) == b'\x1f\x8b'
+
+
+def download_and_save_multinode(download_url: str, save_path: Path, force_overwrite: bool = False) -> None:
+    """Download and save multi-node images.
+
+    Args:
+         download_url (str): URL to download
+         save_path (Path): Save destination url
+         force_overwrite (bool): Force to overwrite files
+
+    Raises:
+        AosProvError: If files exists and force_overwrite is false.
+    """
+    _create_downloads_directory()
+
+    node_files = [save_path / NODE0_IMAGE_FILENAME, save_path / NODE1_IMAGE_FILENAME]
+
+    for node_file in node_files:
+        if force_overwrite:
+            node_file.unlink(True)
+        elif node_file.exists():
+            raise AosProvError(f'Destination file {node_file} already exist. Delete it or download with -f key')
+
+    download_file_name = save_path / 'downloaded-multi-node-images.tar.gz'
+
+    with open(download_file_name, 'wb') as save_context:
+        response = requests.get(download_url, stream=True)
+        total_length = response.headers.get('content-length')
+
+        if total_length is None:  # no content length header
+            save_context.write(response.content)
+            return
+
+        with Progress() as progress:
+            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
+            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
+                progress.update(task_id, advance=len(received_data))
+                save_context.write(received_data)
+
+    with tarfile.open(download_file_name) as archive:
+        archive.extractall(save_path)
+
+    download_file_name.unlink()
+
+
+def download_and_save_file(
+    download_url: str,
+    save_path: Path,
+    force_overwrite: bool = False,
+    untargz: bool = False
+) -> None:
+    """Download and save file.
+
+    Args:
+         download_url (str): URL to download
+         save_path (Path): URL to download
+         force_overwrite (bool): URL to download
+
+    Raises:
+        AosProvError: If file exists and force_overwrite is false.
+    """
+    _create_downloads_directory()
+
+    if save_path.exists() and not force_overwrite:
+        raise AosProvError('Destination file already exist.')
+
+    with open(save_path, 'wb') as save_context:
+        response = requests.get(download_url, stream=True)
+        total_length = response.headers.get('content-length')
+
+        if total_length is None:  # no content length header
+            save_context.write(response.content)
+            return
+
+        with Progress() as progress:
+            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
+            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
+                progress.update(task_id, advance=len(received_data))
+                save_context.write(received_data)
+
+    if untargz:
+        with tarfile.open(save_path) as archive:
+            archive.extractall(save_path)
+
+    elif _is_gz_file(save_path):
+        with gzip.open(save_path, 'rb') as f:
+            with open(DOWNLOADS_PATH / 'tmp_unpacked', 'wb') as tmp_file:
+                tmp_file.write(f.read())
+
+        Path(save_path).unlink()
+        Path(DOWNLOADS_PATH / 'tmp_unpacked').rename(save_path)
```

## aos_prov/communication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/cloud/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
```

## aos_prov/communication/cloud/cloud_api.py

```diff
@@ -1,182 +1,183 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-import OpenSSL
-import logging
-import requests
-import sys
-from colorama import Fore, Style
-from urllib.parse import urlencode
-
-if sys.version_info > (3, 9):
-    from importlib import resources as pkg_resources  # noqa: WPS433, WPS440
-else:
-    import importlib_resources as pkg_resources  # noqa: WPS433, WPS440
-
-from aos_prov.utils.common import console
-from aos_prov.utils.errors import DeviceRegisterError, CloudAccessError
-from aos_prov.utils.user_credentials import UserCredentials
-
-logger = logging.getLogger(__name__)
-
-DEFAULT_REGISTER_HOST = 'aoscloud.io'
-DEFAULT_REGISTER_PORT = 10000
-
-
-class CloudAPI:
-    __FILES_DIR = 'aos_prov'
-    __ROOT_CA_CERT_FILENAME = 'files/1rootCA.crt'
-    __REGISTER_URI_TPL = 'https://{}:{}/api/v1/units/provisioning/'
-    __USER_ME_URI_TPL = 'https://{}:{}/api/v1/users/me/'
-    __UNIT_STATUS_URL = 'https://{}:{}/api/v1/units/?{}'
-    __FIND_UNIT_TPL = 'https://{}:{}/api/v1/units/?{}'
-    __LINK_TO_THE_UNIT_ON_CLOUD_TPL = 'https://{}/oem/units/{}'
-
-    def __init__(self, user_credentials: UserCredentials, cloud_api_port: int = DEFAULT_REGISTER_PORT):
-        self._cloud_api_host = user_credentials.cloud_url
-        self._cloud_api_port = cloud_api_port if cloud_api_port else DEFAULT_REGISTER_PORT
-        self._user_credentials = user_credentials
-
-    def check_cloud_access(self) -> None:
-        """Check user have access to the cloud and his role is OEM.
-
-        Raises:
-            CloudAccessError: If user haven't access to the cloud or his role is not OEM.
-        Returns:
-            None
-        """
-        try:
-            url = self.__USER_ME_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
-            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    resp = requests.get(url, verify=server_certificate_path,
-                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-
-                if resp.status_code != 200:
-                    print('Auth error: {}'.format(resp.text))
-                    raise CloudAccessError('You do not have access to the cloud!')
-
-                user_info = resp.json()
-                if user_info['role'] != 'oem':
-                    logger.debug('invalid user role'.format(resp.text))
-                    raise CloudAccessError('You should use OEM account!')
-
-            print(f'Operation will be executed on domain '
-                  f'{Fore.CYAN}{self._cloud_api_host}{Style.RESET_ALL} using OEM '
-                  f'{Fore.CYAN}{user_info["oem"]["title"]}{Style.RESET_ALL} by user: '
-                  f'{Fore.CYAN}{user_info["username"]}{Style.RESET_ALL}')
-        except ConnectionError as e:
-            raise CloudAccessError('Failed to connect to the cloud')
-        except (requests.exceptions.RequestException, ValueError, OSError, OpenSSL.SSL.Error) as e:
-            print('Check access exception: {}'.format(e))
-            raise CloudAccessError('Failed to connect to the cloud')
-        except ConnectionRefusedError as e:
-            raise CloudAccessError('Failed to connect to the cloud')
-
-    def register_device(self, payload):
-        """Registers device in cloud. Returns registered metadata.
-        :param: str - end_point for registering
-        :param: str - path to server pem that contains certs and a private one
-        :param: dict
-        :return: dict
-        """
-        logger.info('Registering the board ...')
-        end_point = self.__REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
-
-        try:
-            logger.debug('Sending to %s payload: %s', end_point, payload)
-            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    ret = requests.post(end_point, json=payload, verify=server_certificate_path,
-                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-
-                    if ret.status_code == 400:
-                        try:
-                            resp_content = ret.content.decode()
-                            print(str(resp_content))
-                            try:
-                                answer = ret.json()['non_field_errors'][0]
-                                logger.info('Registration error: ' + answer)
-                            except:
-                                pass
-
-                        except UnicodeDecodeError:
-                            resp_content = ret.content
-                            print(resp_content)
-                        logger.debug('Cloud response: {}'.format(resp_content))
-                    ret.raise_for_status()
-                    response = ret.json()
-        except (requests.exceptions.RequestException,
-                ValueError, OSError, OpenSSL.SSL.Error) as e:
-            logger.debug(e)
-            print(e)
-            raise DeviceRegisterError('Failed to register board.')
-
-        return response
-
-    def check_unit_is_not_provisioned(self, system_uid):
-        print('Getting unit\'s status on the cloud ...')
-        try:
-            end_point = self.__UNIT_STATUS_URL.format(
-                self._cloud_api_host,
-                self._cloud_api_port,
-                urlencode({'system_uid': system_uid})
-            )
-            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    response = requests.get(end_point, verify=server_certificate_path,
-                                            cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-
-        except (requests.exceptions.RequestException,
-                ValueError, OSError, OpenSSL.SSL.Error) as e:
-            print('Failed to check unit\'s status: %s', e)
-            raise DeviceRegisterError('Failed to HTTP GET: ', e)
-
-        response_json = response.json()
-
-        if 'results' not in response_json or 'count' not in response_json:
-            raise DeviceRegisterError('Invalid answer from the cloud. Please update current library')
-
-        if response_json['count'] == 0:
-            # There is no such board on the cloud
-            return
-
-        status = response_json.get('results', [{}])[0].get('status')
-        if status is None:
-            return
-
-        if status != 'new':
-            raise DeviceRegisterError(f'Unit is in status "{status}". Please do deprovisioning first.')
-
-    def get_unit_link_by_system_uid(self, system_uid):
-        end_point = self.__FIND_UNIT_TPL.format(
-            self._cloud_api_host,
-            self._cloud_api_port,
-            urlencode({'system_uid': system_uid})
-        )
-        try:
-            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    response = requests.get(end_point, verify=server_certificate_path,
-                                            cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-            unit_id = response.json()['results'][0]['id']
-            unit_domain = self._cloud_api_host
-            if not unit_domain.startswith('api.'):
-                unit_domain = f'api.{unit_domain}'
-            return self.__LINK_TO_THE_UNIT_ON_CLOUD_TPL.format(unit_domain, unit_id)
-        except Exception:
-            return None
-
-    def use_model_name_param(self) -> bool:
-        end_point = self.__REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
-        server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-        with pkg_resources.as_file(server_certificate) as server_certificate_path:
-            with self._user_credentials.user_credentials as temp_creds:
-                resp = requests.options(end_point, verify=server_certificate_path,
-                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-                return 'model_name' in resp.json()['actions']['POST']
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+import logging
+import sys
+from urllib.parse import urlencode
+
+import OpenSSL
+import requests
+
+from aos_prov.utils.common import print_message, print_left, print_success
+
+if sys.version_info > (3, 9):
+    from importlib import resources as pkg_resources  # noqa: WPS433, WPS440
+else:
+    import importlib_resources as pkg_resources  # noqa: WPS433, WPS440
+
+from aos_prov.utils.errors import DeviceRegisterError, CloudAccessError
+from aos_prov.utils.user_credentials import UserCredentials
+
+logger = logging.getLogger(__name__)
+
+DEFAULT_REGISTER_HOST = 'aoscloud.io'
+DEFAULT_REGISTER_PORT = 10000
+
+
+class CloudAPI:
+    __FILES_DIR = 'aos_prov'
+    __ROOT_CA_CERT_FILENAME = 'files/1rootCA.crt'
+    __REGISTER_URI_TPL = 'https://{}:{}/api/v1/units/provisioning/'
+    __USER_ME_URI_TPL = 'https://{}:{}/api/v1/users/me/'
+    __UNIT_STATUS_URL = 'https://{}:{}/api/v1/units/?{}'
+    __FIND_UNIT_TPL = 'https://{}:{}/api/v1/units/?{}'
+    __LINK_TO_THE_UNIT_ON_CLOUD_TPL = 'https://{}/oem/units/{}'
+
+    def __init__(self, user_credentials: UserCredentials, cloud_api_port: int = DEFAULT_REGISTER_PORT):
+        self._cloud_api_host = user_credentials.cloud_url
+        self._cloud_api_port = cloud_api_port if cloud_api_port else DEFAULT_REGISTER_PORT
+        self._user_credentials = user_credentials
+
+    def check_cloud_access(self) -> None:
+        """Check user access on the cloud and his role is OEM.
+
+        Raises:
+            CloudAccessError: If user haven't access to the cloud or his role is not OEM.
+        Returns:
+            None
+        """
+        try:
+            url = self.__USER_ME_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
+            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    resp = requests.get(url, verify=server_certificate_path,
+                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+
+                if resp.status_code != 200:
+                    print_message('[red]Received not HTTP 200 response. ' + str(resp.text))
+                    raise CloudAccessError('You do not have access to the cloud!')
+
+                user_info = resp.json()
+                if user_info['role'] != 'oem':
+                    print_message(f'[red]invalid user role: {resp.text}')
+                    raise CloudAccessError('You should use OEM account!')
+
+            print_left('Operation will be executed on domain:')
+            print_success(self._cloud_api_host)
+            print_left('OEM:')
+            print_success(user_info["oem"]["title"])
+            print_left('user:')
+            print_success(user_info["username"])
+        except ConnectionError as e:
+            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(e))
+        except (requests.exceptions.RequestException, ValueError, OSError, OpenSSL.SSL.Error) as e:
+            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(e) )
+
+
+    def register_device(self, payload):
+        """Registers device in cloud. Returns registered metadata.
+        :param: str - end_point for registering
+        :param: str - path to server pem that contains certs and a private one
+        :param: dict
+        :return: dict
+        """
+        logger.info('Registering the board ...')
+        end_point = self.__REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
+
+        try:
+            logger.debug('Sending to %s payload: %s', end_point, payload)
+            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    ret = requests.post(end_point, json=payload, verify=server_certificate_path,
+                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+
+                    if ret.status_code == 400:
+                        try:
+                            resp_content = ret.content.decode()
+                            print(str(resp_content))
+                            try:
+                                answer = ret.json()['non_field_errors'][0]
+                                logger.info('Registration error: ' + answer)
+                            except:
+                                pass
+
+                        except UnicodeDecodeError:
+                            resp_content = ret.content
+                            print(resp_content)
+                        logger.debug('Cloud response: {}'.format(resp_content))
+                    ret.raise_for_status()
+                    response = ret.json()
+        except (requests.exceptions.RequestException,
+                ValueError, OSError, OpenSSL.SSL.Error) as e:
+            logger.debug(e)
+            print(e)
+            raise DeviceRegisterError('Failed to register board.')
+
+        return response
+
+    def check_unit_is_not_provisioned(self, system_uid):
+        print('Getting unit\'s status on the cloud ...')
+        try:
+            end_point = self.__UNIT_STATUS_URL.format(
+                self._cloud_api_host,
+                self._cloud_api_port,
+                urlencode({'system_uid': system_uid})
+            )
+            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    response = requests.get(end_point, verify=server_certificate_path,
+                                            cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+
+        except (requests.exceptions.RequestException,
+                ValueError, OSError, OpenSSL.SSL.Error) as e:
+            print('Failed to check unit\'s status: %s', e)
+            raise DeviceRegisterError('Failed to HTTP GET: ', e)
+
+        response_json = response.json()
+
+        if 'results' not in response_json or 'count' not in response_json:
+            raise DeviceRegisterError('Invalid answer from the cloud. Please update current library')
+
+        if response_json['count'] == 0:
+            # There is no such board on the cloud
+            return
+
+        status = response_json.get('results', [{}])[0].get('status')
+        if status is None:
+            return
+
+        if status != 'new':
+            raise DeviceRegisterError(f'Unit is in status "{status}". Please do deprovisioning first.')
+
+    def get_unit_link_by_system_uid(self, system_uid):
+        end_point = self.__FIND_UNIT_TPL.format(
+            self._cloud_api_host,
+            self._cloud_api_port,
+            urlencode({'system_uid': system_uid})
+        )
+        try:
+            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    response = requests.get(end_point, verify=server_certificate_path,
+                                            cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+            unit_id = response.json()['results'][0]['id']
+            unit_domain = self._cloud_api_host
+            if not unit_domain.startswith('oem.'):
+                unit_domain = f'oem.{unit_domain}'
+            return self.__LINK_TO_THE_UNIT_ON_CLOUD_TPL.format(unit_domain, unit_id)
+        except Exception:
+            return None
+
+    def use_model_name_param(self) -> bool:
+        end_point = self.__REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
+        server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+        with pkg_resources.as_file(server_certificate) as server_certificate_path:
+            with self._user_credentials.user_credentials as temp_creds:
+                resp = requests.options(end_point, verify=server_certificate_path,
+                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+                return 'model_name' in resp.json()['actions']['POST']
```

## aos_prov/communication/unit/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v0/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v0/unit_communication.py

```diff
@@ -1,126 +1,124 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
-import time
-from contextlib import contextmanager
-
-import grpc
-from colorama import Fore, Style
-
-from aos_prov.communication.unit.v0.generated import api_iamanager_iamanager_pb2 as api_iam_manager, \
-    api_iamanager_iamanager_pb2_grpc as api_iam_manager_grpc
-from aos_prov.utils.errors import BoardError
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-UNIT_DEFAULT_PORT = 8089
-
-
-class UnitCommunication(object):
-    def __init__(self, address: str = 'localhost:8089'):
-        parts = address.split(':')
-        if len(parts) == 2:
-            try:
-                port = int(parts[1])
-                if not 1 <= port <= 65535:
-                    raise BoardError("Unit port is invalid")
-            except ValueError:
-                raise BoardError("Unit port is invalid")
-        else:
-            address = address + ':' + str(UNIT_DEFAULT_PORT)
-        self.__unit_address = address
-        print(f"Will search unit on address: {Fore.GREEN}{self.__unit_address}{Style.RESET_ALL}")
-
-    @contextmanager
-    def unit_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = api_iam_manager_grpc.IAManagerStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-        except grpc.RpcError as e:
-            if catch_inactive and \
-                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
-                return
-            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
-                return
-
-            error_text = (f"{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}"
-                          f"{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}")
-            raise BoardError(error_text)
-
-    def get_protocol_version(self) -> int:
-        return 1
-
-    def get_system_info(self) -> (str, str):
-        with self.unit_stub() as stub:
-            print('Getting System Info...')
-            response = stub.GetSystemInfo(api_iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
-            print('System ID: ' + response.system_id)
-            print('Model name: ' + response.board_model)
-            return response.system_id, response.board_model
-
-    def clear(self, certificate_type: str) -> None:
-        with self.unit_stub() as stub:
-            print('Clear certificate: ' + certificate_type)
-            response = stub.Clear(api_iam_manager.ClearReq(type=certificate_type))
-            return response
-
-    def set_cert_owner(self, certificate_type: str, password: str) -> None:
-        with self.unit_stub() as stub:
-            print('Set owner: ' + certificate_type)
-            response = stub.SetOwner(api_iam_manager.SetOwnerReq(type=certificate_type, password=password))
-            return response
-
-    def get_cert_types(self) -> [str]:
-        with self.unit_stub() as stub:
-            print('Getting certificate types to renew')
-            response = stub.GetCertTypes(api_iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
-            print('Will be renewed: ' + str(response.types))
-            return response.types
-
-    def create_keys(self, cert_type: str, password: str) -> UnitCertificate:
-        with self.unit_stub() as stub:
-            print('Generating key type:' + cert_type)
-            response = stub.CreateKey(api_iam_manager.CreateKeyReq(type=cert_type, password=password))
-            uc = UnitCertificate()
-            uc.cert_type = response.type
-            uc.csr = response.csr
-            return uc
-
-    def apply_certificate(self, unit_cert: UnitCertificate):
-        with self.unit_stub() as stub:
-            stub.ApplyCert(api_iam_manager.ApplyCertReq(type=unit_cert.cert_type, cert=unit_cert.certificate))
-
-    def set_users(self, users: [str]):
-        with self.unit_stub() as stub:
-            stub.SetUsers(api_iam_manager.SetUsersReq(users=users))
-
-    def encrypt_disk(self, password: str):
-        print('Starting disk encryption...')
-        try:
-            with self.unit_stub(wait_for_close=True) as stub:
-                stub.EncryptDisk(api_iam_manager.EncryptDiskReq(password=password))
-                print('Encryption process is finished.')
-        except BoardError as be:
-            print('Disk encryption returned error.')
-            print(be)
-
-    def finish_provisioning(self):
-        with self.unit_stub(True) as stub:
-            stub.FinishProvisioning(api_iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
-
-    def wait_for_connection(self):
-        try:
-            print('Sleep for 5 seconds...')
-            time.sleep(5)
-            print('Waiting for Unit reboot...')
-            grpc.channel_ready_future(grpc.insecure_channel(self.__unit_address)).result(timeout=300)
-            print('Unit is online')
-        except grpc.FutureTimeoutError:
-            raise BoardError('Board didnt went online')
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+import time
+from contextlib import contextmanager
+
+import grpc
+
+from aos_prov.communication.unit.v0.generated import api_iamanager_iamanager_pb2 as api_iam_manager, \
+    api_iamanager_iamanager_pb2_grpc as api_iam_manager_grpc
+from aos_prov.utils.common import print_message
+from aos_prov.utils.errors import BoardError
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+UNIT_DEFAULT_PORT = 8089
+
+
+class UnitCommunication(object):
+    def __init__(self, address: str = 'localhost:8089'):
+        parts = address.split(':')
+        if len(parts) == 2:
+            try:
+                port = int(parts[1])
+                if not 1 <= port <= 65535:
+                    raise BoardError("Unit port is invalid")
+            except ValueError:
+                raise BoardError("Unit port is invalid")
+        else:
+            address = address + ':' + str(UNIT_DEFAULT_PORT)
+        self.__unit_address = address
+        print_message(f'Will search unit on address: [green]{self.__unit_address}')
+
+    @contextmanager
+    def unit_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = api_iam_manager_grpc.IAManagerStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+        except grpc.RpcError as e:
+            if catch_inactive and \
+                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
+                return
+            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
+                return
+
+            raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    def get_protocol_version(self) -> int:
+        return 1
+
+    def get_system_info(self) -> (str, str):
+        with self.unit_stub() as stub:
+            print('Getting System Info...')
+            response = stub.GetSystemInfo(api_iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
+            print('System ID: ' + response.system_id)
+            print('Model name: ' + response.board_model)
+            return response.system_id, response.board_model
+
+    def clear(self, certificate_type: str) -> None:
+        with self.unit_stub() as stub:
+            print('Clear certificate: ' + certificate_type)
+            response = stub.Clear(api_iam_manager.ClearReq(type=certificate_type))
+            return response
+
+    def set_cert_owner(self, certificate_type: str, password: str) -> None:
+        with self.unit_stub() as stub:
+            print('Set owner: ' + certificate_type)
+            response = stub.SetOwner(api_iam_manager.SetOwnerReq(type=certificate_type, password=password))
+            return response
+
+    def get_cert_types(self) -> [str]:
+        with self.unit_stub() as stub:
+            print('Getting certificate types to renew')
+            response = stub.GetCertTypes(api_iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
+            print('Will be renewed: ' + str(response.types))
+            return response.types
+
+    def create_keys(self, cert_type: str, password: str) -> UnitCertificate:
+        with self.unit_stub() as stub:
+            print('Generating key type:' + cert_type)
+            response = stub.CreateKey(api_iam_manager.CreateKeyReq(type=cert_type, password=password))
+            uc = UnitCertificate()
+            uc.cert_type = response.type
+            uc.csr = response.csr
+            return uc
+
+    def apply_certificate(self, unit_cert: UnitCertificate):
+        with self.unit_stub() as stub:
+            stub.ApplyCert(api_iam_manager.ApplyCertReq(type=unit_cert.cert_type, cert=unit_cert.certificate))
+
+    def set_users(self, users: [str]):
+        with self.unit_stub() as stub:
+            stub.SetUsers(api_iam_manager.SetUsersReq(users=users))
+
+    def encrypt_disk(self, password: str):
+        print('Starting disk encryption...')
+        try:
+            with self.unit_stub(wait_for_close=True) as stub:
+                stub.EncryptDisk(api_iam_manager.EncryptDiskReq(password=password))
+                print('Encryption process is finished.')
+        except BoardError as be:
+            print('Disk encryption returned error.')
+            print(be)
+
+    def finish_provisioning(self):
+        with self.unit_stub(True) as stub:
+            stub.FinishProvisioning(api_iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
+
+    def wait_for_connection(self):
+        try:
+            print('Sleep for 5 seconds...')
+            time.sleep(5)
+            print('Waiting for Unit reboot...')
+            grpc.channel_ready_future(grpc.insecure_channel(self.__unit_address)).result(timeout=300)
+            print('Unit is online')
+        except grpc.FutureTimeoutError:
+            raise BoardError('Board didnt went online')
```

## aos_prov/communication/unit/v0/generated/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py

 * *Ordering differences only*

```diff
@@ -1,799 +1,799 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: api_iamanager_iamanager.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='api_iamanager_iamanager.proto',
-  package='iamanager',
-  syntax='proto3',
-  serialized_options=b'Z2gitpct.epam.com/epmd-aepr/aos_common/api/iamanager',
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1d\x61pi_iamanager_iamanager.proto\x12\tiamanager\x1a\x1bgoogle/protobuf/empty.proto\" \n\x0fGetCertTypesRsp\x12\r\n\x05types\x18\x01 \x03(\t\"\x18\n\x08\x43learReq\x12\x0c\n\x04type\x18\x01 \x01(\t\"-\n\x0bSetOwnerReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x0c\x43reateKeyReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\")\n\x0c\x43reateKeyRsp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\"*\n\x0c\x41pplyCertReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\".\n\x0c\x41pplyCertRsp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\":\n\nGetCertReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"=\n\nGetCertRsp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\":\n\x10GetSystemInfoRsp\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1c\n\x0bSetUsersReq\x12\r\n\x05users\x18\x01 \x03(\t\"\x1c\n\x0bGetUsersRsp\x12\r\n\x05users\x18\x01 \x03(\t\" \n\x0fUsersChangedNtf\x12\r\n\x05users\x18\x01 \x03(\t\"\"\n\x0e\x45ncryptDiskReq\x12\x10\n\x08password\x18\x01 \x01(\t2\xa5\x06\n\tIAManager\x12\x44\n\x0cGetCertTypes\x12\x16.google.protobuf.Empty\x1a\x1a.iamanager.GetCertTypesRsp\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x36\n\x05\x43lear\x12\x13.iamanager.ClearReq\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\x08SetOwner\x12\x16.iamanager.SetOwnerReq\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\tCreateKey\x12\x17.iamanager.CreateKeyReq\x1a\x17.iamanager.CreateKeyRsp\"\x00\x12?\n\tApplyCert\x12\x17.iamanager.ApplyCertReq\x1a\x17.iamanager.ApplyCertRsp\"\x00\x12\x39\n\x07GetCert\x12\x15.iamanager.GetCertReq\x1a\x15.iamanager.GetCertRsp\"\x00\x12\x46\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x1b.iamanager.GetSystemInfoRsp\"\x00\x12<\n\x08SetUsers\x12\x16.iamanager.SetUsersReq\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\x08GetUsers\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.GetUsersRsp\"\x00\x12O\n\x15SubscribeUsersChanged\x12\x16.google.protobuf.Empty\x1a\x1a.iamanager.UsersChangedNtf\"\x00\x30\x01\x12\x42\n\x0b\x45ncryptDisk\x12\x19.iamanager.EncryptDiskReq\x1a\x16.google.protobuf.Empty\"\x00\x42\x34Z2gitpct.epam.com/epmd-aepr/aos_common/api/iamanagerb\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,])
-
-
-
-
-_GETCERTTYPESRSP = _descriptor.Descriptor(
-  name='GetCertTypesRsp',
-  full_name='iamanager.GetCertTypesRsp',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='types', full_name='iamanager.GetCertTypesRsp.types', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=73,
-  serialized_end=105,
-)
-
-
-_CLEARREQ = _descriptor.Descriptor(
-  name='ClearReq',
-  full_name='iamanager.ClearReq',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.ClearReq.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=107,
-  serialized_end=131,
-)
-
-
-_SETOWNERREQ = _descriptor.Descriptor(
-  name='SetOwnerReq',
-  full_name='iamanager.SetOwnerReq',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.SetOwnerReq.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.SetOwnerReq.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=133,
-  serialized_end=178,
-)
-
-
-_CREATEKEYREQ = _descriptor.Descriptor(
-  name='CreateKeyReq',
-  full_name='iamanager.CreateKeyReq',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.CreateKeyReq.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.CreateKeyReq.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=180,
-  serialized_end=226,
-)
-
-
-_CREATEKEYRSP = _descriptor.Descriptor(
-  name='CreateKeyRsp',
-  full_name='iamanager.CreateKeyRsp',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.CreateKeyRsp.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='csr', full_name='iamanager.CreateKeyRsp.csr', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=228,
-  serialized_end=269,
-)
-
-
-_APPLYCERTREQ = _descriptor.Descriptor(
-  name='ApplyCertReq',
-  full_name='iamanager.ApplyCertReq',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.ApplyCertReq.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert', full_name='iamanager.ApplyCertReq.cert', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=271,
-  serialized_end=313,
-)
-
-
-_APPLYCERTRSP = _descriptor.Descriptor(
-  name='ApplyCertRsp',
-  full_name='iamanager.ApplyCertRsp',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.ApplyCertRsp.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert_url', full_name='iamanager.ApplyCertRsp.cert_url', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=315,
-  serialized_end=361,
-)
-
-
-_GETCERTREQ = _descriptor.Descriptor(
-  name='GetCertReq',
-  full_name='iamanager.GetCertReq',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.GetCertReq.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='issuer', full_name='iamanager.GetCertReq.issuer', index=1,
-      number=2, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='serial', full_name='iamanager.GetCertReq.serial', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=363,
-  serialized_end=421,
-)
-
-
-_GETCERTRSP = _descriptor.Descriptor(
-  name='GetCertRsp',
-  full_name='iamanager.GetCertRsp',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.GetCertRsp.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert_url', full_name='iamanager.GetCertRsp.cert_url', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='key_url', full_name='iamanager.GetCertRsp.key_url', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=423,
-  serialized_end=484,
-)
-
-
-_GETSYSTEMINFORSP = _descriptor.Descriptor(
-  name='GetSystemInfoRsp',
-  full_name='iamanager.GetSystemInfoRsp',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='system_id', full_name='iamanager.GetSystemInfoRsp.system_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='board_model', full_name='iamanager.GetSystemInfoRsp.board_model', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=486,
-  serialized_end=544,
-)
-
-
-_SETUSERSREQ = _descriptor.Descriptor(
-  name='SetUsersReq',
-  full_name='iamanager.SetUsersReq',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='users', full_name='iamanager.SetUsersReq.users', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=546,
-  serialized_end=574,
-)
-
-
-_GETUSERSRSP = _descriptor.Descriptor(
-  name='GetUsersRsp',
-  full_name='iamanager.GetUsersRsp',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='users', full_name='iamanager.GetUsersRsp.users', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=576,
-  serialized_end=604,
-)
-
-
-_USERSCHANGEDNTF = _descriptor.Descriptor(
-  name='UsersChangedNtf',
-  full_name='iamanager.UsersChangedNtf',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='users', full_name='iamanager.UsersChangedNtf.users', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=606,
-  serialized_end=638,
-)
-
-
-_ENCRYPTDISKREQ = _descriptor.Descriptor(
-  name='EncryptDiskReq',
-  full_name='iamanager.EncryptDiskReq',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.EncryptDiskReq.password', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=640,
-  serialized_end=674,
-)
-
-DESCRIPTOR.message_types_by_name['GetCertTypesRsp'] = _GETCERTTYPESRSP
-DESCRIPTOR.message_types_by_name['ClearReq'] = _CLEARREQ
-DESCRIPTOR.message_types_by_name['SetOwnerReq'] = _SETOWNERREQ
-DESCRIPTOR.message_types_by_name['CreateKeyReq'] = _CREATEKEYREQ
-DESCRIPTOR.message_types_by_name['CreateKeyRsp'] = _CREATEKEYRSP
-DESCRIPTOR.message_types_by_name['ApplyCertReq'] = _APPLYCERTREQ
-DESCRIPTOR.message_types_by_name['ApplyCertRsp'] = _APPLYCERTRSP
-DESCRIPTOR.message_types_by_name['GetCertReq'] = _GETCERTREQ
-DESCRIPTOR.message_types_by_name['GetCertRsp'] = _GETCERTRSP
-DESCRIPTOR.message_types_by_name['GetSystemInfoRsp'] = _GETSYSTEMINFORSP
-DESCRIPTOR.message_types_by_name['SetUsersReq'] = _SETUSERSREQ
-DESCRIPTOR.message_types_by_name['GetUsersRsp'] = _GETUSERSRSP
-DESCRIPTOR.message_types_by_name['UsersChangedNtf'] = _USERSCHANGEDNTF
-DESCRIPTOR.message_types_by_name['EncryptDiskReq'] = _ENCRYPTDISKREQ
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-GetCertTypesRsp = _reflection.GeneratedProtocolMessageType('GetCertTypesRsp', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTTYPESRSP,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.GetCertTypesRsp)
-  })
-_sym_db.RegisterMessage(GetCertTypesRsp)
-
-ClearReq = _reflection.GeneratedProtocolMessageType('ClearReq', (_message.Message,), {
-  'DESCRIPTOR' : _CLEARREQ,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.ClearReq)
-  })
-_sym_db.RegisterMessage(ClearReq)
-
-SetOwnerReq = _reflection.GeneratedProtocolMessageType('SetOwnerReq', (_message.Message,), {
-  'DESCRIPTOR' : _SETOWNERREQ,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.SetOwnerReq)
-  })
-_sym_db.RegisterMessage(SetOwnerReq)
-
-CreateKeyReq = _reflection.GeneratedProtocolMessageType('CreateKeyReq', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYREQ,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.CreateKeyReq)
-  })
-_sym_db.RegisterMessage(CreateKeyReq)
-
-CreateKeyRsp = _reflection.GeneratedProtocolMessageType('CreateKeyRsp', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYRSP,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.CreateKeyRsp)
-  })
-_sym_db.RegisterMessage(CreateKeyRsp)
-
-ApplyCertReq = _reflection.GeneratedProtocolMessageType('ApplyCertReq', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTREQ,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.ApplyCertReq)
-  })
-_sym_db.RegisterMessage(ApplyCertReq)
-
-ApplyCertRsp = _reflection.GeneratedProtocolMessageType('ApplyCertRsp', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTRSP,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.ApplyCertRsp)
-  })
-_sym_db.RegisterMessage(ApplyCertRsp)
-
-GetCertReq = _reflection.GeneratedProtocolMessageType('GetCertReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTREQ,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.GetCertReq)
-  })
-_sym_db.RegisterMessage(GetCertReq)
-
-GetCertRsp = _reflection.GeneratedProtocolMessageType('GetCertRsp', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTRSP,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.GetCertRsp)
-  })
-_sym_db.RegisterMessage(GetCertRsp)
-
-GetSystemInfoRsp = _reflection.GeneratedProtocolMessageType('GetSystemInfoRsp', (_message.Message,), {
-  'DESCRIPTOR' : _GETSYSTEMINFORSP,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.GetSystemInfoRsp)
-  })
-_sym_db.RegisterMessage(GetSystemInfoRsp)
-
-SetUsersReq = _reflection.GeneratedProtocolMessageType('SetUsersReq', (_message.Message,), {
-  'DESCRIPTOR' : _SETUSERSREQ,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.SetUsersReq)
-  })
-_sym_db.RegisterMessage(SetUsersReq)
-
-GetUsersRsp = _reflection.GeneratedProtocolMessageType('GetUsersRsp', (_message.Message,), {
-  'DESCRIPTOR' : _GETUSERSRSP,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.GetUsersRsp)
-  })
-_sym_db.RegisterMessage(GetUsersRsp)
-
-UsersChangedNtf = _reflection.GeneratedProtocolMessageType('UsersChangedNtf', (_message.Message,), {
-  'DESCRIPTOR' : _USERSCHANGEDNTF,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.UsersChangedNtf)
-  })
-_sym_db.RegisterMessage(UsersChangedNtf)
-
-EncryptDiskReq = _reflection.GeneratedProtocolMessageType('EncryptDiskReq', (_message.Message,), {
-  'DESCRIPTOR' : _ENCRYPTDISKREQ,
-  '__module__' : 'api_iamanager_iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.EncryptDiskReq)
-  })
-_sym_db.RegisterMessage(EncryptDiskReq)
-
-
-DESCRIPTOR._options = None
-
-_IAMANAGER = _descriptor.ServiceDescriptor(
-  name='IAManager',
-  full_name='iamanager.IAManager',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=677,
-  serialized_end=1482,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='GetCertTypes',
-    full_name='iamanager.IAManager.GetCertTypes',
-    index=0,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_GETCERTTYPESRSP,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='FinishProvisioning',
-    full_name='iamanager.IAManager.FinishProvisioning',
-    index=1,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='Clear',
-    full_name='iamanager.IAManager.Clear',
-    index=2,
-    containing_service=None,
-    input_type=_CLEARREQ,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SetOwner',
-    full_name='iamanager.IAManager.SetOwner',
-    index=3,
-    containing_service=None,
-    input_type=_SETOWNERREQ,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='CreateKey',
-    full_name='iamanager.IAManager.CreateKey',
-    index=4,
-    containing_service=None,
-    input_type=_CREATEKEYREQ,
-    output_type=_CREATEKEYRSP,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='ApplyCert',
-    full_name='iamanager.IAManager.ApplyCert',
-    index=5,
-    containing_service=None,
-    input_type=_APPLYCERTREQ,
-    output_type=_APPLYCERTRSP,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetCert',
-    full_name='iamanager.IAManager.GetCert',
-    index=6,
-    containing_service=None,
-    input_type=_GETCERTREQ,
-    output_type=_GETCERTRSP,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetSystemInfo',
-    full_name='iamanager.IAManager.GetSystemInfo',
-    index=7,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_GETSYSTEMINFORSP,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SetUsers',
-    full_name='iamanager.IAManager.SetUsers',
-    index=8,
-    containing_service=None,
-    input_type=_SETUSERSREQ,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetUsers',
-    full_name='iamanager.IAManager.GetUsers',
-    index=9,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_GETUSERSRSP,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SubscribeUsersChanged',
-    full_name='iamanager.IAManager.SubscribeUsersChanged',
-    index=10,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_USERSCHANGEDNTF,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='EncryptDisk',
-    full_name='iamanager.IAManager.EncryptDisk',
-    index=11,
-    containing_service=None,
-    input_type=_ENCRYPTDISKREQ,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_IAMANAGER)
-
-DESCRIPTOR.services_by_name['IAManager'] = _IAMANAGER
-
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: api_iamanager_iamanager.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='api_iamanager_iamanager.proto',
+  package='iamanager',
+  syntax='proto3',
+  serialized_options=b'Z2gitpct.epam.com/epmd-aepr/aos_common/api/iamanager',
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n\x1d\x61pi_iamanager_iamanager.proto\x12\tiamanager\x1a\x1bgoogle/protobuf/empty.proto\" \n\x0fGetCertTypesRsp\x12\r\n\x05types\x18\x01 \x03(\t\"\x18\n\x08\x43learReq\x12\x0c\n\x04type\x18\x01 \x01(\t\"-\n\x0bSetOwnerReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x0c\x43reateKeyReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\")\n\x0c\x43reateKeyRsp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\"*\n\x0c\x41pplyCertReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\".\n\x0c\x41pplyCertRsp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\":\n\nGetCertReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"=\n\nGetCertRsp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\":\n\x10GetSystemInfoRsp\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1c\n\x0bSetUsersReq\x12\r\n\x05users\x18\x01 \x03(\t\"\x1c\n\x0bGetUsersRsp\x12\r\n\x05users\x18\x01 \x03(\t\" \n\x0fUsersChangedNtf\x12\r\n\x05users\x18\x01 \x03(\t\"\"\n\x0e\x45ncryptDiskReq\x12\x10\n\x08password\x18\x01 \x01(\t2\xa5\x06\n\tIAManager\x12\x44\n\x0cGetCertTypes\x12\x16.google.protobuf.Empty\x1a\x1a.iamanager.GetCertTypesRsp\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x36\n\x05\x43lear\x12\x13.iamanager.ClearReq\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\x08SetOwner\x12\x16.iamanager.SetOwnerReq\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\tCreateKey\x12\x17.iamanager.CreateKeyReq\x1a\x17.iamanager.CreateKeyRsp\"\x00\x12?\n\tApplyCert\x12\x17.iamanager.ApplyCertReq\x1a\x17.iamanager.ApplyCertRsp\"\x00\x12\x39\n\x07GetCert\x12\x15.iamanager.GetCertReq\x1a\x15.iamanager.GetCertRsp\"\x00\x12\x46\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x1b.iamanager.GetSystemInfoRsp\"\x00\x12<\n\x08SetUsers\x12\x16.iamanager.SetUsersReq\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\x08GetUsers\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.GetUsersRsp\"\x00\x12O\n\x15SubscribeUsersChanged\x12\x16.google.protobuf.Empty\x1a\x1a.iamanager.UsersChangedNtf\"\x00\x30\x01\x12\x42\n\x0b\x45ncryptDisk\x12\x19.iamanager.EncryptDiskReq\x1a\x16.google.protobuf.Empty\"\x00\x42\x34Z2gitpct.epam.com/epmd-aepr/aos_common/api/iamanagerb\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,])
+
+
+
+
+_GETCERTTYPESRSP = _descriptor.Descriptor(
+  name='GetCertTypesRsp',
+  full_name='iamanager.GetCertTypesRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='types', full_name='iamanager.GetCertTypesRsp.types', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=73,
+  serialized_end=105,
+)
+
+
+_CLEARREQ = _descriptor.Descriptor(
+  name='ClearReq',
+  full_name='iamanager.ClearReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.ClearReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=107,
+  serialized_end=131,
+)
+
+
+_SETOWNERREQ = _descriptor.Descriptor(
+  name='SetOwnerReq',
+  full_name='iamanager.SetOwnerReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.SetOwnerReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.SetOwnerReq.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=133,
+  serialized_end=178,
+)
+
+
+_CREATEKEYREQ = _descriptor.Descriptor(
+  name='CreateKeyReq',
+  full_name='iamanager.CreateKeyReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.CreateKeyReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.CreateKeyReq.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=180,
+  serialized_end=226,
+)
+
+
+_CREATEKEYRSP = _descriptor.Descriptor(
+  name='CreateKeyRsp',
+  full_name='iamanager.CreateKeyRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.CreateKeyRsp.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='csr', full_name='iamanager.CreateKeyRsp.csr', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=228,
+  serialized_end=269,
+)
+
+
+_APPLYCERTREQ = _descriptor.Descriptor(
+  name='ApplyCertReq',
+  full_name='iamanager.ApplyCertReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.ApplyCertReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert', full_name='iamanager.ApplyCertReq.cert', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=271,
+  serialized_end=313,
+)
+
+
+_APPLYCERTRSP = _descriptor.Descriptor(
+  name='ApplyCertRsp',
+  full_name='iamanager.ApplyCertRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.ApplyCertRsp.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.ApplyCertRsp.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=315,
+  serialized_end=361,
+)
+
+
+_GETCERTREQ = _descriptor.Descriptor(
+  name='GetCertReq',
+  full_name='iamanager.GetCertReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.GetCertReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='issuer', full_name='iamanager.GetCertReq.issuer', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='serial', full_name='iamanager.GetCertReq.serial', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=363,
+  serialized_end=421,
+)
+
+
+_GETCERTRSP = _descriptor.Descriptor(
+  name='GetCertRsp',
+  full_name='iamanager.GetCertRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.GetCertRsp.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.GetCertRsp.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='key_url', full_name='iamanager.GetCertRsp.key_url', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=423,
+  serialized_end=484,
+)
+
+
+_GETSYSTEMINFORSP = _descriptor.Descriptor(
+  name='GetSystemInfoRsp',
+  full_name='iamanager.GetSystemInfoRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='system_id', full_name='iamanager.GetSystemInfoRsp.system_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='board_model', full_name='iamanager.GetSystemInfoRsp.board_model', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=486,
+  serialized_end=544,
+)
+
+
+_SETUSERSREQ = _descriptor.Descriptor(
+  name='SetUsersReq',
+  full_name='iamanager.SetUsersReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='users', full_name='iamanager.SetUsersReq.users', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=546,
+  serialized_end=574,
+)
+
+
+_GETUSERSRSP = _descriptor.Descriptor(
+  name='GetUsersRsp',
+  full_name='iamanager.GetUsersRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='users', full_name='iamanager.GetUsersRsp.users', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=576,
+  serialized_end=604,
+)
+
+
+_USERSCHANGEDNTF = _descriptor.Descriptor(
+  name='UsersChangedNtf',
+  full_name='iamanager.UsersChangedNtf',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='users', full_name='iamanager.UsersChangedNtf.users', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=606,
+  serialized_end=638,
+)
+
+
+_ENCRYPTDISKREQ = _descriptor.Descriptor(
+  name='EncryptDiskReq',
+  full_name='iamanager.EncryptDiskReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.EncryptDiskReq.password', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=640,
+  serialized_end=674,
+)
+
+DESCRIPTOR.message_types_by_name['GetCertTypesRsp'] = _GETCERTTYPESRSP
+DESCRIPTOR.message_types_by_name['ClearReq'] = _CLEARREQ
+DESCRIPTOR.message_types_by_name['SetOwnerReq'] = _SETOWNERREQ
+DESCRIPTOR.message_types_by_name['CreateKeyReq'] = _CREATEKEYREQ
+DESCRIPTOR.message_types_by_name['CreateKeyRsp'] = _CREATEKEYRSP
+DESCRIPTOR.message_types_by_name['ApplyCertReq'] = _APPLYCERTREQ
+DESCRIPTOR.message_types_by_name['ApplyCertRsp'] = _APPLYCERTRSP
+DESCRIPTOR.message_types_by_name['GetCertReq'] = _GETCERTREQ
+DESCRIPTOR.message_types_by_name['GetCertRsp'] = _GETCERTRSP
+DESCRIPTOR.message_types_by_name['GetSystemInfoRsp'] = _GETSYSTEMINFORSP
+DESCRIPTOR.message_types_by_name['SetUsersReq'] = _SETUSERSREQ
+DESCRIPTOR.message_types_by_name['GetUsersRsp'] = _GETUSERSRSP
+DESCRIPTOR.message_types_by_name['UsersChangedNtf'] = _USERSCHANGEDNTF
+DESCRIPTOR.message_types_by_name['EncryptDiskReq'] = _ENCRYPTDISKREQ
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+GetCertTypesRsp = _reflection.GeneratedProtocolMessageType('GetCertTypesRsp', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTTYPESRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetCertTypesRsp)
+  })
+_sym_db.RegisterMessage(GetCertTypesRsp)
+
+ClearReq = _reflection.GeneratedProtocolMessageType('ClearReq', (_message.Message,), {
+  'DESCRIPTOR' : _CLEARREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.ClearReq)
+  })
+_sym_db.RegisterMessage(ClearReq)
+
+SetOwnerReq = _reflection.GeneratedProtocolMessageType('SetOwnerReq', (_message.Message,), {
+  'DESCRIPTOR' : _SETOWNERREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.SetOwnerReq)
+  })
+_sym_db.RegisterMessage(SetOwnerReq)
+
+CreateKeyReq = _reflection.GeneratedProtocolMessageType('CreateKeyReq', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.CreateKeyReq)
+  })
+_sym_db.RegisterMessage(CreateKeyReq)
+
+CreateKeyRsp = _reflection.GeneratedProtocolMessageType('CreateKeyRsp', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.CreateKeyRsp)
+  })
+_sym_db.RegisterMessage(CreateKeyRsp)
+
+ApplyCertReq = _reflection.GeneratedProtocolMessageType('ApplyCertReq', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.ApplyCertReq)
+  })
+_sym_db.RegisterMessage(ApplyCertReq)
+
+ApplyCertRsp = _reflection.GeneratedProtocolMessageType('ApplyCertRsp', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.ApplyCertRsp)
+  })
+_sym_db.RegisterMessage(ApplyCertRsp)
+
+GetCertReq = _reflection.GeneratedProtocolMessageType('GetCertReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetCertReq)
+  })
+_sym_db.RegisterMessage(GetCertReq)
+
+GetCertRsp = _reflection.GeneratedProtocolMessageType('GetCertRsp', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetCertRsp)
+  })
+_sym_db.RegisterMessage(GetCertRsp)
+
+GetSystemInfoRsp = _reflection.GeneratedProtocolMessageType('GetSystemInfoRsp', (_message.Message,), {
+  'DESCRIPTOR' : _GETSYSTEMINFORSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetSystemInfoRsp)
+  })
+_sym_db.RegisterMessage(GetSystemInfoRsp)
+
+SetUsersReq = _reflection.GeneratedProtocolMessageType('SetUsersReq', (_message.Message,), {
+  'DESCRIPTOR' : _SETUSERSREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.SetUsersReq)
+  })
+_sym_db.RegisterMessage(SetUsersReq)
+
+GetUsersRsp = _reflection.GeneratedProtocolMessageType('GetUsersRsp', (_message.Message,), {
+  'DESCRIPTOR' : _GETUSERSRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetUsersRsp)
+  })
+_sym_db.RegisterMessage(GetUsersRsp)
+
+UsersChangedNtf = _reflection.GeneratedProtocolMessageType('UsersChangedNtf', (_message.Message,), {
+  'DESCRIPTOR' : _USERSCHANGEDNTF,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.UsersChangedNtf)
+  })
+_sym_db.RegisterMessage(UsersChangedNtf)
+
+EncryptDiskReq = _reflection.GeneratedProtocolMessageType('EncryptDiskReq', (_message.Message,), {
+  'DESCRIPTOR' : _ENCRYPTDISKREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.EncryptDiskReq)
+  })
+_sym_db.RegisterMessage(EncryptDiskReq)
+
+
+DESCRIPTOR._options = None
+
+_IAMANAGER = _descriptor.ServiceDescriptor(
+  name='IAManager',
+  full_name='iamanager.IAManager',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=677,
+  serialized_end=1482,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='GetCertTypes',
+    full_name='iamanager.IAManager.GetCertTypes',
+    index=0,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_GETCERTTYPESRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='FinishProvisioning',
+    full_name='iamanager.IAManager.FinishProvisioning',
+    index=1,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='Clear',
+    full_name='iamanager.IAManager.Clear',
+    index=2,
+    containing_service=None,
+    input_type=_CLEARREQ,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetOwner',
+    full_name='iamanager.IAManager.SetOwner',
+    index=3,
+    containing_service=None,
+    input_type=_SETOWNERREQ,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='CreateKey',
+    full_name='iamanager.IAManager.CreateKey',
+    index=4,
+    containing_service=None,
+    input_type=_CREATEKEYREQ,
+    output_type=_CREATEKEYRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='ApplyCert',
+    full_name='iamanager.IAManager.ApplyCert',
+    index=5,
+    containing_service=None,
+    input_type=_APPLYCERTREQ,
+    output_type=_APPLYCERTRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetCert',
+    full_name='iamanager.IAManager.GetCert',
+    index=6,
+    containing_service=None,
+    input_type=_GETCERTREQ,
+    output_type=_GETCERTRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetSystemInfo',
+    full_name='iamanager.IAManager.GetSystemInfo',
+    index=7,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_GETSYSTEMINFORSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetUsers',
+    full_name='iamanager.IAManager.SetUsers',
+    index=8,
+    containing_service=None,
+    input_type=_SETUSERSREQ,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetUsers',
+    full_name='iamanager.IAManager.GetUsers',
+    index=9,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_GETUSERSRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SubscribeUsersChanged',
+    full_name='iamanager.IAManager.SubscribeUsersChanged',
+    index=10,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_USERSCHANGEDNTF,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='EncryptDisk',
+    full_name='iamanager.IAManager.EncryptDisk',
+    index=11,
+    containing_service=None,
+    input_type=_ENCRYPTDISKREQ,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_IAMANAGER)
+
+DESCRIPTOR.services_by_name['IAManager'] = _IAMANAGER
+
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,430 +1,430 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from aos_prov.communication.unit.v0.generated import api_iamanager_iamanager_pb2 as api__iamanager__iamanager__pb2
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-class IAManagerStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetCertTypes = channel.unary_unary(
-                '/iamanager.IAManager/GetCertTypes',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=api__iamanager__iamanager__pb2.GetCertTypesRsp.FromString,
-                )
-        self.FinishProvisioning = channel.unary_unary(
-                '/iamanager.IAManager/FinishProvisioning',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.Clear = channel.unary_unary(
-                '/iamanager.IAManager/Clear',
-                request_serializer=api__iamanager__iamanager__pb2.ClearReq.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.SetOwner = channel.unary_unary(
-                '/iamanager.IAManager/SetOwner',
-                request_serializer=api__iamanager__iamanager__pb2.SetOwnerReq.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.CreateKey = channel.unary_unary(
-                '/iamanager.IAManager/CreateKey',
-                request_serializer=api__iamanager__iamanager__pb2.CreateKeyReq.SerializeToString,
-                response_deserializer=api__iamanager__iamanager__pb2.CreateKeyRsp.FromString,
-                )
-        self.ApplyCert = channel.unary_unary(
-                '/iamanager.IAManager/ApplyCert',
-                request_serializer=api__iamanager__iamanager__pb2.ApplyCertReq.SerializeToString,
-                response_deserializer=api__iamanager__iamanager__pb2.ApplyCertRsp.FromString,
-                )
-        self.GetCert = channel.unary_unary(
-                '/iamanager.IAManager/GetCert',
-                request_serializer=api__iamanager__iamanager__pb2.GetCertReq.SerializeToString,
-                response_deserializer=api__iamanager__iamanager__pb2.GetCertRsp.FromString,
-                )
-        self.GetSystemInfo = channel.unary_unary(
-                '/iamanager.IAManager/GetSystemInfo',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=api__iamanager__iamanager__pb2.GetSystemInfoRsp.FromString,
-                )
-        self.SetUsers = channel.unary_unary(
-                '/iamanager.IAManager/SetUsers',
-                request_serializer=api__iamanager__iamanager__pb2.SetUsersReq.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.GetUsers = channel.unary_unary(
-                '/iamanager.IAManager/GetUsers',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=api__iamanager__iamanager__pb2.GetUsersRsp.FromString,
-                )
-        self.SubscribeUsersChanged = channel.unary_stream(
-                '/iamanager.IAManager/SubscribeUsersChanged',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=api__iamanager__iamanager__pb2.UsersChangedNtf.FromString,
-                )
-        self.EncryptDisk = channel.unary_unary(
-                '/iamanager.IAManager/EncryptDisk',
-                request_serializer=api__iamanager__iamanager__pb2.EncryptDiskReq.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAManagerServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetCertTypes(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def FinishProvisioning(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Clear(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetOwner(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def CreateKey(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ApplyCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetSystemInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetUsers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetUsers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SubscribeUsersChanged(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def EncryptDisk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAManagerServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCertTypes,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=api__iamanager__iamanager__pb2.GetCertTypesRsp.SerializeToString,
-            ),
-            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
-                    servicer.FinishProvisioning,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'Clear': grpc.unary_unary_rpc_method_handler(
-                    servicer.Clear,
-                    request_deserializer=api__iamanager__iamanager__pb2.ClearReq.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'SetOwner': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetOwner,
-                    request_deserializer=api__iamanager__iamanager__pb2.SetOwnerReq.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'CreateKey': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateKey,
-                    request_deserializer=api__iamanager__iamanager__pb2.CreateKeyReq.FromString,
-                    response_serializer=api__iamanager__iamanager__pb2.CreateKeyRsp.SerializeToString,
-            ),
-            'ApplyCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.ApplyCert,
-                    request_deserializer=api__iamanager__iamanager__pb2.ApplyCertReq.FromString,
-                    response_serializer=api__iamanager__iamanager__pb2.ApplyCertRsp.SerializeToString,
-            ),
-            'GetCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCert,
-                    request_deserializer=api__iamanager__iamanager__pb2.GetCertReq.FromString,
-                    response_serializer=api__iamanager__iamanager__pb2.GetCertRsp.SerializeToString,
-            ),
-            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSystemInfo,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=api__iamanager__iamanager__pb2.GetSystemInfoRsp.SerializeToString,
-            ),
-            'SetUsers': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetUsers,
-                    request_deserializer=api__iamanager__iamanager__pb2.SetUsersReq.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'GetUsers': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetUsers,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=api__iamanager__iamanager__pb2.GetUsersRsp.SerializeToString,
-            ),
-            'SubscribeUsersChanged': grpc.unary_stream_rpc_method_handler(
-                    servicer.SubscribeUsersChanged,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=api__iamanager__iamanager__pb2.UsersChangedNtf.SerializeToString,
-            ),
-            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
-                    servicer.EncryptDisk,
-                    request_deserializer=api__iamanager__iamanager__pb2.EncryptDiskReq.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.IAManager', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAManager(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetCertTypes(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/GetCertTypes',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            api__iamanager__iamanager__pb2.GetCertTypesRsp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def FinishProvisioning(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/FinishProvisioning',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Clear(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/Clear',
-            api__iamanager__iamanager__pb2.ClearReq.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetOwner(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/SetOwner',
-            api__iamanager__iamanager__pb2.SetOwnerReq.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def CreateKey(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/CreateKey',
-            api__iamanager__iamanager__pb2.CreateKeyReq.SerializeToString,
-            api__iamanager__iamanager__pb2.CreateKeyRsp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ApplyCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/ApplyCert',
-            api__iamanager__iamanager__pb2.ApplyCertReq.SerializeToString,
-            api__iamanager__iamanager__pb2.ApplyCertRsp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/GetCert',
-            api__iamanager__iamanager__pb2.GetCertReq.SerializeToString,
-            api__iamanager__iamanager__pb2.GetCertRsp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetSystemInfo(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/GetSystemInfo',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            api__iamanager__iamanager__pb2.GetSystemInfoRsp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetUsers(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/SetUsers',
-            api__iamanager__iamanager__pb2.SetUsersReq.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetUsers(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/GetUsers',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            api__iamanager__iamanager__pb2.GetUsersRsp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SubscribeUsersChanged(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iamanager.IAManager/SubscribeUsersChanged',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            api__iamanager__iamanager__pb2.UsersChangedNtf.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def EncryptDisk(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/EncryptDisk',
-            api__iamanager__iamanager__pb2.EncryptDiskReq.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from aos_prov.communication.unit.v0.generated import api_iamanager_iamanager_pb2 as api__iamanager__iamanager__pb2
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+class IAManagerStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetCertTypes = channel.unary_unary(
+                '/iamanager.IAManager/GetCertTypes',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=api__iamanager__iamanager__pb2.GetCertTypesRsp.FromString,
+                )
+        self.FinishProvisioning = channel.unary_unary(
+                '/iamanager.IAManager/FinishProvisioning',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.Clear = channel.unary_unary(
+                '/iamanager.IAManager/Clear',
+                request_serializer=api__iamanager__iamanager__pb2.ClearReq.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.SetOwner = channel.unary_unary(
+                '/iamanager.IAManager/SetOwner',
+                request_serializer=api__iamanager__iamanager__pb2.SetOwnerReq.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.CreateKey = channel.unary_unary(
+                '/iamanager.IAManager/CreateKey',
+                request_serializer=api__iamanager__iamanager__pb2.CreateKeyReq.SerializeToString,
+                response_deserializer=api__iamanager__iamanager__pb2.CreateKeyRsp.FromString,
+                )
+        self.ApplyCert = channel.unary_unary(
+                '/iamanager.IAManager/ApplyCert',
+                request_serializer=api__iamanager__iamanager__pb2.ApplyCertReq.SerializeToString,
+                response_deserializer=api__iamanager__iamanager__pb2.ApplyCertRsp.FromString,
+                )
+        self.GetCert = channel.unary_unary(
+                '/iamanager.IAManager/GetCert',
+                request_serializer=api__iamanager__iamanager__pb2.GetCertReq.SerializeToString,
+                response_deserializer=api__iamanager__iamanager__pb2.GetCertRsp.FromString,
+                )
+        self.GetSystemInfo = channel.unary_unary(
+                '/iamanager.IAManager/GetSystemInfo',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=api__iamanager__iamanager__pb2.GetSystemInfoRsp.FromString,
+                )
+        self.SetUsers = channel.unary_unary(
+                '/iamanager.IAManager/SetUsers',
+                request_serializer=api__iamanager__iamanager__pb2.SetUsersReq.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.GetUsers = channel.unary_unary(
+                '/iamanager.IAManager/GetUsers',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=api__iamanager__iamanager__pb2.GetUsersRsp.FromString,
+                )
+        self.SubscribeUsersChanged = channel.unary_stream(
+                '/iamanager.IAManager/SubscribeUsersChanged',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=api__iamanager__iamanager__pb2.UsersChangedNtf.FromString,
+                )
+        self.EncryptDisk = channel.unary_unary(
+                '/iamanager.IAManager/EncryptDisk',
+                request_serializer=api__iamanager__iamanager__pb2.EncryptDiskReq.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAManagerServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetCertTypes(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def FinishProvisioning(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Clear(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetOwner(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def CreateKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ApplyCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetSystemInfo(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetUsers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetUsers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubscribeUsersChanged(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def EncryptDisk(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAManagerServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCertTypes,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=api__iamanager__iamanager__pb2.GetCertTypesRsp.SerializeToString,
+            ),
+            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
+                    servicer.FinishProvisioning,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'Clear': grpc.unary_unary_rpc_method_handler(
+                    servicer.Clear,
+                    request_deserializer=api__iamanager__iamanager__pb2.ClearReq.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'SetOwner': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetOwner,
+                    request_deserializer=api__iamanager__iamanager__pb2.SetOwnerReq.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'CreateKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateKey,
+                    request_deserializer=api__iamanager__iamanager__pb2.CreateKeyReq.FromString,
+                    response_serializer=api__iamanager__iamanager__pb2.CreateKeyRsp.SerializeToString,
+            ),
+            'ApplyCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.ApplyCert,
+                    request_deserializer=api__iamanager__iamanager__pb2.ApplyCertReq.FromString,
+                    response_serializer=api__iamanager__iamanager__pb2.ApplyCertRsp.SerializeToString,
+            ),
+            'GetCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCert,
+                    request_deserializer=api__iamanager__iamanager__pb2.GetCertReq.FromString,
+                    response_serializer=api__iamanager__iamanager__pb2.GetCertRsp.SerializeToString,
+            ),
+            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSystemInfo,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=api__iamanager__iamanager__pb2.GetSystemInfoRsp.SerializeToString,
+            ),
+            'SetUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetUsers,
+                    request_deserializer=api__iamanager__iamanager__pb2.SetUsersReq.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'GetUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetUsers,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=api__iamanager__iamanager__pb2.GetUsersRsp.SerializeToString,
+            ),
+            'SubscribeUsersChanged': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeUsersChanged,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=api__iamanager__iamanager__pb2.UsersChangedNtf.SerializeToString,
+            ),
+            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
+                    servicer.EncryptDisk,
+                    request_deserializer=api__iamanager__iamanager__pb2.EncryptDiskReq.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.IAManager', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAManager(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetCertTypes(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/GetCertTypes',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            api__iamanager__iamanager__pb2.GetCertTypesRsp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def FinishProvisioning(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/FinishProvisioning',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Clear(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/Clear',
+            api__iamanager__iamanager__pb2.ClearReq.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetOwner(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/SetOwner',
+            api__iamanager__iamanager__pb2.SetOwnerReq.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/CreateKey',
+            api__iamanager__iamanager__pb2.CreateKeyReq.SerializeToString,
+            api__iamanager__iamanager__pb2.CreateKeyRsp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ApplyCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/ApplyCert',
+            api__iamanager__iamanager__pb2.ApplyCertReq.SerializeToString,
+            api__iamanager__iamanager__pb2.ApplyCertRsp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/GetCert',
+            api__iamanager__iamanager__pb2.GetCertReq.SerializeToString,
+            api__iamanager__iamanager__pb2.GetCertRsp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetSystemInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/GetSystemInfo',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            api__iamanager__iamanager__pb2.GetSystemInfoRsp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/SetUsers',
+            api__iamanager__iamanager__pb2.SetUsersReq.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/GetUsers',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            api__iamanager__iamanager__pb2.GetUsersRsp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubscribeUsersChanged(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/iamanager.IAManager/SubscribeUsersChanged',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            api__iamanager__iamanager__pb2.UsersChangedNtf.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def EncryptDisk(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.IAManager/EncryptDisk',
+            api__iamanager__iamanager__pb2.EncryptDiskReq.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/communication/unit/v1/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v1/unit_communication_v1.py

```diff
@@ -1,155 +1,146 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
-import time
-from contextlib import contextmanager
-
-import grpc
-from colorama import Fore, Style
-
-from aos_prov.communication.unit.v1.generated import iamanagerprotected_pb2 as iam_manager
-from aos_prov.communication.unit.v1.generated import iamanagerprotected_pb2_grpc as api_iam_manager_grpc
-
-from aos_prov.communication.unit.v1.generated import iamanagerpublic_pb2 as iam_manager_public
-from aos_prov.communication.unit.v1.generated import iamanagerpublic_pb2_grpc as iam_manager_public_grpc
-
-from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iam_manager_common
-
-from aos_prov.utils.errors import BoardError, GrpcUnimplemented
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-UNIT_DEFAULT_PORT = 8089
-
-
-class UnitCommunicationV1(object):
-    def __init__(self, address: str = 'localhost:8089'):
-        if address is None:
-            address = 'localhost:8089'
-        parts = address.split(':')
-        if len(parts) == 2:
-            try:
-                port = int(parts[1])
-                if not 1 <= port <= 65535:
-                    raise BoardError("Unit port is invalid")
-            except ValueError:
-                raise BoardError("Unit port is invalid")
-        else:
-            address = address + ':' + str(UNIT_DEFAULT_PORT)
-        self.__unit_address = address
-        print(f"Will search unit on address: {Fore.GREEN}{self.__unit_address}{Style.RESET_ALL}")
-
-    @contextmanager
-    def unit_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = api_iam_manager_grpc.IAMProtectedServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):
-                        print(str(state))
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as e:
-            if catch_inactive and \
-                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
-                return
-            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
-                return
-            error_text = (f"{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}"
-                          f"{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}")
-            raise BoardError(error_text)
-
-    @contextmanager
-    def unit_public_stub(self):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_public_grpc.IAMPublicServiceStub(channel)
-                yield stub
-
-        except grpc.RpcError as e:
-            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
-                error_text = (f"{Fore.YELLOW}FAILED! Protocol V1 is not supported: {Style.RESET_ALL}"
-                              f"{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}")
-                raise GrpcUnimplemented(error_text)
-            else:
-                error_text = (f"{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}"
-                              f"{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}")
-                raise BoardError(error_text)
-
-    def get_protocol_version(self) -> int:
-        return 2
-
-    def get_system_info(self) -> (str, str):
-        with self.unit_public_stub() as stub:
-            print('Getting System Info...')
-            response = stub.GetSystemInfo(iam_manager_public.google_dot_protobuf_dot_empty__pb2.Empty())
-            print('System ID: ' + response.system_id)
-            print('Model name: ' + response.board_model)
-            return response.system_id, response.board_model
-
-    def clear(self, certificate_type: str) -> None:
-        with self.unit_stub() as stub:
-            print('Clear certificate: ' + certificate_type)
-            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type))
-            return response
-
-    def set_cert_owner(self, certificate_type: str, password: str) -> None:
-        with self.unit_stub() as stub:
-            print('Set owner: ' + certificate_type)
-            response = stub.SetOwner(iam_manager.SetOwnerRequest(type=certificate_type, password=password))
-            return response
-
-    def get_cert_types(self) -> [str]:
-        with self.unit_stub() as stub:
-            print('Getting certificate types to renew')
-            response = stub.GetCertTypes(iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
-            print('Will be renewed: ' + str(response.types))
-            return response.types
-
-    def create_keys(self, cert_type: str, password: str) -> UnitCertificate:
-        with self.unit_stub() as stub:
-            print('Generating key type:' + cert_type)
-            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password))
-            uc = UnitCertificate()
-            uc.cert_type = response.type
-            uc.csr = response.csr
-            return uc
-
-    def apply_certificate(self, unit_cert: UnitCertificate):
-        with self.unit_stub() as stub:
-            print('Applying type:' + unit_cert.cert_type)
-            stub.ApplyCert(iam_manager.ApplyCertRequest(type=unit_cert.cert_type, cert=unit_cert.certificate))
-
-    def set_users(self, users: [str]):
-        with self.unit_stub() as stub:
-            print('setting users')
-            stub.SetUsers(iam_manager_common.Users(users=users))
-
-    def encrypt_disk(self, password: str):
-        print('Starting disk encryption...')
-        try:
-            with self.unit_stub(wait_for_close=True) as stub:
-                stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password))
-                print('Encryption process is finished.')
-        except BoardError as be:
-            print('Disk encryption returned error.')
-            print(be)
-
-    def finish_provisioning(self):
-        with self.unit_stub(True) as stub:
-            print('Finishing provisioning')
-            stub.FinishProvisioning(iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
-
-    def wait_for_connection(self):
-        try:
-            print('Sleep for 5 seconds...')
-            time.sleep(5)
-            print('Waiting for Unit reboot...')
-            grpc.channel_ready_future(grpc.insecure_channel(self.__unit_address)).result(timeout=300)
-            print('Unit is online')
-        except grpc.FutureTimeoutError:
-            raise BoardError('Board didnt went online')
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+import time
+from contextlib import contextmanager
+
+import grpc
+
+from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iam_manager_common
+from aos_prov.communication.unit.v1.generated import iamanagerprotected_pb2 as iam_manager
+from aos_prov.communication.unit.v1.generated import iamanagerprotected_pb2_grpc as api_iam_manager_grpc
+from aos_prov.communication.unit.v1.generated import iamanagerpublic_pb2 as iam_manager_public
+from aos_prov.communication.unit.v1.generated import iamanagerpublic_pb2_grpc as iam_manager_public_grpc
+from aos_prov.utils.common import print_message
+from aos_prov.utils.errors import BoardError, GrpcUnimplemented
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+UNIT_DEFAULT_PORT = 8089
+
+
+class UnitCommunicationV1(object):
+    def __init__(self, address: str = 'localhost:8089'):
+        if address is None:
+            address = 'localhost:8089'
+        parts = address.split(':')
+        if len(parts) == 2:
+            try:
+                port = int(parts[1])
+                if not 1 <= port <= 65535:
+                    raise BoardError("Unit port is invalid")
+            except ValueError:
+                raise BoardError("Unit port is invalid")
+        else:
+            address = address + ':' + str(UNIT_DEFAULT_PORT)
+        self.__unit_address = address
+        print_message(f'Will search unit on address: [green]{self.__unit_address}')
+
+    @contextmanager
+    def unit_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = api_iam_manager_grpc.IAMProtectedServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):
+                        print(str(state))
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as e:
+            if catch_inactive and \
+                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
+                return
+            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
+                return
+            raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_public_stub(self):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_public_grpc.IAMPublicServiceStub(channel)
+                yield stub
+
+        except grpc.RpcError as e:
+            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
+                raise GrpcUnimplemented(f'Protocol V1 is not supported: \n{e.code()}: {e.details()}')
+            else:
+                raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    def get_protocol_version(self) -> int:
+        return 2
+
+    def get_system_info(self) -> (str, str):
+        with self.unit_public_stub() as stub:
+            print('Getting System Info...')
+            response = stub.GetSystemInfo(iam_manager_public.google_dot_protobuf_dot_empty__pb2.Empty())
+            print('System ID: ' + response.system_id)
+            print('Model name: ' + response.board_model)
+            return response.system_id, response.board_model
+
+    def clear(self, certificate_type: str) -> None:
+        with self.unit_stub() as stub:
+            print('Clear certificate: ' + certificate_type)
+            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type))
+            return response
+
+    def set_cert_owner(self, certificate_type: str, password: str) -> None:
+        with self.unit_stub() as stub:
+            print('Set owner: ' + certificate_type)
+            response = stub.SetOwner(iam_manager.SetOwnerRequest(type=certificate_type, password=password))
+            return response
+
+    def get_cert_types(self) -> [str]:
+        with self.unit_stub() as stub:
+            print('Getting certificate types to renew')
+            response = stub.GetCertTypes(iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
+            print('Will be renewed: ' + str(response.types))
+            return response.types
+
+    def create_keys(self, cert_type: str, password: str) -> UnitCertificate:
+        with self.unit_stub() as stub:
+            print('Generating key type:' + cert_type)
+            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password))
+            uc = UnitCertificate()
+            uc.cert_type = response.type
+            uc.csr = response.csr
+            return uc
+
+    def apply_certificate(self, unit_cert: UnitCertificate):
+        with self.unit_stub() as stub:
+            print('Applying type:' + unit_cert.cert_type)
+            stub.ApplyCert(iam_manager.ApplyCertRequest(type=unit_cert.cert_type, cert=unit_cert.certificate))
+
+    def set_users(self, users: [str]):
+        with self.unit_stub() as stub:
+            print('setting users')
+            stub.SetUsers(iam_manager_common.Users(users=users))
+
+    def encrypt_disk(self, password: str):
+        print('Starting disk encryption...')
+        try:
+            with self.unit_stub(wait_for_close=True) as stub:
+                stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password))
+                print('Encryption process is finished.')
+        except BoardError as be:
+            print('Disk encryption returned error.')
+            print(be)
+
+    def finish_provisioning(self):
+        with self.unit_stub(True) as stub:
+            print('Finishing provisioning')
+            stub.FinishProvisioning(iam_manager.google_dot_protobuf_dot_empty__pb2.Empty())
+
+    def wait_for_connection(self):
+        try:
+            print('Sleep for 5 seconds...')
+            time.sleep(5)
+            print('Waiting for Unit reboot...')
+            grpc.channel_ready_future(grpc.insecure_channel(self.__unit_address)).result(timeout=300)
+            print('Unit is online')
+        except grpc.FutureTimeoutError:
+            raise BoardError('Board didnt went online')
```

## aos_prov/communication/unit/v1/generated/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py

 * *Ordering differences only*

```diff
@@ -1,159 +1,159 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v1/iamanagercommon.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v1/iamanagercommon.proto',
-  package='iamanager.v1',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\"iamanager/v1/iamanagercommon.proto\x12\x0ciamanager.v1\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v1.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x05Users\x12\r\n\x05users\x18\x01 \x03(\tb\x06proto3'
-)
-
-
-
-
-_PERMISSIONS_PERMISSIONSENTRY = _descriptor.Descriptor(
-  name='PermissionsEntry',
-  full_name='iamanager.v1.Permissions.PermissionsEntry',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='key', full_name='iamanager.v1.Permissions.PermissionsEntry.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='iamanager.v1.Permissions.PermissionsEntry.value', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'8\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=133,
-  serialized_end=183,
-)
-
-_PERMISSIONS = _descriptor.Descriptor(
-  name='Permissions',
-  full_name='iamanager.v1.Permissions',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v1.Permissions.permissions', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_PERMISSIONS_PERMISSIONSENTRY, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=53,
-  serialized_end=183,
-)
-
-
-_USERS = _descriptor.Descriptor(
-  name='Users',
-  full_name='iamanager.v1.Users',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='users', full_name='iamanager.v1.Users.users', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=185,
-  serialized_end=207,
-)
-
-_PERMISSIONS_PERMISSIONSENTRY.containing_type = _PERMISSIONS
-_PERMISSIONS.fields_by_name['permissions'].message_type = _PERMISSIONS_PERMISSIONSENTRY
-DESCRIPTOR.message_types_by_name['Permissions'] = _PERMISSIONS
-DESCRIPTOR.message_types_by_name['Users'] = _USERS
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v1.iamanagercommon_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v1.Permissions.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _PERMISSIONS,
-  '__module__' : 'iamanager.v1.iamanagercommon_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.Permissions)
-  })
-_sym_db.RegisterMessage(Permissions)
-_sym_db.RegisterMessage(Permissions.PermissionsEntry)
-
-Users = _reflection.GeneratedProtocolMessageType('Users', (_message.Message,), {
-  'DESCRIPTOR' : _USERS,
-  '__module__' : 'iamanager.v1.iamanagercommon_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.Users)
-  })
-_sym_db.RegisterMessage(Users)
-
-
-_PERMISSIONS_PERMISSIONSENTRY._options = None
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v1/iamanagercommon.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='iamanager/v1/iamanagercommon.proto',
+  package='iamanager.v1',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n\"iamanager/v1/iamanagercommon.proto\x12\x0ciamanager.v1\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v1.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x05Users\x12\r\n\x05users\x18\x01 \x03(\tb\x06proto3'
+)
+
+
+
+
+_PERMISSIONS_PERMISSIONSENTRY = _descriptor.Descriptor(
+  name='PermissionsEntry',
+  full_name='iamanager.v1.Permissions.PermissionsEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='iamanager.v1.Permissions.PermissionsEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='iamanager.v1.Permissions.PermissionsEntry.value', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=133,
+  serialized_end=183,
+)
+
+_PERMISSIONS = _descriptor.Descriptor(
+  name='Permissions',
+  full_name='iamanager.v1.Permissions',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='iamanager.v1.Permissions.permissions', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_PERMISSIONS_PERMISSIONSENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=53,
+  serialized_end=183,
+)
+
+
+_USERS = _descriptor.Descriptor(
+  name='Users',
+  full_name='iamanager.v1.Users',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='users', full_name='iamanager.v1.Users.users', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=185,
+  serialized_end=207,
+)
+
+_PERMISSIONS_PERMISSIONSENTRY.containing_type = _PERMISSIONS
+_PERMISSIONS.fields_by_name['permissions'].message_type = _PERMISSIONS_PERMISSIONSENTRY
+DESCRIPTOR.message_types_by_name['Permissions'] = _PERMISSIONS
+DESCRIPTOR.message_types_by_name['Users'] = _USERS
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v1.iamanagercommon_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v1.Permissions.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _PERMISSIONS,
+  '__module__' : 'iamanager.v1.iamanagercommon_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.Permissions)
+  })
+_sym_db.RegisterMessage(Permissions)
+_sym_db.RegisterMessage(Permissions.PermissionsEntry)
+
+Users = _reflection.GeneratedProtocolMessageType('Users', (_message.Message,), {
+  'DESCRIPTOR' : _USERS,
+  '__module__' : 'iamanager.v1.iamanagercommon_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.Users)
+  })
+_sym_db.RegisterMessage(Users)
+
+
+_PERMISSIONS_PERMISSIONSENTRY._options = None
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
```

## aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py

 * *Ordering differences only*

```diff
@@ -1,799 +1,799 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v1/iamanagerprotected.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iamanager_dot_v1_dot_iamanagercommon__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v1/iamanagerprotected.proto',
-  package='iamanager.v1',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n%iamanager/v1/iamanagerprotected.proto\x12\x0ciamanager.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v1/iamanagercommon.proto\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\"\x1c\n\x0c\x43learRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\"1\n\x0fSetOwnerRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"2\n\x10\x43reateKeyRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x11\x43reateKeyResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\".\n\x10\x41pplyCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\"3\n\x11\x41pplyCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"\xc7\x01\n\x16RegisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12J\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x35.iamanager.v1.RegisterServiceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v1.Permissions:\x02\x38\x01\")\n\x17RegisterServiceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\".\n\x18UnregisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\"&\n\x12\x45ncryptDiskRequest\x12\x10\n\x08password\x18\x01 \x01(\t2\xcd\x06\n\x13IAMProtectedService\x12\x41\n\x0cGetCertTypes\x12\x16.google.protobuf.Empty\x1a\x17.iamanager.v1.CertTypes\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v1.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v1.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tCreateKey\x12\x1e.iamanager.v1.CreateKeyRequest\x1a\x1f.iamanager.v1.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v1.ApplyCertRequest\x1a\x1f.iamanager.v1.ApplyCertResponse\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v1.GetCertRequest\x1a\x1d.iamanager.v1.GetCertResponse\"\x00\x12\x39\n\x08SetUsers\x12\x13.iamanager.v1.Users\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x0fRegisterService\x12$.iamanager.v1.RegisterServiceRequest\x1a%.iamanager.v1.RegisterServiceResponse\"\x00\x12U\n\x11UnregisterService\x12&.iamanager.v1.UnregisterServiceRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v1.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v1_dot_iamanagercommon__pb2.DESCRIPTOR,])
-
-
-
-
-_CERTTYPES = _descriptor.Descriptor(
-  name='CertTypes',
-  full_name='iamanager.v1.CertTypes',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='types', full_name='iamanager.v1.CertTypes.types', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=120,
-  serialized_end=146,
-)
-
-
-_CLEARREQUEST = _descriptor.Descriptor(
-  name='ClearRequest',
-  full_name='iamanager.v1.ClearRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v1.ClearRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=148,
-  serialized_end=176,
-)
-
-
-_SETOWNERREQUEST = _descriptor.Descriptor(
-  name='SetOwnerRequest',
-  full_name='iamanager.v1.SetOwnerRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v1.SetOwnerRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v1.SetOwnerRequest.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=178,
-  serialized_end=227,
-)
-
-
-_CREATEKEYREQUEST = _descriptor.Descriptor(
-  name='CreateKeyRequest',
-  full_name='iamanager.v1.CreateKeyRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v1.CreateKeyRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v1.CreateKeyRequest.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=229,
-  serialized_end=279,
-)
-
-
-_CREATEKEYRESPONSE = _descriptor.Descriptor(
-  name='CreateKeyResponse',
-  full_name='iamanager.v1.CreateKeyResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v1.CreateKeyResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='csr', full_name='iamanager.v1.CreateKeyResponse.csr', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=281,
-  serialized_end=327,
-)
-
-
-_APPLYCERTREQUEST = _descriptor.Descriptor(
-  name='ApplyCertRequest',
-  full_name='iamanager.v1.ApplyCertRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v1.ApplyCertRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert', full_name='iamanager.v1.ApplyCertRequest.cert', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=329,
-  serialized_end=375,
-)
-
-
-_APPLYCERTRESPONSE = _descriptor.Descriptor(
-  name='ApplyCertResponse',
-  full_name='iamanager.v1.ApplyCertResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v1.ApplyCertResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert_url', full_name='iamanager.v1.ApplyCertResponse.cert_url', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=377,
-  serialized_end=428,
-)
-
-
-_GETCERTREQUEST = _descriptor.Descriptor(
-  name='GetCertRequest',
-  full_name='iamanager.v1.GetCertRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v1.GetCertRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='issuer', full_name='iamanager.v1.GetCertRequest.issuer', index=1,
-      number=2, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='serial', full_name='iamanager.v1.GetCertRequest.serial', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=430,
-  serialized_end=492,
-)
-
-
-_GETCERTRESPONSE = _descriptor.Descriptor(
-  name='GetCertResponse',
-  full_name='iamanager.v1.GetCertResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v1.GetCertResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert_url', full_name='iamanager.v1.GetCertResponse.cert_url', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='key_url', full_name='iamanager.v1.GetCertResponse.key_url', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=494,
-  serialized_end=560,
-)
-
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY = _descriptor.Descriptor(
-  name='PermissionsEntry',
-  full_name='iamanager.v1.RegisterServiceRequest.PermissionsEntry',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='key', full_name='iamanager.v1.RegisterServiceRequest.PermissionsEntry.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='iamanager.v1.RegisterServiceRequest.PermissionsEntry.value', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'8\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=685,
-  serialized_end=762,
-)
-
-_REGISTERSERVICEREQUEST = _descriptor.Descriptor(
-  name='RegisterServiceRequest',
-  full_name='iamanager.v1.RegisterServiceRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v1.RegisterServiceRequest.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v1.RegisterServiceRequest.permissions', index=1,
-      number=2, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_REGISTERSERVICEREQUEST_PERMISSIONSENTRY, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=563,
-  serialized_end=762,
-)
-
-
-_REGISTERSERVICERESPONSE = _descriptor.Descriptor(
-  name='RegisterServiceResponse',
-  full_name='iamanager.v1.RegisterServiceResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='secret', full_name='iamanager.v1.RegisterServiceResponse.secret', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=764,
-  serialized_end=805,
-)
-
-
-_UNREGISTERSERVICEREQUEST = _descriptor.Descriptor(
-  name='UnregisterServiceRequest',
-  full_name='iamanager.v1.UnregisterServiceRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v1.UnregisterServiceRequest.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=807,
-  serialized_end=853,
-)
-
-
-_ENCRYPTDISKREQUEST = _descriptor.Descriptor(
-  name='EncryptDiskRequest',
-  full_name='iamanager.v1.EncryptDiskRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v1.EncryptDiskRequest.password', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=855,
-  serialized_end=893,
-)
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.fields_by_name['value'].message_type = iamanager_dot_v1_dot_iamanagercommon__pb2._PERMISSIONS
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.containing_type = _REGISTERSERVICEREQUEST
-_REGISTERSERVICEREQUEST.fields_by_name['permissions'].message_type = _REGISTERSERVICEREQUEST_PERMISSIONSENTRY
-DESCRIPTOR.message_types_by_name['CertTypes'] = _CERTTYPES
-DESCRIPTOR.message_types_by_name['ClearRequest'] = _CLEARREQUEST
-DESCRIPTOR.message_types_by_name['SetOwnerRequest'] = _SETOWNERREQUEST
-DESCRIPTOR.message_types_by_name['CreateKeyRequest'] = _CREATEKEYREQUEST
-DESCRIPTOR.message_types_by_name['CreateKeyResponse'] = _CREATEKEYRESPONSE
-DESCRIPTOR.message_types_by_name['ApplyCertRequest'] = _APPLYCERTREQUEST
-DESCRIPTOR.message_types_by_name['ApplyCertResponse'] = _APPLYCERTRESPONSE
-DESCRIPTOR.message_types_by_name['GetCertRequest'] = _GETCERTREQUEST
-DESCRIPTOR.message_types_by_name['GetCertResponse'] = _GETCERTRESPONSE
-DESCRIPTOR.message_types_by_name['RegisterServiceRequest'] = _REGISTERSERVICEREQUEST
-DESCRIPTOR.message_types_by_name['RegisterServiceResponse'] = _REGISTERSERVICERESPONSE
-DESCRIPTOR.message_types_by_name['UnregisterServiceRequest'] = _UNREGISTERSERVICEREQUEST
-DESCRIPTOR.message_types_by_name['EncryptDiskRequest'] = _ENCRYPTDISKREQUEST
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
-  'DESCRIPTOR' : _CERTTYPES,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.CertTypes)
-  })
-_sym_db.RegisterMessage(CertTypes)
-
-ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CLEARREQUEST,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.ClearRequest)
-  })
-_sym_db.RegisterMessage(ClearRequest)
-
-SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETOWNERREQUEST,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.SetOwnerRequest)
-  })
-_sym_db.RegisterMessage(SetOwnerRequest)
-
-CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYREQUEST,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.CreateKeyRequest)
-  })
-_sym_db.RegisterMessage(CreateKeyRequest)
-
-CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYRESPONSE,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.CreateKeyResponse)
-  })
-_sym_db.RegisterMessage(CreateKeyResponse)
-
-ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTREQUEST,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.ApplyCertRequest)
-  })
-_sym_db.RegisterMessage(ApplyCertRequest)
-
-ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTRESPONSE,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.ApplyCertResponse)
-  })
-_sym_db.RegisterMessage(ApplyCertResponse)
-
-GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTREQUEST,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.GetCertRequest)
-  })
-_sym_db.RegisterMessage(GetCertRequest)
-
-GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTRESPONSE,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.GetCertResponse)
-  })
-_sym_db.RegisterMessage(GetCertResponse)
-
-RegisterServiceRequest = _reflection.GeneratedProtocolMessageType('RegisterServiceRequest', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _REGISTERSERVICEREQUEST_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v1.RegisterServiceRequest.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _REGISTERSERVICEREQUEST,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.RegisterServiceRequest)
-  })
-_sym_db.RegisterMessage(RegisterServiceRequest)
-_sym_db.RegisterMessage(RegisterServiceRequest.PermissionsEntry)
-
-RegisterServiceResponse = _reflection.GeneratedProtocolMessageType('RegisterServiceResponse', (_message.Message,), {
-  'DESCRIPTOR' : _REGISTERSERVICERESPONSE,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.RegisterServiceResponse)
-  })
-_sym_db.RegisterMessage(RegisterServiceResponse)
-
-UnregisterServiceRequest = _reflection.GeneratedProtocolMessageType('UnregisterServiceRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UNREGISTERSERVICEREQUEST,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.UnregisterServiceRequest)
-  })
-_sym_db.RegisterMessage(UnregisterServiceRequest)
-
-EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
-  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
-  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.EncryptDiskRequest)
-  })
-_sym_db.RegisterMessage(EncryptDiskRequest)
-
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY._options = None
-
-_IAMPROTECTEDSERVICE = _descriptor.ServiceDescriptor(
-  name='IAMProtectedService',
-  full_name='iamanager.v1.IAMProtectedService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=896,
-  serialized_end=1741,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='GetCertTypes',
-    full_name='iamanager.v1.IAMProtectedService.GetCertTypes',
-    index=0,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_CERTTYPES,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='FinishProvisioning',
-    full_name='iamanager.v1.IAMProtectedService.FinishProvisioning',
-    index=1,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='Clear',
-    full_name='iamanager.v1.IAMProtectedService.Clear',
-    index=2,
-    containing_service=None,
-    input_type=_CLEARREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SetOwner',
-    full_name='iamanager.v1.IAMProtectedService.SetOwner',
-    index=3,
-    containing_service=None,
-    input_type=_SETOWNERREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='CreateKey',
-    full_name='iamanager.v1.IAMProtectedService.CreateKey',
-    index=4,
-    containing_service=None,
-    input_type=_CREATEKEYREQUEST,
-    output_type=_CREATEKEYRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='ApplyCert',
-    full_name='iamanager.v1.IAMProtectedService.ApplyCert',
-    index=5,
-    containing_service=None,
-    input_type=_APPLYCERTREQUEST,
-    output_type=_APPLYCERTRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetCert',
-    full_name='iamanager.v1.IAMProtectedService.GetCert',
-    index=6,
-    containing_service=None,
-    input_type=_GETCERTREQUEST,
-    output_type=_GETCERTRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SetUsers',
-    full_name='iamanager.v1.IAMProtectedService.SetUsers',
-    index=7,
-    containing_service=None,
-    input_type=iamanager_dot_v1_dot_iamanagercommon__pb2._USERS,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='RegisterService',
-    full_name='iamanager.v1.IAMProtectedService.RegisterService',
-    index=8,
-    containing_service=None,
-    input_type=_REGISTERSERVICEREQUEST,
-    output_type=_REGISTERSERVICERESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='UnregisterService',
-    full_name='iamanager.v1.IAMProtectedService.UnregisterService',
-    index=9,
-    containing_service=None,
-    input_type=_UNREGISTERSERVICEREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='EncryptDisk',
-    full_name='iamanager.v1.IAMProtectedService.EncryptDisk',
-    index=10,
-    containing_service=None,
-    input_type=_ENCRYPTDISKREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_IAMPROTECTEDSERVICE)
-
-DESCRIPTOR.services_by_name['IAMProtectedService'] = _IAMPROTECTEDSERVICE
-
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v1/iamanagerprotected.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iamanager_dot_v1_dot_iamanagercommon__pb2
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='iamanager/v1/iamanagerprotected.proto',
+  package='iamanager.v1',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n%iamanager/v1/iamanagerprotected.proto\x12\x0ciamanager.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v1/iamanagercommon.proto\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\"\x1c\n\x0c\x43learRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\"1\n\x0fSetOwnerRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"2\n\x10\x43reateKeyRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x11\x43reateKeyResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\".\n\x10\x41pplyCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\"3\n\x11\x41pplyCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"\xc7\x01\n\x16RegisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12J\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x35.iamanager.v1.RegisterServiceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v1.Permissions:\x02\x38\x01\")\n\x17RegisterServiceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\".\n\x18UnregisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\"&\n\x12\x45ncryptDiskRequest\x12\x10\n\x08password\x18\x01 \x01(\t2\xcd\x06\n\x13IAMProtectedService\x12\x41\n\x0cGetCertTypes\x12\x16.google.protobuf.Empty\x1a\x17.iamanager.v1.CertTypes\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v1.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v1.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tCreateKey\x12\x1e.iamanager.v1.CreateKeyRequest\x1a\x1f.iamanager.v1.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v1.ApplyCertRequest\x1a\x1f.iamanager.v1.ApplyCertResponse\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v1.GetCertRequest\x1a\x1d.iamanager.v1.GetCertResponse\"\x00\x12\x39\n\x08SetUsers\x12\x13.iamanager.v1.Users\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x0fRegisterService\x12$.iamanager.v1.RegisterServiceRequest\x1a%.iamanager.v1.RegisterServiceResponse\"\x00\x12U\n\x11UnregisterService\x12&.iamanager.v1.UnregisterServiceRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v1.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v1_dot_iamanagercommon__pb2.DESCRIPTOR,])
+
+
+
+
+_CERTTYPES = _descriptor.Descriptor(
+  name='CertTypes',
+  full_name='iamanager.v1.CertTypes',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='types', full_name='iamanager.v1.CertTypes.types', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=120,
+  serialized_end=146,
+)
+
+
+_CLEARREQUEST = _descriptor.Descriptor(
+  name='ClearRequest',
+  full_name='iamanager.v1.ClearRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v1.ClearRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=148,
+  serialized_end=176,
+)
+
+
+_SETOWNERREQUEST = _descriptor.Descriptor(
+  name='SetOwnerRequest',
+  full_name='iamanager.v1.SetOwnerRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v1.SetOwnerRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.v1.SetOwnerRequest.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=178,
+  serialized_end=227,
+)
+
+
+_CREATEKEYREQUEST = _descriptor.Descriptor(
+  name='CreateKeyRequest',
+  full_name='iamanager.v1.CreateKeyRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v1.CreateKeyRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.v1.CreateKeyRequest.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=229,
+  serialized_end=279,
+)
+
+
+_CREATEKEYRESPONSE = _descriptor.Descriptor(
+  name='CreateKeyResponse',
+  full_name='iamanager.v1.CreateKeyResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v1.CreateKeyResponse.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='csr', full_name='iamanager.v1.CreateKeyResponse.csr', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=281,
+  serialized_end=327,
+)
+
+
+_APPLYCERTREQUEST = _descriptor.Descriptor(
+  name='ApplyCertRequest',
+  full_name='iamanager.v1.ApplyCertRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v1.ApplyCertRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert', full_name='iamanager.v1.ApplyCertRequest.cert', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=329,
+  serialized_end=375,
+)
+
+
+_APPLYCERTRESPONSE = _descriptor.Descriptor(
+  name='ApplyCertResponse',
+  full_name='iamanager.v1.ApplyCertResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v1.ApplyCertResponse.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.v1.ApplyCertResponse.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=377,
+  serialized_end=428,
+)
+
+
+_GETCERTREQUEST = _descriptor.Descriptor(
+  name='GetCertRequest',
+  full_name='iamanager.v1.GetCertRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v1.GetCertRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='issuer', full_name='iamanager.v1.GetCertRequest.issuer', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='serial', full_name='iamanager.v1.GetCertRequest.serial', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=430,
+  serialized_end=492,
+)
+
+
+_GETCERTRESPONSE = _descriptor.Descriptor(
+  name='GetCertResponse',
+  full_name='iamanager.v1.GetCertResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v1.GetCertResponse.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.v1.GetCertResponse.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='key_url', full_name='iamanager.v1.GetCertResponse.key_url', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=494,
+  serialized_end=560,
+)
+
+
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY = _descriptor.Descriptor(
+  name='PermissionsEntry',
+  full_name='iamanager.v1.RegisterServiceRequest.PermissionsEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='iamanager.v1.RegisterServiceRequest.PermissionsEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='iamanager.v1.RegisterServiceRequest.PermissionsEntry.value', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=685,
+  serialized_end=762,
+)
+
+_REGISTERSERVICEREQUEST = _descriptor.Descriptor(
+  name='RegisterServiceRequest',
+  full_name='iamanager.v1.RegisterServiceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='service_id', full_name='iamanager.v1.RegisterServiceRequest.service_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='iamanager.v1.RegisterServiceRequest.permissions', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_REGISTERSERVICEREQUEST_PERMISSIONSENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=563,
+  serialized_end=762,
+)
+
+
+_REGISTERSERVICERESPONSE = _descriptor.Descriptor(
+  name='RegisterServiceResponse',
+  full_name='iamanager.v1.RegisterServiceResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='secret', full_name='iamanager.v1.RegisterServiceResponse.secret', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=764,
+  serialized_end=805,
+)
+
+
+_UNREGISTERSERVICEREQUEST = _descriptor.Descriptor(
+  name='UnregisterServiceRequest',
+  full_name='iamanager.v1.UnregisterServiceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='service_id', full_name='iamanager.v1.UnregisterServiceRequest.service_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=807,
+  serialized_end=853,
+)
+
+
+_ENCRYPTDISKREQUEST = _descriptor.Descriptor(
+  name='EncryptDiskRequest',
+  full_name='iamanager.v1.EncryptDiskRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.v1.EncryptDiskRequest.password', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=855,
+  serialized_end=893,
+)
+
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.fields_by_name['value'].message_type = iamanager_dot_v1_dot_iamanagercommon__pb2._PERMISSIONS
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.containing_type = _REGISTERSERVICEREQUEST
+_REGISTERSERVICEREQUEST.fields_by_name['permissions'].message_type = _REGISTERSERVICEREQUEST_PERMISSIONSENTRY
+DESCRIPTOR.message_types_by_name['CertTypes'] = _CERTTYPES
+DESCRIPTOR.message_types_by_name['ClearRequest'] = _CLEARREQUEST
+DESCRIPTOR.message_types_by_name['SetOwnerRequest'] = _SETOWNERREQUEST
+DESCRIPTOR.message_types_by_name['CreateKeyRequest'] = _CREATEKEYREQUEST
+DESCRIPTOR.message_types_by_name['CreateKeyResponse'] = _CREATEKEYRESPONSE
+DESCRIPTOR.message_types_by_name['ApplyCertRequest'] = _APPLYCERTREQUEST
+DESCRIPTOR.message_types_by_name['ApplyCertResponse'] = _APPLYCERTRESPONSE
+DESCRIPTOR.message_types_by_name['GetCertRequest'] = _GETCERTREQUEST
+DESCRIPTOR.message_types_by_name['GetCertResponse'] = _GETCERTRESPONSE
+DESCRIPTOR.message_types_by_name['RegisterServiceRequest'] = _REGISTERSERVICEREQUEST
+DESCRIPTOR.message_types_by_name['RegisterServiceResponse'] = _REGISTERSERVICERESPONSE
+DESCRIPTOR.message_types_by_name['UnregisterServiceRequest'] = _UNREGISTERSERVICEREQUEST
+DESCRIPTOR.message_types_by_name['EncryptDiskRequest'] = _ENCRYPTDISKREQUEST
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
+  'DESCRIPTOR' : _CERTTYPES,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.CertTypes)
+  })
+_sym_db.RegisterMessage(CertTypes)
+
+ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CLEARREQUEST,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.ClearRequest)
+  })
+_sym_db.RegisterMessage(ClearRequest)
+
+SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SETOWNERREQUEST,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.SetOwnerRequest)
+  })
+_sym_db.RegisterMessage(SetOwnerRequest)
+
+CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYREQUEST,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.CreateKeyRequest)
+  })
+_sym_db.RegisterMessage(CreateKeyRequest)
+
+CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYRESPONSE,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.CreateKeyResponse)
+  })
+_sym_db.RegisterMessage(CreateKeyResponse)
+
+ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTREQUEST,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.ApplyCertRequest)
+  })
+_sym_db.RegisterMessage(ApplyCertRequest)
+
+ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTRESPONSE,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.ApplyCertResponse)
+  })
+_sym_db.RegisterMessage(ApplyCertResponse)
+
+GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTREQUEST,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.GetCertRequest)
+  })
+_sym_db.RegisterMessage(GetCertRequest)
+
+GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTRESPONSE,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.GetCertResponse)
+  })
+_sym_db.RegisterMessage(GetCertResponse)
+
+RegisterServiceRequest = _reflection.GeneratedProtocolMessageType('RegisterServiceRequest', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _REGISTERSERVICEREQUEST_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v1.RegisterServiceRequest.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _REGISTERSERVICEREQUEST,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.RegisterServiceRequest)
+  })
+_sym_db.RegisterMessage(RegisterServiceRequest)
+_sym_db.RegisterMessage(RegisterServiceRequest.PermissionsEntry)
+
+RegisterServiceResponse = _reflection.GeneratedProtocolMessageType('RegisterServiceResponse', (_message.Message,), {
+  'DESCRIPTOR' : _REGISTERSERVICERESPONSE,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.RegisterServiceResponse)
+  })
+_sym_db.RegisterMessage(RegisterServiceResponse)
+
+UnregisterServiceRequest = _reflection.GeneratedProtocolMessageType('UnregisterServiceRequest', (_message.Message,), {
+  'DESCRIPTOR' : _UNREGISTERSERVICEREQUEST,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.UnregisterServiceRequest)
+  })
+_sym_db.RegisterMessage(UnregisterServiceRequest)
+
+EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
+  '__module__' : 'iamanager.v1.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.EncryptDiskRequest)
+  })
+_sym_db.RegisterMessage(EncryptDiskRequest)
+
+
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY._options = None
+
+_IAMPROTECTEDSERVICE = _descriptor.ServiceDescriptor(
+  name='IAMProtectedService',
+  full_name='iamanager.v1.IAMProtectedService',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=896,
+  serialized_end=1741,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='GetCertTypes',
+    full_name='iamanager.v1.IAMProtectedService.GetCertTypes',
+    index=0,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_CERTTYPES,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='FinishProvisioning',
+    full_name='iamanager.v1.IAMProtectedService.FinishProvisioning',
+    index=1,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='Clear',
+    full_name='iamanager.v1.IAMProtectedService.Clear',
+    index=2,
+    containing_service=None,
+    input_type=_CLEARREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetOwner',
+    full_name='iamanager.v1.IAMProtectedService.SetOwner',
+    index=3,
+    containing_service=None,
+    input_type=_SETOWNERREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='CreateKey',
+    full_name='iamanager.v1.IAMProtectedService.CreateKey',
+    index=4,
+    containing_service=None,
+    input_type=_CREATEKEYREQUEST,
+    output_type=_CREATEKEYRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='ApplyCert',
+    full_name='iamanager.v1.IAMProtectedService.ApplyCert',
+    index=5,
+    containing_service=None,
+    input_type=_APPLYCERTREQUEST,
+    output_type=_APPLYCERTRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetCert',
+    full_name='iamanager.v1.IAMProtectedService.GetCert',
+    index=6,
+    containing_service=None,
+    input_type=_GETCERTREQUEST,
+    output_type=_GETCERTRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetUsers',
+    full_name='iamanager.v1.IAMProtectedService.SetUsers',
+    index=7,
+    containing_service=None,
+    input_type=iamanager_dot_v1_dot_iamanagercommon__pb2._USERS,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='RegisterService',
+    full_name='iamanager.v1.IAMProtectedService.RegisterService',
+    index=8,
+    containing_service=None,
+    input_type=_REGISTERSERVICEREQUEST,
+    output_type=_REGISTERSERVICERESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='UnregisterService',
+    full_name='iamanager.v1.IAMProtectedService.UnregisterService',
+    index=9,
+    containing_service=None,
+    input_type=_UNREGISTERSERVICEREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='EncryptDisk',
+    full_name='iamanager.v1.IAMProtectedService.EncryptDisk',
+    index=10,
+    containing_service=None,
+    input_type=_ENCRYPTDISKREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_IAMPROTECTEDSERVICE)
+
+DESCRIPTOR.services_by_name['IAMProtectedService'] = _IAMPROTECTEDSERVICE
+
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,398 +1,398 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iamanager_dot_v1_dot_iamanagercommon__pb2
-from aos_prov.communication.unit.v1.generated import iamanagerprotected_pb2 as iamanager_dot_v1_dot_iamanagerprotected__pb2
-
-
-class IAMProtectedServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetCertTypes = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/GetCertTypes',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CertTypes.FromString,
-                )
-        self.FinishProvisioning = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/FinishProvisioning',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.Clear = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/Clear',
-                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.SetOwner = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/SetOwner',
-                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.CreateKey = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/CreateKey',
-                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
-                )
-        self.ApplyCert = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/ApplyCert',
-                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
-                )
-        self.GetCert = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/GetCert',
-                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertResponse.FromString,
-                )
-        self.SetUsers = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/SetUsers',
-                request_serializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.RegisterService = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/RegisterService',
-                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
-                )
-        self.UnregisterService = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/UnregisterService',
-                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.EncryptDisk = channel.unary_unary(
-                '/iamanager.v1.IAMProtectedService/EncryptDisk',
-                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAMProtectedServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetCertTypes(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def FinishProvisioning(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Clear(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetOwner(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def CreateKey(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ApplyCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetUsers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def RegisterService(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def UnregisterService(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def EncryptDisk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMProtectedServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCertTypes,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CertTypes.SerializeToString,
-            ),
-            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
-                    servicer.FinishProvisioning,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'Clear': grpc.unary_unary_rpc_method_handler(
-                    servicer.Clear,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ClearRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'SetOwner': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetOwner,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.SetOwnerRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'CreateKey': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateKey,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyRequest.FromString,
-                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyResponse.SerializeToString,
-            ),
-            'ApplyCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.ApplyCert,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertRequest.FromString,
-                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertResponse.SerializeToString,
-            ),
-            'GetCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCert,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertRequest.FromString,
-                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertResponse.SerializeToString,
-            ),
-            'SetUsers': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetUsers,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'RegisterService': grpc.unary_unary_rpc_method_handler(
-                    servicer.RegisterService,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceRequest.FromString,
-                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceResponse.SerializeToString,
-            ),
-            'UnregisterService': grpc.unary_unary_rpc_method_handler(
-                    servicer.UnregisterService,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.UnregisterServiceRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
-                    servicer.EncryptDisk,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.EncryptDiskRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v1.IAMProtectedService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMProtectedService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetCertTypes(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/GetCertTypes',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.CertTypes.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def FinishProvisioning(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/FinishProvisioning',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Clear(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/Clear',
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetOwner(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/SetOwner',
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def CreateKey(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/CreateKey',
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ApplyCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/ApplyCert',
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/GetCert',
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertRequest.SerializeToString,
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetUsers(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/SetUsers',
-            iamanager_dot_v1_dot_iamanagercommon__pb2.Users.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def RegisterService(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/RegisterService',
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def UnregisterService(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/UnregisterService',
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def EncryptDisk(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/EncryptDisk',
-            iamanager_dot_v1_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iamanager_dot_v1_dot_iamanagercommon__pb2
+from aos_prov.communication.unit.v1.generated import iamanagerprotected_pb2 as iamanager_dot_v1_dot_iamanagerprotected__pb2
+
+
+class IAMProtectedServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetCertTypes = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/GetCertTypes',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CertTypes.FromString,
+                )
+        self.FinishProvisioning = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/FinishProvisioning',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.Clear = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/Clear',
+                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.SetOwner = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/SetOwner',
+                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.CreateKey = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/CreateKey',
+                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
+                )
+        self.ApplyCert = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/ApplyCert',
+                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
+                )
+        self.GetCert = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/GetCert',
+                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertResponse.FromString,
+                )
+        self.SetUsers = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/SetUsers',
+                request_serializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.RegisterService = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/RegisterService',
+                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
+                )
+        self.UnregisterService = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/UnregisterService',
+                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.EncryptDisk = channel.unary_unary(
+                '/iamanager.v1.IAMProtectedService/EncryptDisk',
+                request_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAMProtectedServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetCertTypes(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def FinishProvisioning(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Clear(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetOwner(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def CreateKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ApplyCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetUsers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def RegisterService(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UnregisterService(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def EncryptDisk(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMProtectedServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCertTypes,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CertTypes.SerializeToString,
+            ),
+            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
+                    servicer.FinishProvisioning,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'Clear': grpc.unary_unary_rpc_method_handler(
+                    servicer.Clear,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ClearRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'SetOwner': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetOwner,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.SetOwnerRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'CreateKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateKey,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyRequest.FromString,
+                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyResponse.SerializeToString,
+            ),
+            'ApplyCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.ApplyCert,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertRequest.FromString,
+                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertResponse.SerializeToString,
+            ),
+            'GetCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCert,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertRequest.FromString,
+                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertResponse.SerializeToString,
+            ),
+            'SetUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetUsers,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'RegisterService': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterService,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceRequest.FromString,
+                    response_serializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceResponse.SerializeToString,
+            ),
+            'UnregisterService': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnregisterService,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.UnregisterServiceRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
+                    servicer.EncryptDisk,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagerprotected__pb2.EncryptDiskRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v1.IAMProtectedService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMProtectedService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetCertTypes(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/GetCertTypes',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.CertTypes.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def FinishProvisioning(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/FinishProvisioning',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Clear(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/Clear',
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetOwner(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/SetOwner',
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/CreateKey',
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ApplyCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/ApplyCert',
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/GetCert',
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertRequest.SerializeToString,
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.GetCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/SetUsers',
+            iamanager_dot_v1_dot_iamanagercommon__pb2.Users.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RegisterService(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/RegisterService',
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UnregisterService(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/UnregisterService',
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def EncryptDisk(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMProtectedService/EncryptDisk',
+            iamanager_dot_v1_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py

 * *Ordering differences only*

```diff
@@ -1,231 +1,231 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v1/iamanagerpublic.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iamanager_dot_v1_dot_iamanagercommon__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v1/iamanagerpublic.proto',
-  package='iamanager.v1',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\"iamanager/v1/iamanagerpublic.proto\x12\x0ciamanager.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v1/iamanagercommon.proto\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"Y\n\x13PermissionsResponse\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v1.Permissions\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t2\xb5\x02\n\x10IAMPublicService\x12W\n\x0eGetPermissions\x12 .iamanager.v1.PermissionsRequest\x1a!.iamanager.v1.PermissionsResponse\"\x00\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v1.SystemInfo\"\x00\x12\x39\n\x08GetUsers\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v1.Users\"\x00\x12H\n\x15SubscribeUsersChanged\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v1.Users\"\x00\x30\x01\x62\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v1_dot_iamanagercommon__pb2.DESCRIPTOR,])
-
-
-
-
-_PERMISSIONSREQUEST = _descriptor.Descriptor(
-  name='PermissionsRequest',
-  full_name='iamanager.v1.PermissionsRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='secret', full_name='iamanager.v1.PermissionsRequest.secret', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='functional_server_id', full_name='iamanager.v1.PermissionsRequest.functional_server_id', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=117,
-  serialized_end=183,
-)
-
-
-_PERMISSIONSRESPONSE = _descriptor.Descriptor(
-  name='PermissionsResponse',
-  full_name='iamanager.v1.PermissionsResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v1.PermissionsResponse.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v1.PermissionsResponse.permissions', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=185,
-  serialized_end=274,
-)
-
-
-_SYSTEMINFO = _descriptor.Descriptor(
-  name='SystemInfo',
-  full_name='iamanager.v1.SystemInfo',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='system_id', full_name='iamanager.v1.SystemInfo.system_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='board_model', full_name='iamanager.v1.SystemInfo.board_model', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=276,
-  serialized_end=328,
-)
-
-_PERMISSIONSRESPONSE.fields_by_name['permissions'].message_type = iamanager_dot_v1_dot_iamanagercommon__pb2._PERMISSIONS
-DESCRIPTOR.message_types_by_name['PermissionsRequest'] = _PERMISSIONSREQUEST
-DESCRIPTOR.message_types_by_name['PermissionsResponse'] = _PERMISSIONSRESPONSE
-DESCRIPTOR.message_types_by_name['SystemInfo'] = _SYSTEMINFO
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSREQUEST,
-  '__module__' : 'iamanager.v1.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.PermissionsRequest)
-  })
-_sym_db.RegisterMessage(PermissionsRequest)
-
-PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
-  '__module__' : 'iamanager.v1.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.PermissionsResponse)
-  })
-_sym_db.RegisterMessage(PermissionsResponse)
-
-SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
-  'DESCRIPTOR' : _SYSTEMINFO,
-  '__module__' : 'iamanager.v1.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v1.SystemInfo)
-  })
-_sym_db.RegisterMessage(SystemInfo)
-
-
-
-_IAMPUBLICSERVICE = _descriptor.ServiceDescriptor(
-  name='IAMPublicService',
-  full_name='iamanager.v1.IAMPublicService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=331,
-  serialized_end=640,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='GetPermissions',
-    full_name='iamanager.v1.IAMPublicService.GetPermissions',
-    index=0,
-    containing_service=None,
-    input_type=_PERMISSIONSREQUEST,
-    output_type=_PERMISSIONSRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetSystemInfo',
-    full_name='iamanager.v1.IAMPublicService.GetSystemInfo',
-    index=1,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_SYSTEMINFO,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetUsers',
-    full_name='iamanager.v1.IAMPublicService.GetUsers',
-    index=2,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=iamanager_dot_v1_dot_iamanagercommon__pb2._USERS,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SubscribeUsersChanged',
-    full_name='iamanager.v1.IAMPublicService.SubscribeUsersChanged',
-    index=3,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=iamanager_dot_v1_dot_iamanagercommon__pb2._USERS,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_IAMPUBLICSERVICE)
-
-DESCRIPTOR.services_by_name['IAMPublicService'] = _IAMPUBLICSERVICE
-
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v1/iamanagerpublic.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iamanager_dot_v1_dot_iamanagercommon__pb2
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='iamanager/v1/iamanagerpublic.proto',
+  package='iamanager.v1',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n\"iamanager/v1/iamanagerpublic.proto\x12\x0ciamanager.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v1/iamanagercommon.proto\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"Y\n\x13PermissionsResponse\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v1.Permissions\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t2\xb5\x02\n\x10IAMPublicService\x12W\n\x0eGetPermissions\x12 .iamanager.v1.PermissionsRequest\x1a!.iamanager.v1.PermissionsResponse\"\x00\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v1.SystemInfo\"\x00\x12\x39\n\x08GetUsers\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v1.Users\"\x00\x12H\n\x15SubscribeUsersChanged\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v1.Users\"\x00\x30\x01\x62\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v1_dot_iamanagercommon__pb2.DESCRIPTOR,])
+
+
+
+
+_PERMISSIONSREQUEST = _descriptor.Descriptor(
+  name='PermissionsRequest',
+  full_name='iamanager.v1.PermissionsRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='secret', full_name='iamanager.v1.PermissionsRequest.secret', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='functional_server_id', full_name='iamanager.v1.PermissionsRequest.functional_server_id', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=117,
+  serialized_end=183,
+)
+
+
+_PERMISSIONSRESPONSE = _descriptor.Descriptor(
+  name='PermissionsResponse',
+  full_name='iamanager.v1.PermissionsResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='service_id', full_name='iamanager.v1.PermissionsResponse.service_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='iamanager.v1.PermissionsResponse.permissions', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=185,
+  serialized_end=274,
+)
+
+
+_SYSTEMINFO = _descriptor.Descriptor(
+  name='SystemInfo',
+  full_name='iamanager.v1.SystemInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='system_id', full_name='iamanager.v1.SystemInfo.system_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='board_model', full_name='iamanager.v1.SystemInfo.board_model', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=276,
+  serialized_end=328,
+)
+
+_PERMISSIONSRESPONSE.fields_by_name['permissions'].message_type = iamanager_dot_v1_dot_iamanagercommon__pb2._PERMISSIONS
+DESCRIPTOR.message_types_by_name['PermissionsRequest'] = _PERMISSIONSREQUEST
+DESCRIPTOR.message_types_by_name['PermissionsResponse'] = _PERMISSIONSRESPONSE
+DESCRIPTOR.message_types_by_name['SystemInfo'] = _SYSTEMINFO
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSREQUEST,
+  '__module__' : 'iamanager.v1.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.PermissionsRequest)
+  })
+_sym_db.RegisterMessage(PermissionsRequest)
+
+PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
+  '__module__' : 'iamanager.v1.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.PermissionsResponse)
+  })
+_sym_db.RegisterMessage(PermissionsResponse)
+
+SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMINFO,
+  '__module__' : 'iamanager.v1.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v1.SystemInfo)
+  })
+_sym_db.RegisterMessage(SystemInfo)
+
+
+
+_IAMPUBLICSERVICE = _descriptor.ServiceDescriptor(
+  name='IAMPublicService',
+  full_name='iamanager.v1.IAMPublicService',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=331,
+  serialized_end=640,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='GetPermissions',
+    full_name='iamanager.v1.IAMPublicService.GetPermissions',
+    index=0,
+    containing_service=None,
+    input_type=_PERMISSIONSREQUEST,
+    output_type=_PERMISSIONSRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetSystemInfo',
+    full_name='iamanager.v1.IAMPublicService.GetSystemInfo',
+    index=1,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_SYSTEMINFO,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetUsers',
+    full_name='iamanager.v1.IAMPublicService.GetUsers',
+    index=2,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=iamanager_dot_v1_dot_iamanagercommon__pb2._USERS,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SubscribeUsersChanged',
+    full_name='iamanager.v1.IAMPublicService.SubscribeUsersChanged',
+    index=3,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=iamanager_dot_v1_dot_iamanagercommon__pb2._USERS,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_IAMPUBLICSERVICE)
+
+DESCRIPTOR.services_by_name['IAMPublicService'] = _IAMPUBLICSERVICE
+
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,167 +1,167 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iamanager_dot_v1_dot_iamanagercommon__pb2
-from aos_prov.communication.unit.v1.generated import iamanagerpublic_pb2 as iamanager_dot_v1_dot_iamanagerpublic__pb2
-
-
-class IAMPublicServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetPermissions = channel.unary_unary(
-                '/iamanager.v1.IAMPublicService/GetPermissions',
-                request_serializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
-                )
-        self.GetSystemInfo = channel.unary_unary(
-                '/iamanager.v1.IAMPublicService/GetSystemInfo',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.SystemInfo.FromString,
-                )
-        self.GetUsers = channel.unary_unary(
-                '/iamanager.v1.IAMPublicService/GetUsers',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
-                )
-        self.SubscribeUsersChanged = channel.unary_stream(
-                '/iamanager.v1.IAMPublicService/SubscribeUsersChanged',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
-                )
-
-
-class IAMPublicServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetPermissions(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetSystemInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetUsers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SubscribeUsersChanged(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetPermissions': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetPermissions,
-                    request_deserializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsRequest.FromString,
-                    response_serializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsResponse.SerializeToString,
-            ),
-            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSystemInfo,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.SystemInfo.SerializeToString,
-            ),
-            'GetUsers': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetUsers,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.SerializeToString,
-            ),
-            'SubscribeUsersChanged': grpc.unary_stream_rpc_method_handler(
-                    servicer.SubscribeUsersChanged,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v1.IAMPublicService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetPermissions(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMPublicService/GetPermissions',
-            iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
-            iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetSystemInfo(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMPublicService/GetSystemInfo',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v1_dot_iamanagerpublic__pb2.SystemInfo.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetUsers(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMPublicService/GetUsers',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SubscribeUsersChanged(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iamanager.v1.IAMPublicService/SubscribeUsersChanged',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v1.generated import iamanagercommon_pb2 as iamanager_dot_v1_dot_iamanagercommon__pb2
+from aos_prov.communication.unit.v1.generated import iamanagerpublic_pb2 as iamanager_dot_v1_dot_iamanagerpublic__pb2
+
+
+class IAMPublicServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetPermissions = channel.unary_unary(
+                '/iamanager.v1.IAMPublicService/GetPermissions',
+                request_serializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
+                )
+        self.GetSystemInfo = channel.unary_unary(
+                '/iamanager.v1.IAMPublicService/GetSystemInfo',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.SystemInfo.FromString,
+                )
+        self.GetUsers = channel.unary_unary(
+                '/iamanager.v1.IAMPublicService/GetUsers',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
+                )
+        self.SubscribeUsersChanged = channel.unary_stream(
+                '/iamanager.v1.IAMPublicService/SubscribeUsersChanged',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
+                )
+
+
+class IAMPublicServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetPermissions(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetSystemInfo(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetUsers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubscribeUsersChanged(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetPermissions': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPermissions,
+                    request_deserializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsRequest.FromString,
+                    response_serializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsResponse.SerializeToString,
+            ),
+            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSystemInfo,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v1_dot_iamanagerpublic__pb2.SystemInfo.SerializeToString,
+            ),
+            'GetUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetUsers,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.SerializeToString,
+            ),
+            'SubscribeUsersChanged': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeUsersChanged,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v1_dot_iamanagercommon__pb2.Users.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v1.IAMPublicService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetPermissions(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMPublicService/GetPermissions',
+            iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
+            iamanager_dot_v1_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetSystemInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMPublicService/GetSystemInfo',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v1_dot_iamanagerpublic__pb2.SystemInfo.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v1.IAMPublicService/GetUsers',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubscribeUsersChanged(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/iamanager.v1.IAMPublicService/SubscribeUsersChanged',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v1_dot_iamanagercommon__pb2.Users.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/communication/unit/v2/unit_communication_v2.py

```diff
@@ -1,167 +1,161 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
-import time
-from contextlib import contextmanager
-
-import grpc
-from colorama import Fore, Style
-from google.protobuf import empty_pb2
-
-from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iam_manager_common
-from aos_prov.communication.unit.v2.generated import iamanagerprotected_pb2 as iam_manager
-from aos_prov.communication.unit.v2.generated import iamanagerprotected_pb2_grpc as api_iam_manager_grpc
-from aos_prov.communication.unit.v2.generated import iamanagerpublic_pb2_grpc as iam_manager_public_grpc
-from aos_prov.utils.errors import BoardError, GrpcUnimplemented
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-UNIT_DEFAULT_PORT = 8089
-
-
-class UnitCommunicationV2:
-    def __init__(self, address: str = 'localhost:8089', set_users=True):
-        self._need_set_users = True
-
-        if address is None:
-            address = 'localhost:8089'
-        parts = address.split(':')
-        if len(parts) == 2:
-            try:
-                port = int(parts[1])
-                if not 1 <= port <= 65535:
-                    raise BoardError("Unit port is invalid")
-            except ValueError:
-                raise BoardError("Unit port is invalid")
-        else:
-            address = address + ':' + str(UNIT_DEFAULT_PORT)
-        self.__unit_address = address
-        print(f"Will search unit on address: {Fore.GREEN}{self.__unit_address}{Style.RESET_ALL}")
-
-    @property
-    def need_set_users(self):
-        return self._need_set_users
-
-    @need_set_users.setter
-    def need_set_users(self, value):
-        self._need_set_users = value
-
-    @contextmanager
-    def unit_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = api_iam_manager_grpc.IAMProtectedServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):
-                        print(str(state))
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as e:
-            print(e)
-            if catch_inactive and \
-                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
-                return
-            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
-                return
-            error_text = (f"{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}"
-                          f"{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}")
-            raise BoardError(error_text)
-
-    @contextmanager
-    def unit_public_stub(self):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_public_grpc.IAMPublicServiceStub(channel)
-                yield stub
-
-        except grpc.RpcError as e:
-            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
-                error_text = (f'{Fore.YELLOW}FAILED! Protocol V2 is not supported: {Style.RESET_ALL}'
-                              f'{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}')
-                raise GrpcUnimplemented(error_text)
-            else:
-                error_text = (f'{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}'
-                              f'{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}')
-                raise BoardError(error_text)
-
-    def get_protocol_version(self) -> int:
-        with self.unit_public_stub() as stub:
-            print('Getting protocol version...')
-            response = stub.GetAPIVersion(empty_pb2.Empty())
-            print(f'Unit responded with version: {response.version}')
-            return int(response.version)
-
-    def get_system_info(self) -> (str, str):
-        with self.unit_public_stub() as stub:
-            print('Getting System Info...')
-            response = stub.GetSystemInfo(empty_pb2.Empty())
-            print('System ID: ' + response.system_id)
-            print('Model name: ' + response.board_model)
-            return response.system_id, response.board_model
-
-    def clear(self, certificate_type: str) -> None:
-        with self.unit_stub() as stub:
-            print('Clear certificate: ' + certificate_type)
-            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type))
-            return response
-
-    def set_cert_owner(self, certificate_type: str, password: str) -> None:
-        with self.unit_stub() as stub:
-            print('Set owner: ' + certificate_type)
-            response = stub.SetOwner(iam_manager.SetOwnerRequest(type=certificate_type, password=password))
-            return response
-
-    def get_cert_types(self) -> [str]:
-        with self.unit_public_stub() as stub:
-            print('Getting certificate types to renew')
-            response = stub.GetCertTypes(empty_pb2.Empty())
-            print('Will be renewed: ' + str(response.types))
-            return response.types
-
-    def create_keys(self, cert_type: str, password: str) -> UnitCertificate:
-        with self.unit_stub() as stub:
-            print('Generating key type:' + cert_type)
-            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password))
-            uc = UnitCertificate()
-            uc.cert_type = response.type
-            uc.csr = response.csr
-            return uc
-
-    def apply_certificate(self, unit_cert: UnitCertificate):
-        with self.unit_stub() as stub:
-            print('Applying type:' + unit_cert.cert_type)
-            stub.ApplyCert(iam_manager.ApplyCertRequest(type=unit_cert.cert_type, cert=unit_cert.certificate))
-
-    def set_users(self, users: [str]):
-        with self.unit_stub() as stub:
-            print('setting users')
-            stub.SetUsers(iam_manager_common.Users(users=users))
-
-    def encrypt_disk(self, password: str):
-        print('Starting disk encryption...')
-        try:
-            with self.unit_stub(wait_for_close=True) as stub:
-                stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password))
-                print('Encryption process is finished.')
-        except BoardError as be:
-            print('Disk encryption returned error.')
-            print(be)
-
-    def finish_provisioning(self):
-        with self.unit_stub(True) as stub:
-            print('Finishing provisioning')
-            stub.FinishProvisioning(empty_pb2.Empty())
-
-    def wait_for_connection(self):
-        try:
-            print('Sleep for 5 seconds...')
-            time.sleep(5)
-            print('Waiting for Unit reboot...')
-            grpc.channel_ready_future(grpc.insecure_channel(self.__unit_address)).result(timeout=300)
-            print('Unit is online')
-        except grpc.FutureTimeoutError:
-            raise BoardError('Board didnt went online')
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+import time
+from contextlib import contextmanager
+
+import grpc
+from google.protobuf import empty_pb2
+
+from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iam_manager_common
+from aos_prov.communication.unit.v2.generated import iamanagerprotected_pb2 as iam_manager
+from aos_prov.communication.unit.v2.generated import iamanagerprotected_pb2_grpc as api_iam_manager_grpc
+from aos_prov.communication.unit.v2.generated import iamanagerpublic_pb2_grpc as iam_manager_public_grpc
+from aos_prov.utils.common import print_message
+from aos_prov.utils.errors import BoardError, GrpcUnimplemented
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+UNIT_DEFAULT_PORT = 8089
+
+
+class UnitCommunicationV2:
+    def __init__(self, address: str = 'localhost:8089', set_users=True):
+        self._need_set_users = True
+
+        if address is None:
+            address = 'localhost:8089'
+        parts = address.split(':')
+        if len(parts) == 2:
+            try:
+                port = int(parts[1])
+                if not 1 <= port <= 65535:
+                    raise BoardError("Unit port is invalid")
+            except ValueError:
+                raise BoardError("Unit port is invalid")
+        else:
+            address = address + ':' + str(UNIT_DEFAULT_PORT)
+        self.__unit_address = address
+        print_message(f'Will search unit on address: [green]{self.__unit_address}')
+
+    @property
+    def need_set_users(self):
+        return self._need_set_users
+
+    @need_set_users.setter
+    def need_set_users(self, value):
+        self._need_set_users = value
+
+    @contextmanager
+    def unit_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = api_iam_manager_grpc.IAMProtectedServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):
+                        print(str(state))
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as e:
+            print(e)
+            if catch_inactive and \
+                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
+                return
+            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
+                return
+            raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_public_stub(self):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_public_grpc.IAMPublicServiceStub(channel)
+                yield stub
+
+        except grpc.RpcError as e:
+            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
+                raise GrpcUnimplemented(f'Protocol V2 is not supported: \n{e.code()}: {e.details()}')
+            else:
+                raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    def get_protocol_version(self) -> int:
+        with self.unit_public_stub() as stub:
+            print('Getting protocol version...')
+            response = stub.GetAPIVersion(empty_pb2.Empty())
+            print(f'Unit responded with version: {response.version}')
+            return int(response.version)
+
+    def get_system_info(self) -> (str, str):
+        with self.unit_public_stub() as stub:
+            print('Getting System Info...')
+            response = stub.GetSystemInfo(empty_pb2.Empty())
+            print('System ID: ' + response.system_id)
+            print('Model name: ' + response.board_model)
+            return response.system_id, response.board_model
+
+    def clear(self, certificate_type: str) -> None:
+        with self.unit_stub() as stub:
+            print('Clear certificate: ' + certificate_type)
+            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type))
+            return response
+
+    def set_cert_owner(self, certificate_type: str, password: str) -> None:
+        with self.unit_stub() as stub:
+            print('Set owner: ' + certificate_type)
+            response = stub.SetOwner(iam_manager.SetOwnerRequest(type=certificate_type, password=password))
+            return response
+
+    def get_cert_types(self) -> [str]:
+        with self.unit_public_stub() as stub:
+            print('Getting certificate types to renew')
+            response = stub.GetCertTypes(empty_pb2.Empty())
+            print('Will be renewed: ' + str(response.types))
+            return response.types
+
+    def create_keys(self, cert_type: str, password: str) -> UnitCertificate:
+        with self.unit_stub() as stub:
+            print('Generating key type:' + cert_type)
+            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password))
+            uc = UnitCertificate()
+            uc.cert_type = response.type
+            uc.csr = response.csr
+            return uc
+
+    def apply_certificate(self, unit_cert: UnitCertificate):
+        with self.unit_stub() as stub:
+            print('Applying type:' + unit_cert.cert_type)
+            stub.ApplyCert(iam_manager.ApplyCertRequest(type=unit_cert.cert_type, cert=unit_cert.certificate))
+
+    def set_users(self, users: [str]):
+        with self.unit_stub() as stub:
+            print('setting users')
+            stub.SetUsers(iam_manager_common.Users(users=users))
+
+    def encrypt_disk(self, password: str):
+        print('Starting disk encryption...')
+        try:
+            with self.unit_stub(wait_for_close=True) as stub:
+                stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password))
+                print('Encryption process is finished.')
+        except BoardError as be:
+            print('Disk encryption returned error.')
+            print(be)
+
+    def finish_provisioning(self):
+        with self.unit_stub(True) as stub:
+            print('Finishing provisioning')
+            stub.FinishProvisioning(empty_pb2.Empty())
+
+    def wait_for_connection(self):
+        try:
+            print('Sleep for 5 seconds...')
+            time.sleep(5)
+            print('Waiting for Unit reboot...')
+            grpc.channel_ready_future(grpc.insecure_channel(self.__unit_address)).result(timeout=300)
+            print('Unit is online')
+        except grpc.FutureTimeoutError:
+            raise BoardError('Board didnt went online')
```

## aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py

 * *Ordering differences only*

```diff
@@ -1,159 +1,159 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v2/iamanagercommon.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v2/iamanagercommon.proto',
-  package='iamanager.v2',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\"iamanager/v2/iamanagercommon.proto\x12\x0ciamanager.v2\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v2.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x05Users\x12\r\n\x05users\x18\x01 \x03(\tb\x06proto3'
-)
-
-
-
-
-_PERMISSIONS_PERMISSIONSENTRY = _descriptor.Descriptor(
-  name='PermissionsEntry',
-  full_name='iamanager.v2.Permissions.PermissionsEntry',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='key', full_name='iamanager.v2.Permissions.PermissionsEntry.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='iamanager.v2.Permissions.PermissionsEntry.value', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'8\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=133,
-  serialized_end=183,
-)
-
-_PERMISSIONS = _descriptor.Descriptor(
-  name='Permissions',
-  full_name='iamanager.v2.Permissions',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v2.Permissions.permissions', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_PERMISSIONS_PERMISSIONSENTRY, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=53,
-  serialized_end=183,
-)
-
-
-_USERS = _descriptor.Descriptor(
-  name='Users',
-  full_name='iamanager.v2.Users',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='users', full_name='iamanager.v2.Users.users', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=185,
-  serialized_end=207,
-)
-
-_PERMISSIONS_PERMISSIONSENTRY.containing_type = _PERMISSIONS
-_PERMISSIONS.fields_by_name['permissions'].message_type = _PERMISSIONS_PERMISSIONSENTRY
-DESCRIPTOR.message_types_by_name['Permissions'] = _PERMISSIONS
-DESCRIPTOR.message_types_by_name['Users'] = _USERS
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v2.iamanagercommon_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v2.Permissions.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _PERMISSIONS,
-  '__module__' : 'iamanager.v2.iamanagercommon_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.Permissions)
-  })
-_sym_db.RegisterMessage(Permissions)
-_sym_db.RegisterMessage(Permissions.PermissionsEntry)
-
-Users = _reflection.GeneratedProtocolMessageType('Users', (_message.Message,), {
-  'DESCRIPTOR' : _USERS,
-  '__module__' : 'iamanager.v2.iamanagercommon_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.Users)
-  })
-_sym_db.RegisterMessage(Users)
-
-
-_PERMISSIONS_PERMISSIONSENTRY._options = None
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v2/iamanagercommon.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='iamanager/v2/iamanagercommon.proto',
+  package='iamanager.v2',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n\"iamanager/v2/iamanagercommon.proto\x12\x0ciamanager.v2\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v2.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x05Users\x12\r\n\x05users\x18\x01 \x03(\tb\x06proto3'
+)
+
+
+
+
+_PERMISSIONS_PERMISSIONSENTRY = _descriptor.Descriptor(
+  name='PermissionsEntry',
+  full_name='iamanager.v2.Permissions.PermissionsEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='iamanager.v2.Permissions.PermissionsEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='iamanager.v2.Permissions.PermissionsEntry.value', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=133,
+  serialized_end=183,
+)
+
+_PERMISSIONS = _descriptor.Descriptor(
+  name='Permissions',
+  full_name='iamanager.v2.Permissions',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='iamanager.v2.Permissions.permissions', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_PERMISSIONS_PERMISSIONSENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=53,
+  serialized_end=183,
+)
+
+
+_USERS = _descriptor.Descriptor(
+  name='Users',
+  full_name='iamanager.v2.Users',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='users', full_name='iamanager.v2.Users.users', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=185,
+  serialized_end=207,
+)
+
+_PERMISSIONS_PERMISSIONSENTRY.containing_type = _PERMISSIONS
+_PERMISSIONS.fields_by_name['permissions'].message_type = _PERMISSIONS_PERMISSIONSENTRY
+DESCRIPTOR.message_types_by_name['Permissions'] = _PERMISSIONS
+DESCRIPTOR.message_types_by_name['Users'] = _USERS
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v2.iamanagercommon_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v2.Permissions.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _PERMISSIONS,
+  '__module__' : 'iamanager.v2.iamanagercommon_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.Permissions)
+  })
+_sym_db.RegisterMessage(Permissions)
+_sym_db.RegisterMessage(Permissions.PermissionsEntry)
+
+Users = _reflection.GeneratedProtocolMessageType('Users', (_message.Message,), {
+  'DESCRIPTOR' : _USERS,
+  '__module__' : 'iamanager.v2.iamanagercommon_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.Users)
+  })
+_sym_db.RegisterMessage(Users)
+
+
+_PERMISSIONS_PERMISSIONSENTRY._options = None
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
```

## aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py

 * *Ordering differences only*

```diff
@@ -1,631 +1,631 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v2/iamanagerprotected.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v2/iamanagerprotected.proto',
-  package='iamanager.v2',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n%iamanager/v2/iamanagerprotected.proto\x12\x0ciamanager.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v2/iamanagercommon.proto\"\x1c\n\x0c\x43learRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\"1\n\x0fSetOwnerRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"2\n\x10\x43reateKeyRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x11\x43reateKeyResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\".\n\x10\x41pplyCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\"3\n\x11\x41pplyCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\"\xc7\x01\n\x16RegisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12J\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x35.iamanager.v2.RegisterServiceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v2.Permissions:\x02\x38\x01\")\n\x17RegisterServiceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\".\n\x18UnregisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\"&\n\x12\x45ncryptDiskRequest\x12\x10\n\x08password\x18\x01 \x01(\t2\xc0\x05\n\x13IAMProtectedService\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v2.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v2.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tCreateKey\x12\x1e.iamanager.v2.CreateKeyRequest\x1a\x1f.iamanager.v2.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v2.ApplyCertRequest\x1a\x1f.iamanager.v2.ApplyCertResponse\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v2.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x39\n\x08SetUsers\x12\x13.iamanager.v2.Users\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x0fRegisterService\x12$.iamanager.v2.RegisterServiceRequest\x1a%.iamanager.v2.RegisterServiceResponse\"\x00\x12U\n\x11UnregisterService\x12&.iamanager.v2.UnregisterServiceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v2_dot_iamanagercommon__pb2.DESCRIPTOR,])
-
-
-
-
-_CLEARREQUEST = _descriptor.Descriptor(
-  name='ClearRequest',
-  full_name='iamanager.v2.ClearRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.ClearRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=120,
-  serialized_end=148,
-)
-
-
-_SETOWNERREQUEST = _descriptor.Descriptor(
-  name='SetOwnerRequest',
-  full_name='iamanager.v2.SetOwnerRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.SetOwnerRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v2.SetOwnerRequest.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=150,
-  serialized_end=199,
-)
-
-
-_CREATEKEYREQUEST = _descriptor.Descriptor(
-  name='CreateKeyRequest',
-  full_name='iamanager.v2.CreateKeyRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.CreateKeyRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v2.CreateKeyRequest.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=201,
-  serialized_end=251,
-)
-
-
-_CREATEKEYRESPONSE = _descriptor.Descriptor(
-  name='CreateKeyResponse',
-  full_name='iamanager.v2.CreateKeyResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.CreateKeyResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='csr', full_name='iamanager.v2.CreateKeyResponse.csr', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=253,
-  serialized_end=299,
-)
-
-
-_APPLYCERTREQUEST = _descriptor.Descriptor(
-  name='ApplyCertRequest',
-  full_name='iamanager.v2.ApplyCertRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.ApplyCertRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert', full_name='iamanager.v2.ApplyCertRequest.cert', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=301,
-  serialized_end=347,
-)
-
-
-_APPLYCERTRESPONSE = _descriptor.Descriptor(
-  name='ApplyCertResponse',
-  full_name='iamanager.v2.ApplyCertResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.ApplyCertResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert_url', full_name='iamanager.v2.ApplyCertResponse.cert_url', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=349,
-  serialized_end=400,
-)
-
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY = _descriptor.Descriptor(
-  name='PermissionsEntry',
-  full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='key', full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry.value', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'8\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=525,
-  serialized_end=602,
-)
-
-_REGISTERSERVICEREQUEST = _descriptor.Descriptor(
-  name='RegisterServiceRequest',
-  full_name='iamanager.v2.RegisterServiceRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v2.RegisterServiceRequest.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v2.RegisterServiceRequest.permissions', index=1,
-      number=2, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_REGISTERSERVICEREQUEST_PERMISSIONSENTRY, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=403,
-  serialized_end=602,
-)
-
-
-_REGISTERSERVICERESPONSE = _descriptor.Descriptor(
-  name='RegisterServiceResponse',
-  full_name='iamanager.v2.RegisterServiceResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='secret', full_name='iamanager.v2.RegisterServiceResponse.secret', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=604,
-  serialized_end=645,
-)
-
-
-_UNREGISTERSERVICEREQUEST = _descriptor.Descriptor(
-  name='UnregisterServiceRequest',
-  full_name='iamanager.v2.UnregisterServiceRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v2.UnregisterServiceRequest.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=647,
-  serialized_end=693,
-)
-
-
-_ENCRYPTDISKREQUEST = _descriptor.Descriptor(
-  name='EncryptDiskRequest',
-  full_name='iamanager.v2.EncryptDiskRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v2.EncryptDiskRequest.password', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=695,
-  serialized_end=733,
-)
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.fields_by_name['value'].message_type = iamanager_dot_v2_dot_iamanagercommon__pb2._PERMISSIONS
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.containing_type = _REGISTERSERVICEREQUEST
-_REGISTERSERVICEREQUEST.fields_by_name['permissions'].message_type = _REGISTERSERVICEREQUEST_PERMISSIONSENTRY
-DESCRIPTOR.message_types_by_name['ClearRequest'] = _CLEARREQUEST
-DESCRIPTOR.message_types_by_name['SetOwnerRequest'] = _SETOWNERREQUEST
-DESCRIPTOR.message_types_by_name['CreateKeyRequest'] = _CREATEKEYREQUEST
-DESCRIPTOR.message_types_by_name['CreateKeyResponse'] = _CREATEKEYRESPONSE
-DESCRIPTOR.message_types_by_name['ApplyCertRequest'] = _APPLYCERTREQUEST
-DESCRIPTOR.message_types_by_name['ApplyCertResponse'] = _APPLYCERTRESPONSE
-DESCRIPTOR.message_types_by_name['RegisterServiceRequest'] = _REGISTERSERVICEREQUEST
-DESCRIPTOR.message_types_by_name['RegisterServiceResponse'] = _REGISTERSERVICERESPONSE
-DESCRIPTOR.message_types_by_name['UnregisterServiceRequest'] = _UNREGISTERSERVICEREQUEST
-DESCRIPTOR.message_types_by_name['EncryptDiskRequest'] = _ENCRYPTDISKREQUEST
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CLEARREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.ClearRequest)
-  })
-_sym_db.RegisterMessage(ClearRequest)
-
-SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETOWNERREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.SetOwnerRequest)
-  })
-_sym_db.RegisterMessage(SetOwnerRequest)
-
-CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.CreateKeyRequest)
-  })
-_sym_db.RegisterMessage(CreateKeyRequest)
-
-CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYRESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.CreateKeyResponse)
-  })
-_sym_db.RegisterMessage(CreateKeyResponse)
-
-ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.ApplyCertRequest)
-  })
-_sym_db.RegisterMessage(ApplyCertRequest)
-
-ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTRESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.ApplyCertResponse)
-  })
-_sym_db.RegisterMessage(ApplyCertResponse)
-
-RegisterServiceRequest = _reflection.GeneratedProtocolMessageType('RegisterServiceRequest', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _REGISTERSERVICEREQUEST_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceRequest.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _REGISTERSERVICEREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceRequest)
-  })
-_sym_db.RegisterMessage(RegisterServiceRequest)
-_sym_db.RegisterMessage(RegisterServiceRequest.PermissionsEntry)
-
-RegisterServiceResponse = _reflection.GeneratedProtocolMessageType('RegisterServiceResponse', (_message.Message,), {
-  'DESCRIPTOR' : _REGISTERSERVICERESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceResponse)
-  })
-_sym_db.RegisterMessage(RegisterServiceResponse)
-
-UnregisterServiceRequest = _reflection.GeneratedProtocolMessageType('UnregisterServiceRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UNREGISTERSERVICEREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.UnregisterServiceRequest)
-  })
-_sym_db.RegisterMessage(UnregisterServiceRequest)
-
-EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
-  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.EncryptDiskRequest)
-  })
-_sym_db.RegisterMessage(EncryptDiskRequest)
-
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY._options = None
-
-_IAMPROTECTEDSERVICE = _descriptor.ServiceDescriptor(
-  name='IAMProtectedService',
-  full_name='iamanager.v2.IAMProtectedService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=736,
-  serialized_end=1440,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='SetOwner',
-    full_name='iamanager.v2.IAMProtectedService.SetOwner',
-    index=0,
-    containing_service=None,
-    input_type=_SETOWNERREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='Clear',
-    full_name='iamanager.v2.IAMProtectedService.Clear',
-    index=1,
-    containing_service=None,
-    input_type=_CLEARREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='CreateKey',
-    full_name='iamanager.v2.IAMProtectedService.CreateKey',
-    index=2,
-    containing_service=None,
-    input_type=_CREATEKEYREQUEST,
-    output_type=_CREATEKEYRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='ApplyCert',
-    full_name='iamanager.v2.IAMProtectedService.ApplyCert',
-    index=3,
-    containing_service=None,
-    input_type=_APPLYCERTREQUEST,
-    output_type=_APPLYCERTRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='EncryptDisk',
-    full_name='iamanager.v2.IAMProtectedService.EncryptDisk',
-    index=4,
-    containing_service=None,
-    input_type=_ENCRYPTDISKREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='FinishProvisioning',
-    full_name='iamanager.v2.IAMProtectedService.FinishProvisioning',
-    index=5,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SetUsers',
-    full_name='iamanager.v2.IAMProtectedService.SetUsers',
-    index=6,
-    containing_service=None,
-    input_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='RegisterService',
-    full_name='iamanager.v2.IAMProtectedService.RegisterService',
-    index=7,
-    containing_service=None,
-    input_type=_REGISTERSERVICEREQUEST,
-    output_type=_REGISTERSERVICERESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='UnregisterService',
-    full_name='iamanager.v2.IAMProtectedService.UnregisterService',
-    index=8,
-    containing_service=None,
-    input_type=_UNREGISTERSERVICEREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_IAMPROTECTEDSERVICE)
-
-DESCRIPTOR.services_by_name['IAMProtectedService'] = _IAMPROTECTEDSERVICE
-
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v2/iamanagerprotected.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='iamanager/v2/iamanagerprotected.proto',
+  package='iamanager.v2',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n%iamanager/v2/iamanagerprotected.proto\x12\x0ciamanager.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v2/iamanagercommon.proto\"\x1c\n\x0c\x43learRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\"1\n\x0fSetOwnerRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"2\n\x10\x43reateKeyRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x11\x43reateKeyResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\".\n\x10\x41pplyCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\"3\n\x11\x41pplyCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\"\xc7\x01\n\x16RegisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12J\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x35.iamanager.v2.RegisterServiceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v2.Permissions:\x02\x38\x01\")\n\x17RegisterServiceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\".\n\x18UnregisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\"&\n\x12\x45ncryptDiskRequest\x12\x10\n\x08password\x18\x01 \x01(\t2\xc0\x05\n\x13IAMProtectedService\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v2.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v2.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tCreateKey\x12\x1e.iamanager.v2.CreateKeyRequest\x1a\x1f.iamanager.v2.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v2.ApplyCertRequest\x1a\x1f.iamanager.v2.ApplyCertResponse\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v2.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x39\n\x08SetUsers\x12\x13.iamanager.v2.Users\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x0fRegisterService\x12$.iamanager.v2.RegisterServiceRequest\x1a%.iamanager.v2.RegisterServiceResponse\"\x00\x12U\n\x11UnregisterService\x12&.iamanager.v2.UnregisterServiceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v2_dot_iamanagercommon__pb2.DESCRIPTOR,])
+
+
+
+
+_CLEARREQUEST = _descriptor.Descriptor(
+  name='ClearRequest',
+  full_name='iamanager.v2.ClearRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.ClearRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=120,
+  serialized_end=148,
+)
+
+
+_SETOWNERREQUEST = _descriptor.Descriptor(
+  name='SetOwnerRequest',
+  full_name='iamanager.v2.SetOwnerRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.SetOwnerRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.v2.SetOwnerRequest.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=150,
+  serialized_end=199,
+)
+
+
+_CREATEKEYREQUEST = _descriptor.Descriptor(
+  name='CreateKeyRequest',
+  full_name='iamanager.v2.CreateKeyRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.CreateKeyRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.v2.CreateKeyRequest.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=201,
+  serialized_end=251,
+)
+
+
+_CREATEKEYRESPONSE = _descriptor.Descriptor(
+  name='CreateKeyResponse',
+  full_name='iamanager.v2.CreateKeyResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.CreateKeyResponse.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='csr', full_name='iamanager.v2.CreateKeyResponse.csr', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=253,
+  serialized_end=299,
+)
+
+
+_APPLYCERTREQUEST = _descriptor.Descriptor(
+  name='ApplyCertRequest',
+  full_name='iamanager.v2.ApplyCertRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.ApplyCertRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert', full_name='iamanager.v2.ApplyCertRequest.cert', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=301,
+  serialized_end=347,
+)
+
+
+_APPLYCERTRESPONSE = _descriptor.Descriptor(
+  name='ApplyCertResponse',
+  full_name='iamanager.v2.ApplyCertResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.ApplyCertResponse.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.v2.ApplyCertResponse.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=349,
+  serialized_end=400,
+)
+
+
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY = _descriptor.Descriptor(
+  name='PermissionsEntry',
+  full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry.value', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=525,
+  serialized_end=602,
+)
+
+_REGISTERSERVICEREQUEST = _descriptor.Descriptor(
+  name='RegisterServiceRequest',
+  full_name='iamanager.v2.RegisterServiceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='service_id', full_name='iamanager.v2.RegisterServiceRequest.service_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='iamanager.v2.RegisterServiceRequest.permissions', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_REGISTERSERVICEREQUEST_PERMISSIONSENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=403,
+  serialized_end=602,
+)
+
+
+_REGISTERSERVICERESPONSE = _descriptor.Descriptor(
+  name='RegisterServiceResponse',
+  full_name='iamanager.v2.RegisterServiceResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='secret', full_name='iamanager.v2.RegisterServiceResponse.secret', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=604,
+  serialized_end=645,
+)
+
+
+_UNREGISTERSERVICEREQUEST = _descriptor.Descriptor(
+  name='UnregisterServiceRequest',
+  full_name='iamanager.v2.UnregisterServiceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='service_id', full_name='iamanager.v2.UnregisterServiceRequest.service_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=647,
+  serialized_end=693,
+)
+
+
+_ENCRYPTDISKREQUEST = _descriptor.Descriptor(
+  name='EncryptDiskRequest',
+  full_name='iamanager.v2.EncryptDiskRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.v2.EncryptDiskRequest.password', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=695,
+  serialized_end=733,
+)
+
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.fields_by_name['value'].message_type = iamanager_dot_v2_dot_iamanagercommon__pb2._PERMISSIONS
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.containing_type = _REGISTERSERVICEREQUEST
+_REGISTERSERVICEREQUEST.fields_by_name['permissions'].message_type = _REGISTERSERVICEREQUEST_PERMISSIONSENTRY
+DESCRIPTOR.message_types_by_name['ClearRequest'] = _CLEARREQUEST
+DESCRIPTOR.message_types_by_name['SetOwnerRequest'] = _SETOWNERREQUEST
+DESCRIPTOR.message_types_by_name['CreateKeyRequest'] = _CREATEKEYREQUEST
+DESCRIPTOR.message_types_by_name['CreateKeyResponse'] = _CREATEKEYRESPONSE
+DESCRIPTOR.message_types_by_name['ApplyCertRequest'] = _APPLYCERTREQUEST
+DESCRIPTOR.message_types_by_name['ApplyCertResponse'] = _APPLYCERTRESPONSE
+DESCRIPTOR.message_types_by_name['RegisterServiceRequest'] = _REGISTERSERVICEREQUEST
+DESCRIPTOR.message_types_by_name['RegisterServiceResponse'] = _REGISTERSERVICERESPONSE
+DESCRIPTOR.message_types_by_name['UnregisterServiceRequest'] = _UNREGISTERSERVICEREQUEST
+DESCRIPTOR.message_types_by_name['EncryptDiskRequest'] = _ENCRYPTDISKREQUEST
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CLEARREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.ClearRequest)
+  })
+_sym_db.RegisterMessage(ClearRequest)
+
+SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SETOWNERREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.SetOwnerRequest)
+  })
+_sym_db.RegisterMessage(SetOwnerRequest)
+
+CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.CreateKeyRequest)
+  })
+_sym_db.RegisterMessage(CreateKeyRequest)
+
+CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYRESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.CreateKeyResponse)
+  })
+_sym_db.RegisterMessage(CreateKeyResponse)
+
+ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.ApplyCertRequest)
+  })
+_sym_db.RegisterMessage(ApplyCertRequest)
+
+ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTRESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.ApplyCertResponse)
+  })
+_sym_db.RegisterMessage(ApplyCertResponse)
+
+RegisterServiceRequest = _reflection.GeneratedProtocolMessageType('RegisterServiceRequest', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _REGISTERSERVICEREQUEST_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceRequest.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _REGISTERSERVICEREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceRequest)
+  })
+_sym_db.RegisterMessage(RegisterServiceRequest)
+_sym_db.RegisterMessage(RegisterServiceRequest.PermissionsEntry)
+
+RegisterServiceResponse = _reflection.GeneratedProtocolMessageType('RegisterServiceResponse', (_message.Message,), {
+  'DESCRIPTOR' : _REGISTERSERVICERESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceResponse)
+  })
+_sym_db.RegisterMessage(RegisterServiceResponse)
+
+UnregisterServiceRequest = _reflection.GeneratedProtocolMessageType('UnregisterServiceRequest', (_message.Message,), {
+  'DESCRIPTOR' : _UNREGISTERSERVICEREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.UnregisterServiceRequest)
+  })
+_sym_db.RegisterMessage(UnregisterServiceRequest)
+
+EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.EncryptDiskRequest)
+  })
+_sym_db.RegisterMessage(EncryptDiskRequest)
+
+
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY._options = None
+
+_IAMPROTECTEDSERVICE = _descriptor.ServiceDescriptor(
+  name='IAMProtectedService',
+  full_name='iamanager.v2.IAMProtectedService',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=736,
+  serialized_end=1440,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='SetOwner',
+    full_name='iamanager.v2.IAMProtectedService.SetOwner',
+    index=0,
+    containing_service=None,
+    input_type=_SETOWNERREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='Clear',
+    full_name='iamanager.v2.IAMProtectedService.Clear',
+    index=1,
+    containing_service=None,
+    input_type=_CLEARREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='CreateKey',
+    full_name='iamanager.v2.IAMProtectedService.CreateKey',
+    index=2,
+    containing_service=None,
+    input_type=_CREATEKEYREQUEST,
+    output_type=_CREATEKEYRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='ApplyCert',
+    full_name='iamanager.v2.IAMProtectedService.ApplyCert',
+    index=3,
+    containing_service=None,
+    input_type=_APPLYCERTREQUEST,
+    output_type=_APPLYCERTRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='EncryptDisk',
+    full_name='iamanager.v2.IAMProtectedService.EncryptDisk',
+    index=4,
+    containing_service=None,
+    input_type=_ENCRYPTDISKREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='FinishProvisioning',
+    full_name='iamanager.v2.IAMProtectedService.FinishProvisioning',
+    index=5,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetUsers',
+    full_name='iamanager.v2.IAMProtectedService.SetUsers',
+    index=6,
+    containing_service=None,
+    input_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='RegisterService',
+    full_name='iamanager.v2.IAMProtectedService.RegisterService',
+    index=7,
+    containing_service=None,
+    input_type=_REGISTERSERVICEREQUEST,
+    output_type=_REGISTERSERVICERESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='UnregisterService',
+    full_name='iamanager.v2.IAMProtectedService.UnregisterService',
+    index=8,
+    containing_service=None,
+    input_type=_UNREGISTERSERVICEREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_IAMPROTECTEDSERVICE)
+
+DESCRIPTOR.services_by_name['IAMProtectedService'] = _IAMPROTECTEDSERVICE
+
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,332 +1,332 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2
-from aos_prov.communication.unit.v2.generated import iamanagerprotected_pb2 as iamanager_dot_v2_dot_iamanagerprotected__pb2
-
-
-class IAMProtectedServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.SetOwner = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/SetOwner',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.Clear = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/Clear',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.CreateKey = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/CreateKey',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
-                )
-        self.ApplyCert = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/ApplyCert',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
-                )
-        self.EncryptDisk = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/EncryptDisk',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.FinishProvisioning = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/FinishProvisioning',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.SetUsers = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/SetUsers',
-                request_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.RegisterService = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/RegisterService',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
-                )
-        self.UnregisterService = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/UnregisterService',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAMProtectedServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def SetOwner(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Clear(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def CreateKey(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ApplyCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def EncryptDisk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def FinishProvisioning(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetUsers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def RegisterService(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def UnregisterService(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMProtectedServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'SetOwner': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetOwner,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'Clear': grpc.unary_unary_rpc_method_handler(
-                    servicer.Clear,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'CreateKey': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateKey,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.SerializeToString,
-            ),
-            'ApplyCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.ApplyCert,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.SerializeToString,
-            ),
-            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
-                    servicer.EncryptDisk,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
-                    servicer.FinishProvisioning,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'SetUsers': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetUsers,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'RegisterService': grpc.unary_unary_rpc_method_handler(
-                    servicer.RegisterService,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.SerializeToString,
-            ),
-            'UnregisterService': grpc.unary_unary_rpc_method_handler(
-                    servicer.UnregisterService,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v2.IAMProtectedService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMProtectedService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def SetOwner(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/SetOwner',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Clear(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/Clear',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def CreateKey(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/CreateKey',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ApplyCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/ApplyCert',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def EncryptDisk(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/EncryptDisk',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def FinishProvisioning(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/FinishProvisioning',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetUsers(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/SetUsers',
-            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def RegisterService(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/RegisterService',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def UnregisterService(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/UnregisterService',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2
+from aos_prov.communication.unit.v2.generated import iamanagerprotected_pb2 as iamanager_dot_v2_dot_iamanagerprotected__pb2
+
+
+class IAMProtectedServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.SetOwner = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/SetOwner',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.Clear = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/Clear',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.CreateKey = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/CreateKey',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
+                )
+        self.ApplyCert = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/ApplyCert',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
+                )
+        self.EncryptDisk = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/EncryptDisk',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.FinishProvisioning = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/FinishProvisioning',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.SetUsers = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/SetUsers',
+                request_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.RegisterService = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/RegisterService',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
+                )
+        self.UnregisterService = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/UnregisterService',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAMProtectedServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def SetOwner(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Clear(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def CreateKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ApplyCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def EncryptDisk(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def FinishProvisioning(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetUsers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def RegisterService(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UnregisterService(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMProtectedServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'SetOwner': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetOwner,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'Clear': grpc.unary_unary_rpc_method_handler(
+                    servicer.Clear,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'CreateKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateKey,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.SerializeToString,
+            ),
+            'ApplyCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.ApplyCert,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.SerializeToString,
+            ),
+            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
+                    servicer.EncryptDisk,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
+                    servicer.FinishProvisioning,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'SetUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetUsers,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'RegisterService': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterService,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.SerializeToString,
+            ),
+            'UnregisterService': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnregisterService,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v2.IAMProtectedService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMProtectedService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def SetOwner(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/SetOwner',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Clear(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/Clear',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/CreateKey',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ApplyCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/ApplyCert',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def EncryptDisk(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/EncryptDisk',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def FinishProvisioning(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/FinishProvisioning',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/SetUsers',
+            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RegisterService(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/RegisterService',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UnregisterService(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/UnregisterService',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py

 * *Ordering differences only*

```diff
@@ -1,449 +1,449 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v2/iamanagerpublic.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v2/iamanagerpublic.proto',
-  package='iamanager.v2',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\"iamanager/v2/iamanagerpublic.proto\x12\x0ciamanager.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v2/iamanagercommon.proto\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"Y\n\x13PermissionsResponse\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v2.Permissions\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\x32\x87\x04\n\x10IAMPublicService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v2.SystemInfo\"\x00\x12\x41\n\x0cGetCertTypes\x12\x16.google.protobuf.Empty\x1a\x17.iamanager.v2.CertTypes\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v2.GetCertRequest\x1a\x1d.iamanager.v2.GetCertResponse\"\x00\x12W\n\x0eGetPermissions\x12 .iamanager.v2.PermissionsRequest\x1a!.iamanager.v2.PermissionsResponse\"\x00\x12\x39\n\x08GetUsers\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v2.Users\"\x00\x12H\n\x15SubscribeUsersChanged\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v2.Users\"\x00\x30\x01\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v2.APIVersion\"\x00\x62\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v2_dot_iamanagercommon__pb2.DESCRIPTOR,])
-
-
-
-
-_SYSTEMINFO = _descriptor.Descriptor(
-  name='SystemInfo',
-  full_name='iamanager.v2.SystemInfo',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='system_id', full_name='iamanager.v2.SystemInfo.system_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='board_model', full_name='iamanager.v2.SystemInfo.board_model', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=117,
-  serialized_end=169,
-)
-
-
-_CERTTYPES = _descriptor.Descriptor(
-  name='CertTypes',
-  full_name='iamanager.v2.CertTypes',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='types', full_name='iamanager.v2.CertTypes.types', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=171,
-  serialized_end=197,
-)
-
-
-_GETCERTREQUEST = _descriptor.Descriptor(
-  name='GetCertRequest',
-  full_name='iamanager.v2.GetCertRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.GetCertRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='issuer', full_name='iamanager.v2.GetCertRequest.issuer', index=1,
-      number=2, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='serial', full_name='iamanager.v2.GetCertRequest.serial', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=199,
-  serialized_end=261,
-)
-
-
-_GETCERTRESPONSE = _descriptor.Descriptor(
-  name='GetCertResponse',
-  full_name='iamanager.v2.GetCertResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.GetCertResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert_url', full_name='iamanager.v2.GetCertResponse.cert_url', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='key_url', full_name='iamanager.v2.GetCertResponse.key_url', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=263,
-  serialized_end=329,
-)
-
-
-_PERMISSIONSREQUEST = _descriptor.Descriptor(
-  name='PermissionsRequest',
-  full_name='iamanager.v2.PermissionsRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='secret', full_name='iamanager.v2.PermissionsRequest.secret', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='functional_server_id', full_name='iamanager.v2.PermissionsRequest.functional_server_id', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=331,
-  serialized_end=397,
-)
-
-
-_PERMISSIONSRESPONSE = _descriptor.Descriptor(
-  name='PermissionsResponse',
-  full_name='iamanager.v2.PermissionsResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v2.PermissionsResponse.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v2.PermissionsResponse.permissions', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=399,
-  serialized_end=488,
-)
-
-
-_APIVERSION = _descriptor.Descriptor(
-  name='APIVersion',
-  full_name='iamanager.v2.APIVersion',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='version', full_name='iamanager.v2.APIVersion.version', index=0,
-      number=1, type=4, cpp_type=4, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=490,
-  serialized_end=519,
-)
-
-_PERMISSIONSRESPONSE.fields_by_name['permissions'].message_type = iamanager_dot_v2_dot_iamanagercommon__pb2._PERMISSIONS
-DESCRIPTOR.message_types_by_name['SystemInfo'] = _SYSTEMINFO
-DESCRIPTOR.message_types_by_name['CertTypes'] = _CERTTYPES
-DESCRIPTOR.message_types_by_name['GetCertRequest'] = _GETCERTREQUEST
-DESCRIPTOR.message_types_by_name['GetCertResponse'] = _GETCERTRESPONSE
-DESCRIPTOR.message_types_by_name['PermissionsRequest'] = _PERMISSIONSREQUEST
-DESCRIPTOR.message_types_by_name['PermissionsResponse'] = _PERMISSIONSRESPONSE
-DESCRIPTOR.message_types_by_name['APIVersion'] = _APIVERSION
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
-  'DESCRIPTOR' : _SYSTEMINFO,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.SystemInfo)
-  })
-_sym_db.RegisterMessage(SystemInfo)
-
-CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
-  'DESCRIPTOR' : _CERTTYPES,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.CertTypes)
-  })
-_sym_db.RegisterMessage(CertTypes)
-
-GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.GetCertRequest)
-  })
-_sym_db.RegisterMessage(GetCertRequest)
-
-GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTRESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.GetCertResponse)
-  })
-_sym_db.RegisterMessage(GetCertResponse)
-
-PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.PermissionsRequest)
-  })
-_sym_db.RegisterMessage(PermissionsRequest)
-
-PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.PermissionsResponse)
-  })
-_sym_db.RegisterMessage(PermissionsResponse)
-
-APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
-  'DESCRIPTOR' : _APIVERSION,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.APIVersion)
-  })
-_sym_db.RegisterMessage(APIVersion)
-
-
-
-_IAMPUBLICSERVICE = _descriptor.ServiceDescriptor(
-  name='IAMPublicService',
-  full_name='iamanager.v2.IAMPublicService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=522,
-  serialized_end=1041,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='GetSystemInfo',
-    full_name='iamanager.v2.IAMPublicService.GetSystemInfo',
-    index=0,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_SYSTEMINFO,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetCertTypes',
-    full_name='iamanager.v2.IAMPublicService.GetCertTypes',
-    index=1,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_CERTTYPES,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetCert',
-    full_name='iamanager.v2.IAMPublicService.GetCert',
-    index=2,
-    containing_service=None,
-    input_type=_GETCERTREQUEST,
-    output_type=_GETCERTRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetPermissions',
-    full_name='iamanager.v2.IAMPublicService.GetPermissions',
-    index=3,
-    containing_service=None,
-    input_type=_PERMISSIONSREQUEST,
-    output_type=_PERMISSIONSRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetUsers',
-    full_name='iamanager.v2.IAMPublicService.GetUsers',
-    index=4,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SubscribeUsersChanged',
-    full_name='iamanager.v2.IAMPublicService.SubscribeUsersChanged',
-    index=5,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetAPIVersion',
-    full_name='iamanager.v2.IAMPublicService.GetAPIVersion',
-    index=6,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_APIVERSION,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_IAMPUBLICSERVICE)
-
-DESCRIPTOR.services_by_name['IAMPublicService'] = _IAMPUBLICSERVICE
-
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v2/iamanagerpublic.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='iamanager/v2/iamanagerpublic.proto',
+  package='iamanager.v2',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n\"iamanager/v2/iamanagerpublic.proto\x12\x0ciamanager.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v2/iamanagercommon.proto\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"Y\n\x13PermissionsResponse\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v2.Permissions\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\x32\x87\x04\n\x10IAMPublicService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v2.SystemInfo\"\x00\x12\x41\n\x0cGetCertTypes\x12\x16.google.protobuf.Empty\x1a\x17.iamanager.v2.CertTypes\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v2.GetCertRequest\x1a\x1d.iamanager.v2.GetCertResponse\"\x00\x12W\n\x0eGetPermissions\x12 .iamanager.v2.PermissionsRequest\x1a!.iamanager.v2.PermissionsResponse\"\x00\x12\x39\n\x08GetUsers\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v2.Users\"\x00\x12H\n\x15SubscribeUsersChanged\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v2.Users\"\x00\x30\x01\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v2.APIVersion\"\x00\x62\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v2_dot_iamanagercommon__pb2.DESCRIPTOR,])
+
+
+
+
+_SYSTEMINFO = _descriptor.Descriptor(
+  name='SystemInfo',
+  full_name='iamanager.v2.SystemInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='system_id', full_name='iamanager.v2.SystemInfo.system_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='board_model', full_name='iamanager.v2.SystemInfo.board_model', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=117,
+  serialized_end=169,
+)
+
+
+_CERTTYPES = _descriptor.Descriptor(
+  name='CertTypes',
+  full_name='iamanager.v2.CertTypes',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='types', full_name='iamanager.v2.CertTypes.types', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=171,
+  serialized_end=197,
+)
+
+
+_GETCERTREQUEST = _descriptor.Descriptor(
+  name='GetCertRequest',
+  full_name='iamanager.v2.GetCertRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.GetCertRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='issuer', full_name='iamanager.v2.GetCertRequest.issuer', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='serial', full_name='iamanager.v2.GetCertRequest.serial', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=199,
+  serialized_end=261,
+)
+
+
+_GETCERTRESPONSE = _descriptor.Descriptor(
+  name='GetCertResponse',
+  full_name='iamanager.v2.GetCertResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.GetCertResponse.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.v2.GetCertResponse.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='key_url', full_name='iamanager.v2.GetCertResponse.key_url', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=263,
+  serialized_end=329,
+)
+
+
+_PERMISSIONSREQUEST = _descriptor.Descriptor(
+  name='PermissionsRequest',
+  full_name='iamanager.v2.PermissionsRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='secret', full_name='iamanager.v2.PermissionsRequest.secret', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='functional_server_id', full_name='iamanager.v2.PermissionsRequest.functional_server_id', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=331,
+  serialized_end=397,
+)
+
+
+_PERMISSIONSRESPONSE = _descriptor.Descriptor(
+  name='PermissionsResponse',
+  full_name='iamanager.v2.PermissionsResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='service_id', full_name='iamanager.v2.PermissionsResponse.service_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='iamanager.v2.PermissionsResponse.permissions', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=399,
+  serialized_end=488,
+)
+
+
+_APIVERSION = _descriptor.Descriptor(
+  name='APIVersion',
+  full_name='iamanager.v2.APIVersion',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='version', full_name='iamanager.v2.APIVersion.version', index=0,
+      number=1, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=490,
+  serialized_end=519,
+)
+
+_PERMISSIONSRESPONSE.fields_by_name['permissions'].message_type = iamanager_dot_v2_dot_iamanagercommon__pb2._PERMISSIONS
+DESCRIPTOR.message_types_by_name['SystemInfo'] = _SYSTEMINFO
+DESCRIPTOR.message_types_by_name['CertTypes'] = _CERTTYPES
+DESCRIPTOR.message_types_by_name['GetCertRequest'] = _GETCERTREQUEST
+DESCRIPTOR.message_types_by_name['GetCertResponse'] = _GETCERTRESPONSE
+DESCRIPTOR.message_types_by_name['PermissionsRequest'] = _PERMISSIONSREQUEST
+DESCRIPTOR.message_types_by_name['PermissionsResponse'] = _PERMISSIONSRESPONSE
+DESCRIPTOR.message_types_by_name['APIVersion'] = _APIVERSION
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMINFO,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.SystemInfo)
+  })
+_sym_db.RegisterMessage(SystemInfo)
+
+CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
+  'DESCRIPTOR' : _CERTTYPES,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.CertTypes)
+  })
+_sym_db.RegisterMessage(CertTypes)
+
+GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.GetCertRequest)
+  })
+_sym_db.RegisterMessage(GetCertRequest)
+
+GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTRESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.GetCertResponse)
+  })
+_sym_db.RegisterMessage(GetCertResponse)
+
+PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.PermissionsRequest)
+  })
+_sym_db.RegisterMessage(PermissionsRequest)
+
+PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.PermissionsResponse)
+  })
+_sym_db.RegisterMessage(PermissionsResponse)
+
+APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
+  'DESCRIPTOR' : _APIVERSION,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.APIVersion)
+  })
+_sym_db.RegisterMessage(APIVersion)
+
+
+
+_IAMPUBLICSERVICE = _descriptor.ServiceDescriptor(
+  name='IAMPublicService',
+  full_name='iamanager.v2.IAMPublicService',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=522,
+  serialized_end=1041,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='GetSystemInfo',
+    full_name='iamanager.v2.IAMPublicService.GetSystemInfo',
+    index=0,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_SYSTEMINFO,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetCertTypes',
+    full_name='iamanager.v2.IAMPublicService.GetCertTypes',
+    index=1,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_CERTTYPES,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetCert',
+    full_name='iamanager.v2.IAMPublicService.GetCert',
+    index=2,
+    containing_service=None,
+    input_type=_GETCERTREQUEST,
+    output_type=_GETCERTRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetPermissions',
+    full_name='iamanager.v2.IAMPublicService.GetPermissions',
+    index=3,
+    containing_service=None,
+    input_type=_PERMISSIONSREQUEST,
+    output_type=_PERMISSIONSRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetUsers',
+    full_name='iamanager.v2.IAMPublicService.GetUsers',
+    index=4,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SubscribeUsersChanged',
+    full_name='iamanager.v2.IAMPublicService.SubscribeUsersChanged',
+    index=5,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetAPIVersion',
+    full_name='iamanager.v2.IAMPublicService.GetAPIVersion',
+    index=6,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_APIVERSION,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_IAMPUBLICSERVICE)
+
+DESCRIPTOR.services_by_name['IAMPublicService'] = _IAMPUBLICSERVICE
+
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,266 +1,266 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2
-from aos_prov.communication.unit.v2.generated import iamanagerpublic_pb2 as iamanager_dot_v2_dot_iamanagerpublic__pb2
-
-
-class IAMPublicServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetSystemInfo = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetSystemInfo',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.FromString,
-                )
-        self.GetCertTypes = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetCertTypes',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.FromString,
-                )
-        self.GetCert = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetCert',
-                request_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.FromString,
-                )
-        self.GetPermissions = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetPermissions',
-                request_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
-                )
-        self.GetUsers = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetUsers',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-                )
-        self.SubscribeUsersChanged = channel.unary_stream(
-                '/iamanager.v2.IAMPublicService/SubscribeUsersChanged',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-                )
-        self.GetAPIVersion = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetAPIVersion',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.FromString,
-                )
-
-
-class IAMPublicServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetSystemInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCertTypes(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetPermissions(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetUsers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SubscribeUsersChanged(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetAPIVersion(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSystemInfo,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.SerializeToString,
-            ),
-            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCertTypes,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.SerializeToString,
-            ),
-            'GetCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCert,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.SerializeToString,
-            ),
-            'GetPermissions': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetPermissions,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.SerializeToString,
-            ),
-            'GetUsers': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetUsers,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
-            ),
-            'SubscribeUsersChanged': grpc.unary_stream_rpc_method_handler(
-                    servicer.SubscribeUsersChanged,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
-            ),
-            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAPIVersion,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v2.IAMPublicService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetSystemInfo(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetSystemInfo',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCertTypes(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetCertTypes',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetCert',
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetPermissions(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetPermissions',
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetUsers(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetUsers',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SubscribeUsersChanged(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iamanager.v2.IAMPublicService/SubscribeUsersChanged',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetAPIVersion(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetAPIVersion',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v2.generated import iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2
+from aos_prov.communication.unit.v2.generated import iamanagerpublic_pb2 as iamanager_dot_v2_dot_iamanagerpublic__pb2
+
+
+class IAMPublicServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetSystemInfo = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetSystemInfo',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.FromString,
+                )
+        self.GetCertTypes = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetCertTypes',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.FromString,
+                )
+        self.GetCert = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetCert',
+                request_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.FromString,
+                )
+        self.GetPermissions = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetPermissions',
+                request_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
+                )
+        self.GetUsers = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetUsers',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+                )
+        self.SubscribeUsersChanged = channel.unary_stream(
+                '/iamanager.v2.IAMPublicService/SubscribeUsersChanged',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+                )
+        self.GetAPIVersion = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetAPIVersion',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.FromString,
+                )
+
+
+class IAMPublicServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetSystemInfo(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCertTypes(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetPermissions(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetUsers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubscribeUsersChanged(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetAPIVersion(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSystemInfo,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.SerializeToString,
+            ),
+            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCertTypes,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.SerializeToString,
+            ),
+            'GetCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCert,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.SerializeToString,
+            ),
+            'GetPermissions': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPermissions,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.SerializeToString,
+            ),
+            'GetUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetUsers,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
+            ),
+            'SubscribeUsersChanged': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeUsersChanged,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
+            ),
+            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAPIVersion,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v2.IAMPublicService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetSystemInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetSystemInfo',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCertTypes(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetCertTypes',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetCert',
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetPermissions(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetPermissions',
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetUsers',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubscribeUsersChanged(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/iamanager.v2.IAMPublicService/SubscribeUsersChanged',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetAPIVersion(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetAPIVersion',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/communication/unit/v4/unit_communication_v4.py

```diff
@@ -1,244 +1,221 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-import time
-from contextlib import contextmanager
-
-import grpc
-from colorama import Fore, Style
-from google.protobuf import empty_pb2
-
-from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iam_manager
-from aos_prov.communication.unit.v4.generated import iamanager_pb2_grpc as iam_manager_grpc
-from aos_prov.utils.errors import BoardError, GrpcUnimplemented
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-UNIT_DEFAULT_PORT = 8089
-
-
-class UnitCommunicationV4:
-    def __init__(self, address: str = 'localhost:8089'):
-        self._need_set_users = False
-
-        if address is None:
-            address = 'localhost:8089'
-        parts = address.split(':')
-        if len(parts) == 2:
-            try:
-                port = int(parts[1])
-                if not 1 <= port <= 65535:
-                    raise BoardError("Unit port is invalid")
-            except ValueError:
-                raise BoardError("Unit port is invalid")
-        else:
-            address = address + ':' + str(UNIT_DEFAULT_PORT)
-        self.__unit_address = address
-        print(f"Will search unit on address: {Fore.GREEN}{self.__unit_address}{Style.RESET_ALL}")
-
-    @property
-    def need_set_users(self):
-        return self._need_set_users
-
-    @need_set_users.setter
-    def need_set_users(self, value):
-        self._need_set_users = value
-
-    @contextmanager
-    def unit_certificate_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMCertificateServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):
-                        print(str(state))
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as e:
-            print(e)
-            if catch_inactive and \
-                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
-                return
-            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
-                return
-            error_text = (f"{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}"
-                          f"{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}")
-            raise BoardError(error_text)
-
-    @contextmanager
-    def unit_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):
-                        print(str(state))
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as e:
-            print(e)
-            if catch_inactive and \
-                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
-                return
-            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
-                return
-            error_text = (f"{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}"
-                          f"{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}")
-            raise BoardError(error_text)
-
-    @contextmanager
-    def unit_identify_stub(self):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMPublicIdentityServiceStub(channel)
-                yield stub
-
-        except grpc.RpcError as e:
-            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
-                error_text = (f'{Fore.YELLOW}FAILED! Protocol V4 is not supported: {Style.RESET_ALL}'
-                              f'{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}')
-                raise GrpcUnimplemented(error_text)
-            else:
-                error_text = (f'{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}'
-                              f'{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}')
-                raise BoardError(error_text)
-
-    @contextmanager
-    def unit_provisioning_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMProvisioningServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):
-                        print(str(state))
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as e:
-            print(e)
-            if catch_inactive and \
-                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
-                return
-            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
-                return
-            error_text = (f"{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}"
-                          f"{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}")
-            raise BoardError(error_text)
-
-    @contextmanager
-    def unit_public_stub(self):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
-                yield stub
-
-        except grpc.RpcError as e:
-            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
-                error_text = (f'{Fore.YELLOW}FAILED! Protocol V4 is not supported: {Style.RESET_ALL}'
-                              f'{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}')
-                raise GrpcUnimplemented(error_text)
-            else:
-                error_text = (f'{Fore.RED}FAILED! Error occurred: {Style.RESET_ALL}'
-                              f'{Fore.RED}{e.code()}: {e.details()}{Style.RESET_ALL}')
-                raise BoardError(error_text)
-
-    def get_protocol_version(self) -> int:
-        with self.unit_public_stub() as stub:
-            print('Getting protocol version...')
-            response = stub.GetAPIVersion(empty_pb2.Empty())
-            print(f'Unit responded with version: {response.version}')
-            return int(response.version)
-
-    def get_system_info(self) -> (str, str):
-        with self.unit_identify_stub() as stub:
-            print('Getting System Info...')
-            response = stub.GetSystemInfo(empty_pb2.Empty())
-            print('System ID: ' + response.system_id)
-            print('Model name: ' + response.board_model)
-            return response.system_id, response.board_model
-
-    def clear(self, certificate_type: str, node_id: str) -> None:
-        with self.unit_provisioning_stub() as stub:
-            print('Clear certificate: ' + certificate_type + ' Node ID: ' + node_id)
-            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type, node_id=node_id))
-            return response
-
-    def set_cert_owner(self, certificate_type: str, password: str, node_id: str) -> None:
-        with self.unit_provisioning_stub() as stub:
-            print('Set owner: ' + certificate_type)
-            response = stub.SetOwner(
-                iam_manager.SetOwnerRequest(type=certificate_type, password=password, node_id=node_id),
-            )
-            return response
-
-    def get_all_node_ids(self) -> [str]:
-        with self.unit_provisioning_stub() as stub:
-            print('Getting Node IDs')
-            response = stub.GetAllNodeIDs(empty_pb2.Empty())
-            print('Node IDs: ' + str(response.ids))
-            return response.ids
-
-    def get_cert_types(self, node_id: str) -> [str]:
-        with self.unit_provisioning_stub() as stub:
-            print('Getting certificate types to renew')
-            response = stub.GetCertTypes(iam_manager.GetCertTypesRequest(node_id=node_id))
-            print('Will be renewed: ' + str(response.types))
-            return response.types
-
-    def create_keys(self, cert_type: str, password: str, node_id: str) -> UnitCertificate:
-        with self.unit_certificate_stub() as stub:
-            print('Generating key type: ' + cert_type + ' Node ID: ' + node_id)
-            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password, node_id=node_id))
-            uc = UnitCertificate()
-            uc.cert_type = response.type
-            uc.node_id = response.node_id
-            uc.csr = response.csr
-            return uc
-
-    def apply_certificate(self, unit_cert: UnitCertificate):
-        with self.unit_certificate_stub() as stub:
-            node_id = ''
-            if unit_cert.node_id:
-                node_id = str(unit_cert.node_id)
-            print('Applying type: ' + unit_cert.cert_type + ' Node ID: ' + node_id)
-            stub.ApplyCert(iam_manager.ApplyCertRequest(
-                type=unit_cert.cert_type,
-                cert=unit_cert.certificate,
-                node_id=node_id,
-            ))
-
-    def encrypt_disk(self, password: str, node_id: str):
-        print('Starting disk encryption...')
-        try:
-            with self.unit_provisioning_stub(wait_for_close=True) as stub:
-                stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password, node_id=node_id))
-                print('Encryption process is finished.')
-        except BoardError as be:
-            print('Disk encryption returned error.')
-            print(be)
-
-    def finish_provisioning(self):
-        with self.unit_provisioning_stub(True) as stub:
-            print('Finishing provisioning')
-            stub.FinishProvisioning(empty_pb2.Empty())
-
-    def wait_for_connection(self):
-        try:
-            print('Sleep for 5 seconds...')
-            time.sleep(5)
-            print('Waiting for Unit reboot...')
-            grpc.channel_ready_future(grpc.insecure_channel(self.__unit_address)).result(timeout=300)
-            print('Unit is online')
-        except grpc.FutureTimeoutError:
-            raise BoardError('Board didnt went online')
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+from contextlib import contextmanager
+
+import grpc
+from google.protobuf import empty_pb2
+
+from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iam_manager
+from aos_prov.communication.unit.v4.generated import iamanager_pb2_grpc as iam_manager_grpc
+from aos_prov.utils.common import print_message, print_done, print_left, print_success
+from aos_prov.utils.errors import BoardError, GrpcUnimplemented
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+UNIT_DEFAULT_PORT = 8089
+
+
+class UnitCommunicationV4:
+    def __init__(self, address: str = 'localhost:8089'):
+        self._need_set_users = False
+
+        if address is None:
+            address = 'localhost:8089'
+        parts = address.split(':')
+        if len(parts) == 2:
+            try:
+                port = int(parts[1])
+                if not 1 <= port <= 65535:
+                    raise BoardError('Unit port is invalid')
+            except ValueError:
+                raise BoardError('Unit port is invalid')
+        else:
+            address = address + ':' + str(UNIT_DEFAULT_PORT)
+        self.__unit_address = address
+        print_message(f'Will search unit on address: [green]{self.__unit_address}')
+
+    @property
+    def need_set_users(self):
+        return self._need_set_users
+
+    @need_set_users.setter
+    def need_set_users(self, value):
+        self._need_set_users = value
+
+    @contextmanager
+    def unit_certificate_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMCertificateServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as e:
+            if catch_inactive and \
+                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
+                return
+            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
+                return
+            raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as e:
+            if catch_inactive and \
+                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
+                return
+            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
+                return
+            raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_identify_stub(self):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMPublicIdentityServiceStub(channel)
+                yield stub
+
+        except grpc.RpcError as e:
+            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
+                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e.code()}: {e.details()}')
+            else:
+                raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_provisioning_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMProvisioningServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as e:
+            if catch_inactive and \
+                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
+                return
+            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
+                return
+            raise BoardError(f"Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_public_stub(self):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
+                yield stub
+
+        except grpc.RpcError as e:
+            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
+                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e.code()}: {e.details()}')
+            else:
+                raise BoardError(f"Error occurred: \n{e.code()}: {e.details()}")
+
+    def get_protocol_version(self) -> int:
+        with self.unit_public_stub() as stub:
+            print_left('Getting protocol version...')
+            response = stub.GetAPIVersion(empty_pb2.Empty())
+            print_success(str(response.version))
+            return int(response.version)
+
+    def get_system_info(self) -> (str, str):
+        with self.unit_identify_stub() as stub:
+            print_left('Getting System Info...')
+            response = stub.GetSystemInfo(empty_pb2.Empty())
+            print_done()
+            print_left('System ID:')
+            print_success(response.system_id)
+            print_left('Model name:')
+            print_success(response.board_model)
+            return response.system_id, response.board_model
+
+    def clear(self, certificate_type: str, node_id: str) -> None:
+        with self.unit_provisioning_stub() as stub:
+            print_left(f'Clearing certificate: {certificate_type} on Node ID: {node_id}...')
+            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type, node_id=node_id))
+            print_done()
+            return response
+
+    def set_cert_owner(self, certificate_type: str, password: str, node_id: str) -> None:
+        with self.unit_provisioning_stub() as stub:
+            print_left(f'Setting owner for: {certificate_type} on Node ID: {node_id}...')
+            response = stub.SetOwner(
+                iam_manager.SetOwnerRequest(type=certificate_type, password=password, node_id=node_id),
+            )
+            print_done()
+            return response
+
+    def get_all_node_ids(self) -> [str]:
+        with self.unit_provisioning_stub() as stub:
+            print_left('Getting Node IDs...')
+            response = stub.GetAllNodeIDs(empty_pb2.Empty())
+            print_success(response.ids)
+            return response.ids
+
+    def get_cert_types(self, node_id: str) -> [str]:
+        with self.unit_provisioning_stub() as stub:
+            print_left(f'Getting certificate types to renew on node {node_id}...')
+            response = stub.GetCertTypes(iam_manager.GetCertTypesRequest(node_id=node_id))
+            print_success(response.types)
+            return response.types
+
+    def create_keys(self, cert_type: str, password: str, node_id: str) -> UnitCertificate:
+        with self.unit_certificate_stub() as stub:
+            print_left(f'Generating key type: {cert_type} on Node: {node_id}...')
+            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password, node_id=node_id))
+            uc = UnitCertificate()
+            uc.cert_type = response.type
+            uc.node_id = response.node_id
+            uc.csr = response.csr
+            print_done()
+            return uc
+
+    def apply_certificate(self, unit_cert: UnitCertificate):
+        with self.unit_certificate_stub() as stub:
+            node_id = ''
+            if unit_cert.node_id:
+                node_id = str(unit_cert.node_id)
+            print_left(f'Applying certificate type: {unit_cert.cert_type} Node ID: {node_id}...')
+            stub.ApplyCert(iam_manager.ApplyCertRequest(
+                type=unit_cert.cert_type,
+                cert=unit_cert.certificate,
+                node_id=node_id,
+            ))
+            print_done()
+
+    def encrypt_disk(self, password: str, node_id: str):
+        print_left(f'Starting disk encryption on node {node_id}...')
+        try:
+            with self.unit_provisioning_stub(wait_for_close=False) as stub:
+                stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password, node_id=node_id))
+                print_done()
+        except BoardError as be:
+            print_message(f'[red] Error.')
+            print_message(be)
+
+    def finish_provisioning(self):
+        with self.unit_provisioning_stub(True) as stub:
+            print_left('Finishing provisioning...')
+            stub.FinishProvisioning(empty_pb2.Empty())
+            print_done()
```

## aos_prov/communication/unit/v4/generated/iamanager_pb2.py

 * *Ordering differences only*

```diff
@@ -1,299 +1,299 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v4/iamanager.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ciamanager/v4/iamanager.proto\x12\x0ciamanager.v4\x1a\x1bgoogle/protobuf/empty.proto\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\"\x19\n\x06NodeID\x12\x0f\n\x07node_id\x18\x01 \x01(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1c\n\x08Subjects\x12\x10\n\x08subjects\x18\x01 \x03(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"I\n\rInstanceIdent\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x12\n\nsubject_id\x18\x02 \x01(\t\x12\x10\n\x08instance\x18\x03 \x01(\x04\"t\n\x13PermissionsResponse\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions\"\x16\n\x07NodesID\x12\x0b\n\x03ids\x18\x01 \x03(\t\"&\n\x13GetCertTypesRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\"B\n\x0fSetOwnerRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"-\n\x0c\x43learRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"7\n\x12\x45ncryptDiskRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"T\n\x10\x43reateKeyRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\"?\n\x11\x43reateKeyResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03\x63sr\x18\x03 \x01(\t\"?\n\x10\x41pplyCertRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x03 \x01(\t\"D\n\x11\x41pplyCertResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x03 \x01(\t\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v4.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe4\x01\n\x17RegisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12K\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x36.iamanager.v4.RegisterInstanceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions:\x02\x38\x01\"*\n\x18RegisterInstanceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\"J\n\x19UnregisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent2\xde\x01\n\x10IAMPublicService\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.APIVersion\"\x00\x12;\n\tGetNodeID\x12\x16.google.protobuf.Empty\x1a\x14.iamanager.v4.NodeID\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v4.GetCertRequest\x1a\x1d.iamanager.v4.GetCertResponse\"\x00\x32\xf0\x01\n\x18IAMPublicIdentityService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.SystemInfo\"\x00\x12?\n\x0bGetSubjects\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x12N\n\x18SubscribeSubjectsChanged\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x30\x01\x32v\n\x1bIAMPublicPermissionsService\x12W\n\x0eGetPermissions\x12 .iamanager.v4.PermissionsRequest\x1a!.iamanager.v4.PermissionsResponse\"\x00\x32\xbf\x03\n\x16IAMProvisioningService\x12@\n\rGetAllNodeIDs\x12\x16.google.protobuf.Empty\x1a\x15.iamanager.v4.NodesID\"\x00\x12L\n\x0cGetCertTypes\x12!.iamanager.v4.GetCertTypesRequest\x1a\x17.iamanager.v4.CertTypes\"\x00\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v4.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v4.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v4.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x32\xb7\x01\n\x15IAMCertificateService\x12N\n\tCreateKey\x12\x1e.iamanager.v4.CreateKeyRequest\x1a\x1f.iamanager.v4.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v4.ApplyCertRequest\x1a\x1f.iamanager.v4.ApplyCertResponse\"\x00\x32\xd5\x01\n\x15IAMPermissionsService\x12\x63\n\x10RegisterInstance\x12%.iamanager.v4.RegisterInstanceRequest\x1a&.iamanager.v4.RegisterInstanceResponse\"\x00\x12W\n\x12UnregisterInstance\x12\'.iamanager.v4.UnregisterInstanceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
-
-
-
-_APIVERSION = DESCRIPTOR.message_types_by_name['APIVersion']
-_NODEID = DESCRIPTOR.message_types_by_name['NodeID']
-_GETCERTREQUEST = DESCRIPTOR.message_types_by_name['GetCertRequest']
-_GETCERTRESPONSE = DESCRIPTOR.message_types_by_name['GetCertResponse']
-_SYSTEMINFO = DESCRIPTOR.message_types_by_name['SystemInfo']
-_SUBJECTS = DESCRIPTOR.message_types_by_name['Subjects']
-_PERMISSIONSREQUEST = DESCRIPTOR.message_types_by_name['PermissionsRequest']
-_INSTANCEIDENT = DESCRIPTOR.message_types_by_name['InstanceIdent']
-_PERMISSIONSRESPONSE = DESCRIPTOR.message_types_by_name['PermissionsResponse']
-_NODESID = DESCRIPTOR.message_types_by_name['NodesID']
-_GETCERTTYPESREQUEST = DESCRIPTOR.message_types_by_name['GetCertTypesRequest']
-_CERTTYPES = DESCRIPTOR.message_types_by_name['CertTypes']
-_SETOWNERREQUEST = DESCRIPTOR.message_types_by_name['SetOwnerRequest']
-_CLEARREQUEST = DESCRIPTOR.message_types_by_name['ClearRequest']
-_ENCRYPTDISKREQUEST = DESCRIPTOR.message_types_by_name['EncryptDiskRequest']
-_CREATEKEYREQUEST = DESCRIPTOR.message_types_by_name['CreateKeyRequest']
-_CREATEKEYRESPONSE = DESCRIPTOR.message_types_by_name['CreateKeyResponse']
-_APPLYCERTREQUEST = DESCRIPTOR.message_types_by_name['ApplyCertRequest']
-_APPLYCERTRESPONSE = DESCRIPTOR.message_types_by_name['ApplyCertResponse']
-_PERMISSIONS = DESCRIPTOR.message_types_by_name['Permissions']
-_PERMISSIONS_PERMISSIONSENTRY = _PERMISSIONS.nested_types_by_name['PermissionsEntry']
-_REGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['RegisterInstanceRequest']
-_REGISTERINSTANCEREQUEST_PERMISSIONSENTRY = _REGISTERINSTANCEREQUEST.nested_types_by_name['PermissionsEntry']
-_REGISTERINSTANCERESPONSE = DESCRIPTOR.message_types_by_name['RegisterInstanceResponse']
-_UNREGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['UnregisterInstanceRequest']
-APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
-  'DESCRIPTOR' : _APIVERSION,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.APIVersion)
-  })
-_sym_db.RegisterMessage(APIVersion)
-
-NodeID = _reflection.GeneratedProtocolMessageType('NodeID', (_message.Message,), {
-  'DESCRIPTOR' : _NODEID,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.NodeID)
-  })
-_sym_db.RegisterMessage(NodeID)
-
-GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertRequest)
-  })
-_sym_db.RegisterMessage(GetCertRequest)
-
-GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertResponse)
-  })
-_sym_db.RegisterMessage(GetCertResponse)
-
-SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
-  'DESCRIPTOR' : _SYSTEMINFO,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.SystemInfo)
-  })
-_sym_db.RegisterMessage(SystemInfo)
-
-Subjects = _reflection.GeneratedProtocolMessageType('Subjects', (_message.Message,), {
-  'DESCRIPTOR' : _SUBJECTS,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.Subjects)
-  })
-_sym_db.RegisterMessage(Subjects)
-
-PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsRequest)
-  })
-_sym_db.RegisterMessage(PermissionsRequest)
-
-InstanceIdent = _reflection.GeneratedProtocolMessageType('InstanceIdent', (_message.Message,), {
-  'DESCRIPTOR' : _INSTANCEIDENT,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.InstanceIdent)
-  })
-_sym_db.RegisterMessage(InstanceIdent)
-
-PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsResponse)
-  })
-_sym_db.RegisterMessage(PermissionsResponse)
-
-NodesID = _reflection.GeneratedProtocolMessageType('NodesID', (_message.Message,), {
-  'DESCRIPTOR' : _NODESID,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.NodesID)
-  })
-_sym_db.RegisterMessage(NodesID)
-
-GetCertTypesRequest = _reflection.GeneratedProtocolMessageType('GetCertTypesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTTYPESREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertTypesRequest)
-  })
-_sym_db.RegisterMessage(GetCertTypesRequest)
-
-CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
-  'DESCRIPTOR' : _CERTTYPES,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.CertTypes)
-  })
-_sym_db.RegisterMessage(CertTypes)
-
-SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETOWNERREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.SetOwnerRequest)
-  })
-_sym_db.RegisterMessage(SetOwnerRequest)
-
-ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CLEARREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.ClearRequest)
-  })
-_sym_db.RegisterMessage(ClearRequest)
-
-EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
-  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.EncryptDiskRequest)
-  })
-_sym_db.RegisterMessage(EncryptDiskRequest)
-
-CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyRequest)
-  })
-_sym_db.RegisterMessage(CreateKeyRequest)
-
-CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyResponse)
-  })
-_sym_db.RegisterMessage(CreateKeyResponse)
-
-ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertRequest)
-  })
-_sym_db.RegisterMessage(ApplyCertRequest)
-
-ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertResponse)
-  })
-_sym_db.RegisterMessage(ApplyCertResponse)
-
-Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v4.iamanager_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _PERMISSIONS,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions)
-  })
-_sym_db.RegisterMessage(Permissions)
-_sym_db.RegisterMessage(Permissions.PermissionsEntry)
-
-RegisterInstanceRequest = _reflection.GeneratedProtocolMessageType('RegisterInstanceRequest', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v4.iamanager_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _REGISTERINSTANCEREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest)
-  })
-_sym_db.RegisterMessage(RegisterInstanceRequest)
-_sym_db.RegisterMessage(RegisterInstanceRequest.PermissionsEntry)
-
-RegisterInstanceResponse = _reflection.GeneratedProtocolMessageType('RegisterInstanceResponse', (_message.Message,), {
-  'DESCRIPTOR' : _REGISTERINSTANCERESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceResponse)
-  })
-_sym_db.RegisterMessage(RegisterInstanceResponse)
-
-UnregisterInstanceRequest = _reflection.GeneratedProtocolMessageType('UnregisterInstanceRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UNREGISTERINSTANCEREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.UnregisterInstanceRequest)
-  })
-_sym_db.RegisterMessage(UnregisterInstanceRequest)
-
-_IAMPUBLICSERVICE = DESCRIPTOR.services_by_name['IAMPublicService']
-_IAMPUBLICIDENTITYSERVICE = DESCRIPTOR.services_by_name['IAMPublicIdentityService']
-_IAMPUBLICPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPublicPermissionsService']
-_IAMPROVISIONINGSERVICE = DESCRIPTOR.services_by_name['IAMProvisioningService']
-_IAMCERTIFICATESERVICE = DESCRIPTOR.services_by_name['IAMCertificateService']
-_IAMPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPermissionsService']
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  _PERMISSIONS_PERMISSIONSENTRY._options = None
-  _PERMISSIONS_PERMISSIONSENTRY._serialized_options = b'8\001'
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._options = None
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_options = b'8\001'
-  _APIVERSION._serialized_start=75
-  _APIVERSION._serialized_end=104
-  _NODEID._serialized_start=106
-  _NODEID._serialized_end=131
-  _GETCERTREQUEST._serialized_start=133
-  _GETCERTREQUEST._serialized_end=195
-  _GETCERTRESPONSE._serialized_start=197
-  _GETCERTRESPONSE._serialized_end=263
-  _SYSTEMINFO._serialized_start=265
-  _SYSTEMINFO._serialized_end=317
-  _SUBJECTS._serialized_start=319
-  _SUBJECTS._serialized_end=347
-  _PERMISSIONSREQUEST._serialized_start=349
-  _PERMISSIONSREQUEST._serialized_end=415
-  _INSTANCEIDENT._serialized_start=417
-  _INSTANCEIDENT._serialized_end=490
-  _PERMISSIONSRESPONSE._serialized_start=492
-  _PERMISSIONSRESPONSE._serialized_end=608
-  _NODESID._serialized_start=610
-  _NODESID._serialized_end=632
-  _GETCERTTYPESREQUEST._serialized_start=634
-  _GETCERTTYPESREQUEST._serialized_end=672
-  _CERTTYPES._serialized_start=674
-  _CERTTYPES._serialized_end=700
-  _SETOWNERREQUEST._serialized_start=702
-  _SETOWNERREQUEST._serialized_end=768
-  _CLEARREQUEST._serialized_start=770
-  _CLEARREQUEST._serialized_end=815
-  _ENCRYPTDISKREQUEST._serialized_start=817
-  _ENCRYPTDISKREQUEST._serialized_end=872
-  _CREATEKEYREQUEST._serialized_start=874
-  _CREATEKEYREQUEST._serialized_end=958
-  _CREATEKEYRESPONSE._serialized_start=960
-  _CREATEKEYRESPONSE._serialized_end=1023
-  _APPLYCERTREQUEST._serialized_start=1025
-  _APPLYCERTREQUEST._serialized_end=1088
-  _APPLYCERTRESPONSE._serialized_start=1090
-  _APPLYCERTRESPONSE._serialized_end=1158
-  _PERMISSIONS._serialized_start=1161
-  _PERMISSIONS._serialized_end=1291
-  _PERMISSIONS_PERMISSIONSENTRY._serialized_start=1241
-  _PERMISSIONS_PERMISSIONSENTRY._serialized_end=1291
-  _REGISTERINSTANCEREQUEST._serialized_start=1294
-  _REGISTERINSTANCEREQUEST._serialized_end=1522
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_start=1445
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_end=1522
-  _REGISTERINSTANCERESPONSE._serialized_start=1524
-  _REGISTERINSTANCERESPONSE._serialized_end=1566
-  _UNREGISTERINSTANCEREQUEST._serialized_start=1568
-  _UNREGISTERINSTANCEREQUEST._serialized_end=1642
-  _IAMPUBLICSERVICE._serialized_start=1645
-  _IAMPUBLICSERVICE._serialized_end=1867
-  _IAMPUBLICIDENTITYSERVICE._serialized_start=1870
-  _IAMPUBLICIDENTITYSERVICE._serialized_end=2110
-  _IAMPUBLICPERMISSIONSSERVICE._serialized_start=2112
-  _IAMPUBLICPERMISSIONSSERVICE._serialized_end=2230
-  _IAMPROVISIONINGSERVICE._serialized_start=2233
-  _IAMPROVISIONINGSERVICE._serialized_end=2680
-  _IAMCERTIFICATESERVICE._serialized_start=2683
-  _IAMCERTIFICATESERVICE._serialized_end=2866
-  _IAMPERMISSIONSSERVICE._serialized_start=2869
-  _IAMPERMISSIONSSERVICE._serialized_end=3082
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v4/iamanager.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ciamanager/v4/iamanager.proto\x12\x0ciamanager.v4\x1a\x1bgoogle/protobuf/empty.proto\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\"\x19\n\x06NodeID\x12\x0f\n\x07node_id\x18\x01 \x01(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1c\n\x08Subjects\x12\x10\n\x08subjects\x18\x01 \x03(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"I\n\rInstanceIdent\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x12\n\nsubject_id\x18\x02 \x01(\t\x12\x10\n\x08instance\x18\x03 \x01(\x04\"t\n\x13PermissionsResponse\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions\"\x16\n\x07NodesID\x12\x0b\n\x03ids\x18\x01 \x03(\t\"&\n\x13GetCertTypesRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\"B\n\x0fSetOwnerRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"-\n\x0c\x43learRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"7\n\x12\x45ncryptDiskRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"T\n\x10\x43reateKeyRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\"?\n\x11\x43reateKeyResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03\x63sr\x18\x03 \x01(\t\"?\n\x10\x41pplyCertRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x03 \x01(\t\"D\n\x11\x41pplyCertResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x03 \x01(\t\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v4.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe4\x01\n\x17RegisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12K\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x36.iamanager.v4.RegisterInstanceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions:\x02\x38\x01\"*\n\x18RegisterInstanceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\"J\n\x19UnregisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent2\xde\x01\n\x10IAMPublicService\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.APIVersion\"\x00\x12;\n\tGetNodeID\x12\x16.google.protobuf.Empty\x1a\x14.iamanager.v4.NodeID\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v4.GetCertRequest\x1a\x1d.iamanager.v4.GetCertResponse\"\x00\x32\xf0\x01\n\x18IAMPublicIdentityService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.SystemInfo\"\x00\x12?\n\x0bGetSubjects\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x12N\n\x18SubscribeSubjectsChanged\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x30\x01\x32v\n\x1bIAMPublicPermissionsService\x12W\n\x0eGetPermissions\x12 .iamanager.v4.PermissionsRequest\x1a!.iamanager.v4.PermissionsResponse\"\x00\x32\xbf\x03\n\x16IAMProvisioningService\x12@\n\rGetAllNodeIDs\x12\x16.google.protobuf.Empty\x1a\x15.iamanager.v4.NodesID\"\x00\x12L\n\x0cGetCertTypes\x12!.iamanager.v4.GetCertTypesRequest\x1a\x17.iamanager.v4.CertTypes\"\x00\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v4.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v4.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v4.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x32\xb7\x01\n\x15IAMCertificateService\x12N\n\tCreateKey\x12\x1e.iamanager.v4.CreateKeyRequest\x1a\x1f.iamanager.v4.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v4.ApplyCertRequest\x1a\x1f.iamanager.v4.ApplyCertResponse\"\x00\x32\xd5\x01\n\x15IAMPermissionsService\x12\x63\n\x10RegisterInstance\x12%.iamanager.v4.RegisterInstanceRequest\x1a&.iamanager.v4.RegisterInstanceResponse\"\x00\x12W\n\x12UnregisterInstance\x12\'.iamanager.v4.UnregisterInstanceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
+
+
+
+_APIVERSION = DESCRIPTOR.message_types_by_name['APIVersion']
+_NODEID = DESCRIPTOR.message_types_by_name['NodeID']
+_GETCERTREQUEST = DESCRIPTOR.message_types_by_name['GetCertRequest']
+_GETCERTRESPONSE = DESCRIPTOR.message_types_by_name['GetCertResponse']
+_SYSTEMINFO = DESCRIPTOR.message_types_by_name['SystemInfo']
+_SUBJECTS = DESCRIPTOR.message_types_by_name['Subjects']
+_PERMISSIONSREQUEST = DESCRIPTOR.message_types_by_name['PermissionsRequest']
+_INSTANCEIDENT = DESCRIPTOR.message_types_by_name['InstanceIdent']
+_PERMISSIONSRESPONSE = DESCRIPTOR.message_types_by_name['PermissionsResponse']
+_NODESID = DESCRIPTOR.message_types_by_name['NodesID']
+_GETCERTTYPESREQUEST = DESCRIPTOR.message_types_by_name['GetCertTypesRequest']
+_CERTTYPES = DESCRIPTOR.message_types_by_name['CertTypes']
+_SETOWNERREQUEST = DESCRIPTOR.message_types_by_name['SetOwnerRequest']
+_CLEARREQUEST = DESCRIPTOR.message_types_by_name['ClearRequest']
+_ENCRYPTDISKREQUEST = DESCRIPTOR.message_types_by_name['EncryptDiskRequest']
+_CREATEKEYREQUEST = DESCRIPTOR.message_types_by_name['CreateKeyRequest']
+_CREATEKEYRESPONSE = DESCRIPTOR.message_types_by_name['CreateKeyResponse']
+_APPLYCERTREQUEST = DESCRIPTOR.message_types_by_name['ApplyCertRequest']
+_APPLYCERTRESPONSE = DESCRIPTOR.message_types_by_name['ApplyCertResponse']
+_PERMISSIONS = DESCRIPTOR.message_types_by_name['Permissions']
+_PERMISSIONS_PERMISSIONSENTRY = _PERMISSIONS.nested_types_by_name['PermissionsEntry']
+_REGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['RegisterInstanceRequest']
+_REGISTERINSTANCEREQUEST_PERMISSIONSENTRY = _REGISTERINSTANCEREQUEST.nested_types_by_name['PermissionsEntry']
+_REGISTERINSTANCERESPONSE = DESCRIPTOR.message_types_by_name['RegisterInstanceResponse']
+_UNREGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['UnregisterInstanceRequest']
+APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
+  'DESCRIPTOR' : _APIVERSION,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.APIVersion)
+  })
+_sym_db.RegisterMessage(APIVersion)
+
+NodeID = _reflection.GeneratedProtocolMessageType('NodeID', (_message.Message,), {
+  'DESCRIPTOR' : _NODEID,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.NodeID)
+  })
+_sym_db.RegisterMessage(NodeID)
+
+GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertRequest)
+  })
+_sym_db.RegisterMessage(GetCertRequest)
+
+GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertResponse)
+  })
+_sym_db.RegisterMessage(GetCertResponse)
+
+SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMINFO,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.SystemInfo)
+  })
+_sym_db.RegisterMessage(SystemInfo)
+
+Subjects = _reflection.GeneratedProtocolMessageType('Subjects', (_message.Message,), {
+  'DESCRIPTOR' : _SUBJECTS,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.Subjects)
+  })
+_sym_db.RegisterMessage(Subjects)
+
+PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsRequest)
+  })
+_sym_db.RegisterMessage(PermissionsRequest)
+
+InstanceIdent = _reflection.GeneratedProtocolMessageType('InstanceIdent', (_message.Message,), {
+  'DESCRIPTOR' : _INSTANCEIDENT,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.InstanceIdent)
+  })
+_sym_db.RegisterMessage(InstanceIdent)
+
+PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsResponse)
+  })
+_sym_db.RegisterMessage(PermissionsResponse)
+
+NodesID = _reflection.GeneratedProtocolMessageType('NodesID', (_message.Message,), {
+  'DESCRIPTOR' : _NODESID,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.NodesID)
+  })
+_sym_db.RegisterMessage(NodesID)
+
+GetCertTypesRequest = _reflection.GeneratedProtocolMessageType('GetCertTypesRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTTYPESREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertTypesRequest)
+  })
+_sym_db.RegisterMessage(GetCertTypesRequest)
+
+CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
+  'DESCRIPTOR' : _CERTTYPES,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.CertTypes)
+  })
+_sym_db.RegisterMessage(CertTypes)
+
+SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SETOWNERREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.SetOwnerRequest)
+  })
+_sym_db.RegisterMessage(SetOwnerRequest)
+
+ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CLEARREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.ClearRequest)
+  })
+_sym_db.RegisterMessage(ClearRequest)
+
+EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.EncryptDiskRequest)
+  })
+_sym_db.RegisterMessage(EncryptDiskRequest)
+
+CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyRequest)
+  })
+_sym_db.RegisterMessage(CreateKeyRequest)
+
+CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyResponse)
+  })
+_sym_db.RegisterMessage(CreateKeyResponse)
+
+ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertRequest)
+  })
+_sym_db.RegisterMessage(ApplyCertRequest)
+
+ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertResponse)
+  })
+_sym_db.RegisterMessage(ApplyCertResponse)
+
+Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v4.iamanager_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _PERMISSIONS,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions)
+  })
+_sym_db.RegisterMessage(Permissions)
+_sym_db.RegisterMessage(Permissions.PermissionsEntry)
+
+RegisterInstanceRequest = _reflection.GeneratedProtocolMessageType('RegisterInstanceRequest', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v4.iamanager_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _REGISTERINSTANCEREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest)
+  })
+_sym_db.RegisterMessage(RegisterInstanceRequest)
+_sym_db.RegisterMessage(RegisterInstanceRequest.PermissionsEntry)
+
+RegisterInstanceResponse = _reflection.GeneratedProtocolMessageType('RegisterInstanceResponse', (_message.Message,), {
+  'DESCRIPTOR' : _REGISTERINSTANCERESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceResponse)
+  })
+_sym_db.RegisterMessage(RegisterInstanceResponse)
+
+UnregisterInstanceRequest = _reflection.GeneratedProtocolMessageType('UnregisterInstanceRequest', (_message.Message,), {
+  'DESCRIPTOR' : _UNREGISTERINSTANCEREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.UnregisterInstanceRequest)
+  })
+_sym_db.RegisterMessage(UnregisterInstanceRequest)
+
+_IAMPUBLICSERVICE = DESCRIPTOR.services_by_name['IAMPublicService']
+_IAMPUBLICIDENTITYSERVICE = DESCRIPTOR.services_by_name['IAMPublicIdentityService']
+_IAMPUBLICPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPublicPermissionsService']
+_IAMPROVISIONINGSERVICE = DESCRIPTOR.services_by_name['IAMProvisioningService']
+_IAMCERTIFICATESERVICE = DESCRIPTOR.services_by_name['IAMCertificateService']
+_IAMPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPermissionsService']
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _PERMISSIONS_PERMISSIONSENTRY._options = None
+  _PERMISSIONS_PERMISSIONSENTRY._serialized_options = b'8\001'
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._options = None
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_options = b'8\001'
+  _APIVERSION._serialized_start=75
+  _APIVERSION._serialized_end=104
+  _NODEID._serialized_start=106
+  _NODEID._serialized_end=131
+  _GETCERTREQUEST._serialized_start=133
+  _GETCERTREQUEST._serialized_end=195
+  _GETCERTRESPONSE._serialized_start=197
+  _GETCERTRESPONSE._serialized_end=263
+  _SYSTEMINFO._serialized_start=265
+  _SYSTEMINFO._serialized_end=317
+  _SUBJECTS._serialized_start=319
+  _SUBJECTS._serialized_end=347
+  _PERMISSIONSREQUEST._serialized_start=349
+  _PERMISSIONSREQUEST._serialized_end=415
+  _INSTANCEIDENT._serialized_start=417
+  _INSTANCEIDENT._serialized_end=490
+  _PERMISSIONSRESPONSE._serialized_start=492
+  _PERMISSIONSRESPONSE._serialized_end=608
+  _NODESID._serialized_start=610
+  _NODESID._serialized_end=632
+  _GETCERTTYPESREQUEST._serialized_start=634
+  _GETCERTTYPESREQUEST._serialized_end=672
+  _CERTTYPES._serialized_start=674
+  _CERTTYPES._serialized_end=700
+  _SETOWNERREQUEST._serialized_start=702
+  _SETOWNERREQUEST._serialized_end=768
+  _CLEARREQUEST._serialized_start=770
+  _CLEARREQUEST._serialized_end=815
+  _ENCRYPTDISKREQUEST._serialized_start=817
+  _ENCRYPTDISKREQUEST._serialized_end=872
+  _CREATEKEYREQUEST._serialized_start=874
+  _CREATEKEYREQUEST._serialized_end=958
+  _CREATEKEYRESPONSE._serialized_start=960
+  _CREATEKEYRESPONSE._serialized_end=1023
+  _APPLYCERTREQUEST._serialized_start=1025
+  _APPLYCERTREQUEST._serialized_end=1088
+  _APPLYCERTRESPONSE._serialized_start=1090
+  _APPLYCERTRESPONSE._serialized_end=1158
+  _PERMISSIONS._serialized_start=1161
+  _PERMISSIONS._serialized_end=1291
+  _PERMISSIONS_PERMISSIONSENTRY._serialized_start=1241
+  _PERMISSIONS_PERMISSIONSENTRY._serialized_end=1291
+  _REGISTERINSTANCEREQUEST._serialized_start=1294
+  _REGISTERINSTANCEREQUEST._serialized_end=1522
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_start=1445
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_end=1522
+  _REGISTERINSTANCERESPONSE._serialized_start=1524
+  _REGISTERINSTANCERESPONSE._serialized_end=1566
+  _UNREGISTERINSTANCEREQUEST._serialized_start=1568
+  _UNREGISTERINSTANCEREQUEST._serialized_end=1642
+  _IAMPUBLICSERVICE._serialized_start=1645
+  _IAMPUBLICSERVICE._serialized_end=1867
+  _IAMPUBLICIDENTITYSERVICE._serialized_start=1870
+  _IAMPUBLICIDENTITYSERVICE._serialized_end=2110
+  _IAMPUBLICPERMISSIONSSERVICE._serialized_start=2112
+  _IAMPUBLICPERMISSIONSSERVICE._serialized_end=2230
+  _IAMPROVISIONINGSERVICE._serialized_start=2233
+  _IAMPROVISIONINGSERVICE._serialized_end=2680
+  _IAMCERTIFICATESERVICE._serialized_start=2683
+  _IAMCERTIFICATESERVICE._serialized_end=2866
+  _IAMPERMISSIONSSERVICE._serialized_start=2869
+  _IAMPERMISSIONSSERVICE._serialized_end=3082
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,735 +1,735 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iamanager_dot_v4_dot_iamanager__pb2
-
-
-class IAMPublicServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetAPIVersion = channel.unary_unary(
-                '/iamanager.v4.IAMPublicService/GetAPIVersion',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
-                )
-        self.GetNodeID = channel.unary_unary(
-                '/iamanager.v4.IAMPublicService/GetNodeID',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
-                )
-        self.GetCert = channel.unary_unary(
-                '/iamanager.v4.IAMPublicService/GetCert',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
-                )
-
-
-class IAMPublicServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetAPIVersion(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetNodeID(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAPIVersion,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.SerializeToString,
-            ),
-            'GetNodeID': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNodeID,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.SerializeToString,
-            ),
-            'GetCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCert,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPublicService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetAPIVersion(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetAPIVersion',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetNodeID(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetNodeID',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetCert',
-            iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMPublicIdentityServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetSystemInfo = channel.unary_unary(
-                '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
-                )
-        self.GetSubjects = channel.unary_unary(
-                '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-                )
-        self.SubscribeSubjectsChanged = channel.unary_stream(
-                '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-                )
-
-
-class IAMPublicIdentityServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetSystemInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetSubjects(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SubscribeSubjectsChanged(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicIdentityServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSystemInfo,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.SerializeToString,
-            ),
-            'GetSubjects': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSubjects,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
-            ),
-            'SubscribeSubjectsChanged': grpc.unary_stream_rpc_method_handler(
-                    servicer.SubscribeSubjectsChanged,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPublicIdentityService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicIdentityService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetSystemInfo(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetSubjects(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SubscribeSubjectsChanged(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMPublicPermissionsServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetPermissions = channel.unary_unary(
-                '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
-                )
-
-
-class IAMPublicPermissionsServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetPermissions(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicPermissionsServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetPermissions': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetPermissions,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPublicPermissionsService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicPermissionsService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetPermissions(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
-            iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMProvisioningServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetAllNodeIDs = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
-                )
-        self.GetCertTypes = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/GetCertTypes',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
-                )
-        self.SetOwner = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/SetOwner',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.Clear = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/Clear',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.EncryptDisk = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/EncryptDisk',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.FinishProvisioning = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAMProvisioningServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetAllNodeIDs(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCertTypes(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetOwner(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Clear(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def EncryptDisk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def FinishProvisioning(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMProvisioningServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetAllNodeIDs': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAllNodeIDs,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.SerializeToString,
-            ),
-            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCertTypes,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.SerializeToString,
-            ),
-            'SetOwner': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetOwner,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'Clear': grpc.unary_unary_rpc_method_handler(
-                    servicer.Clear,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
-                    servicer.EncryptDisk,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
-                    servicer.FinishProvisioning,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMProvisioningService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMProvisioningService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetAllNodeIDs(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCertTypes(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetCertTypes',
-            iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetOwner(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/SetOwner',
-            iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Clear(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/Clear',
-            iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def EncryptDisk(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/EncryptDisk',
-            iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def FinishProvisioning(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMCertificateServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.CreateKey = channel.unary_unary(
-                '/iamanager.v4.IAMCertificateService/CreateKey',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
-                )
-        self.ApplyCert = channel.unary_unary(
-                '/iamanager.v4.IAMCertificateService/ApplyCert',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
-                )
-
-
-class IAMCertificateServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def CreateKey(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ApplyCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMCertificateServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'CreateKey': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateKey,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.SerializeToString,
-            ),
-            'ApplyCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.ApplyCert,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMCertificateService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMCertificateService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def CreateKey(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/CreateKey',
-            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ApplyCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/ApplyCert',
-            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMPermissionsServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.RegisterInstance = channel.unary_unary(
-                '/iamanager.v4.IAMPermissionsService/RegisterInstance',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
-                )
-        self.UnregisterInstance = channel.unary_unary(
-                '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAMPermissionsServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def RegisterInstance(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def UnregisterInstance(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPermissionsServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'RegisterInstance': grpc.unary_unary_rpc_method_handler(
-                    servicer.RegisterInstance,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.SerializeToString,
-            ),
-            'UnregisterInstance': grpc.unary_unary_rpc_method_handler(
-                    servicer.UnregisterInstance,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPermissionsService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPermissionsService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def RegisterInstance(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/RegisterInstance',
-            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def UnregisterInstance(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
-            iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iamanager_dot_v4_dot_iamanager__pb2
+
+
+class IAMPublicServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetAPIVersion = channel.unary_unary(
+                '/iamanager.v4.IAMPublicService/GetAPIVersion',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
+                )
+        self.GetNodeID = channel.unary_unary(
+                '/iamanager.v4.IAMPublicService/GetNodeID',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
+                )
+        self.GetCert = channel.unary_unary(
+                '/iamanager.v4.IAMPublicService/GetCert',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
+                )
+
+
+class IAMPublicServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetAPIVersion(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetNodeID(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAPIVersion,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.SerializeToString,
+            ),
+            'GetNodeID': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetNodeID,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.SerializeToString,
+            ),
+            'GetCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCert,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPublicService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetAPIVersion(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetAPIVersion',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetNodeID(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetNodeID',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetCert',
+            iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMPublicIdentityServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetSystemInfo = channel.unary_unary(
+                '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
+                )
+        self.GetSubjects = channel.unary_unary(
+                '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+                )
+        self.SubscribeSubjectsChanged = channel.unary_stream(
+                '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+                )
+
+
+class IAMPublicIdentityServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetSystemInfo(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetSubjects(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubscribeSubjectsChanged(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicIdentityServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSystemInfo,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.SerializeToString,
+            ),
+            'GetSubjects': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSubjects,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
+            ),
+            'SubscribeSubjectsChanged': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeSubjectsChanged,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPublicIdentityService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicIdentityService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetSystemInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetSubjects(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubscribeSubjectsChanged(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMPublicPermissionsServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetPermissions = channel.unary_unary(
+                '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
+                )
+
+
+class IAMPublicPermissionsServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetPermissions(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicPermissionsServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetPermissions': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPermissions,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPublicPermissionsService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicPermissionsService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetPermissions(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
+            iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMProvisioningServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetAllNodeIDs = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
+                )
+        self.GetCertTypes = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/GetCertTypes',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
+                )
+        self.SetOwner = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/SetOwner',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.Clear = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/Clear',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.EncryptDisk = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/EncryptDisk',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.FinishProvisioning = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAMProvisioningServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetAllNodeIDs(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCertTypes(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetOwner(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Clear(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def EncryptDisk(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def FinishProvisioning(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMProvisioningServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetAllNodeIDs': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAllNodeIDs,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.SerializeToString,
+            ),
+            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCertTypes,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.SerializeToString,
+            ),
+            'SetOwner': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetOwner,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'Clear': grpc.unary_unary_rpc_method_handler(
+                    servicer.Clear,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
+                    servicer.EncryptDisk,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
+                    servicer.FinishProvisioning,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMProvisioningService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMProvisioningService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetAllNodeIDs(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCertTypes(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetCertTypes',
+            iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetOwner(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/SetOwner',
+            iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Clear(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/Clear',
+            iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def EncryptDisk(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/EncryptDisk',
+            iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def FinishProvisioning(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMCertificateServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.CreateKey = channel.unary_unary(
+                '/iamanager.v4.IAMCertificateService/CreateKey',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
+                )
+        self.ApplyCert = channel.unary_unary(
+                '/iamanager.v4.IAMCertificateService/ApplyCert',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
+                )
+
+
+class IAMCertificateServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def CreateKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ApplyCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMCertificateServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'CreateKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateKey,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.SerializeToString,
+            ),
+            'ApplyCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.ApplyCert,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMCertificateService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMCertificateService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def CreateKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/CreateKey',
+            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ApplyCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/ApplyCert',
+            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMPermissionsServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.RegisterInstance = channel.unary_unary(
+                '/iamanager.v4.IAMPermissionsService/RegisterInstance',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
+                )
+        self.UnregisterInstance = channel.unary_unary(
+                '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAMPermissionsServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def RegisterInstance(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UnregisterInstance(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPermissionsServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'RegisterInstance': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterInstance,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.SerializeToString,
+            ),
+            'UnregisterInstance': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnregisterInstance,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPermissionsService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPermissionsService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def RegisterInstance(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/RegisterInstance',
+            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UnregisterInstance(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
+            iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/files/1rootCA.crt

```diff
@@ -1,172 +1,170 @@
 00000000: 2d2d 2d2d 2d42 4547 494e 2043 4552 5449  -----BEGIN CERTI
-00000010: 4649 4341 5445 2d2d 2d2d 2d0d 0a4d 4949  FICATE-----..MII
-00000020: 4541 6a43 4341 7571 6741 7749 4241 6749  EAjCCAuqgAwIBAgI
-00000030: 4a41 5077 6b32 4e46 6653 4450 6a4d 4130  JAPwk2NFfSDPjMA0
-00000040: 4743 5371 4753 4962 3344 5145 4243 7755  GCSqGSIb3DQEBCwU
-00000050: 414d 4947 4e4d 5263 7746 5159 440d 0a56  AMIGNMRcwFQYD..V
-00000060: 5151 4444 4135 4764 584e 7062 3234 6755  QQDDA5GdXNpb24gU
-00000070: 6d39 7664 4342 4451 5445 704d 4363 4743  m9vdCBDQTEpMCcGC
-00000080: 5371 4753 4962 3344 5145 4a41 5259 6164  SqGSIb3DQEJARYad
-00000090: 6d39 7362 3252 3562 586c 7958 324a 680d  m9sb2R5bXlyX2Jh.
-000000a0: 0a59 6d4e 6f64 5774 415a 5842 6862 5335  .YmNodWtAZXBhbS5
-000000b0: 6a62 3230 7844 5441 4c42 674e 5642 416f  jb20xDTALBgNVBAo
-000000c0: 4d42 4556 5151 5530 7848 4441 6142 674e  MBEVQQU0xHDAaBgN
-000000d0: 5642 4173 4d45 3035 7664 6e56 7a49 4539  VBAsME05vdnVzIE9
-000000e0: 790d 0a5a 4738 6755 3256 6a62 4739 7964  y..ZG8gU2VjbG9yd
-000000f0: 5730 7844 5441 4c42 674e 5642 4163 4d42  W0xDTALBgNVBAcMB
-00000100: 4574 3561 5859 7843 7a41 4a42 674e 5642  Et5aXYxCzAJBgNVB
-00000110: 4159 5441 6c56 424d 4234 5844 5445 344d  AYTAlVBMB4XDTE4M
-00000120: 4451 780d 0a4d 4445 784d 7a4d 774d 466f  DQx..MDExMzMwMFo
-00000130: 5844 5449 324d 4459 794e 7a45 784d 7a4d  XDTI2MDYyNzExMzM
-00000140: 774d 466f 7767 5930 7846 7a41 5642 674e  wMFowgY0xFzAVBgN
-00000150: 5642 414d 4d44 6b5a 3163 326c 7662 6942  VBAMMDkZ1c2lvbiB
-00000160: 5362 3239 300d 0a49 454e 424d 536b 774a  Sb290..IENBMSkwJ
-00000170: 7759 4a4b 6f5a 4968 7663 4e41 516b 4246  wYJKoZIhvcNAQkBF
-00000180: 6870 3262 3278 765a 486c 7465 584a 6659  hp2b2xvZHlteXJfY
-00000190: 6d46 6959 3268 3161 3042 6c63 4746 744c  mFiY2h1a0BlcGFtL
-000001a0: 6d4e 7662 5445 4e0d 0a4d 4173 4741 3155  mNvbTEN..MAsGA1U
-000001b0: 4543 6777 4552 5642 4254 5445 634d 426f  ECgwERVBBTTEcMBo
-000001c0: 4741 3155 4543 7777 5454 6d39 3264 584d  GA1UECwwTTm92dXM
-000001d0: 6754 334a 6b62 7942 545a 574e 7362 334a  gT3JkbyBTZWNsb3J
-000001e0: 3162 5445 4e4d 4173 470d 0a41 3155 4542  1bTENMAsG..A1UEB
-000001f0: 7777 4553 336c 7064 6a45 4c4d 416b 4741  wwES3lpdjELMAkGA
-00000200: 3155 4542 684d 4356 5545 7767 6745 694d  1UEBhMCVUEwggEiM
-00000210: 4130 4743 5371 4753 4962 3344 5145 4241  A0GCSqGSIb3DQEBA
-00000220: 5155 4141 3449 4244 7741 770d 0a67 6745  QUAA4IBDwAw..ggE
-00000230: 4b41 6f49 4241 5143 2b4b 326f 7732 484f  KAoIBAQC+K2ow2HO
-00000240: 372b 5355 5666 4f71 3574 5474 6d48 6a34  7+SUVfOq5tTtmHj4
-00000250: 4c51 696a 484a 3830 336d 4c6b 3970 6b50  LQijHJ803mLk9pkP
-00000260: 6566 2b47 6c6d 6579 7039 4858 650d 0a6a  ef+Glmeyp9HXe..j
-00000270: 446c 5143 3034 4d65 6f76 4d42 654e 5461  DlQC04MeovMBeNTa
-00000280: 7130 7769 6266 3771 6173 396e 6958 6265  q0wibf7qas9niXbe
-00000290: 5852 567a 6865 5a49 467a 694d 5871 5275  XRVzheZIFziMXqRu
-000002a0: 774c 7163 304b 5864 4478 4944 5054 620d  wLqc0KXdDxIDPTb.
-000002b0: 0a54 5733 4b30 4845 364d 2f65 4174 5466  .TW3K0HE6M/eAtTf
-000002c0: 6e39 2b5a 2f4c 6e6b 5774 347a 4d58 6173  n9+Z/LnkWt4zMXas
-000002d0: 6330 3268 7675 6673 6d49 5645 754e 6263  c02hvufsmIVEuNbc
-000002e0: 3156 6872 734a 4a67 3575 6b38 386c 6450  1VhrsJJg5uk88ldP
-000002f0: 4d0d 0a4c 5346 376e 6666 3965 595a 5448  M..LSF7nff9eYZTH
-00000300: 5967 4379 426b 7439 614c 2b66 776f 584f  YgCyBkt9aL+fwoXO
-00000310: 3665 5344 5341 686a 6f70 5833 6c68 6469  6eSDSAhjopX3lhdi
-00000320: 646b 4d2b 6e69 3745 4f68 6c4e 3753 546d  dkM+ni7EOhlN7STm
-00000330: 6744 4d0d 0a57 4b68 396e 4d6a 5844 3566  gDM..WKh9nMjXD5f
-00000340: 3238 5047 6874 572f 645a 766e 3453 7a61  28PGhtW/dZvn4Sza
-00000350: 7352 4535 4d65 6145 7849 6c42 6d68 6b57  sRE5MeaExIlBmhkW
-00000360: 4555 6756 4379 5037 4c76 7551 4752 5550  EUgVCyP7LvuQGRUP
-00000370: 4b2b 4e59 7a0d 0a46 4532 434c 5275 6972  K+NYz..FE2CLRuir
-00000380: 4c43 5779 3148 4974 396c 4c7a 6950 6a6c  LCWy1HIt9lLziPjl
-00000390: 5a34 3336 316d 4e41 674d 4241 4147 6a59  Z4361mNAgMBAAGjY
-000003a0: 7a42 684d 4230 4741 3155 6444 6751 5742  zBhMB0GA1UdDgQWB
-000003b0: 4252 3053 6868 7a0d 0a4f 754d 3935 4268  BR0Shhz..OuM95Bh
-000003c0: 4430 6d57 7843 316a 2b4b 7245 3655 6a41  D0mWxC1j+KrE6UjA
-000003d0: 4d42 674e 5648 524d 4542 5441 4441 5148  MBgNVHRMEBTADAQH
-000003e0: 2f4d 4173 4741 3155 6444 7751 4541 7749  /MAsGA1UdDwQEAwI
-000003f0: 4242 6a41 6c42 674e 560d 0a48 5245 4548  BBjAlBgNV..HREEH
-00000400: 6a41 6367 5270 3262 3278 765a 486c 7465  jAcgRp2b2xvZHlte
-00000410: 584a 6659 6d46 6959 3268 3161 3042 6c63  XJfYmFiY2h1a0Blc
-00000420: 4746 744c 6d4e 7662 5441 4e42 676b 7168  GFtLmNvbTANBgkqh
-00000430: 6b69 4739 7730 4241 5173 460d 0a41 414f  kiG9w0BAQsF..AAO
-00000440: 4341 5145 416c 3862 7631 4854 5965 336c  CAQEAl8bv1HTYe3l
-00000450: 3459 2b67 3054 565a 5237 6259 4c35 424e  4Y+g0TVZR7bYL5BN
-00000460: 736e 4767 7179 3071 5335 6675 3939 316b  snGgqy0qS5fu991k
-00000470: 6858 5766 2b5a 7761 324d 4c56 6e0d 0a59  hXWf+Zwa2MLVn..Y
-00000480: 616b 4d6e 4c6b 6a76 6448 7155 7057 4d4a  akMnLkjvdHqUpWMJ
-00000490: 2f53 3832 6f32 7a57 476d 6d75 7863 6135  /S82o2zWGmmuxca5
-000004a0: 3665 686a 7843 6950 2f6e 6b6d 344d 3734  6ehjxCiP/nkm4M74
-000004b0: 7958 7a32 5238 6375 3532 5778 596e 460d  yXz2R8cu52WxYnF.
-000004c0: 0a79 4d76 6761 777a 5136 6331 7968 765a  .yMvgawzQ6c1yhvZ
-000004d0: 6976 2f67 4545 374b 6462 5952 564b 4c48  iv/gEE7KdbYRVKLH
-000004e0: 5067 427a 6679 7570 3231 6935 6e67 536c  PgBzfyup21i5ngSl
-000004f0: 5463 4d52 5253 376f 4f42 6d6f 7965 3471  TcMRRS7oOBmoye4q
-00000500: 630d 0a36 6164 7136 4874 5936 582f 4f6e  c..6adq6HtY6X/On
-00000510: 5a39 4935 786f 524e 3147 6376 614c 5567  Z9I5xoRN1GcvaLUg
-00000520: 5545 3669 6754 6956 6131 7046 386b 6564  UE6igTiVa1pF8ked
-00000530: 5768 4859 3777 7a54 5842 787a 5376 495a  WhHY7wzTXBxzSvIZ
-00000540: 6b43 550d 0a56 4845 4f7a 7661 476b 396d  kCU..VHEOzvaGk9m
-00000550: 6950 366e 4272 4466 4e76 376d 496b 6745  iP6nBrDfNv7mIkgE
-00000560: 4b41 5272 6a6a 5370 6d4a 6173 4945 552b  KARrjjSpmJasIEU+
-00000570: 6d4e 747a 654f 4945 694d 7457 3145 4d52  mNtzeOIEiMtW1EMR
-00000580: 6334 3537 6f0d 0a30 5064 4649 336a 7365  c457o..0PdFI3jse
-00000590: 794c 5650 5668 457a 556b 7543 376d 776a  yLVPVhEzUkuC7mwj
-000005a0: 6237 4365 513d 3d0d 0a2d 2d2d 2d2d 454e  b7CeQ==..-----EN
-000005b0: 4420 4345 5254 4946 4943 4154 452d 2d2d  D CERTIFICATE---
-000005c0: 2d2d 0d0a 2d2d 2d2d 2d42 4547 494e 2043  --..-----BEGIN C
-000005d0: 4552 5449 4649 4341 5445 2d2d 2d2d 2d0d  ERTIFICATE-----.
-000005e0: 0a4d 4949 4463 5443 4341 6c6d 6741 7749  .MIIDcTCCAlmgAwI
-000005f0: 4241 6749 5561 4161 6539 2b76 576e 4b56  BAgIUaAae9+vWnKV
-00000600: 7451 4b2f 536c 6c54 436e 696b 4d43 666f  tQK/SllTCnikMCfo
-00000610: 7744 5159 4a4b 6f5a 4968 7663 4e41 5145  wDQYJKoZIhvcNAQE
-00000620: 4c0d 0a42 5141 7751 6a45 554d 4249 4741  L..BQAwQjEUMBIGA
-00000630: 3155 4541 7777 4c51 5739 7a49 464a 7662  1UEAwwLQW9zIFJvb
-00000640: 3351 6751 3045 7844 7a41 4e42 674e 5642  3QgQ0ExDzANBgNVB
-00000650: 416f 4d42 6b35 3159 5735 6a5a 5445 4d4d  AoMBk51YW5jZTEMM
-00000660: 416f 470d 0a41 3155 4543 7777 4451 5739  AoG..A1UECwwDQW9
-00000670: 7a4d 5173 7743 5159 4456 5151 4745 774a  zMQswCQYDVQQGEwJ
-00000680: 5655 7a41 6746 7730 794d 4445 784d 5463  VUzAgFw0yMDExMTc
-00000690: 784d 4449 344d 444e 6147 4138 794d 4455  xMDI4MDNaGA8yMDU
-000006a0: 774d 5445 780d 0a4d 4445 774d 6a67 774d  wMTEx..MDEwMjgwM
-000006b0: 316f 7751 6a45 554d 4249 4741 3155 4541  1owQjEUMBIGA1UEA
-000006c0: 7777 4c51 5739 7a49 464a 7662 3351 6751  wwLQW9zIFJvb3QgQ
-000006d0: 3045 7844 7a41 4e42 674e 5642 416f 4d42  0ExDzANBgNVBAoMB
-000006e0: 6b35 3159 5735 6a0d 0a5a 5445 4d4d 416f  k51YW5j..ZTEMMAo
-000006f0: 4741 3155 4543 7777 4451 5739 7a4d 5173  GA1UECwwDQW9zMQs
-00000700: 7743 5159 4456 5151 4745 774a 5655 7a43  wCQYDVQQGEwJVUzC
-00000710: 4341 5349 7744 5159 4a4b 6f5a 4968 7663  CASIwDQYJKoZIhvc
-00000720: 4e41 5145 4242 5141 440d 0a67 6745 5041  NAQEBBQAD..ggEPA
-00000730: 4443 4341 516f 4367 6745 4241 4e73 4a65  DCCAQoCggEBANsJe
-00000740: 624b 4d6f 7232 7844 6c51 7241 3739 4566  bKMor2xDlQrA79Ef
-00000750: 4c51 3531 596e 6344 745a 6d78 4c4b 382b  LQ51YncDtZmxLK8+
-00000760: 5968 4c78 4c2f 3234 5853 420d 0a58 4454  YhLxL/24XSB..XDT
-00000770: 6f44 474c 6174 6563 7273 3631 4551 6953  oDGLatecrs61EQiS
-00000780: 6f74 4c4f 3749 6c5a 7742 3367 665a 554b  otLO7IlZwB3gfZUK
-00000790: 6d4c 6451 7953 6757 4169 5253 6968 6c7a  mLdQySgWAiRSihlz
-000007a0: 7678 396d 3043 4873 5366 4833 650d 0a72  vx9m0CHsSfH3e..r
-000007b0: 704a 4c6a 6e6a 6953 365a 4a68 426b 5177  pJLjnjiS6ZJhBkQw
-000007c0: 732b 6241 5669 4e34 795a 7551 7063 4b73  s+bAViN4yZuQpcKs
-000007d0: 7879 6762 3177 7a37 6172 4f79 6c32 6e59  xygb1wz7arOyl2nY
-000007e0: 4544 4d7a 2b68 7964 3863 7337 5531 480d  EDMz+hyd8cs7U1H.
-000007f0: 0a30 4a4a 6749 3170 5042 554c 634b 654c  .0JJgI1pPBULcKeL
-00000800: 6643 4750 475a 7566 4236 5965 4966 5054  fCGPGZufB6YeIfPT
-00000810: 5550 2f43 4534 3968 6277 4d75 4858 6870  UP/CE49hbwMuHXhp
-00000820: 4463 354c 7330 5342 5857 5556 666b 424d  Dc5Ls0SBXWUVfkBM
-00000830: 450d 0a4a 7275 654d 497a 4a52 5177 5532  E..JrueMIzJRQwU2
-00000840: 394e 2b33 3250 6867 624c 5a75 776f 544a  9N+32PhgbLZuwoTJ
-00000850: 5669 2b56 634b 5266 4632 4f62 7773 647a  Vi+VcKRfF2Obwsdz
-00000860: 6348 3633 6454 4169 796a 4372 4d59 5934  cH63dTAiyjCrMYY4
-00000870: 6764 630d 0a32 3075 626a 6479 6e57 3778  gdc..20ubjdynW7x
-00000880: 3367 784f 5751 6830 4f32 696b 6e69 2f4f  3gxOWQh0O2ikni/O
-00000890: 5478 6f7a 7758 3738 6c72 4345 4341 7745  TxozwX78lrCECAwE
-000008a0: 4141 614e 644d 4673 7744 4159 4456 5230  AAaNdMFswDAYDVR0
-000008b0: 5442 4155 770d 0a41 7745 422f 7a41 6442  TBAUw..AwEB/zAdB
-000008c0: 674e 5648 5134 4546 6751 554f 656e 4436  gNVHQ4EFgQUOenD6
-000008d0: 5562 4f43 6c49 3344 4d67 4a36 3041 3266  UbOClI3DMgJ60A2f
-000008e0: 5537 536a 5938 7748 7759 4456 5230 6a42  U7SjY8wHwYDVR0jB
-000008f0: 4267 7746 6f41 550d 0a4f 656e 4436 5562  BgwFoAU..OenD6Ub
-00000900: 4f43 6c49 3344 4d67 4a36 3041 3266 5537  OClI3DMgJ60A2fU7
-00000910: 536a 5938 7743 7759 4456 5230 5042 4151  SjY8wCwYDVR0PBAQ
-00000920: 4441 6747 474d 4130 4743 5371 4753 4962  DAgGGMA0GCSqGSIb
-00000930: 3344 5145 4243 7755 410d 0a41 3449 4241  3DQEBCwUA..A4IBA
-00000940: 5142 5151 6f69 3638 6c6d 4541 506d 6373  QBQQoi68lmEAPmcs
-00000950: 4941 6958 3367 696c 6d76 7565 6164 6963  IAiX3gilmvueadic
-00000960: 5a65 6f42 4b61 4b61 4846 4a6c 4c31 4341  ZeoBKaKaHFJlL1CA
-00000970: 7648 5748 544c 6330 474c 720d 0a6f 4c33  vHWHTLc0GLr..oL3
-00000980: 5871 5657 3569 7165 474c 3865 7533 4f6d  XqVW5iqeGL8eu3Om
-00000990: 6961 7850 4959 3466 327a 786f 4148 474c  iaxPIY4f2zxoAHGL
-000009a0: 5459 3375 722f 4f30 3347 4251 4532 6a42  TY3ur/O03GBQE2jB
-000009b0: 7556 3675 4f70 5874 4e63 3064 360d 0a58  uV6uOpXtNc0d6..X
-000009c0: 4470 342f 772f 704d 6345 6458 7337 5439  Dp4/w/pMcEdXs7T9
-000009d0: 4f38 6c4c 496a 7976 532b 6866 6f53 4764  O8lLIjyvS+hfoSGd
-000009e0: 3958 346b 4e4b 694d 6135 536d 6f35 5530  9X4kNKiMa5Smo5U0
-000009f0: 566f 414c 4f4d 4667 5245 3656 5a46 660d  VoALOMFgRE6VZFf.
-00000a00: 0a57 7132 4575 7541 5445 7837 4643 5a64  .Wq2EuuATEx7FCZd
-00000a10: 3450 6b63 4f4c 7346 666f 614c 7465 4561  4PkcOLsFfoaLteEa
-00000a20: 326c 5734 356f 5749 626c 6c4d 6e33 6557  2lW45oWIbllMn3eW
-00000a30: 796f 382b 4332 5139 5277 336b 627a 496f  yo8+C2Q9Rw3kbzIo
-00000a40: 740d 0a32 5962 5059 6b50 6273 4633 452f  t..2YbPYkPbsF3E/
-00000a50: 6352 3455 5a46 386a 4742 6e65 4838 304d  cR4UZF8jGBneH80M
-00000a60: 746b 3034 4577 5635 6f62 6e67 4642 7174  tk04EwV5obngFBqt
-00000a70: 3355 655a 796a 5658 4168 7775 6d5a 7436  3UeZyjVXAhwumZt6
-00000a80: 522b 4a0d 0a72 467a 5a6c 6443 626d 3478  R+J..rFzZldCbm4x
-00000a90: 6a2b 7052 4668 7935 4643 6b48 4970 6950  j+pRFhy5FCkHIpiP
-00000aa0: 6a0d 0a2d 2d2d 2d2d 454e 4420 4345 5254  j..-----END CERT
-00000ab0: 4946 4943 4154 452d 2d2d 2d2d 0d0a       IFICATE-----..
+00000010: 4649 4341 5445 2d2d 2d2d 2d0a 4d49 4945  FICATE-----.MIIE
+00000020: 416a 4343 4175 7167 4177 4942 4167 494a  AjCCAuqgAwIBAgIJ
+00000030: 4150 776b 324e 4666 5344 506a 4d41 3047  APwk2NFfSDPjMA0G
+00000040: 4353 7147 5349 6233 4451 4542 4377 5541  CSqGSIb3DQEBCwUA
+00000050: 4d49 474e 4d52 6377 4651 5944 0a56 5151  MIGNMRcwFQYD.VQQ
+00000060: 4444 4135 4764 584e 7062 3234 6755 6d39  DDA5GdXNpb24gUm9
+00000070: 7664 4342 4451 5445 704d 4363 4743 5371  vdCBDQTEpMCcGCSq
+00000080: 4753 4962 3344 5145 4a41 5259 6164 6d39  GSIb3DQEJARYadm9
+00000090: 7362 3252 3562 586c 7958 324a 680a 596d  sb2R5bXlyX2Jh.Ym
+000000a0: 4e6f 6457 7441 5a58 4268 6253 356a 6232  NodWtAZXBhbS5jb2
+000000b0: 3078 4454 414c 4267 4e56 4241 6f4d 4245  0xDTALBgNVBAoMBE
+000000c0: 5651 5155 3078 4844 4161 4267 4e56 4241  VQQU0xHDAaBgNVBA
+000000d0: 734d 4530 3576 646e 567a 4945 3979 0a5a  sME05vdnVzIE9y.Z
+000000e0: 4738 6755 3256 6a62 4739 7964 5730 7844  G8gU2VjbG9ydW0xD
+000000f0: 5441 4c42 674e 5642 4163 4d42 4574 3561  TALBgNVBAcMBEt5a
+00000100: 5859 7843 7a41 4a42 674e 5642 4159 5441  XYxCzAJBgNVBAYTA
+00000110: 6c56 424d 4234 5844 5445 344d 4451 780a  lVBMB4XDTE4MDQx.
+00000120: 4d44 4578 4d7a 4d77 4d46 6f58 4454 4932  MDExMzMwMFoXDTI2
+00000130: 4d44 5979 4e7a 4578 4d7a 4d77 4d46 6f77  MDYyNzExMzMwMFow
+00000140: 6759 3078 467a 4156 4267 4e56 4241 4d4d  gY0xFzAVBgNVBAMM
+00000150: 446b 5a31 6332 6c76 6269 4253 6232 3930  DkZ1c2lvbiBSb290
+00000160: 0a49 454e 424d 536b 774a 7759 4a4b 6f5a  .IENBMSkwJwYJKoZ
+00000170: 4968 7663 4e41 516b 4246 6870 3262 3278  IhvcNAQkBFhp2b2x
+00000180: 765a 486c 7465 584a 6659 6d46 6959 3268  vZHlteXJfYmFiY2h
+00000190: 3161 3042 6c63 4746 744c 6d4e 7662 5445  1a0BlcGFtLmNvbTE
+000001a0: 4e0a 4d41 7347 4131 5545 4367 7745 5256  N.MAsGA1UECgwERV
+000001b0: 4242 5454 4563 4d42 6f47 4131 5545 4377  BBTTEcMBoGA1UECw
+000001c0: 7754 546d 3932 6458 4d67 5433 4a6b 6279  wTTm92dXMgT3Jkby
+000001d0: 4254 5a57 4e73 6233 4a31 6254 454e 4d41  BTZWNsb3J1bTENMA
+000001e0: 7347 0a41 3155 4542 7777 4553 336c 7064  sG.A1UEBwwES3lpd
+000001f0: 6a45 4c4d 416b 4741 3155 4542 684d 4356  jELMAkGA1UEBhMCV
+00000200: 5545 7767 6745 694d 4130 4743 5371 4753  UEwggEiMA0GCSqGS
+00000210: 4962 3344 5145 4241 5155 4141 3449 4244  Ib3DQEBAQUAA4IBD
+00000220: 7741 770a 6767 454b 416f 4942 4151 432b  wAw.ggEKAoIBAQC+
+00000230: 4b32 6f77 3248 4f37 2b53 5556 664f 7135  K2ow2HO7+SUVfOq5
+00000240: 7454 746d 486a 344c 5169 6a48 4a38 3033  tTtmHj4LQijHJ803
+00000250: 6d4c 6b39 706b 5065 662b 476c 6d65 7970  mLk9pkPef+Glmeyp
+00000260: 3948 5865 0a6a 446c 5143 3034 4d65 6f76  9HXe.jDlQC04Meov
+00000270: 4d42 654e 5461 7130 7769 6266 3771 6173  MBeNTaq0wibf7qas
+00000280: 396e 6958 6265 5852 567a 6865 5a49 467a  9niXbeXRVzheZIFz
+00000290: 694d 5871 5275 774c 7163 304b 5864 4478  iMXqRuwLqc0KXdDx
+000002a0: 4944 5054 620a 5457 334b 3048 4536 4d2f  IDPTb.TW3K0HE6M/
+000002b0: 6541 7454 666e 392b 5a2f 4c6e 6b57 7434  eAtTfn9+Z/LnkWt4
+000002c0: 7a4d 5861 7363 3032 6876 7566 736d 4956  zMXasc02hvufsmIV
+000002d0: 4575 4e62 6331 5668 7273 4a4a 6735 756b  EuNbc1VhrsJJg5uk
+000002e0: 3838 6c64 504d 0a4c 5346 376e 6666 3965  88ldPM.LSF7nff9e
+000002f0: 595a 5448 5967 4379 426b 7439 614c 2b66  YZTHYgCyBkt9aL+f
+00000300: 776f 584f 3665 5344 5341 686a 6f70 5833  woXO6eSDSAhjopX3
+00000310: 6c68 6469 646b 4d2b 6e69 3745 4f68 6c4e  lhdidkM+ni7EOhlN
+00000320: 3753 546d 6744 4d0a 574b 6839 6e4d 6a58  7STmgDM.WKh9nMjX
+00000330: 4435 6632 3850 4768 7457 2f64 5a76 6e34  D5f28PGhtW/dZvn4
+00000340: 537a 6173 5245 354d 6561 4578 496c 426d  SzasRE5MeaExIlBm
+00000350: 686b 5745 5567 5643 7950 374c 7675 5147  hkWEUgVCyP7LvuQG
+00000360: 5255 504b 2b4e 597a 0a46 4532 434c 5275  RUPK+NYz.FE2CLRu
+00000370: 6972 4c43 5779 3148 4974 396c 4c7a 6950  irLCWy1HIt9lLziP
+00000380: 6a6c 5a34 3336 316d 4e41 674d 4241 4147  jlZ4361mNAgMBAAG
+00000390: 6a59 7a42 684d 4230 4741 3155 6444 6751  jYzBhMB0GA1UdDgQ
+000003a0: 5742 4252 3053 6868 7a0a 4f75 4d39 3542  WBBR0Shhz.OuM95B
+000003b0: 6844 306d 5778 4331 6a2b 4b72 4536 556a  hD0mWxC1j+KrE6Uj
+000003c0: 414d 4267 4e56 4852 4d45 4254 4144 4151  AMBgNVHRMEBTADAQ
+000003d0: 482f 4d41 7347 4131 5564 4477 5145 4177  H/MAsGA1UdDwQEAw
+000003e0: 4942 426a 416c 4267 4e56 0a48 5245 4548  IBBjAlBgNV.HREEH
+000003f0: 6a41 6367 5270 3262 3278 765a 486c 7465  jAcgRp2b2xvZHlte
+00000400: 584a 6659 6d46 6959 3268 3161 3042 6c63  XJfYmFiY2h1a0Blc
+00000410: 4746 744c 6d4e 7662 5441 4e42 676b 7168  GFtLmNvbTANBgkqh
+00000420: 6b69 4739 7730 4241 5173 460a 4141 4f43  kiG9w0BAQsF.AAOC
+00000430: 4151 4541 6c38 6276 3148 5459 6533 6c34  AQEAl8bv1HTYe3l4
+00000440: 592b 6730 5456 5a52 3762 594c 3542 4e73  Y+g0TVZR7bYL5BNs
+00000450: 6e47 6771 7930 7153 3566 7539 3931 6b68  nGgqy0qS5fu991kh
+00000460: 5857 662b 5a77 6132 4d4c 566e 0a59 616b  XWf+Zwa2MLVn.Yak
+00000470: 4d6e 4c6b 6a76 6448 7155 7057 4d4a 2f53  MnLkjvdHqUpWMJ/S
+00000480: 3832 6f32 7a57 476d 6d75 7863 6135 3665  82o2zWGmmuxca56e
+00000490: 686a 7843 6950 2f6e 6b6d 344d 3734 7958  hjxCiP/nkm4M74yX
+000004a0: 7a32 5238 6375 3532 5778 596e 460a 794d  z2R8cu52WxYnF.yM
+000004b0: 7667 6177 7a51 3663 3179 6876 5a69 762f  vgawzQ6c1yhvZiv/
+000004c0: 6745 4537 4b64 6259 5256 4b4c 4850 6742  gEE7KdbYRVKLHPgB
+000004d0: 7a66 7975 7032 3169 356e 6753 6c54 634d  zfyup21i5ngSlTcM
+000004e0: 5252 5337 6f4f 426d 6f79 6534 7163 0a36  RRS7oOBmoye4qc.6
+000004f0: 6164 7136 4874 5936 582f 4f6e 5a39 4935  adq6HtY6X/OnZ9I5
+00000500: 786f 524e 3147 6376 614c 5567 5545 3669  xoRN1GcvaLUgUE6i
+00000510: 6754 6956 6131 7046 386b 6564 5768 4859  gTiVa1pF8kedWhHY
+00000520: 3777 7a54 5842 787a 5376 495a 6b43 550a  7wzTXBxzSvIZkCU.
+00000530: 5648 454f 7a76 6147 6b39 6d69 5036 6e42  VHEOzvaGk9miP6nB
+00000540: 7244 664e 7637 6d49 6b67 454b 4152 726a  rDfNv7mIkgEKARrj
+00000550: 6a53 706d 4a61 7349 4555 2b6d 4e74 7a65  jSpmJasIEU+mNtze
+00000560: 4f49 4569 4d74 5731 454d 5263 3435 376f  OIEiMtW1EMRc457o
+00000570: 0a30 5064 4649 336a 7365 794c 5650 5668  .0PdFI3jseyLVPVh
+00000580: 457a 556b 7543 376d 776a 6237 4365 513d  EzUkuC7mwjb7CeQ=
+00000590: 3d0a 2d2d 2d2d 2d45 4e44 2043 4552 5449  =.-----END CERTI
+000005a0: 4649 4341 5445 2d2d 2d2d 2d0a 2d2d 2d2d  FICATE-----.----
+000005b0: 2d42 4547 494e 2043 4552 5449 4649 4341  -BEGIN CERTIFICA
+000005c0: 5445 2d2d 2d2d 2d0a 4d49 4944 6354 4343  TE-----.MIIDcTCC
+000005d0: 416c 6d67 4177 4942 4167 4955 6141 6165  AlmgAwIBAgIUaAae
+000005e0: 392b 7657 6e4b 5674 514b 2f53 6c6c 5443  9+vWnKVtQK/SllTC
+000005f0: 6e69 6b4d 4366 6f77 4451 594a 4b6f 5a49  nikMCfowDQYJKoZI
+00000600: 6876 634e 4151 454c 0a42 5141 7751 6a45  hvcNAQEL.BQAwQjE
+00000610: 554d 4249 4741 3155 4541 7777 4c51 5739  UMBIGA1UEAwwLQW9
+00000620: 7a49 464a 7662 3351 6751 3045 7844 7a41  zIFJvb3QgQ0ExDzA
+00000630: 4e42 674e 5642 416f 4d42 6b35 3159 5735  NBgNVBAoMBk51YW5
+00000640: 6a5a 5445 4d4d 416f 470a 4131 5545 4377  jZTEMMAoG.A1UECw
+00000650: 7744 5157 397a 4d51 7377 4351 5944 5651  wDQW9zMQswCQYDVQ
+00000660: 5147 4577 4a56 557a 4167 4677 3079 4d44  QGEwJVUzAgFw0yMD
+00000670: 4578 4d54 6378 4d44 4934 4d44 4e61 4741  ExMTcxMDI4MDNaGA
+00000680: 3879 4d44 5577 4d54 4578 0a4d 4445 774d  8yMDUwMTEx.MDEwM
+00000690: 6a67 774d 316f 7751 6a45 554d 4249 4741  jgwM1owQjEUMBIGA
+000006a0: 3155 4541 7777 4c51 5739 7a49 464a 7662  1UEAwwLQW9zIFJvb
+000006b0: 3351 6751 3045 7844 7a41 4e42 674e 5642  3QgQ0ExDzANBgNVB
+000006c0: 416f 4d42 6b35 3159 5735 6a0a 5a54 454d  AoMBk51YW5j.ZTEM
+000006d0: 4d41 6f47 4131 5545 4377 7744 5157 397a  MAoGA1UECwwDQW9z
+000006e0: 4d51 7377 4351 5944 5651 5147 4577 4a56  MQswCQYDVQQGEwJV
+000006f0: 557a 4343 4153 4977 4451 594a 4b6f 5a49  UzCCASIwDQYJKoZI
+00000700: 6876 634e 4151 4542 4251 4144 0a67 6745  hvcNAQEBBQAD.ggE
+00000710: 5041 4443 4341 516f 4367 6745 4241 4e73  PADCCAQoCggEBANs
+00000720: 4a65 624b 4d6f 7232 7844 6c51 7241 3739  JebKMor2xDlQrA79
+00000730: 4566 4c51 3531 596e 6344 745a 6d78 4c4b  EfLQ51YncDtZmxLK
+00000740: 382b 5968 4c78 4c2f 3234 5853 420a 5844  8+YhLxL/24XSB.XD
+00000750: 546f 4447 4c61 7465 6372 7336 3145 5169  ToDGLatecrs61EQi
+00000760: 536f 744c 4f37 496c 5a77 4233 6766 5a55  SotLO7IlZwB3gfZU
+00000770: 4b6d 4c64 5179 5367 5741 6952 5369 686c  KmLdQySgWAiRSihl
+00000780: 7a76 7839 6d30 4348 7353 6648 3365 0a72  zvx9m0CHsSfH3e.r
+00000790: 704a 4c6a 6e6a 6953 365a 4a68 426b 5177  pJLjnjiS6ZJhBkQw
+000007a0: 732b 6241 5669 4e34 795a 7551 7063 4b73  s+bAViN4yZuQpcKs
+000007b0: 7879 6762 3177 7a37 6172 4f79 6c32 6e59  xygb1wz7arOyl2nY
+000007c0: 4544 4d7a 2b68 7964 3863 7337 5531 480a  EDMz+hyd8cs7U1H.
+000007d0: 304a 4a67 4931 7050 4255 4c63 4b65 4c66  0JJgI1pPBULcKeLf
+000007e0: 4347 5047 5a75 6642 3659 6549 6650 5455  CGPGZufB6YeIfPTU
+000007f0: 502f 4345 3439 6862 774d 7548 5868 7044  P/CE49hbwMuHXhpD
+00000800: 6335 4c73 3053 4258 5755 5666 6b42 4d45  c5Ls0SBXWUVfkBME
+00000810: 0a4a 7275 654d 497a 4a52 5177 5532 394e  .JrueMIzJRQwU29N
+00000820: 2b33 3250 6867 624c 5a75 776f 544a 5669  +32PhgbLZuwoTJVi
+00000830: 2b56 634b 5266 4632 4f62 7773 647a 6348  +VcKRfF2ObwsdzcH
+00000840: 3633 6454 4169 796a 4372 4d59 5934 6764  63dTAiyjCrMYY4gd
+00000850: 630a 3230 7562 6a64 796e 5737 7833 6778  c.20ubjdynW7x3gx
+00000860: 4f57 5168 304f 3269 6b6e 692f 4f54 786f  OWQh0O2ikni/OTxo
+00000870: 7a77 5837 386c 7243 4543 4177 4541 4161  zwX78lrCECAwEAAa
+00000880: 4e64 4d46 7377 4441 5944 5652 3054 4241  NdMFswDAYDVR0TBA
+00000890: 5577 0a41 7745 422f 7a41 6442 674e 5648  Uw.AwEB/zAdBgNVH
+000008a0: 5134 4546 6751 554f 656e 4436 5562 4f43  Q4EFgQUOenD6UbOC
+000008b0: 6c49 3344 4d67 4a36 3041 3266 5537 536a  lI3DMgJ60A2fU7Sj
+000008c0: 5938 7748 7759 4456 5230 6a42 4267 7746  Y8wHwYDVR0jBBgwF
+000008d0: 6f41 550a 4f65 6e44 3655 624f 436c 4933  oAU.OenD6UbOClI3
+000008e0: 444d 674a 3630 4132 6655 3753 6a59 3877  DMgJ60A2fU7SjY8w
+000008f0: 4377 5944 5652 3050 4241 5144 4167 4747  CwYDVR0PBAQDAgGG
+00000900: 4d41 3047 4353 7147 5349 6233 4451 4542  MA0GCSqGSIb3DQEB
+00000910: 4377 5541 0a41 3449 4241 5142 5151 6f69  CwUA.A4IBAQBQQoi
+00000920: 3638 6c6d 4541 506d 6373 4941 6958 3367  68lmEAPmcsIAiX3g
+00000930: 696c 6d76 7565 6164 6963 5a65 6f42 4b61  ilmvueadicZeoBKa
+00000940: 4b61 4846 4a6c 4c31 4341 7648 5748 544c  KaHFJlL1CAvHWHTL
+00000950: 6330 474c 720a 6f4c 3358 7156 5735 6971  c0GLr.oL3XqVW5iq
+00000960: 6547 4c38 6575 334f 6d69 6178 5049 5934  eGL8eu3OmiaxPIY4
+00000970: 6632 7a78 6f41 4847 4c54 5933 7572 2f4f  f2zxoAHGLTY3ur/O
+00000980: 3033 4742 5145 326a 4275 5636 754f 7058  03GBQE2jBuV6uOpX
+00000990: 744e 6330 6436 0a58 4470 342f 772f 704d  tNc0d6.XDp4/w/pM
+000009a0: 6345 6458 7337 5439 4f38 6c4c 496a 7976  cEdXs7T9O8lLIjyv
+000009b0: 532b 6866 6f53 4764 3958 346b 4e4b 694d  S+hfoSGd9X4kNKiM
+000009c0: 6135 536d 6f35 5530 566f 414c 4f4d 4667  a5Smo5U0VoALOMFg
+000009d0: 5245 3656 5a46 660a 5771 3245 7575 4154  RE6VZFf.Wq2EuuAT
+000009e0: 4578 3746 435a 6434 506b 634f 4c73 4666  Ex7FCZd4PkcOLsFf
+000009f0: 6f61 4c74 6545 6132 6c57 3435 6f57 4962  oaLteEa2lW45oWIb
+00000a00: 6c6c 4d6e 3365 5779 6f38 2b43 3251 3952  llMn3eWyo8+C2Q9R
+00000a10: 7733 6b62 7a49 6f74 0a32 5962 5059 6b50  w3kbzIot.2YbPYkP
+00000a20: 6273 4633 452f 6352 3455 5a46 386a 4742  bsF3E/cR4UZF8jGB
+00000a30: 6e65 4838 304d 746b 3034 4577 5635 6f62  neH80Mtk04EwV5ob
+00000a40: 6e67 4642 7174 3355 655a 796a 5658 4168  ngFBqt3UeZyjVXAh
+00000a50: 7775 6d5a 7436 522b 4a0a 7246 7a5a 6c64  wumZt6R+J.rFzZld
+00000a60: 4362 6d34 786a 2b70 5246 6879 3546 436b  Cbm4xj+pRFhy5FCk
+00000a70: 4849 7069 506a 0a2d 2d2d 2d2d 454e 4420  HIpiPj.-----END 
+00000a80: 4345 5254 4946 4943 4154 452d 2d2d 2d2d  CERTIFICATE-----
+00000a90: 0a                                       .
```

## aos_prov/files/vm.xml

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: ASCII text, with CRLF line terminators*

```diff
@@ -1,173 +1,169 @@
 00000000: 3c64 6f6d 6169 6e20 7479 7065 3d22 6b76  <domain type="kv
 00000010: 6d22 2078 6d6c 6e73 3a71 656d 753d 2768  m" xmlns:qemu='h
 00000020: 7474 703a 2f2f 6c69 6276 6972 742e 6f72  ttp://libvirt.or
 00000030: 672f 7363 6865 6d61 732f 646f 6d61 696e  g/schemas/domain
-00000040: 2f71 656d 752f 312e 3027 3e0d 0a20 203c  /qemu/1.0'>..  <
-00000050: 6e61 6d65 3e7b 766d 5f6e 616d 657d 3c2f  name>{vm_name}</
-00000060: 6e61 6d65 3e0d 0a20 203c 7575 6964 3e7b  name>..  <uuid>{
-00000070: 7575 6964 7d3c 2f75 7569 643e 0d0a 2020  uuid}</uuid>..  
-00000080: 3c6d 656d 6f72 7920 756e 6974 3d22 4b69  <memory unit="Ki
-00000090: 4222 3e35 3234 3238 383c 2f6d 656d 6f72  B">524288</memor
-000000a0: 793e 0d0a 2020 3c76 6370 753e 313c 2f76  y>..  <vcpu>1</v
-000000b0: 6370 753e 0d0a 2020 3c6f 733e 0d0a 2020  cpu>..  <os>..  
-000000c0: 2020 3c74 7970 6520 6172 6368 3d22 7838    <type arch="x8
-000000d0: 365f 3634 223e 6876 6d3c 2f74 7970 653e  6_64">hvm</type>
-000000e0: 0d0a 2020 2020 3c6c 6f61 6465 7220 7265  ..    <loader re
-000000f0: 6164 6f6e 6c79 3d22 7965 7322 2074 7970  adonly="yes" typ
-00000100: 653d 2270 666c 6173 6822 3e2f 7573 722f  e="pflash">/usr/
-00000110: 7368 6172 652f 4f56 4d46 2f4f 564d 465f  share/OVMF/OVMF_
-00000120: 434f 4445 2e66 643c 2f6c 6f61 6465 723e  CODE.fd</loader>
-00000130: 0d0a 2020 2020 3c6e 7672 616d 3e2f 7661  ..    <nvram>/va
-00000140: 722f 6c69 622f 6c69 6276 6972 742f 7165  r/lib/libvirt/qe
-00000150: 6d75 2f6e 7672 616d 2f76 6d31 5f56 4152  mu/nvram/vm1_VAR
-00000160: 532e 6664 3c2f 6e76 7261 6d3e 0d0a 2020  S.fd</nvram>..  
-00000170: 2020 3c62 6f6f 7420 6465 763d 2268 6422    <boot dev="hd"
-00000180: 2f3e 0d0a 2020 3c2f 6f73 3e0d 0a20 203c  />..  </os>..  <
-00000190: 6665 6174 7572 6573 3e0d 0a20 2020 203c  features>..    <
-000001a0: 6163 7069 2f3e 0d0a 2020 2020 3c61 7069  acpi/>..    <api
-000001b0: 632f 3e0d 0a20 2020 203c 766d 706f 7274  c/>..    <vmport
-000001c0: 2073 7461 7465 3d22 6f66 6622 2f3e 0d0a   state="off"/>..
-000001d0: 2020 3c2f 6665 6174 7572 6573 3e0d 0a20    </features>.. 
-000001e0: 203c 6370 7520 6d6f 6465 3d22 686f 7374   <cpu mode="host
-000001f0: 2d6d 6f64 656c 2220 6368 6563 6b3d 2270  -model" check="p
-00000200: 6172 7469 616c 222f 3e0d 0a20 203c 636c  artial"/>..  <cl
-00000210: 6f63 6b20 6f66 6673 6574 3d22 7574 6322  ock offset="utc"
-00000220: 3e0d 0a20 2020 203c 7469 6d65 7220 6e61  >..    <timer na
-00000230: 6d65 3d22 7274 6322 2074 6963 6b70 6f6c  me="rtc" tickpol
-00000240: 6963 793d 2263 6174 6368 7570 222f 3e0d  icy="catchup"/>.
-00000250: 0a20 2020 203c 7469 6d65 7220 6e61 6d65  .    <timer name
-00000260: 3d22 7069 7422 2074 6963 6b70 6f6c 6963  ="pit" tickpolic
-00000270: 793d 2264 656c 6179 222f 3e0d 0a20 2020  y="delay"/>..   
-00000280: 203c 7469 6d65 7220 6e61 6d65 3d22 6870   <timer name="hp
-00000290: 6574 2220 7072 6573 656e 743d 226e 6f22  et" present="no"
-000002a0: 2f3e 0d0a 2020 3c2f 636c 6f63 6b3e 0d0a  />..  </clock>..
-000002b0: 2020 3c6f 6e5f 706f 7765 726f 6666 3e64    <on_poweroff>d
-000002c0: 6573 7472 6f79 3c2f 6f6e 5f70 6f77 6572  estroy</on_power
-000002d0: 6f66 663e 0d0a 2020 3c6f 6e5f 7265 626f  off>..  <on_rebo
-000002e0: 6f74 3e72 6573 7461 7274 3c2f 6f6e 5f72  ot>restart</on_r
-000002f0: 6562 6f6f 743e 0d0a 2020 3c6f 6e5f 6372  eboot>..  <on_cr
-00000300: 6173 683e 6465 7374 726f 793c 2f6f 6e5f  ash>destroy</on_
-00000310: 6372 6173 683e 0d0a 2020 3c70 6d3e 0d0a  crash>..  <pm>..
-00000320: 2020 2020 3c73 7573 7065 6e64 2d74 6f2d      <suspend-to-
-00000330: 6d65 6d20 656e 6162 6c65 643d 226e 6f22  mem enabled="no"
-00000340: 2f3e 0d0a 2020 2020 3c73 7573 7065 6e64  />..    <suspend
-00000350: 2d74 6f2d 6469 736b 2065 6e61 626c 6564  -to-disk enabled
-00000360: 3d22 6e6f 222f 3e0d 0a20 203c 2f70 6d3e  ="no"/>..  </pm>
-00000370: 0d0a 2020 3c64 6576 6963 6573 3e0d 0a20  ..  <devices>.. 
-00000380: 2020 203c 656d 756c 6174 6f72 3e2f 7573     <emulator>/us
-00000390: 722f 6269 6e2f 7165 6d75 2d73 7973 7465  r/bin/qemu-syste
-000003a0: 6d2d 7838 365f 3634 3c2f 656d 756c 6174  m-x86_64</emulat
-000003b0: 6f72 3e0d 0a20 2020 203c 6469 736b 2074  or>..    <disk t
-000003c0: 7970 653d 2266 696c 6522 2064 6576 6963  ype="file" devic
-000003d0: 653d 2264 6973 6b22 3e0d 0a20 2020 2020  e="disk">..     
-000003e0: 203c 6472 6976 6572 206e 616d 653d 2271   <driver name="q
-000003f0: 656d 7522 2074 7970 653d 2276 6d64 6b22  emu" type="vmdk"
-00000400: 2f3e 0d0a 2020 2020 2020 3c73 6f75 7263  />..      <sourc
-00000410: 6520 6669 6c65 3d22 7b64 6973 6b5f 7061  e file="{disk_pa
-00000420: 7468 7d22 2f3e 0d0a 2020 2020 2020 3c74  th}"/>..      <t
-00000430: 6172 6765 7420 6465 763d 2268 6461 2220  arget dev="hda" 
-00000440: 6275 733d 2269 6465 222f 3e0d 0a20 2020  bus="ide"/>..   
-00000450: 2020 203c 6164 6472 6573 7320 7479 7065     <address type
-00000460: 3d22 6472 6976 6522 2063 6f6e 7472 6f6c  ="drive" control
-00000470: 6c65 723d 2230 2220 6275 733d 2230 2220  ler="0" bus="0" 
-00000480: 7461 7267 6574 3d22 3022 2075 6e69 743d  target="0" unit=
-00000490: 2230 222f 3e0d 0a20 2020 203c 2f64 6973  "0"/>..    </dis
-000004a0: 6b3e 0d0a 2020 2020 3c63 6f6e 7472 6f6c  k>..    <control
-000004b0: 6c65 7220 7479 7065 3d22 7063 6922 2069  ler type="pci" i
-000004c0: 6e64 6578 3d22 3022 206d 6f64 656c 3d22  ndex="0" model="
-000004d0: 7063 692d 726f 6f74 222f 3e0d 0a20 2020  pci-root"/>..   
-000004e0: 203c 636f 6e74 726f 6c6c 6572 2074 7970   <controller typ
-000004f0: 653d 2269 6465 2220 696e 6465 783d 2230  e="ide" index="0
-00000500: 223e 0d0a 2020 2020 2020 3c61 6464 7265  ">..      <addre
-00000510: 7373 2074 7970 653d 2270 6369 2220 646f  ss type="pci" do
-00000520: 6d61 696e 3d22 3078 3030 3030 2220 6275  main="0x0000" bu
-00000530: 733d 2230 7830 3022 2073 6c6f 743d 2230  s="0x00" slot="0
-00000540: 7830 3122 2066 756e 6374 696f 6e3d 2230  x01" function="0
-00000550: 7831 222f 3e0d 0a20 2020 203c 2f63 6f6e  x1"/>..    </con
-00000560: 7472 6f6c 6c65 723e 0d0a 2020 2020 3c63  troller>..    <c
-00000570: 6f6e 7472 6f6c 6c65 7220 7479 7065 3d22  ontroller type="
-00000580: 7669 7274 696f 2d73 6572 6961 6c22 2069  virtio-serial" i
-00000590: 6e64 6578 3d22 3022 3e0d 0a20 2020 2020  ndex="0">..     
-000005a0: 203c 6164 6472 6573 7320 7479 7065 3d22   <address type="
-000005b0: 7063 6922 2064 6f6d 6169 6e3d 2230 7830  pci" domain="0x0
-000005c0: 3030 3022 2062 7573 3d22 3078 3030 2220  000" bus="0x00" 
-000005d0: 736c 6f74 3d22 3078 3036 2220 6675 6e63  slot="0x06" func
-000005e0: 7469 6f6e 3d22 3078 3022 2f3e 0d0a 2020  tion="0x0"/>..  
-000005f0: 2020 3c2f 636f 6e74 726f 6c6c 6572 3e0d    </controller>.
-00000600: 0a20 2020 203c 7365 7269 616c 2074 7970  .    <serial typ
-00000610: 653d 2270 7479 223e 0d0a 2020 2020 2020  e="pty">..      
-00000620: 3c74 6172 6765 7420 7479 7065 3d22 6973  <target type="is
-00000630: 612d 7365 7269 616c 2220 706f 7274 3d22  a-serial" port="
-00000640: 3022 3e0d 0a20 2020 2020 2020 203c 6d6f  0">..        <mo
-00000650: 6465 6c20 6e61 6d65 3d22 6973 612d 7365  del name="isa-se
-00000660: 7269 616c 222f 3e0d 0a20 2020 2020 203c  rial"/>..      <
-00000670: 2f74 6172 6765 743e 0d0a 2020 2020 3c2f  /target>..    </
-00000680: 7365 7269 616c 3e0d 0a20 2020 203c 636f  serial>..    <co
-00000690: 6e73 6f6c 6520 7479 7065 3d22 7074 7922  nsole type="pty"
-000006a0: 3e0d 0a20 2020 2020 203c 7461 7267 6574  >..      <target
-000006b0: 2074 7970 653d 2273 6572 6961 6c22 2070   type="serial" p
-000006c0: 6f72 743d 2230 222f 3e0d 0a20 2020 203c  ort="0"/>..    <
-000006d0: 2f63 6f6e 736f 6c65 3e0d 0a20 2020 203c  /console>..    <
-000006e0: 6368 616e 6e65 6c20 7479 7065 3d22 7370  channel type="sp
-000006f0: 6963 6576 6d63 223e 0d0a 2020 2020 2020  icevmc">..      
-00000700: 3c74 6172 6765 7420 7479 7065 3d22 7669  <target type="vi
-00000710: 7274 696f 2220 6e61 6d65 3d22 636f 6d2e  rtio" name="com.
-00000720: 7265 6468 6174 2e73 7069 6365 2e30 222f  redhat.spice.0"/
-00000730: 3e0d 0a20 2020 2020 203c 6164 6472 6573  >..      <addres
-00000740: 7320 7479 7065 3d22 7669 7274 696f 2d73  s type="virtio-s
-00000750: 6572 6961 6c22 2063 6f6e 7472 6f6c 6c65  erial" controlle
-00000760: 723d 2230 2220 6275 733d 2230 2220 706f  r="0" bus="0" po
-00000770: 7274 3d22 3122 2f3e 0d0a 2020 2020 3c2f  rt="1"/>..    </
-00000780: 6368 616e 6e65 6c3e 0d0a 2020 2020 3c69  channel>..    <i
-00000790: 6e70 7574 2074 7970 653d 226d 6f75 7365  nput type="mouse
-000007a0: 2220 6275 733d 2270 7332 222f 3e0d 0a20  " bus="ps2"/>.. 
-000007b0: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
-000007c0: 6b65 7962 6f61 7264 2220 6275 733d 2270  keyboard" bus="p
-000007d0: 7332 222f 3e0d 0a20 2020 203c 6772 6170  s2"/>..    <grap
-000007e0: 6869 6373 2074 7970 653d 2273 7069 6365  hics type="spice
-000007f0: 2220 6175 746f 706f 7274 3d22 7965 7322  " autoport="yes"
-00000800: 3e0d 0a20 2020 2020 203c 6c69 7374 656e  >..      <listen
-00000810: 2074 7970 653d 2261 6464 7265 7373 222f   type="address"/
-00000820: 3e0d 0a20 2020 2020 203c 696d 6167 6520  >..      <image 
-00000830: 636f 6d70 7265 7373 696f 6e3d 226f 6666  compression="off
-00000840: 222f 3e0d 0a20 2020 203c 2f67 7261 7068  "/>..    </graph
-00000850: 6963 733e 0d0a 2020 2020 3c76 6964 656f  ics>..    <video
-00000860: 3e0d 0a20 2020 2020 203c 6d6f 6465 6c20  >..      <model 
-00000870: 7479 7065 3d22 7178 6c22 2072 616d 3d22  type="qxl" ram="
-00000880: 3635 3533 3622 2076 7261 6d3d 2236 3535  65536" vram="655
-00000890: 3336 2220 7667 616d 656d 3d22 3136 3338  36" vgamem="1638
-000008a0: 3422 2068 6561 6473 3d22 3122 2070 7269  4" heads="1" pri
-000008b0: 6d61 7279 3d22 7965 7322 2f3e 0d0a 2020  mary="yes"/>..  
-000008c0: 2020 2020 3c61 6464 7265 7373 2074 7970      <address typ
-000008d0: 653d 2270 6369 2220 646f 6d61 696e 3d22  e="pci" domain="
-000008e0: 3078 3030 3030 2220 6275 733d 2230 7830  0x0000" bus="0x0
-000008f0: 3022 2073 6c6f 743d 2230 7830 3222 2066  0" slot="0x02" f
-00000900: 756e 6374 696f 6e3d 2230 7830 222f 3e0d  unction="0x0"/>.
-00000910: 0a20 2020 203c 2f76 6964 656f 3e0d 0a20  .    </video>.. 
-00000920: 2020 203c 6d65 6d62 616c 6c6f 6f6e 206d     <memballoon m
-00000930: 6f64 656c 3d22 7669 7274 696f 223e 0d0a  odel="virtio">..
-00000940: 2020 2020 2020 3c61 6464 7265 7373 2074        <address t
-00000950: 7970 653d 2270 6369 2220 646f 6d61 696e  ype="pci" domain
-00000960: 3d22 3078 3030 3030 2220 6275 733d 2230  ="0x0000" bus="0
-00000970: 7830 3022 2073 6c6f 743d 2230 7830 3722  x00" slot="0x07"
-00000980: 2066 756e 6374 696f 6e3d 2230 7830 222f   function="0x0"/
-00000990: 3e0d 0a20 2020 203c 2f6d 656d 6261 6c6c  >..    </memball
-000009a0: 6f6f 6e3e 0d0a 2020 3c2f 6465 7669 6365  oon>..  </device
-000009b0: 733e 0d0a 2020 3c71 656d 753a 636f 6d6d  s>..  <qemu:comm
-000009c0: 616e 646c 696e 653e 0d0a 2020 2020 3c71  andline>..    <q
-000009d0: 656d 753a 6172 6720 7661 6c75 653d 272d  emu:arg value='-
-000009e0: 6e65 7464 6576 272f 3e0d 0a20 2020 203c  netdev'/>..    <
-000009f0: 7165 6d75 3a61 7267 2076 616c 7565 3d27  qemu:arg value='
-00000a00: 7573 6572 2c69 643d 706f 7274 666f 7277  user,id=portforw
-00000a10: 6172 6469 6e67 6e69 632c 686f 7374 6677  ardingnic,hostfw
-00000a20: 643d 7463 703a 3a7b 706f 7274 5f66 6f72  d=tcp::{port_for
-00000a30: 7761 7264 7d2d 3a38 3038 3927 2f3e 0d0a  ward}-:8089'/>..
-00000a40: 2020 2020 3c71 656d 753a 6172 6720 7661      <qemu:arg va
-00000a50: 6c75 653d 272d 6465 7669 6365 272f 3e0d  lue='-device'/>.
-00000a60: 0a20 2020 203c 7165 6d75 3a61 7267 2076  .    <qemu:arg v
-00000a70: 616c 7565 3d27 7274 6c38 3133 392c 6e65  alue='rtl8139,ne
-00000a80: 7464 6576 3d70 6f72 7466 6f72 7761 7264  tdev=portforward
-00000a90: 696e 676e 6963 2c6d 6163 3d7b 6d61 635f  ingnic,mac={mac_
-00000aa0: 6164 6472 6573 737d 272f 3e0d 0a20 203c  address}'/>..  <
-00000ab0: 2f71 656d 753a 636f 6d6d 616e 646c 696e  /qemu:commandlin
-00000ac0: 653e 0d0a 3c2f 646f 6d61 696e 3e0d 0a    e>..</domain>..
+00000040: 2f71 656d 752f 312e 3027 3e0a 2020 3c6e  /qemu/1.0'>.  <n
+00000050: 616d 653e 7b76 6d5f 6e61 6d65 7d3c 2f6e  ame>{vm_name}</n
+00000060: 616d 653e 0a20 203c 7575 6964 3e7b 7575  ame>.  <uuid>{uu
+00000070: 6964 7d3c 2f75 7569 643e 0a20 203c 6d65  id}</uuid>.  <me
+00000080: 6d6f 7279 2075 6e69 743d 224b 6942 223e  mory unit="KiB">
+00000090: 3532 3432 3838 3c2f 6d65 6d6f 7279 3e0a  524288</memory>.
+000000a0: 2020 3c76 6370 753e 313c 2f76 6370 753e    <vcpu>1</vcpu>
+000000b0: 0a20 203c 6f73 3e0a 2020 2020 3c74 7970  .  <os>.    <typ
+000000c0: 6520 6172 6368 3d22 7838 365f 3634 223e  e arch="x86_64">
+000000d0: 6876 6d3c 2f74 7970 653e 0a20 2020 203c  hvm</type>.    <
+000000e0: 6c6f 6164 6572 2072 6561 646f 6e6c 793d  loader readonly=
+000000f0: 2279 6573 2220 7479 7065 3d22 7066 6c61  "yes" type="pfla
+00000100: 7368 223e 2f75 7372 2f73 6861 7265 2f4f  sh">/usr/share/O
+00000110: 564d 462f 4f56 4d46 5f43 4f44 452e 6664  VMF/OVMF_CODE.fd
+00000120: 3c2f 6c6f 6164 6572 3e0a 2020 2020 3c6e  </loader>.    <n
+00000130: 7672 616d 3e2f 7661 722f 6c69 622f 6c69  vram>/var/lib/li
+00000140: 6276 6972 742f 7165 6d75 2f6e 7672 616d  bvirt/qemu/nvram
+00000150: 2f76 6d31 5f56 4152 532e 6664 3c2f 6e76  /vm1_VARS.fd</nv
+00000160: 7261 6d3e 0a20 2020 203c 626f 6f74 2064  ram>.    <boot d
+00000170: 6576 3d22 6864 222f 3e0a 2020 3c2f 6f73  ev="hd"/>.  </os
+00000180: 3e0a 2020 3c66 6561 7475 7265 733e 0a20  >.  <features>. 
+00000190: 2020 203c 6163 7069 2f3e 0a20 2020 203c     <acpi/>.    <
+000001a0: 6170 6963 2f3e 0a20 2020 203c 766d 706f  apic/>.    <vmpo
+000001b0: 7274 2073 7461 7465 3d22 6f66 6622 2f3e  rt state="off"/>
+000001c0: 0a20 203c 2f66 6561 7475 7265 733e 0a20  .  </features>. 
+000001d0: 203c 6370 7520 6d6f 6465 3d22 686f 7374   <cpu mode="host
+000001e0: 2d6d 6f64 656c 2220 6368 6563 6b3d 2270  -model" check="p
+000001f0: 6172 7469 616c 222f 3e0a 2020 3c63 6c6f  artial"/>.  <clo
+00000200: 636b 206f 6666 7365 743d 2275 7463 223e  ck offset="utc">
+00000210: 0a20 2020 203c 7469 6d65 7220 6e61 6d65  .    <timer name
+00000220: 3d22 7274 6322 2074 6963 6b70 6f6c 6963  ="rtc" tickpolic
+00000230: 793d 2263 6174 6368 7570 222f 3e0a 2020  y="catchup"/>.  
+00000240: 2020 3c74 696d 6572 206e 616d 653d 2270    <timer name="p
+00000250: 6974 2220 7469 636b 706f 6c69 6379 3d22  it" tickpolicy="
+00000260: 6465 6c61 7922 2f3e 0a20 2020 203c 7469  delay"/>.    <ti
+00000270: 6d65 7220 6e61 6d65 3d22 6870 6574 2220  mer name="hpet" 
+00000280: 7072 6573 656e 743d 226e 6f22 2f3e 0a20  present="no"/>. 
+00000290: 203c 2f63 6c6f 636b 3e0a 2020 3c6f 6e5f   </clock>.  <on_
+000002a0: 706f 7765 726f 6666 3e64 6573 7472 6f79  poweroff>destroy
+000002b0: 3c2f 6f6e 5f70 6f77 6572 6f66 663e 0a20  </on_poweroff>. 
+000002c0: 203c 6f6e 5f72 6562 6f6f 743e 7265 7374   <on_reboot>rest
+000002d0: 6172 743c 2f6f 6e5f 7265 626f 6f74 3e0a  art</on_reboot>.
+000002e0: 2020 3c6f 6e5f 6372 6173 683e 6465 7374    <on_crash>dest
+000002f0: 726f 793c 2f6f 6e5f 6372 6173 683e 0a20  roy</on_crash>. 
+00000300: 203c 706d 3e0a 2020 2020 3c73 7573 7065   <pm>.    <suspe
+00000310: 6e64 2d74 6f2d 6d65 6d20 656e 6162 6c65  nd-to-mem enable
+00000320: 643d 226e 6f22 2f3e 0a20 2020 203c 7375  d="no"/>.    <su
+00000330: 7370 656e 642d 746f 2d64 6973 6b20 656e  spend-to-disk en
+00000340: 6162 6c65 643d 226e 6f22 2f3e 0a20 203c  abled="no"/>.  <
+00000350: 2f70 6d3e 0a20 203c 6465 7669 6365 733e  /pm>.  <devices>
+00000360: 0a20 2020 203c 656d 756c 6174 6f72 3e2f  .    <emulator>/
+00000370: 7573 722f 6269 6e2f 7165 6d75 2d73 7973  usr/bin/qemu-sys
+00000380: 7465 6d2d 7838 365f 3634 3c2f 656d 756c  tem-x86_64</emul
+00000390: 6174 6f72 3e0a 2020 2020 3c64 6973 6b20  ator>.    <disk 
+000003a0: 7479 7065 3d22 6669 6c65 2220 6465 7669  type="file" devi
+000003b0: 6365 3d22 6469 736b 223e 0a20 2020 2020  ce="disk">.     
+000003c0: 203c 6472 6976 6572 206e 616d 653d 2271   <driver name="q
+000003d0: 656d 7522 2074 7970 653d 2276 6d64 6b22  emu" type="vmdk"
+000003e0: 2f3e 0a20 2020 2020 203c 736f 7572 6365  />.      <source
+000003f0: 2066 696c 653d 227b 6469 736b 5f70 6174   file="{disk_pat
+00000400: 687d 222f 3e0a 2020 2020 2020 3c74 6172  h}"/>.      <tar
+00000410: 6765 7420 6465 763d 2268 6461 2220 6275  get dev="hda" bu
+00000420: 733d 2269 6465 222f 3e0a 2020 2020 2020  s="ide"/>.      
+00000430: 3c61 6464 7265 7373 2074 7970 653d 2264  <address type="d
+00000440: 7269 7665 2220 636f 6e74 726f 6c6c 6572  rive" controller
+00000450: 3d22 3022 2062 7573 3d22 3022 2074 6172  ="0" bus="0" tar
+00000460: 6765 743d 2230 2220 756e 6974 3d22 3022  get="0" unit="0"
+00000470: 2f3e 0a20 2020 203c 2f64 6973 6b3e 0a20  />.    </disk>. 
+00000480: 2020 203c 636f 6e74 726f 6c6c 6572 2074     <controller t
+00000490: 7970 653d 2270 6369 2220 696e 6465 783d  ype="pci" index=
+000004a0: 2230 2220 6d6f 6465 6c3d 2270 6369 2d72  "0" model="pci-r
+000004b0: 6f6f 7422 2f3e 0a20 2020 203c 636f 6e74  oot"/>.    <cont
+000004c0: 726f 6c6c 6572 2074 7970 653d 2269 6465  roller type="ide
+000004d0: 2220 696e 6465 783d 2230 223e 0a20 2020  " index="0">.   
+000004e0: 2020 203c 6164 6472 6573 7320 7479 7065     <address type
+000004f0: 3d22 7063 6922 2064 6f6d 6169 6e3d 2230  ="pci" domain="0
+00000500: 7830 3030 3022 2062 7573 3d22 3078 3030  x0000" bus="0x00
+00000510: 2220 736c 6f74 3d22 3078 3031 2220 6675  " slot="0x01" fu
+00000520: 6e63 7469 6f6e 3d22 3078 3122 2f3e 0a20  nction="0x1"/>. 
+00000530: 2020 203c 2f63 6f6e 7472 6f6c 6c65 723e     </controller>
+00000540: 0a20 2020 203c 636f 6e74 726f 6c6c 6572  .    <controller
+00000550: 2074 7970 653d 2276 6972 7469 6f2d 7365   type="virtio-se
+00000560: 7269 616c 2220 696e 6465 783d 2230 223e  rial" index="0">
+00000570: 0a20 2020 2020 203c 6164 6472 6573 7320  .      <address 
+00000580: 7479 7065 3d22 7063 6922 2064 6f6d 6169  type="pci" domai
+00000590: 6e3d 2230 7830 3030 3022 2062 7573 3d22  n="0x0000" bus="
+000005a0: 3078 3030 2220 736c 6f74 3d22 3078 3036  0x00" slot="0x06
+000005b0: 2220 6675 6e63 7469 6f6e 3d22 3078 3022  " function="0x0"
+000005c0: 2f3e 0a20 2020 203c 2f63 6f6e 7472 6f6c  />.    </control
+000005d0: 6c65 723e 0a20 2020 203c 7365 7269 616c  ler>.    <serial
+000005e0: 2074 7970 653d 2270 7479 223e 0a20 2020   type="pty">.   
+000005f0: 2020 203c 7461 7267 6574 2074 7970 653d     <target type=
+00000600: 2269 7361 2d73 6572 6961 6c22 2070 6f72  "isa-serial" por
+00000610: 743d 2230 223e 0a20 2020 2020 2020 203c  t="0">.        <
+00000620: 6d6f 6465 6c20 6e61 6d65 3d22 6973 612d  model name="isa-
+00000630: 7365 7269 616c 222f 3e0a 2020 2020 2020  serial"/>.      
+00000640: 3c2f 7461 7267 6574 3e0a 2020 2020 3c2f  </target>.    </
+00000650: 7365 7269 616c 3e0a 2020 2020 3c63 6f6e  serial>.    <con
+00000660: 736f 6c65 2074 7970 653d 2270 7479 223e  sole type="pty">
+00000670: 0a20 2020 2020 203c 7461 7267 6574 2074  .      <target t
+00000680: 7970 653d 2273 6572 6961 6c22 2070 6f72  ype="serial" por
+00000690: 743d 2230 222f 3e0a 2020 2020 3c2f 636f  t="0"/>.    </co
+000006a0: 6e73 6f6c 653e 0a20 2020 203c 6368 616e  nsole>.    <chan
+000006b0: 6e65 6c20 7479 7065 3d22 7370 6963 6576  nel type="spicev
+000006c0: 6d63 223e 0a20 2020 2020 203c 7461 7267  mc">.      <targ
+000006d0: 6574 2074 7970 653d 2276 6972 7469 6f22  et type="virtio"
+000006e0: 206e 616d 653d 2263 6f6d 2e72 6564 6861   name="com.redha
+000006f0: 742e 7370 6963 652e 3022 2f3e 0a20 2020  t.spice.0"/>.   
+00000700: 2020 203c 6164 6472 6573 7320 7479 7065     <address type
+00000710: 3d22 7669 7274 696f 2d73 6572 6961 6c22  ="virtio-serial"
+00000720: 2063 6f6e 7472 6f6c 6c65 723d 2230 2220   controller="0" 
+00000730: 6275 733d 2230 2220 706f 7274 3d22 3122  bus="0" port="1"
+00000740: 2f3e 0a20 2020 203c 2f63 6861 6e6e 656c  />.    </channel
+00000750: 3e0a 2020 2020 3c69 6e70 7574 2074 7970  >.    <input typ
+00000760: 653d 226d 6f75 7365 2220 6275 733d 2270  e="mouse" bus="p
+00000770: 7332 222f 3e0a 2020 2020 3c69 6e70 7574  s2"/>.    <input
+00000780: 2074 7970 653d 226b 6579 626f 6172 6422   type="keyboard"
+00000790: 2062 7573 3d22 7073 3222 2f3e 0a20 2020   bus="ps2"/>.   
+000007a0: 203c 6772 6170 6869 6373 2074 7970 653d   <graphics type=
+000007b0: 2273 7069 6365 2220 6175 746f 706f 7274  "spice" autoport
+000007c0: 3d22 7965 7322 3e0a 2020 2020 2020 3c6c  ="yes">.      <l
+000007d0: 6973 7465 6e20 7479 7065 3d22 6164 6472  isten type="addr
+000007e0: 6573 7322 2f3e 0a20 2020 2020 203c 696d  ess"/>.      <im
+000007f0: 6167 6520 636f 6d70 7265 7373 696f 6e3d  age compression=
+00000800: 226f 6666 222f 3e0a 2020 2020 3c2f 6772  "off"/>.    </gr
+00000810: 6170 6869 6373 3e0a 2020 2020 3c76 6964  aphics>.    <vid
+00000820: 656f 3e0a 2020 2020 2020 3c6d 6f64 656c  eo>.      <model
+00000830: 2074 7970 653d 2271 786c 2220 7261 6d3d   type="qxl" ram=
+00000840: 2236 3535 3336 2220 7672 616d 3d22 3635  "65536" vram="65
+00000850: 3533 3622 2076 6761 6d65 6d3d 2231 3633  536" vgamem="163
+00000860: 3834 2220 6865 6164 733d 2231 2220 7072  84" heads="1" pr
+00000870: 696d 6172 793d 2279 6573 222f 3e0a 2020  imary="yes"/>.  
+00000880: 2020 2020 3c61 6464 7265 7373 2074 7970      <address typ
+00000890: 653d 2270 6369 2220 646f 6d61 696e 3d22  e="pci" domain="
+000008a0: 3078 3030 3030 2220 6275 733d 2230 7830  0x0000" bus="0x0
+000008b0: 3022 2073 6c6f 743d 2230 7830 3222 2066  0" slot="0x02" f
+000008c0: 756e 6374 696f 6e3d 2230 7830 222f 3e0a  unction="0x0"/>.
+000008d0: 2020 2020 3c2f 7669 6465 6f3e 0a20 2020      </video>.   
+000008e0: 203c 6d65 6d62 616c 6c6f 6f6e 206d 6f64   <memballoon mod
+000008f0: 656c 3d22 7669 7274 696f 223e 0a20 2020  el="virtio">.   
+00000900: 2020 203c 6164 6472 6573 7320 7479 7065     <address type
+00000910: 3d22 7063 6922 2064 6f6d 6169 6e3d 2230  ="pci" domain="0
+00000920: 7830 3030 3022 2062 7573 3d22 3078 3030  x0000" bus="0x00
+00000930: 2220 736c 6f74 3d22 3078 3037 2220 6675  " slot="0x07" fu
+00000940: 6e63 7469 6f6e 3d22 3078 3022 2f3e 0a20  nction="0x0"/>. 
+00000950: 2020 203c 2f6d 656d 6261 6c6c 6f6f 6e3e     </memballoon>
+00000960: 0a20 203c 2f64 6576 6963 6573 3e0a 2020  .  </devices>.  
+00000970: 3c71 656d 753a 636f 6d6d 616e 646c 696e  <qemu:commandlin
+00000980: 653e 0a20 2020 203c 7165 6d75 3a61 7267  e>.    <qemu:arg
+00000990: 2076 616c 7565 3d27 2d6e 6574 6465 7627   value='-netdev'
+000009a0: 2f3e 0a20 2020 203c 7165 6d75 3a61 7267  />.    <qemu:arg
+000009b0: 2076 616c 7565 3d27 7573 6572 2c69 643d   value='user,id=
+000009c0: 706f 7274 666f 7277 6172 6469 6e67 6e69  portforwardingni
+000009d0: 632c 686f 7374 6677 643d 7463 703a 3a7b  c,hostfwd=tcp::{
+000009e0: 706f 7274 5f66 6f72 7761 7264 7d2d 3a38  port_forward}-:8
+000009f0: 3038 3927 2f3e 0a20 2020 203c 7165 6d75  089'/>.    <qemu
+00000a00: 3a61 7267 2076 616c 7565 3d27 2d64 6576  :arg value='-dev
+00000a10: 6963 6527 2f3e 0a20 2020 203c 7165 6d75  ice'/>.    <qemu
+00000a20: 3a61 7267 2076 616c 7565 3d27 7274 6c38  :arg value='rtl8
+00000a30: 3133 392c 6e65 7464 6576 3d70 6f72 7466  139,netdev=portf
+00000a40: 6f72 7761 7264 696e 676e 6963 2c6d 6163  orwardingnic,mac
+00000a50: 3d7b 6d61 635f 6164 6472 6573 737d 272f  ={mac_address}'/
+00000a60: 3e0a 2020 3c2f 7165 6d75 3a63 6f6d 6d61  >.  </qemu:comma
+00000a70: 6e64 6c69 6e65 3e0a 3c2f 646f 6d61 696e  ndline>.</domain
+00000a80: 3e0a                                     >.
```

## aos_prov/utils/__init__.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
-
-import os
-
-# SDK home directory name
-SDK_TOOL_DIR_NAME = '.aos'
-# SDK home directory full path
-SDK_FULL_PATH = os.path.join(os.path.expanduser("~"), SDK_TOOL_DIR_NAME)
-# Default directory with user keys and certificates
-SDK_SECURITY_PATH = os.path.join(SDK_FULL_PATH, 'security')
-
-# Default user certificate filename
-USER_CERTIFICATE_FILE_NAME = 'oem-client.pem'
-# Default user key filename
-USER_KEY_FILE_NAME = 'private_key.pem'
-
-# Default user certificate full path
-DEFAULT_USER_CERT_PATH = os.path.join(SDK_SECURITY_PATH, USER_CERTIFICATE_FILE_NAME)
-# Default user key full path
-DEFAULT_USER_KEY_PATH = os.path.join(SDK_SECURITY_PATH, USER_KEY_FILE_NAME)
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+
+import os
+
+# SDK home directory name
+SDK_TOOL_DIR_NAME = '.aos'
+# SDK home directory full path
+SDK_FULL_PATH = os.path.join(os.path.expanduser("~"), SDK_TOOL_DIR_NAME)
+# Default directory with user keys and certificates
+SDK_SECURITY_PATH = os.path.join(SDK_FULL_PATH, 'security')
+
+# Default user certificate filename
+USER_CERTIFICATE_FILE_NAME = 'oem-client.pem'
+# Default user key filename
+USER_KEY_FILE_NAME = 'private_key.pem'
+
+# Default user certificate full path
+DEFAULT_USER_CERT_PATH = os.path.join(SDK_SECURITY_PATH, USER_CERTIFICATE_FILE_NAME)
+# Default user key full path
+DEFAULT_USER_KEY_PATH = os.path.join(SDK_SECURITY_PATH, USER_KEY_FILE_NAME)
```

## aos_prov/utils/common.py

```diff
@@ -1,36 +1,50 @@
 #
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
 #
 
 import random
 import string
 from pathlib import Path
 
 from rich.console import Console
 
 CONTENT_ENCRYPTION_ALGORITHM = 'aes256_cbc'
 DOWNLOADS_PATH = Path.home() / '.aos' / 'downloads'
-AOS_DISK_PATH = DOWNLOADS_PATH / 'aos-disk.vmdk'
 AOS_DISKS_PATH = DOWNLOADS_PATH
-VBOX_SDK_PATH = DOWNLOADS_PATH / 'vbox-sdk.zip'
+NODE0_IMAGE_FILENAME = 'aos-vm-node0-genericx86-64.wic.vmdk'
+NODE1_IMAGE_FILENAME = 'aos-vm-node1-genericx86-64.wic.vmdk'
 
-# DISK_IMAGE_DOWNLOAD_URL = 'https://aos-prod-cdn-endpoint.azureedge.net/vm/aos-image-vm-genericx86-64_3.0.1.wic.vmdk' \
-#                           '.gz?0b4230d66ef2f41ec6b9bbc796ff2b938d5a317b9009c6a2474fb2c24e86a127a05b5d535a0d115bcd729' \
-#                           '79c3c78413c9ef5176e48a41361eacf458d20e071d696cd048e072025192f256428051c6d526c2fe6d55c34' \
-#                           'd46a130945cb73813a'
-
-DISK_IMAGE_DOWNLOAD_URL = 'https://aos-prod-cdn-endpoint.azureedge.net/vm/aos-unit-two-nodes-R4.0.1.tar.gz' \
-                          '?0b423ef722c6ce5e7a8a02625179b0e36ea045d977b0be0ce8dad6327fbe9410d8fac497e4169c' \
-                          'c1a7810156d077954105258e7211ef5130b544063ed90c177cba28eb24bd5584a6900e382f1991'
-VIRTUAL_BOX_DOWNLOAD_URL = 'https://download.virtualbox.org/virtualbox/6.1.32/VirtualBoxSDK-6.1.32-149290.zip'
+DISK_IMAGE_DOWNLOAD_URL = 'https://aos-prod-cdn-endpoint.azureedge.net/vm/R4.0.5.tar.gz?' \
+                          '0b4212dd0fd3cf5e29e44f35e2b3fafa474156bf99a8b9399de3b40bb0586a' \
+                          '0822e3a9396e05a96aed7f8e79650aeabdd0abe0d1876b2a621c37e28ebc' \
 
 console = Console()
+error_console = Console(stderr=True, style='red')
+allow_print = True
 
+def print_message(formatted_text, end="\n", ljust: int = 0):
+    if allow_print:
+        if ljust > 0:
+            formatted_text = formatted_text.ljust(ljust)
+        console.print(formatted_text, end=end)
+
+def print_left(formatted_text, ljust=60):
+    print_message(formatted_text, end='', ljust = ljust)
+
+def print_done():
+    print_message('[green]DONE')
+
+def print_success(message):
+    print_message(f'[green]{str(message)}')
+
+def print_error(message):
+    if allow_print:
+        error_console.print(message)
 
 def generate_random_password() -> str:
     """
     Generate random password from letters and digits.
 
     Returns:
         str: Random string password
```

## aos_prov/utils/config.py

 * *Ordering differences only*

```diff
@@ -1,88 +1,88 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-
-class Config(object):
-    """Contains a provisioning procedure configuration."""
-
-    def __init__(self):
-        self._system_id = None
-        self._model_name = None
-        self._model_version = None
-        self._user_claim = None
-        self._supported_cert_types = None
-        self._protocol_version = None
-        self._node_ids = None
-        self._unit_certificates = []
-
-    @property
-    def system_id(self) -> str:
-        """Return System ID of the Unit."""
-        return self._system_id
-
-    @system_id.setter
-    def system_id(self, sys_id):
-        self._system_id = sys_id
-
-    @property
-    def model_name(self) -> str:
-        """Return Model/Board Name of the Unit. It is defined by the manufacturer."""
-        return self._model_name
-
-    @property
-    def model_version(self) -> str:
-        """Return Model/Board Version or Revision of the Unit. It is defined by the manufacturer."""
-        return self._model_version
-
-    @property
-    def supported_cert_types(self) -> [str]:
-        """Return list of certificate names to be set on the Unit."""
-        return self._supported_cert_types
-
-    @supported_cert_types.setter
-    def supported_cert_types(self, cert_types):
-        self._supported_cert_types = cert_types
-
-    @property
-    def protocol_version(self) -> int:
-        """Return api version."""
-        return self._protocol_version
-
-    @protocol_version.setter
-    def protocol_version(self, protocol_version):
-        self._protocol_version = protocol_version
-
-    @property
-    def node_ids(self) -> [str]:
-        """Return list of node Ids."""
-        return self._node_ids
-
-    @node_ids.setter
-    def node_ids(self, node_ids):
-        self._node_ids = node_ids
-
-    @property
-    def unit_certificates(self) -> [UnitCertificate]:
-        """Return list of Unit certificates objects."""
-        return self._unit_certificates
-
-    @unit_certificates.setter
-    def unit_certificates(self, unit_certs):
-        self._unit_certificates = unit_certs
-
-    def set_model(self, model_string):
-        """Parse model name and version received from the Unit.
-
-        Args:
-            model_string: model info returned by Unit.
-        """
-        model_chunks = model_string.strip().split(';')
-        self._model_name = model_chunks[0].strip()
-        if len(model_chunks) > 1:
-            self._model_version = model_chunks[1].strip()
-        else:
-            self._model_version = 'Unknown'
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+
+class Config(object):
+    """Contains a provisioning procedure configuration."""
+
+    def __init__(self):
+        self._system_id = None
+        self._model_name = None
+        self._model_version = None
+        self._user_claim = None
+        self._supported_cert_types = None
+        self._protocol_version = None
+        self._node_ids = None
+        self._unit_certificates = []
+
+    @property
+    def system_id(self) -> str:
+        """Return System ID of the Unit."""
+        return self._system_id
+
+    @system_id.setter
+    def system_id(self, sys_id):
+        self._system_id = sys_id
+
+    @property
+    def model_name(self) -> str:
+        """Return Model/Board Name of the Unit. It is defined by the manufacturer."""
+        return self._model_name
+
+    @property
+    def model_version(self) -> str:
+        """Return Model/Board Version or Revision of the Unit. It is defined by the manufacturer."""
+        return self._model_version
+
+    @property
+    def supported_cert_types(self) -> [str]:
+        """Return list of certificate names to be set on the Unit."""
+        return self._supported_cert_types
+
+    @supported_cert_types.setter
+    def supported_cert_types(self, cert_types):
+        self._supported_cert_types = cert_types
+
+    @property
+    def protocol_version(self) -> int:
+        """Return api version."""
+        return self._protocol_version
+
+    @protocol_version.setter
+    def protocol_version(self, protocol_version):
+        self._protocol_version = protocol_version
+
+    @property
+    def node_ids(self) -> [str]:
+        """Return list of node Ids."""
+        return self._node_ids
+
+    @node_ids.setter
+    def node_ids(self, node_ids):
+        self._node_ids = node_ids
+
+    @property
+    def unit_certificates(self) -> [UnitCertificate]:
+        """Return list of Unit certificates objects."""
+        return self._unit_certificates
+
+    @unit_certificates.setter
+    def unit_certificates(self, unit_certs):
+        self._unit_certificates = unit_certs
+
+    def set_model(self, model_string):
+        """Parse model name and version received from the Unit.
+
+        Args:
+            model_string: model info returned by Unit.
+        """
+        model_chunks = model_string.strip().split(';')
+        self._model_name = model_chunks[0].strip()
+        if len(model_chunks) > 1:
+            self._model_version = model_chunks[1].strip()
+        else:
+            self._model_version = 'Unknown'
```

## aos_prov/utils/errors.py

 * *Ordering differences only*

```diff
@@ -1,36 +1,36 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-
-
-class OnBoardingError(Exception):
-    pass
-
-
-class UserCredentialsError(OnBoardingError):
-    pass
-
-
-class DeviceRegisterError(OnBoardingError):
-    pass
-
-
-class DeviceDeregisterError(OnBoardingError):
-    pass
-
-
-class BoardError(OnBoardingError):
-    pass
-
-
-class GrpcUnimplemented(OnBoardingError):
-    pass
-
-
-class CloudAccessError(OnBoardingError):
-    pass
-
-
-class AosProvError(OnBoardingError):
-    pass
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+
+
+class OnBoardingError(Exception):
+    pass
+
+
+class UserCredentialsError(OnBoardingError):
+    pass
+
+
+class DeviceRegisterError(OnBoardingError):
+    pass
+
+
+class DeviceDeregisterError(OnBoardingError):
+    pass
+
+
+class BoardError(OnBoardingError):
+    pass
+
+
+class GrpcUnimplemented(OnBoardingError):
+    pass
+
+
+class CloudAccessError(OnBoardingError):
+    pass
+
+
+class AosProvError(OnBoardingError):
+    pass
```

## aos_prov/utils/unit_certificate.py

 * *Ordering differences only*

```diff
@@ -1,53 +1,53 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-
-"""Unit certificate object."""
-
-
-class UnitCertificate:
-    """Unit certificate object."""
-
-    def __init__(self):
-        """Unit certificate object."""
-        self._cert_type = None
-        self._csr = None
-        self._node_id = None
-        self._certificate = None
-
-    @property
-    def cert_type(self) -> str:
-        """Certificate type (Required type list is taken from unit)."""
-        return self._cert_type
-
-    @cert_type.setter
-    def cert_type(self, cert_type):
-        self._cert_type = cert_type
-
-    @property
-    def csr(self) -> str:
-        """Certificate Signing Request."""
-        return self._csr
-
-    @csr.setter
-    def csr(self, csr_value):
-        self._csr = csr_value
-
-    @property
-    def node_id(self) -> str:
-        """Node ID."""
-        return self._node_id
-
-    @node_id.setter
-    def node_id(self, node_id):
-        self._node_id = node_id
-
-    @property
-    def certificate(self) -> str:
-        """Certificate."""
-        return self._certificate
-
-    @certificate.setter
-    def certificate(self, cert):
-        self._certificate = cert
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+
+"""Unit certificate object."""
+
+
+class UnitCertificate:
+    """Unit certificate object."""
+
+    def __init__(self):
+        """Unit certificate object."""
+        self._cert_type = None
+        self._csr = None
+        self._node_id = None
+        self._certificate = None
+
+    @property
+    def cert_type(self) -> str:
+        """Certificate type (Required type list is taken from unit)."""
+        return self._cert_type
+
+    @cert_type.setter
+    def cert_type(self, cert_type):
+        self._cert_type = cert_type
+
+    @property
+    def csr(self) -> str:
+        """Certificate Signing Request."""
+        return self._csr
+
+    @csr.setter
+    def csr(self, csr_value):
+        self._csr = csr_value
+
+    @property
+    def node_id(self) -> str:
+        """Node ID."""
+        return self._node_id
+
+    @node_id.setter
+    def node_id(self, node_id):
+        self._node_id = node_id
+
+    @property
+    def certificate(self) -> str:
+        """Certificate."""
+        return self._certificate
+
+    @certificate.setter
+    def certificate(self, cert):
+        self._certificate = cert
```

## aos_prov/utils/user_credentials.py

```diff
@@ -1,185 +1,184 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
-import os
-import tempfile
-from os.path import isfile
-from pathlib import Path
-from typing import Optional
-
-import OpenSSL
-from colorama import Fore, Style
-from cryptography.x509.oid import NameOID
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives._serialization import Encoding, PrivateFormat, NoEncryption
-from cryptography.hazmat.primitives.serialization.pkcs12 import load_key_and_certificates
-
-from aos_prov.utils import SDK_SECURITY_PATH
-from aos_prov.utils.errors import UserCredentialsError
-
-
-def _extract_cloud_domain_from_cert(cert_bytes: bytes) -> str:
-    """Get the Cloud domain name from user certificate."""
-    private_key, certificate, additional_certificates = load_key_and_certificates(cert_bytes, None)
-    return certificate.subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)[0].value
-
-
-def _pkcs12_to_pem(pkcs12_bytes: bytes):
-    private_key, certificate, additional_certificates = \
-        load_key_and_certificates(pkcs12_bytes, ''.encode('utf8'), default_backend())
-
-    cert_bytes = bytearray(certificate.public_bytes(Encoding.PEM))
-    for add_cert in additional_certificates:
-        cert_bytes += add_cert.public_bytes(Encoding.PEM)
-    key_bytes = private_key.private_bytes(Encoding.PEM, PrivateFormat.PKCS8, NoEncryption())
-    cert_bytes = bytes(cert_bytes)
-    return cert_bytes, key_bytes
-
-
-def _create_temp_file(data: bytes):
-    tmp_file = tempfile.NamedTemporaryFile(delete=False)
-    tmp_file.write(data)
-    tmp_file.close()
-    return tmp_file.name
-
-
-class TempCredentials:
-    def __init__(self, certificate: Optional[bytes], key: Optional[bytes],
-                 cert_file_name: Optional[str], key_file_name: Optional[str]):
-        self._key_file_name = key_file_name
-        self._cert_file_name = cert_file_name
-
-        self._key = None
-        self._certificate = None
-
-        if certificate and key:
-            self._key = key
-            self._certificate = certificate
-
-    def __enter__(self):
-        if not self._key_file_name:
-            self._key_file_name = _create_temp_file(self._key)
-        if not self._cert_file_name:
-            self._cert_file_name = _create_temp_file(self._certificate)
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if self._key:
-            os.unlink(self._key_file_name)
-            self._key_file_name = None
-        if self._certificate:
-            os.unlink(self._cert_file_name)
-            self._cert_file_name = None
-
-    @property
-    def key_file_name(self):
-        return self._key_file_name
-
-    @property
-    def cert_file_name(self):
-        return self._cert_file_name
-
-
-class UserCredentials:
-
-    def __init__(self, cert_file_path: Optional[str], key_file_path: Optional[str], pkcs12: Optional[str]):
-        self._cert_file_path = cert_file_path
-        self._key_file_path = key_file_path
-        self._cloud_url = None
-        if pkcs12:
-            if Path(pkcs12).exists():
-                with open(pkcs12, 'rb') as pkcs12_file:
-                    pkcs12_file_content = pkcs12_file.read()
-                    cert_bytes, key_bytes = _pkcs12_to_pem(pkcs12_file_content)
-                    self._user_credentials = TempCredentials(certificate=cert_bytes, key=key_bytes,
-                                                             cert_file_name=None, key_file_name=None)
-                    self._cloud_url = _extract_cloud_domain_from_cert(pkcs12_file_content)
-            else:
-                if not Path(cert_file_path).exists() or not Path(key_file_path).exists():
-                    raise UserCredentialsError(f'User credentials file {pkcs12} not found.')
-                else:
-                    self._user_credentials = TempCredentials(cert_file_name=cert_file_path, key_file_name=key_file_path,
-                                                             certificate=None, key=None)
-                    self._validate_credentials_format()
-                    self._cloud_url = self._extract_cloud_url()
-
-        else:
-            if not Path(cert_file_path).exists():
-                raise UserCredentialsError(f'User credentials file {cert_file_path} not found.')
-            elif not Path(key_file_path).exists():
-                raise UserCredentialsError(f'User credentials file {key_file_path} not found.')
-            else:
-                self._user_credentials = TempCredentials(cert_file_name=cert_file_path, key_file_name=key_file_path,
-                                                         certificate=None, key=None)
-                self._validate_credentials_format()
-                self._cloud_url = self._extract_cloud_url()
-
-    @property
-    def cloud_url(self):
-        return self._cloud_url
-
-    @property
-    def user_credentials(self):
-        return self._user_credentials
-
-    def _check_credentials_access(self):
-        """ Validate existence and access to user credential files
-
-            Raises:
-                UserCredentialsError: If credentials files are not found
-            Returns:
-                None
-        """
-
-        if not isfile(self._cert_file_path):
-            text = (f"{Fore.RED}Can't find user certificate file...{Style.RESET_ALL}\n\n"
-                    f"Copy file to the default directory: [{SDK_SECURITY_PATH}] \n"
-                    f"or set path to the certificate file with argument: --cert \n"
-                    f"(Example: aos-prov -u 127.0.0.1 --cert /path/to/certfile) \n")
-            raise UserCredentialsError(text)
-
-        if not isfile(self._key_file_path):
-            text = (f"{Fore.RED}Can't find user key file...{Style.RESET_ALL}\n\n"
-                    f"Copy file to the default directory: [{SDK_SECURITY_PATH}] \n"
-                    f"or set path to the key file with argument: --key \n"
-                    f"(Example: aos-prov -u 127.0.0.1 --key /path/to/keyfile) \n")
-            raise UserCredentialsError(text)
-
-    def _validate_credentials_format(self):
-        """ Validate format of user credential files
-
-            Raises:
-                UserCredentialsError: If credentials files are in wrong format or with errors
-            Returns:
-                None
-        """
-        with open(self._cert_file_path, "rb") as c, open(self._key_file_path, "r") as k:
-            cert_content = c.read()
-            key_content = k.read()
-
-        try:
-            private_key_obj = OpenSSL.crypto.load_privatekey(OpenSSL.crypto.FILETYPE_PEM, key_content)
-        except OpenSSL.crypto.Error:
-            raise UserCredentialsError('private key is not correct')
-
-        try:
-            cert_obj = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, cert_content)
-        except OpenSSL.crypto.Error:
-            raise UserCredentialsError('Certificate is not correct: %s' % key_content)
-
-        context = OpenSSL.SSL.Context(OpenSSL.SSL.TLSv1_2_METHOD)
-        context.use_privatekey(private_key_obj)
-        context.use_certificate(cert_obj)
-        try:
-            context.check_privatekey()
-        except OpenSSL.SSL.Error:
-            raise UserCredentialsError('User private key does not match certificate')
-
-    def _extract_cloud_url(self):
-        """Get the Cloud domain name from user certificate"""
-        with open(self._cert_file_path, "rb") as cert:
-            return OpenSSL.crypto.load_certificate(
-                OpenSSL.crypto.FILETYPE_PEM,
-                cert.read()
-            ).get_subject().organizationName
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+import os
+import tempfile
+from os.path import isfile
+from pathlib import Path
+from typing import Optional
+
+import OpenSSL
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives._serialization import Encoding, PrivateFormat, NoEncryption
+from cryptography.hazmat.primitives.serialization.pkcs12 import load_key_and_certificates
+from cryptography.x509.oid import NameOID
+
+from aos_prov.utils import SDK_SECURITY_PATH
+from aos_prov.utils.errors import UserCredentialsError
+
+
+def _extract_cloud_domain_from_cert(cert_bytes: bytes) -> str:
+    """Get the Cloud domain name from user certificate."""
+    private_key, certificate, additional_certificates = load_key_and_certificates(cert_bytes, None)
+    return certificate.subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)[0].value
+
+
+def _pkcs12_to_pem(pkcs12_bytes: bytes):
+    private_key, certificate, additional_certificates = \
+        load_key_and_certificates(pkcs12_bytes, ''.encode('utf8'), default_backend())
+
+    cert_bytes = bytearray(certificate.public_bytes(Encoding.PEM))
+    for add_cert in additional_certificates:
+        cert_bytes += add_cert.public_bytes(Encoding.PEM)
+    key_bytes = private_key.private_bytes(Encoding.PEM, PrivateFormat.PKCS8, NoEncryption())
+    cert_bytes = bytes(cert_bytes)
+    return cert_bytes, key_bytes
+
+
+def _create_temp_file(data: bytes):
+    tmp_file = tempfile.NamedTemporaryFile(delete=False)
+    tmp_file.write(data)
+    tmp_file.close()
+    return tmp_file.name
+
+
+class TempCredentials:
+    def __init__(self, certificate: Optional[bytes], key: Optional[bytes],
+                 cert_file_name: Optional[str], key_file_name: Optional[str]):
+        self._key_file_name = key_file_name
+        self._cert_file_name = cert_file_name
+
+        self._key = None
+        self._certificate = None
+
+        if certificate and key:
+            self._key = key
+            self._certificate = certificate
+
+    def __enter__(self):
+        if not self._key_file_name:
+            self._key_file_name = _create_temp_file(self._key)
+        if not self._cert_file_name:
+            self._cert_file_name = _create_temp_file(self._certificate)
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self._key:
+            os.unlink(self._key_file_name)
+            self._key_file_name = None
+        if self._certificate:
+            os.unlink(self._cert_file_name)
+            self._cert_file_name = None
+
+    @property
+    def key_file_name(self):
+        return self._key_file_name
+
+    @property
+    def cert_file_name(self):
+        return self._cert_file_name
+
+
+class UserCredentials:
+
+    def __init__(self, cert_file_path: Optional[str], key_file_path: Optional[str], pkcs12: Optional[str]):
+        self._cert_file_path = cert_file_path
+        self._key_file_path = key_file_path
+        self._cloud_url = None
+        if pkcs12:
+            if Path(pkcs12).exists():
+                with open(pkcs12, 'rb') as pkcs12_file:
+                    pkcs12_file_content = pkcs12_file.read()
+                    cert_bytes, key_bytes = _pkcs12_to_pem(pkcs12_file_content)
+                    self._user_credentials = TempCredentials(certificate=cert_bytes, key=key_bytes,
+                                                             cert_file_name=None, key_file_name=None)
+                    self._cloud_url = _extract_cloud_domain_from_cert(pkcs12_file_content)
+            else:
+                if not Path(cert_file_path).exists() or not Path(key_file_path).exists():
+                    raise UserCredentialsError(f'User credentials file {pkcs12} not found.')
+                else:
+                    self._user_credentials = TempCredentials(cert_file_name=cert_file_path, key_file_name=key_file_path,
+                                                             certificate=None, key=None)
+                    self._validate_credentials_format()
+                    self._cloud_url = self._extract_cloud_url()
+
+        else:
+            if not Path(cert_file_path).exists():
+                raise UserCredentialsError(f'User credentials file {cert_file_path} not found.')
+            elif not Path(key_file_path).exists():
+                raise UserCredentialsError(f'User credentials file {key_file_path} not found.')
+            else:
+                self._user_credentials = TempCredentials(cert_file_name=cert_file_path, key_file_name=key_file_path,
+                                                         certificate=None, key=None)
+                self._validate_credentials_format()
+                self._cloud_url = self._extract_cloud_url()
+
+    @property
+    def cloud_url(self):
+        return self._cloud_url
+
+    @property
+    def user_credentials(self):
+        return self._user_credentials
+
+    def _check_credentials_access(self):
+        """ Validate existence and access to user credential files
+
+            Raises:
+                UserCredentialsError: If credentials files are not found
+            Returns:
+                None
+        """
+
+        if not isfile(self._cert_file_path):
+            text = (f"[red]Can't find user certificate file...[/red]\n\n"
+                    f"Copy file to the default directory: [{SDK_SECURITY_PATH}] \n"
+                    f"or set path to the certificate file with argument: --cert \n"
+                    f"(Example: aos-prov -u 127.0.0.1 --cert /path/to/certfile) \n")
+            raise UserCredentialsError(text)
+
+        if not isfile(self._key_file_path):
+            text = (f"[red]Can't find user key file...[/red]\n\n"
+                    f"Copy file to the default directory: [{SDK_SECURITY_PATH}] \n"
+                    f"or set path to the key file with argument: --key \n"
+                    f"(Example: aos-prov -u 127.0.0.1 --key /path/to/keyfile) \n")
+            raise UserCredentialsError(text)
+
+    def _validate_credentials_format(self):
+        """ Validate format of user credential files
+
+            Raises:
+                UserCredentialsError: If credentials files are in wrong format or with errors
+            Returns:
+                None
+        """
+        with open(self._cert_file_path, "rb") as c, open(self._key_file_path, "r") as k:
+            cert_content = c.read()
+            key_content = k.read()
+
+        try:
+            private_key_obj = OpenSSL.crypto.load_privatekey(OpenSSL.crypto.FILETYPE_PEM, key_content)
+        except OpenSSL.crypto.Error:
+            raise UserCredentialsError('private key is not correct')
+
+        try:
+            cert_obj = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, cert_content)
+        except OpenSSL.crypto.Error:
+            raise UserCredentialsError('Certificate is not correct: %s' % key_content)
+
+        context = OpenSSL.SSL.Context(OpenSSL.SSL.TLSv1_2_METHOD)
+        context.use_privatekey(private_key_obj)
+        context.use_certificate(cert_obj)
+        try:
+            context.check_privatekey()
+        except OpenSSL.SSL.Error:
+            raise UserCredentialsError('User private key does not match certificate')
+
+    def _extract_cloud_url(self):
+        """Get the Cloud domain name from user certificate"""
+        with open(self._cert_file_path, "rb") as cert:
+            return OpenSSL.crypto.load_certificate(
+                OpenSSL.crypto.FILETYPE_PEM,
+                cert.read()
+            ).get_subject().organizationName
```

## test/utils/test_config.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-import unittest
-from aos_prov.utils.config import Config
-
-
-class TestConfig(unittest.TestCase):
-    def test_config_can_be_created(self):
-        c = Config()
-        self.assertIsInstance(c, Config)
-
-    def test_setters_and_getters(self):
-        c = Config()
-        c.system_id = 'some system id'
-        self.assertEqual(c.system_id, 'some system id')
-
-        c.protocol_version = 5
-        self.assertEqual(c.protocol_version, 5)
-
-        c.node_ids = ['dom0', 'dom1']
-        self.assertEqual(c.node_ids, ['dom0', 'dom1'])
-
-        c.supported_cert_types = ['um', 'sm']
-        self.assertEqual(c.supported_cert_types, ['um', 'sm'])
-
+import unittest
+from aos_prov.utils.config import Config
+
+
+class TestConfig(unittest.TestCase):
+    def test_config_can_be_created(self):
+        c = Config()
+        self.assertIsInstance(c, Config)
+
+    def test_setters_and_getters(self):
+        c = Config()
+        c.system_id = 'some system id'
+        self.assertEqual(c.system_id, 'some system id')
+
+        c.protocol_version = 5
+        self.assertEqual(c.protocol_version, 5)
+
+        c.node_ids = ['dom0', 'dom1']
+        self.assertEqual(c.node_ids, ['dom0', 'dom1'])
+
+        c.supported_cert_types = ['um', 'sm']
+        self.assertEqual(c.supported_cert_types, ['um', 'sm'])
+
```

## test/utils/test_unit_certificate.py

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
-import unittest
-
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-
-class TestUnitCertificate(unittest.TestCase):
-    def test_object_can_be_created(self):
-        uc = UnitCertificate()
-        self.assertIsInstance(uc, UnitCertificate)
-
-    def test_attributes(self):
-        uc = UnitCertificate()
-
-        uc.cert_type = 'type1'
-        self.assertEqual(uc.cert_type, 'type1')
-
-        uc.certificate = 'some cert 1'
-        self.assertEqual(uc.certificate, 'some cert 1')
-
-        uc.node_id = 'node_id'
-        self.assertEqual(uc.node_id, 'node_id')
-
-        uc.csr = 'csr'
-        self.assertEqual(uc.csr, 'csr')
+import unittest
+
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+
+class TestUnitCertificate(unittest.TestCase):
+    def test_object_can_be_created(self):
+        uc = UnitCertificate()
+        self.assertIsInstance(uc, UnitCertificate)
+
+    def test_attributes(self):
+        uc = UnitCertificate()
+
+        uc.cert_type = 'type1'
+        self.assertEqual(uc.cert_type, 'type1')
+
+        uc.certificate = 'some cert 1'
+        self.assertEqual(uc.certificate, 'some cert 1')
+
+        uc.node_id = 'node_id'
+        self.assertEqual(uc.node_id, 'node_id')
+
+        uc.csr = 'csr'
+        self.assertEqual(uc.csr, 'csr')
```

## test/utils/test_user_credentials.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-import unittest
-
-from aos_prov.utils.user_credentials import UserCredentials
-
-
-class TestUserCredentials(unittest.TestCase):
-    def test_attributes(self):
-        uc = UserCredentials('zzz', 'zz1')
-
-        uc.cert_type = 'type1'
-        self.assertEqual(uc.cert_type, 'type1')
-
-        uc.certificate = 'some cert 1'
-        self.assertEqual(uc.certificate, 'some cert 1')
-
-        uc.csr = 'csr'
-        self.assertEqual(uc.csr, 'csr')
+import unittest
+
+from aos_prov.utils.user_credentials import UserCredentials
+
+
+class TestUserCredentials(unittest.TestCase):
+    def test_attributes(self):
+        uc = UserCredentials('zzz', 'zz1')
+
+        uc.cert_type = 'type1'
+        self.assertEqual(uc.cert_type, 'type1')
+
+        uc.certificate = 'some cert 1'
+        self.assertEqual(uc.certificate, 'some cert 1')
+
+        uc.csr = 'csr'
+        self.assertEqual(uc.csr, 'csr')
```

## Comparing `aos_prov-4.0.1b6.dist-info/METADATA` & `aos_prov-4.0.2b2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,100 @@
 Metadata-Version: 2.1
 Name: aos-prov
-Version: 4.0.1b6
-Summary: Aos Unit provisioning tool
-Home-page: UNKNOWN
+Version: 4.0.2b2
+Summary: AosEdge Unit provisioning tool
 Author: EPAM Systems
 Author-email: support@aoscloud.io
 License: Apache License 2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: grpcio (>=1.44.0)
 Requires-Dist: requests (>=2.22.0)
-Requires-Dist: requests-pkcs12 (>=1.13)
+Requires-Dist: urllib3 (<1.27,>=1.26.13)
+Requires-Dist: requests-pkcs12 (>=1.14)
 Requires-Dist: protobuf (<=3.20.1,>=3.14)
 Requires-Dist: asn1crypto (>=1.4.0)
 Requires-Dist: pyOpenSSL (==23.0.0)
 Requires-Dist: cryptography (==39.0.0)
 Requires-Dist: rich (>=10.13)
-Requires-Dist: colorama (>=0.4.0)
 Requires-Dist: importlib-resources (>=3.0) ; python_version < "3.7"
 Requires-Dist: importlib-metadata (>=4.11.2) ; python_version < "3.8"
 Provides-Extra: dev
 Requires-Dist: grpcio-tools (~=1.34) ; extra == 'dev'
-Provides-Extra: virt
-Requires-Dist: virtualbox (>=2.1.1) ; extra == 'virt'
 
 Aos provisioning tool
 =====================
 This tool is part of the Aos SDK.
 
 
 Overview
 --------
-This tool will help you to provision new Units on the Aos Cloud.
+This tool will help you to create and provision new AosCore-powered Units on the Aos Cloud.
 
 Using this tool you'll be able to:
-* create a new development Unit using **Oracle VirtualBox** using our disk image.
+* create a new development multi-node Unit using **Oracle VirtualBox** with our disk images.
 * provision virtual Unit.
 * provision Renesas Dev-kit for Aos Cloud.
 
 
-Prepequicities
+Prerequisites
 --------------
-* Python 3.6+ 
-* Oracle Virtual Box installed on you system
-* Aos user certificate to access Aos cloud. You may create one with **aos-key** tool
+* Python 3.7+ .
+* Oracle Virtual Box 7 installed on your system.
+* Aos user certificate to access Aos cloud. You may create one with the **aos-key** tool.
 
 
 Installation
 ------------
 ```bash
 pip install aos-prov
 ```
 
 Usage
 ------------
 
-###Create a new Unit based on Oracle VirtualBox image and provision it on Aos Cloud:
+### Create a new Unit based on Oracle VirtualBox image and provision it on Aos Cloud:
 
 
 ```bash
 aos-prov unit-new --name {vm-name}
 ```
 >Where: 
 >* **vm-name** - Uniq name of a new Virtual Machine
 
 Example:
 ```bash
-aos-prov unit-new --nane DevUnit1
+aos-prov unit-new --name DevUnit1
 ```
 
-###Provision dev-kit or VM:
+### Provision dev-kit or VM:
 To provision Renesas dev-kit you have to know IP address of device. Use command ot provision
 ```bash
 aos-prov -u 'IP-ADDR:PORT'
 ```
 Example:
 ```bash
 aos-prov -u '127.0.0.1:8089'
 ```
 
+### Download images for Units:
+```bash
+aos-prov download
+```
 
+### Create Unit VMs without provisioning:
+```bash
+aos-prov vm-new --name {vm-name}
+```
+
+### Start Unit VMs:
+```bash
+aos-prov vm-start --name {vm-name}
+```
```

## Comparing `aos_prov-4.0.1b6.dist-info/RECORD` & `aos_prov-4.0.2b2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,59 @@
-aos_prov/__init__.py,sha256=lJlMhnUS4oONIEGs9ER8BXIp3GPfTurWn3Ko52JUvAk,93
-aos_prov/actions.py,sha256=cLFaOfOZvif_WX9048F3_9QfoUVmuBqIwydrnwlIS10,2619
-aos_prov/main.py,sha256=oWxFETschTJZLcDahVk6AC4rhYHhBIDV6AJSalnzrMU,7077
-aos_prov/commands/__init__.py,sha256=lJlMhnUS4oONIEGs9ER8BXIp3GPfTurWn3Ko52JUvAk,93
-aos_prov/commands/command_provision.py,sha256=iRRePiTcCQ1dsH9ZQtE9sl0kDDcNnntp8XcPdAkbXlU,7452
-aos_prov/commands/command_vm.py,sha256=PL3qv5ggk-teSZIbWnvUZ2hPQL4KFkT7YGOp2vIZX-s,5021
-aos_prov/commands/command_vm_libvirt.py,sha256=OUrIgwOlg-AcR-6dkwX8dK1RtqiRK6PUikdOXflt91A,2406
-aos_prov/commands/command_vm_multi_node.py,sha256=-EzjEKpJMSnoQXZOB5H917LTTiBiRY-2TcDfQIythUU,5398
-aos_prov/commands/download.py,sha256=yD9KV2WnMrZTfWc-9BeTFJsm6pGLsbBRtPm93gY_ccE,3864
-aos_prov/communication/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
-aos_prov/communication/cloud/__init__.py,sha256=lJlMhnUS4oONIEGs9ER8BXIp3GPfTurWn3Ko52JUvAk,93
-aos_prov/communication/cloud/cloud_api.py,sha256=nPjIo55l3z2UmHxxW6NRJJs1JPsV4xijZw0WDyKb4dk,8856
-aos_prov/communication/unit/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
-aos_prov/communication/unit/v0/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
-aos_prov/communication/unit/v0/unit_communacation.py,sha256=UQiVrAesx9DudZTk1cEP6ABxHD4hBsl5LzuAr3OmqLo,5403
-aos_prov/communication/unit/v0/unit_communication.py,sha256=7AGG0V1kzJsq2u6svUNMvMk4W5ZMoGS0ZtdJcJzcCTI,5467
-aos_prov/communication/unit/v0/generated/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
-aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py,sha256=Gqx7tDoWsZSuxbW0fypbAWahUzcHWumeFZZiyZmc9To,29503
-aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py,sha256=BjS_7qY0yPjiT0lL7wwsEs82tFDWBpeBrQYGSoGJ4IQ,20612
-aos_prov/communication/unit/v1/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
-aos_prov/communication/unit/v1/unit_communacation_v1.py,sha256=YLlrJ6ntjHja4GBsWQHrWbwBEBniJygPjIeC0npjW2g,6942
-aos_prov/communication/unit/v1/unit_communication_v1.py,sha256=E2AK9jO70GqR-duHBQmva3IIo-LmUosQt4PK0fIPJ-o,6926
-aos_prov/communication/unit/v1/generated/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
-aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py,sha256=14W0zcUq2O_2fJK7W0LiGhYAMThduF0q6rGgM7Dd_J0,5568
-aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py,sha256=_bXoS025FcWrXR1E_3Mh4GHB1RMvgz8lIpit-Awnf-s,163
-aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py,sha256=qpB2-86Yn9avtG1H7Z-e5X8G2aehFSc3NIJECXcCxiM,31801
-aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py,sha256=URWN8YCm0W6sOVDZGCS-HyZ700S4cHEcJJBLE3gtC8w,20208
-aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py,sha256=MOsdukOrcgOI-Dgde8swlUCTTYzG2zJsfGmZiEUQz-g,9306
-aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py,sha256=OVb5eMqUlTmE2MVe6BTk9Qx8i-spafJjun4irYr1SrM,8101
+aos_prov/__init__.py,sha256=GG0w5d4OL0uOtGiHjbqIxaTR64BEYWYw1CULBI3cz-8,89
+aos_prov/actions.py,sha256=nFG7HDWRs9v8kpuztVyM3zXnYH6fVYi5qFmnb8QLBcQ,2842
+aos_prov/main.py,sha256=4z6XrPUXlc9UO_Pk-Gz0mhK7NhyMueAKWrWnvLRC4M8,7271
+aos_prov/commands/__init__.py,sha256=GG0w5d4OL0uOtGiHjbqIxaTR64BEYWYw1CULBI3cz-8,89
+aos_prov/commands/command_provision.py,sha256=_q0hdHIntYiky7RIvG0rVIHqajzqD45nTriAnXLZpko,7501
+aos_prov/commands/command_vm.py,sha256=ASTlpDw95_4TqF5Lhi75SP03AAHLGy-gS86YZn1L3B8,4883
+aos_prov/commands/command_vm_libvirt.py,sha256=tynTeJIybqWNRjWYYJYnB-0HGyS4-KPZj_km3-JML3k,2326
+aos_prov/commands/command_vm_multi_node_manage.py,sha256=-_rjolNtBlVAu4UgA8VhX8U3vVA6PKIqeC2K_ofRq0w,9689
+aos_prov/commands/download.py,sha256=IltafRwLmlXz5JsCCTOpIFUTwP-g4KXZlPTJXTdR9kg,3799
+aos_prov/communication/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
+aos_prov/communication/cloud/__init__.py,sha256=GG0w5d4OL0uOtGiHjbqIxaTR64BEYWYw1CULBI3cz-8,89
+aos_prov/communication/cloud/cloud_api.py,sha256=hvCKoqQzdJ3RIw1uYYWoeaADWFM6W3BCU7nDKF9nLA0,8552
+aos_prov/communication/unit/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
+aos_prov/communication/unit/v0/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
+aos_prov/communication/unit/v0/unit_communication.py,sha256=K9Nyv5tfwT3RvSxeXxRWNZkPall__7a88HB_rlHtu9I,5222
+aos_prov/communication/unit/v0/generated/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
+aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py,sha256=47YlU3wgNoS4VrxMz6FZstFhF3Pv1yh_0LCeqyT8_J0,28704
+aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py,sha256=JSvwlP-oA3Fj2nXhnII_d9P0BM9OxA3PW7Sr4xFEojE,20182
+aos_prov/communication/unit/v1/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
+aos_prov/communication/unit/v1/unit_communication_v1.py,sha256=PYFUY12dznS9vbhxIgNelC7uVXYIW_ox2nXZHB_frag,6382
+aos_prov/communication/unit/v1/generated/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
+aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py,sha256=bJ6LaLZ2rORZ0L6AP0b0s4RjejkGEFkjqcHuE-oL_fY,5409
+aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
+aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py,sha256=opDC5-NeVg5TGUkaftJRG8odqHtQ5qzRUwxd5Ufb9VA,31002
+aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py,sha256=CxpYgMw_rTltk_OJm0gth1Q9trJ3JBkVKiifN2POHpY,19810
+aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py,sha256=3kne5AMCW8SqOXneyXwf9zda0IDc_VJ6FMCy0tS9U9w,9075
+aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py,sha256=NO3RJFGGXjwuY2DYfiAk8xvdfQFIPm0I4efyO828F0A,7934
 aos_prov/communication/unit/v2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v2/unit_communacation_v2.py,sha256=bkL8neI0c5TOjP-0yqAWxUMhLkdIJO6OAoTNGL3ggNM,7346
-aos_prov/communication/unit/v2/unit_communication_v2.py,sha256=3U74pyDOCkeJoyXDEKLfeC-PqevDr3OHs1u1iYbjjmI,7266
+aos_prov/communication/unit/v2/unit_communication_v2.py,sha256=bbN6mbiYa79ir9_pFV3Jc7ZsNGOnPho2WP5kHXNfsTY,6713
 aos_prov/communication/unit/v2/generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py,sha256=92EuoKs8B_1PQGQy7nh9J6VyEakCiU0O5A_VB_q2to4,5568
-aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py,sha256=_bXoS025FcWrXR1E_3Mh4GHB1RMvgz8lIpit-Awnf-s,163
-aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py,sha256=ONb-bnn1LNHBuhGNTqXbdP2AOIj88hODCVPEFXNIbQg,25101
-aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py,sha256=GZqxbkQzjCE4IewO11oY7KMQCDQW-fC02TxetQedP-s,16786
-aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py,sha256=9m4KsouTBHOiUomoFwn-8n7G59SiQQUQr3I0bP9VWkI,17715
-aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py,sha256=fm9rJKSnej7pJt35b3RMxlCc9ZxV-dQOfC6EDz0oANs,13170
+aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py,sha256=IL-89Gf3kM9k2NCEuKJi2_BWmPtKl8umCNKRUZw7n68,5409
+aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
+aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py,sha256=DO7soVNFEPWMN0bXpClz1OPa0Jc_n1P0cevrbt21fZc,24470
+aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py,sha256=QBlVknX0EqzkYcdcxkkiWSCo4cYc3_LHai4-itPeZYo,16454
+aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py,sha256=gQHROjMihFGRaPhdptxVOa_ROlm7BuL_BZsi9wVFBkM,17266
+aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py,sha256=lW-qgXE-T05_Xgiu-ejHdh-08ushwoCGExYYwp-5iC0,12904
 aos_prov/communication/unit/v4/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v4/unit_communication_v4.py,sha256=PkylTKSnZeO0YNMDc-zeEt-jOyNIBEWbOTtXL2YW9sU,11042
+aos_prov/communication/unit/v4/unit_communication_v4.py,sha256=jSwFMEv2JbnIG_rcwU4Rbz1I9viGB1VfvaxSZ3o_AAo,9592
 aos_prov/communication/unit/v4/generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v4/generated/iamanager_pb2.py,sha256=P0Xx1TV4ymcLyLhyHLUU9OR1hZqn0jPIVp32ZyFGh84,18732
-aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py,sha256=1C3DLG1-k5tUWKd7jzjWa3MHykb9gpKiseta3d_UlEI,34140
-aos_prov/files/1rootCA.crt,sha256=X3mH5kWiKpchVXfrW0HAhI94103mLhjftx2dR4KyWbw,2750
-aos_prov/files/vm.xml,sha256=67Z-mGXFGmiekJCfV1vzluEZWKKKeQXfcAmFn4DwKf8,2767
-aos_prov/utils/__init__.py,sha256=EfRSGsK_O0hF3vTrYEs5StBNfhuDk-RDquRYIm1aGBc,771
-aos_prov/utils/common.py,sha256=hi3xUV6sP4BZ6wMzAwzWAShHGhJ9uRPESz2yYxkAFnc,1614
-aos_prov/utils/config.py,sha256=eWCc54iv8PmCDo9GTcFaAsM33a7k0STSwYXSgsK5StY,2679
-aos_prov/utils/errors.py,sha256=HJS2X7EysuT1q8nl25gCYrZSYzkD18gjuCWQ47KLvng,537
-aos_prov/utils/unit_certificate.py,sha256=aKi3tYOCe-0gFpfiv5_9QxlX5z9mOMK2gQbAz7oIFh4,1229
-aos_prov/utils/user_credentials.py,sha256=N5k9d3lCx37tSzIPZ5to0dgdIMdKwG2NfXk488hjV4U,7725
+aos_prov/communication/unit/v4/generated/iamanager_pb2.py,sha256=VNNHm-5L2JX8rQkv-Sidgzlu_wus98Tjw1v44JrEzq8,18433
+aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py,sha256=pOin6Yl556SQgo1J_l-lTmypm8TeMx__U5kArMyum9A,33405
+aos_prov/files/1rootCA.crt,sha256=ToJxPHzLkJQmYdXNPVJA3ACBf7uv0THJK8ypR18etws,2705
+aos_prov/files/vm.xml,sha256=QMguS8KGVurCJgQmkjCIyZfU4CPs8-rmIlX-xwVEWYI,2690
+aos_prov/utils/__init__.py,sha256=FXJpTks2FyzbRUI3vSk-bRK1EPpQfyc2mC1OCMmPnw4,748
+aos_prov/utils/common.py,sha256=XFuewA2HYRo0MzFkZrs0j-Jcs3HUiSWLgQhUf1uB-u4,1649
+aos_prov/utils/config.py,sha256=agWFGFFBj2Y0icjCVKLCVR2KsFxgKaHVl0ZPLoJjDZM,2591
+aos_prov/utils/errors.py,sha256=0pAtbvFDd6cBKbaqexXmP0IfJu8rrY-i-bmv32ogtZI,501
+aos_prov/utils/unit_certificate.py,sha256=WYhSiQOuK7OmAK4aTWpaQRxjufJ3WKdHXpmNJSRwhkY,1176
+aos_prov/utils/user_credentials.py,sha256=4916YJfDQLkOIs3hynjftlf2c10L47jToLkkSH3iyhg,7475
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test/utils/test_config.py,sha256=JuofpwzS7FGqWcfRHOaGSlrvqVYu9rS55K-yE5JhrNs,665
-test/utils/test_unit_certificate.py,sha256=ayJbD0Qrj1FICnDRjVPBpH0zMqLEMjqzR3ZNTxSAzHU,656
-test/utils/test_user_credentials.py,sha256=_g-oGXprFMiqRD9ZklnTiqxWsvsXtW0As5oJpWOqQW0,456
-aos_prov-4.0.1b6.dist-info/METADATA,sha256=o18K5s8B4Wsxv4x3g_3O6O11M62w2otPvZn7RJs9FKA,2279
-aos_prov-4.0.1b6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-aos_prov-4.0.1b6.dist-info/entry_points.txt,sha256=pSYEWtSRNsmqfdoCn0tQJAqVxSOeLGpaSi6UPJv_kfA,49
-aos_prov-4.0.1b6.dist-info/top_level.txt,sha256=2vX7skeG9R6AfX6SK6xeAwN_SW1w1Jub2V2W_3u8Prc,14
-aos_prov-4.0.1b6.dist-info/RECORD,,
+test/utils/test_config.py,sha256=696gxCTKBDuXMe3aKd3ucGsx8qZItMGNlp53NgczEOI,642
+test/utils/test_unit_certificate.py,sha256=hh6fN3qCeZbizfgzF1V5DEYUSuCxzSNDq1qI7YrpZqs,632
+test/utils/test_user_credentials.py,sha256=CGjW9zhm3NxGP3JXTMI8p1gupqSWozbWHUCou7EUUw0,439
+aos_prov-4.0.2b2.dist-info/METADATA,sha256=JxVQNo2lC3TywdL5shNv8AYN5WhuAR1qaPuH7b2jfbk,2484
+aos_prov-4.0.2b2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+aos_prov-4.0.2b2.dist-info/entry_points.txt,sha256=fkaEe75Sm0Z8TQtunDs5iah-ilcOouPDsCnNyQaZg18,48
+aos_prov-4.0.2b2.dist-info/top_level.txt,sha256=2vX7skeG9R6AfX6SK6xeAwN_SW1w1Jub2V2W_3u8Prc,14
+aos_prov-4.0.2b2.dist-info/RECORD,,
```

