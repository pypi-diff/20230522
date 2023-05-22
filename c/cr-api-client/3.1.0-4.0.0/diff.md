# Comparing `tmp/cr_api_client-3.1.0.tar.gz` & `tmp/cr_api_client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cr_api_client-3.1.0.tar", max compression
+gzip compressed data, was "cr_api_client-4.0.0.tar", max compression
```

## Comparing `cr_api_client-3.1.0.tar` & `cr_api_client-4.0.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1056 2023-02-01 13:48:03.836850 cr_api_client-3.1.0/LICENSE
--rw-r--r--   0        0        0    11574 2023-02-17 09:00:09.001671 cr_api_client-3.1.0/README.md
--rw-r--r--   0        0        0      746 2023-03-27 14:25:11.176378 cr_api_client-3.1.0/cr_api_client/__init__.py
--rw-r--r--   0        0        0     2080 2023-02-17 08:29:45.675662 cr_api_client-3.1.0/cr_api_client/config.py
--rw-r--r--   0        0        0    94345 2023-03-07 12:43:16.110663 cr_api_client-3.1.0/cr_api_client/core_api.py
--rwxr-xr-x   0        0        0   121453 2023-03-27 14:25:11.179711 cr_api_client-3.1.0/cr_api_client/cyber_range.py
--rw-r--r--   0        0        0    20334 2023-03-07 12:43:16.113996 cr_api_client-3.1.0/cr_api_client/provisioning_api.py
--rw-r--r--   0        0        0     7763 2023-02-17 08:29:45.675662 cr_api_client-3.1.0/cr_api_client/publish_api.py
--rw-r--r--   0        0        0    22549 2023-03-27 14:25:11.179711 cr_api_client-3.1.0/cr_api_client/redteam_api.py
--rw-r--r--   0        0        0     6861 2023-02-01 13:48:03.836850 cr_api_client-3.1.0/cr_api_client/topology/TopologyElements.py
--rw-r--r--   0        0        0    14750 2023-02-17 08:29:45.675662 cr_api_client-3.1.0/cr_api_client/topology/TopologyGenerator.py
--rw-r--r--   0        0        0     2635 2023-02-01 13:48:03.836850 cr_api_client-3.1.0/cr_api_client/topology/TopologyLinksGenerator.py
--rw-r--r--   0        0        0     3328 2023-02-01 13:48:03.836850 cr_api_client-3.1.0/cr_api_client/topology/TopologyNodeGenerator.py
--rw-r--r--   0        0        0     3821 2023-02-01 13:48:03.836850 cr_api_client-3.1.0/cr_api_client/topology/TopologyNodesGenerator.py
--rw-r--r--   0        0        0      346 2023-02-01 13:48:03.836850 cr_api_client-3.1.0/cr_api_client/topology/validator/__init__.py
--rw-r--r--   0        0        0     1429 2023-02-01 13:48:03.836850 cr_api_client-3.1.0/cr_api_client/topology/validator/common.py
--rw-r--r--   0        0        0     1730 2023-02-17 08:29:45.675662 cr_api_client-3.1.0/cr_api_client/topology/validator/link.py
--rw-r--r--   0        0        0     4063 2023-02-01 13:48:03.836850 cr_api_client-3.1.0/cr_api_client/topology/validator/node.py
--rw-r--r--   0        0        0     1360 2023-02-01 13:48:03.836850 cr_api_client-3.1.0/cr_api_client/topology/validator/topology.py
--rw-r--r--   0        0        0    10126 2023-03-03 12:45:07.539117 cr_api_client-3.1.0/cr_api_client/user_activity_api.py
--rw-r--r--   0        0        0     3279 2023-02-17 08:29:45.675662 cr_api_client-3.1.0/cr_api_client/yaml_helper.py
--rw-r--r--   0        0        0     1219 2023-03-27 14:25:11.179711 cr_api_client-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    13141 1970-01-01 00:00:00.000000 cr_api_client-3.1.0/setup.py
--rw-r--r--   0        0        0    12658 1970-01-01 00:00:00.000000 cr_api_client-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/LICENSE
+-rw-r--r--   0        0        0    11574 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/README.md
+-rw-r--r--   0        0        0      746 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/__init__.py
+-rw-r--r--   0        0        0     2161 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/config.py
+-rw-r--r--   0        0        0    95387 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/core_api.py
+-rwxr-xr-x   0        0        0   121386 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/cyber_range.py
+-rw-r--r--   0        0        0    20433 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/provisioning_api.py
+-rw-r--r--   0        0        0     7763 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/publish_api.py
+-rw-r--r--   0        0        0    23855 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/redteam_api.py
+-rw-r--r--   0        0        0     6861 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/topology/TopologyElements.py
+-rw-r--r--   0        0        0    14750 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/topology/TopologyGenerator.py
+-rw-r--r--   0        0        0     2635 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/topology/TopologyLinksGenerator.py
+-rw-r--r--   0        0        0     3328 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/topology/TopologyNodeGenerator.py
+-rw-r--r--   0        0        0     3821 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/topology/TopologyNodesGenerator.py
+-rw-r--r--   0        0        0      346 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/topology/validator/__init__.py
+-rw-r--r--   0        0        0     1429 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/topology/validator/common.py
+-rw-r--r--   0        0        0     1730 2023-05-22 10:39:00.972069 cr_api_client-4.0.0/cr_api_client/topology/validator/link.py
+-rw-r--r--   0        0        0     4063 2023-05-22 10:39:00.976069 cr_api_client-4.0.0/cr_api_client/topology/validator/node.py
+-rw-r--r--   0        0        0     1360 2023-05-22 10:39:00.976069 cr_api_client-4.0.0/cr_api_client/topology/validator/topology.py
+-rw-r--r--   0        0        0    10126 2023-05-22 10:39:00.976069 cr_api_client-4.0.0/cr_api_client/user_activity_api.py
+-rw-r--r--   0        0        0     3279 2023-05-22 10:39:00.976069 cr_api_client-4.0.0/cr_api_client/yaml_helper.py
+-rw-r--r--   0        0        0     1243 2023-05-22 10:39:00.976069 cr_api_client-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    12658 1970-01-01 00:00:00.000000 cr_api_client-4.0.0/PKG-INFO
```

### Comparing `cr_api_client-3.1.0/LICENSE` & `cr_api_client-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/README.md` & `cr_api_client-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/__init__.py` & `cr_api_client-4.0.0/cr_api_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import threading
 from pathlib import Path
 
 from loguru import logger
 
 # Component version
-__version__ = "3.1.0"
+__version__ = "4.0.0"
 
 # Get component full version from file generated at build time
 current_file_dir = Path(__file__).resolve().parent
 fullversion_file = Path(current_file_dir, "fullversion.txt")
 if os.path.isfile(fullversion_file):
     __fullversion__ = open(fullversion_file, "r").read().strip()
 else:
```

### Comparing `cr_api_client-3.1.0/cr_api_client/config.py` & `cr_api_client-4.0.0/cr_api_client/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,13 +37,14 @@
         "${oc.env:USER_ACTIVITY_API_URL,http://${._api_host}:5002}"
     )
     provisioning_api_url: str = (
         "${oc.env:PROVISIONING_API_URL,http://${._api_host}:5003}"
     )
     redteam_api_url: str = "${oc.env:REDTEAM_API_URL,http://${._api_host}:5004}"
     publish_api_url: str = "${oc.env:PUBLISH_API_URL,http://${._api_host}:5007}"
+    publish_web_url: str = "${oc.env:PUBLISH_WEB_URL,http://${._api_host}:5008}"
     cacert: Optional[Path] = SI("${oc.env:CR_CA_CERT,null}")
     cert: Optional[Path] = SI("${oc.env:CR_CLIENT_CERT,null}")
     key: Optional[Path] = SI("${oc.env:CR_CLIENT_KEY,null}")
 
 
 cr_api_client_config = OmegaConf.structured(CrApiClientConfig)
```

### Comparing `cr_api_client-3.1.0/cr_api_client/core_api.py` & `cr_api_client-4.0.0/cr_api_client/core_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,5814 +84,5879 @@
 00000530: 6720 696d 706f 7274 2044 6963 740a 6672  g import Dict.fr
 00000540: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
 00000550: 204c 6973 740a 6672 6f6d 2074 7970 696e   List.from typin
 00000560: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
 00000570: 6c0a 6672 6f6d 2074 7970 696e 6720 696d  l.from typing im
 00000580: 706f 7274 2054 7570 6c65 0a0a 696d 706f  port Tuple..impo
 00000590: 7274 2072 6571 7565 7374 730a 6672 6f6d  rt requests.from
-000005a0: 2068 756d 616e 697a 6520 696d 706f 7274   humanize import
-000005b0: 206e 6174 7572 616c 7369 7a65 0a66 726f   naturalsize.fro
-000005c0: 6d20 6c6f 6775 7275 2069 6d70 6f72 7420  m loguru import 
-000005d0: 6c6f 6767 6572 0a66 726f 6d20 7275 616d  logger.from ruam
-000005e0: 656c 2e79 616d 6c20 696d 706f 7274 2059  el.yaml import Y
-000005f0: 414d 4c0a 0a66 726f 6d20 6372 5f61 7069  AML..from cr_api
-00000600: 5f63 6c69 656e 7420 696d 706f 7274 2073  _client import s
-00000610: 6875 7469 6c5f 6d61 6b65 5f61 7263 6869  hutil_make_archi
-00000620: 7665 5f6c 6f63 6b0a 6672 6f6d 2063 725f  ve_lock.from cr_
-00000630: 6170 695f 636c 6965 6e74 2e63 6f6e 6669  api_client.confi
-00000640: 6720 696d 706f 7274 2063 725f 6170 695f  g import cr_api_
-00000650: 636c 6965 6e74 5f63 6f6e 6669 670a 0a0a  client_config...
-00000660: 2320 5369 6d75 6c61 7469 6f6e 2073 7461  # Simulation sta
-00000670: 7475 7320 6d61 7070 696e 670a 6d61 705f  tus mapping.map_
-00000680: 7374 6174 7573 203d 207b 0a20 2020 2022  status = {.    "
-00000690: 4352 4541 5445 4422 3a20 312c 0a20 2020  CREATED": 1,.   
-000006a0: 2022 5052 4550 4152 494e 4722 3a20 322c   "PREPARING": 2,
-000006b0: 0a20 2020 2022 5245 4144 5922 3a20 332c  .    "READY": 3,
-000006c0: 0a20 2020 2022 5354 4152 5449 4e47 223a  .    "STARTING":
-000006d0: 2034 2c0a 2020 2020 2250 524f 5649 5349   4,.    "PROVISI
-000006e0: 4f4e 494e 4722 3a20 352c 0a20 2020 2022  ONING": 5,.    "
-000006f0: 5255 4e4e 494e 4722 3a20 362c 0a20 2020  RUNNING": 6,.   
-00000700: 2022 5553 4552 5f41 4354 4956 4954 595f   "USER_ACTIVITY_
-00000710: 504c 4159 494e 4722 3a20 372c 0a20 2020  PLAYING": 7,.   
-00000720: 2022 5354 4f50 5049 4e47 223a 2038 2c0a   "STOPPING": 8,.
-00000730: 2020 2020 2244 4553 5452 4f59 4544 223a      "DESTROYED":
-00000740: 2039 2c0a 2020 2020 2243 4c4f 4e49 4e47   9,.    "CLONING
-00000750: 223a 2031 302c 0a20 2020 2022 5041 5553  ": 10,.    "PAUS
-00000760: 494e 4722 3a20 3131 2c0a 2020 2020 2255  ING": 11,.    "U
-00000770: 4e50 4155 5349 4e47 223a 2031 322c 0a20  NPAUSING": 12,. 
-00000780: 2020 2022 5041 5553 4544 223a 2031 332c     "PAUSED": 13,
-00000790: 0a20 2020 2022 4552 524f 5222 3a20 3134  .    "ERROR": 14
-000007a0: 2c0a 7d0a 0a0a 2320 2d2d 2d2d 2d2d 2d2d  ,.}...# --------
+000005a0: 206c 6f67 7572 7520 696d 706f 7274 206c   loguru import l
+000005b0: 6f67 6765 720a 6672 6f6d 2072 7561 6d65  ogger.from ruame
+000005c0: 6c2e 7961 6d6c 2069 6d70 6f72 7420 5941  l.yaml import YA
+000005d0: 4d4c 0a0a 6672 6f6d 2063 725f 6170 695f  ML..from cr_api_
+000005e0: 636c 6965 6e74 2069 6d70 6f72 7420 7368  client import sh
+000005f0: 7574 696c 5f6d 616b 655f 6172 6368 6976  util_make_archiv
+00000600: 655f 6c6f 636b 0a66 726f 6d20 6372 5f61  e_lock.from cr_a
+00000610: 7069 5f63 6c69 656e 742e 636f 6e66 6967  pi_client.config
+00000620: 2069 6d70 6f72 7420 6372 5f61 7069 5f63   import cr_api_c
+00000630: 6c69 656e 745f 636f 6e66 6967 0a0a 2320  lient_config..# 
+00000640: 6672 6f6d 2068 756d 616e 697a 6520 696d  from humanize im
+00000650: 706f 7274 206e 6174 7572 616c 7369 7a65  port naturalsize
+00000660: 0a0a 0a23 2053 696d 756c 6174 696f 6e20  ...# Simulation 
+00000670: 7374 6174 7573 206d 6170 7069 6e67 0a6d  status mapping.m
+00000680: 6170 5f73 7461 7475 7320 3d20 7b0a 2020  ap_status = {.  
+00000690: 2020 2243 5245 4154 4544 223a 2031 2c0a    "CREATED": 1,.
+000006a0: 2020 2020 2250 5245 5041 5249 4e47 223a      "PREPARING":
+000006b0: 2032 2c0a 2020 2020 2252 4541 4459 223a   2,.    "READY":
+000006c0: 2033 2c0a 2020 2020 2253 5441 5254 494e   3,.    "STARTIN
+000006d0: 4722 3a20 342c 0a20 2020 2022 5052 4f56  G": 4,.    "PROV
+000006e0: 4953 494f 4e49 4e47 223a 2035 2c0a 2020  ISIONING": 5,.  
+000006f0: 2020 2252 554e 4e49 4e47 223a 2036 2c0a    "RUNNING": 6,.
+00000700: 2020 2020 2255 5345 525f 4143 5449 5649      "USER_ACTIVI
+00000710: 5459 5f50 4c41 5949 4e47 223a 2037 2c0a  TY_PLAYING": 7,.
+00000720: 2020 2020 2253 544f 5050 494e 4722 3a20      "STOPPING": 
+00000730: 382c 0a20 2020 2022 4445 5354 524f 5945  8,.    "DESTROYE
+00000740: 4422 3a20 392c 0a20 2020 2022 434c 4f4e  D": 9,.    "CLON
+00000750: 494e 4722 3a20 3130 2c0a 2020 2020 2250  ING": 10,.    "P
+00000760: 4155 5349 4e47 223a 2031 312c 0a20 2020  AUSING": 11,.   
+00000770: 2022 554e 5041 5553 494e 4722 3a20 3132   "UNPAUSING": 12
+00000780: 2c0a 2020 2020 2250 4155 5345 4422 3a20  ,.    "PAUSED": 
+00000790: 3133 2c0a 2020 2020 2245 5252 4f52 223a  13,.    "ERROR":
+000007a0: 2031 342c 0a7d 0a0a 0a23 202d 2d2d 2d2d   14,.}...# -----
 000007b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000007c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000007d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000007e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000007f0: 2d2d 2023 0a23 2049 6e74 6572 6e61 6c20  -- #.# Internal 
-00000800: 6865 6c70 6572 730a 2320 2d2d 2d2d 2d2d  helpers.# ------
+000007f0: 2d2d 2d2d 2d20 230a 2320 496e 7465 726e  ----- #.# Intern
+00000800: 616c 2068 656c 7065 7273 0a23 202d 2d2d  al helpers.# ---
 00000810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000850: 2d2d 2d2d 2023 0a0a 0a64 6566 205f 6765  ---- #...def _ge
-00000860: 7428 726f 7574 653a 2073 7472 2c20 2a2a  t(route: str, **
-00000870: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
-00000880: 7265 7175 6573 7473 2e52 6573 706f 6e73  requests.Respons
-00000890: 653a 0a20 2020 2072 6574 7572 6e20 7265  e:.    return re
-000008a0: 7175 6573 7473 2e67 6574 280a 2020 2020  quests.get(.    
-000008b0: 2020 2020 6622 7b63 725f 6170 695f 636c      f"{cr_api_cl
-000008c0: 6965 6e74 5f63 6f6e 6669 672e 636f 7265  ient_config.core
-000008d0: 5f61 7069 5f75 726c 7d7b 726f 7574 657d  _api_url}{route}
-000008e0: 222c 0a20 2020 2020 2020 2076 6572 6966  ",.        verif
-000008f0: 793d 6372 5f61 7069 5f63 6c69 656e 745f  y=cr_api_client_
-00000900: 636f 6e66 6967 2e63 6163 6572 742c 0a20  config.cacert,. 
-00000910: 2020 2020 2020 2063 6572 743d 2863 725f         cert=(cr_
-00000920: 6170 695f 636c 6965 6e74 5f63 6f6e 6669  api_client_confi
-00000930: 672e 6365 7274 2c20 6372 5f61 7069 5f63  g.cert, cr_api_c
-00000940: 6c69 656e 745f 636f 6e66 6967 2e6b 6579  lient_config.key
-00000950: 292c 0a20 2020 2020 2020 202a 2a6b 7761  ),.        **kwa
-00000960: 7267 732c 0a20 2020 2029 0a0a 0a64 6566  rgs,.    )...def
-00000970: 205f 706f 7374 2872 6f75 7465 3a20 7374   _post(route: st
-00000980: 722c 202a 2a6b 7761 7267 733a 2041 6e79  r, **kwargs: Any
-00000990: 2920 2d3e 2072 6571 7565 7374 732e 5265  ) -> requests.Re
-000009a0: 7370 6f6e 7365 3a0a 2020 2020 7265 7475  sponse:.    retu
-000009b0: 726e 2072 6571 7565 7374 732e 706f 7374  rn requests.post
-000009c0: 280a 2020 2020 2020 2020 6622 7b63 725f  (.        f"{cr_
-000009d0: 6170 695f 636c 6965 6e74 5f63 6f6e 6669  api_client_confi
-000009e0: 672e 636f 7265 5f61 7069 5f75 726c 7d7b  g.core_api_url}{
-000009f0: 726f 7574 657d 222c 0a20 2020 2020 2020  route}",.       
-00000a00: 2076 6572 6966 793d 6372 5f61 7069 5f63   verify=cr_api_c
-00000a10: 6c69 656e 745f 636f 6e66 6967 2e63 6163  lient_config.cac
-00000a20: 6572 742c 0a20 2020 2020 2020 2063 6572  ert,.        cer
-00000a30: 743d 2863 725f 6170 695f 636c 6965 6e74  t=(cr_api_client
-00000a40: 5f63 6f6e 6669 672e 6365 7274 2c20 6372  _config.cert, cr
-00000a50: 5f61 7069 5f63 6c69 656e 745f 636f 6e66  _api_client_conf
-00000a60: 6967 2e6b 6579 292c 0a20 2020 2020 2020  ig.key),.       
-00000a70: 202a 2a6b 7761 7267 732c 0a20 2020 2029   **kwargs,.    )
-00000a80: 0a0a 0a64 6566 205f 7075 7428 726f 7574  ...def _put(rout
-00000a90: 653a 2073 7472 2c20 2a2a 6b77 6172 6773  e: str, **kwargs
-00000aa0: 3a20 416e 7929 202d 3e20 7265 7175 6573  : Any) -> reques
-00000ab0: 7473 2e52 6573 706f 6e73 653a 0a20 2020  ts.Response:.   
-00000ac0: 2072 6574 7572 6e20 7265 7175 6573 7473   return requests
-00000ad0: 2e70 7574 280a 2020 2020 2020 2020 6622  .put(.        f"
-00000ae0: 7b63 725f 6170 695f 636c 6965 6e74 5f63  {cr_api_client_c
-00000af0: 6f6e 6669 672e 636f 7265 5f61 7069 5f75  onfig.core_api_u
-00000b00: 726c 7d7b 726f 7574 657d 222c 0a20 2020  rl}{route}",.   
-00000b10: 2020 2020 2076 6572 6966 793d 6372 5f61       verify=cr_a
-00000b20: 7069 5f63 6c69 656e 745f 636f 6e66 6967  pi_client_config
-00000b30: 2e63 6163 6572 742c 0a20 2020 2020 2020  .cacert,.       
-00000b40: 2063 6572 743d 2863 725f 6170 695f 636c   cert=(cr_api_cl
-00000b50: 6965 6e74 5f63 6f6e 6669 672e 6365 7274  ient_config.cert
-00000b60: 2c20 6372 5f61 7069 5f63 6c69 656e 745f  , cr_api_client_
-00000b70: 636f 6e66 6967 2e6b 6579 292c 0a20 2020  config.key),.   
-00000b80: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
-00000b90: 2020 2029 0a0a 0a64 6566 205f 6465 6c65     )...def _dele
-00000ba0: 7465 2872 6f75 7465 3a20 7374 722c 202a  te(route: str, *
-00000bb0: 2a6b 7761 7267 733a 2041 6e79 2920 2d3e  *kwargs: Any) ->
-00000bc0: 2072 6571 7565 7374 732e 5265 7370 6f6e   requests.Respon
-00000bd0: 7365 3a0a 2020 2020 7265 7475 726e 2072  se:.    return r
-00000be0: 6571 7565 7374 732e 6465 6c65 7465 280a  equests.delete(.
-00000bf0: 2020 2020 2020 2020 6622 7b63 725f 6170          f"{cr_ap
-00000c00: 695f 636c 6965 6e74 5f63 6f6e 6669 672e  i_client_config.
-00000c10: 636f 7265 5f61 7069 5f75 726c 7d7b 726f  core_api_url}{ro
-00000c20: 7574 657d 222c 0a20 2020 2020 2020 2076  ute}",.        v
-00000c30: 6572 6966 793d 6372 5f61 7069 5f63 6c69  erify=cr_api_cli
-00000c40: 656e 745f 636f 6e66 6967 2e63 6163 6572  ent_config.cacer
-00000c50: 742c 0a20 2020 2020 2020 2063 6572 743d  t,.        cert=
-00000c60: 2863 725f 6170 695f 636c 6965 6e74 5f63  (cr_api_client_c
-00000c70: 6f6e 6669 672e 6365 7274 2c20 6372 5f61  onfig.cert, cr_a
-00000c80: 7069 5f63 6c69 656e 745f 636f 6e66 6967  pi_client_config
-00000c90: 2e6b 6579 292c 0a20 2020 2020 2020 202a  .key),.        *
-00000ca0: 2a6b 7761 7267 732c 0a20 2020 2029 0a0a  *kwargs,.    )..
-00000cb0: 0a64 6566 205f 6861 6e64 6c65 5f65 7272  .def _handle_err
-00000cc0: 6f72 2872 6573 756c 743a 2072 6571 7565  or(result: reque
-00000cd0: 7374 732e 5265 7370 6f6e 7365 2c20 636f  sts.Response, co
-00000ce0: 6e74 6578 745f 6572 726f 725f 6d73 673a  ntext_error_msg:
-00000cf0: 2073 7472 2920 2d3e 204e 6f6e 653a 0a20   str) -> None:. 
-00000d00: 2020 2065 7272 6f72 5f6d 7367 3a20 4f70     error_msg: Op
-00000d10: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00000d20: 6e65 0a0a 2020 2020 6966 2072 6573 756c  ne..    if resul
-00000d30: 742e 6865 6164 6572 732e 6765 7428 2263  t.headers.get("c
-00000d40: 6f6e 7465 6e74 2d74 7970 6522 2920 3d3d  ontent-type") ==
-00000d50: 2022 6170 706c 6963 6174 696f 6e2f 6a73   "application/js
-00000d60: 6f6e 223a 0a20 2020 2020 2020 2072 6573  on":.        res
-00000d70: 756c 745f 6a73 6f6e 203d 2072 6573 756c  ult_json = resul
-00000d80: 742e 6a73 6f6e 2829 0a20 2020 2020 2020  t.json().       
-00000d90: 2069 6620 226d 6573 7361 6765 2220 696e   if "message" in
-00000da0: 2072 6573 756c 745f 6a73 6f6e 3a0a 2020   result_json:.  
-00000db0: 2020 2020 2020 2020 2020 6572 726f 725f            error_
-00000dc0: 6d73 6720 3d20 7265 7375 6c74 5f6a 736f  msg = result_jso
-00000dd0: 6e5b 226d 6573 7361 6765 225d 0a20 2020  n["message"].   
-00000de0: 2020 2020 2065 6c69 6620 2264 6574 6169       elif "detai
-00000df0: 6c22 2069 6e20 7265 7375 6c74 5f6a 736f  l" in result_jso
-00000e00: 6e3a 0a20 2020 2020 2020 2020 2020 2065  n:.            e
-00000e10: 7272 6f72 5f6d 7367 203d 2072 6573 756c  rror_msg = resul
-00000e20: 745f 6a73 6f6e 5b22 6465 7461 696c 225d  t_json["detail"]
-00000e30: 0a0a 2020 2020 6966 2065 7272 6f72 5f6d  ..    if error_m
-00000e40: 7367 2069 7320 4e6f 6e65 3a0a 2020 2020  sg is None:.    
-00000e50: 2020 2020 6572 726f 725f 6d73 6720 3d20      error_msg = 
-00000e60: 7265 7375 6c74 2e74 6578 740a 0a20 2020  result.text..   
-00000e70: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-00000e80: 280a 2020 2020 2020 2020 6622 7b63 6f6e  (.        f"{con
-00000e90: 7465 7874 5f65 7272 6f72 5f6d 7367 7d2e  text_error_msg}.
-00000ea0: 2022 0a20 2020 2020 2020 2066 2253 7461   ".        f"Sta
-00000eb0: 7475 7320 636f 6465 3a20 277b 7265 7375  tus code: '{resu
-00000ec0: 6c74 2e73 7461 7475 735f 636f 6465 7d27  lt.status_code}'
-00000ed0: 2e20 220a 2020 2020 2020 2020 6622 4572  . ".        f"Er
-00000ee0: 726f 7220 6d65 7373 6167 653a 2027 7b65  ror message: '{e
-00000ef0: 7272 6f72 5f6d 7367 7d27 2e22 0a20 2020  rror_msg}'.".   
-00000f00: 2029 0a0a 0a23 2047 656e 6572 6174 6520   )...# Generate 
-00000f10: 6120 756e 6971 7565 2061 7363 6969 206e  a unique ascii n
-00000f20: 616d 650a 6465 6620 5f67 6574 5f72 616e  ame.def _get_ran
-00000f30: 646f 6d5f 7374 7269 6e67 286c 656e 6774  dom_string(lengt
-00000f40: 683a 2069 6e74 2920 2d3e 2073 7472 3a0a  h: int) -> str:.
-00000f50: 2020 2020 6c65 7474 6572 7320 3d20 7374      letters = st
-00000f60: 7269 6e67 2e61 7363 6969 5f6c 6f77 6572  ring.ascii_lower
-00000f70: 6361 7365 0a20 2020 2072 6573 756c 745f  case.    result_
-00000f80: 7374 7220 3d20 2222 2e6a 6f69 6e28 7261  str = "".join(ra
-00000f90: 6e64 6f6d 2e63 686f 6963 6528 6c65 7474  ndom.choice(lett
-00000fa0: 6572 7329 2066 6f72 2069 2069 6e20 7261  ers) for i in ra
-00000fb0: 6e67 6528 6c65 6e67 7468 2929 0a20 2020  nge(length)).   
-00000fc0: 2072 6574 7572 6e20 7265 7375 6c74 5f73   return result_s
-00000fd0: 7472 0a0a 0a64 6566 205f 7369 6d75 6c61  tr...def _simula
-00000fe0: 7469 6f6e 5f65 7865 6375 7465 5f6f 7065  tion_execute_ope
-00000ff0: 7261 7469 6f6e 280a 2020 2020 6d65 7468  ration(.    meth
-00001000: 6f64 3a20 7374 722c 0a20 2020 206f 7065  od: str,.    ope
-00001010: 7261 7469 6f6e 3a20 7374 722c 0a20 2020  ration: str,.   
-00001020: 2069 645f 7369 6d75 6c61 7469 6f6e 3a20   id_simulation: 
-00001030: 696e 742c 0a20 2020 2065 7870 6563 7465  int,.    expecte
-00001040: 645f 6375 7272 656e 745f 7369 6d75 6c61  d_current_simula
-00001050: 7469 6f6e 5f73 7461 7475 733a 2073 7472  tion_status: str
-00001060: 2c0a 2020 2020 6f70 7469 6f6e 616c 5f70  ,.    optional_p
-00001070: 6172 616d 313a 204f 7074 696f 6e61 6c5b  aram1: Optional[
-00001080: 416e 795d 203d 204e 6f6e 652c 0a20 2020  Any] = None,.   
-00001090: 206f 7074 696f 6e61 6c5f 7061 7261 6d32   optional_param2
-000010a0: 3a20 4f70 7469 6f6e 616c 5b41 6e79 5d20  : Optional[Any] 
-000010b0: 3d20 4e6f 6e65 2c0a 2020 2020 706f 7374  = None,.    post
-000010c0: 5f64 6174 613a 204f 7074 696f 6e61 6c5b  _data: Optional[
-000010d0: 416e 795d 203d 204e 6f6e 652c 0a29 202d  Any] = None,.) -
-000010e0: 3e20 696e 743a 0a20 2020 2022 2222 0a20  > int:.    """. 
-000010f0: 2020 2047 656e 6572 6963 206d 6574 686f     Generic metho
-00001100: 6420 746f 206c 6175 6e63 6820 4954 2053  d to launch IT S
-00001110: 696d 756c 6174 696f 6e20 4150 4920 6f70  imulation API op
-00001120: 6572 6174 696f 6e20 6f6e 2061 2074 6172  eration on a tar
-00001130: 6765 7420 7369 6d75 6c61 7469 6f6e 2e0a  get simulation..
-00001140: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
-00001150: 6f6e 2053 484f 554c 4420 6265 2075 7365  on SHOULD be use
-00001160: 6420 746f 2063 616c 6c20 616c 6c20 2261  d to call all "a
-00001170: 7379 6e63 6872 6f6e 6f75 7322 206f 7065  synchronous" ope
-00001180: 7261 7469 6f6e 7320 6578 706f 7365 6420  rations exposed 
-00001190: 6279 2074 6865 0a20 2020 2049 5420 5369  by the.    IT Si
-000011a0: 6d75 6c61 7469 6f6e 2041 5049 2e20 5468  mulation API. Th
-000011b0: 6174 2069 732c 2066 6f72 2061 6c6c 2041  at is, for all A
-000011c0: 5049 2065 6e64 706f 696e 7473 2074 6861  PI endpoints tha
-000011d0: 7420 6c61 756e 6368 2061 6e20 2261 7379  t launch an "asy
-000011e0: 6e63 6872 6f6e 6f75 7320 7461 736b 222c  nchronous task",
-000011f0: 0a20 2020 2061 6e64 2077 6869 6368 2068  .    and which h
-00001200: 6176 6520 616e 2061 7373 6f63 6961 7465  ave an associate
-00001210: 6420 222f 6765 745f 7374 6174 7573 2220  d "/get_status" 
-00001220: 656e 6470 6f69 6e74 2e0a 0a20 2020 2054  endpoint...    T
-00001230: 6869 7320 6675 6e63 7469 6f6e 204d 5553  his function MUS
-00001240: 5420 4e4f 5420 6265 2075 7365 6420 666f  T NOT be used fo
-00001250: 7220 7379 6e63 6872 6f6e 6f75 7320 656e  r synchronous en
-00001260: 6470 6f69 6e74 732e 0a20 2020 2022 2222  dpoints..    """
-00001270: 0a0a 2020 2020 6c6f 6767 6572 2e69 6e66  ..    logger.inf
-00001280: 6f28 0a20 2020 2020 2020 2022 5b2b 5d20  o(.        "[+] 
-00001290: 476f 696e 6720 746f 2065 7865 6375 7465  Going to execute
-000012a0: 206f 7065 7261 7469 6f6e 2027 7b7d 2720   operation '{}' 
-000012b0: 6f6e 2073 696d 756c 6174 696f 6e20 4944  on simulation ID
-000012c0: 2027 7b7d 2722 2e66 6f72 6d61 7428 0a20   '{}'".format(. 
-000012d0: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-000012e0: 7469 6f6e 2c20 6964 5f73 696d 756c 6174  tion, id_simulat
-000012f0: 696f 6e0a 2020 2020 2020 2020 290a 2020  ion.        ).  
-00001300: 2020 290a 0a20 2020 2023 2042 7569 6c64    )..    # Build
-00001310: 2055 5249 0a20 2020 2075 7269 203d 2066   URI.    uri = f
-00001320: 222f 7369 6d75 6c61 7469 6f6e 2f7b 6964  "/simulation/{id
-00001330: 5f73 696d 756c 6174 696f 6e7d 2f7b 6f70  _simulation}/{op
-00001340: 6572 6174 696f 6e7d 220a 2020 2020 6966  eration}".    if
-00001350: 206f 7074 696f 6e61 6c5f 7061 7261 6d31   optional_param1
-00001360: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00001370: 2020 2020 2020 7572 6920 3d20 6622 7b75        uri = f"{u
-00001380: 7269 7d2f 7b73 7472 286f 7074 696f 6e61  ri}/{str(optiona
-00001390: 6c5f 7061 7261 6d31 297d 220a 2020 2020  l_param1)}".    
-000013a0: 6966 206f 7074 696f 6e61 6c5f 7061 7261  if optional_para
-000013b0: 6d32 2069 7320 6e6f 7420 4e6f 6e65 3a0a  m2 is not None:.
-000013c0: 2020 2020 2020 2020 7572 6920 3d20 6622          uri = f"
-000013d0: 7b75 7269 7d2f 7b73 7472 286f 7074 696f  {uri}/{str(optio
-000013e0: 6e61 6c5f 7061 7261 6d32 297d 220a 0a20  nal_param2)}".. 
-000013f0: 2020 2023 2053 7461 7274 2074 6865 206f     # Start the o
-00001400: 7065 7261 7469 6f6e 0a20 2020 2072 6573  peration.    res
-00001410: 756c 742c 2074 6173 6b5f 6964 656e 7469  ult, task_identi
-00001420: 6669 6572 203d 205f 7369 6d75 6c61 7469  fier = _simulati
-00001430: 6f6e 5f73 7461 7274 5f6f 7065 7261 7469  on_start_operati
-00001440: 6f6e 280a 2020 2020 2020 2020 6d65 7468  on(.        meth
-00001450: 6f64 2c20 6f70 6572 6174 696f 6e2c 2075  od, operation, u
-00001460: 7269 2c20 706f 7374 5f64 6174 610a 2020  ri, post_data.  
-00001470: 2020 290a 0a20 2020 2023 2042 7569 6c64    )..    # Build
-00001480: 2055 5249 2074 6f20 6765 7420 7468 6520   URI to get the 
-00001490: 7374 6174 7573 206f 6620 7468 6520 7461  status of the ta
-000014a0: 736b 0a20 2020 2075 7269 5f67 6574 5f73  sk.    uri_get_s
-000014b0: 7461 7475 7320 3d20 280a 2020 2020 2020  tatus = (.      
-000014c0: 2020 6622 2f73 696d 756c 6174 696f 6e2f    f"/simulation/
-000014d0: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d2f  {id_simulation}/
-000014e0: 7b6f 7065 7261 7469 6f6e 7d2f 6765 745f  {operation}/get_
-000014f0: 7374 6174 7573 2f7b 7461 736b 5f69 6465  status/{task_ide
-00001500: 6e74 6966 6965 727d 220a 2020 2020 290a  ntifier}".    ).
-00001510: 0a20 2020 2023 2048 616e 646c 6520 636c  .    # Handle cl
-00001520: 6f6e 696e 6720 6361 7365 2077 6865 7265  oning case where
-00001530: 2061 206e 6577 2069 645f 7369 6d75 6c61   a new id_simula
-00001540: 7469 6f6e 206f 7220 6e65 7720 6461 7461  tion or new data
-00001550: 7365 745f 6964 2069 7320 7265 7475 726e  set_id is return
-00001560: 6564 0a20 2020 2069 6620 6f70 6572 6174  ed.    if operat
-00001570: 696f 6e20 3d3d 2022 636c 6f6e 6522 3a0a  ion == "clone":.
-00001580: 2020 2020 2020 2020 6964 5f73 696d 756c          id_simul
-00001590: 6174 696f 6e20 3d20 7265 7375 6c74 2e6a  ation = result.j
-000015a0: 736f 6e28 295b 2269 6422 5d0a 0a20 2020  son()["id"]..   
-000015b0: 2023 2057 6169 7420 666f 7220 7468 6520   # Wait for the 
-000015c0: 6f70 6572 6174 696f 6e20 746f 2062 6520  operation to be 
-000015d0: 636f 6d70 6c65 7465 6420 696e 2062 6163  completed in bac
-000015e0: 6b65 6e64 0a20 2020 2063 7572 7265 6e74  kend.    current
-000015f0: 5f6f 7065 7261 7469 6f6e 5f73 7461 7475  _operation_statu
-00001600: 733a 2044 6963 745b 7374 722c 2041 6e79  s: Dict[str, Any
-00001610: 5d20 3d20 7b7d 0a20 2020 2064 6973 706c  ] = {}.    displ
-00001620: 6179 5f69 6478 203d 2030 0a20 2020 2077  ay_idx = 0.    w
-00001630: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
-00001640: 2020 2023 2053 6c65 6570 2062 6566 6f72     # Sleep befor
-00001650: 6520 6e65 7874 2069 7465 7261 7469 6f6e  e next iteration
-00001660: 0a20 2020 2020 2020 2074 696d 652e 736c  .        time.sl
-00001670: 6565 7028 302e 3529 0a0a 2020 2020 2020  eep(0.5)..      
-00001680: 2020 2320 446f 206e 6f74 2064 6973 706c    # Do not displ
-00001690: 6179 2064 6562 7567 2069 6e66 6f20 6174  ay debug info at
-000016a0: 2065 6163 6820 6c6f 6f70 2069 7465 7261   each loop itera
-000016b0: 696f 6e0a 2020 2020 2020 2020 6966 2064  ion.        if d
-000016c0: 6973 706c 6179 5f69 6478 2025 2031 3020  isplay_idx % 10 
-000016d0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-000016e0: 2020 6c6f 6767 6572 2e69 6e66 6f28 0a20    logger.info(. 
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001700: 2020 5b2b 5d20 4375 7272 656e 746c 7920    [+] Currently 
-00001710: 6578 6563 7574 696e 6720 6f70 6572 6174  executing operat
-00001720: 696f 6e20 277b 7d27 206f 6e20 220a 2020  ion '{}' on ".  
-00001730: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001740: 696d 756c 6174 696f 6e20 4944 2027 7b7d  imulation ID '{}
-00001750: 272c 2077 6974 6820 7461 736b 2069 6420  ', with task id 
-00001760: 7b7d 2e2e 2e22 2e66 6f72 6d61 7428 0a20  {}...".format(. 
-00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001780: 2020 206f 7065 7261 7469 6f6e 2c20 6964     operation, id
-00001790: 5f73 696d 756c 6174 696f 6e2c 2074 6173  _simulation, tas
-000017a0: 6b5f 6964 656e 7469 6669 6572 0a20 2020  k_identifier.   
-000017b0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000017c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000017d0: 2020 2020 2064 6973 706c 6179 5f69 6478       display_idx
-000017e0: 202b 3d20 310a 0a20 2020 2020 2020 2072   += 1..        r
-000017f0: 6573 756c 7420 3d20 5f67 6574 2875 7269  esult = _get(uri
-00001800: 5f67 6574 5f73 7461 7475 7329 0a20 2020  _get_status).   
-00001810: 2020 2020 2069 6620 7265 7375 6c74 2e73       if result.s
-00001820: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-00001830: 303a 0a20 2020 2020 2020 2020 2020 205f  0:.            _
-00001840: 6861 6e64 6c65 5f65 7272 6f72 280a 2020  handle_error(.  
-00001850: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00001860: 7375 6c74 2c0a 2020 2020 2020 2020 2020  sult,.          
-00001870: 2020 2020 2020 6622 4572 726f 7220 7768        f"Error wh
-00001880: 696c 6520 6765 7474 696e 6720 7468 6520  ile getting the 
-00001890: 7374 6174 7573 206f 6620 7468 6520 6f70  status of the op
-000018a0: 6572 6174 696f 6e20 277b 6f70 6572 6174  eration '{operat
-000018b0: 696f 6e7d 2720 2874 6173 6b20 6964 207b  ion}' (task id {
-000018c0: 7461 736b 5f69 6465 6e74 6966 6965 727d  task_identifier}
-000018d0: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
-000018e0: 290a 0a20 2020 2020 2020 2063 7572 7265  )..        curre
-000018f0: 6e74 5f6f 7065 7261 7469 6f6e 5f73 7461  nt_operation_sta
-00001900: 7475 7320 3d20 7265 7375 6c74 2e6a 736f  tus = result.jso
-00001910: 6e28 290a 2020 2020 2020 2020 6966 206e  n().        if n
-00001920: 6f74 2061 6c6c 280a 2020 2020 2020 2020  ot all(.        
-00001930: 2020 2020 6b20 696e 2063 7572 7265 6e74      k in current
-00001940: 5f6f 7065 7261 7469 6f6e 5f73 7461 7475  _operation_statu
-00001950: 7320 666f 7220 6b20 696e 205b 2273 7461  s for k in ["sta
-00001960: 7465 222c 2022 6572 726f 725f 6d73 6722  te", "error_msg"
-00001970: 2c20 2272 6573 756c 7422 5d0a 2020 2020  , "result"].    
-00001980: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00001990: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
-000019a0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-000019b0: 2020 2020 6622 4572 726f 7220 7768 696c      f"Error whil
-000019c0: 6520 6765 7474 696e 6720 7468 6520 7374  e getting the st
-000019d0: 6174 7573 206f 6620 7468 6520 6f6e 676f  atus of the ongo
-000019e0: 696e 6720 277b 6f70 6572 6174 696f 6e7d  ing '{operation}
-000019f0: 2720 6f70 6572 6174 696f 6e20 2874 6173  ' operation (tas
-00001a00: 6b20 6964 207b 7461 736b 5f69 6465 6e74  k id {task_ident
-00001a10: 6966 6965 727d 293a 2072 6574 7572 6e65  ifier}): returne
-00001a20: 6420 696e 666f 726d 6174 696f 6e20 6672  d information fr
-00001a30: 6f6d 2041 5049 2069 7320 6e6f 7420 7765  om API is not we
-00001a40: 6c6c 2066 6f72 6d65 6422 0a20 2020 2020  ll formed".     
-00001a50: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00001a60: 2020 6966 2063 7572 7265 6e74 5f6f 7065    if current_ope
-00001a70: 7261 7469 6f6e 5f73 7461 7475 735b 2273  ration_status["s
-00001a80: 7461 7465 225d 203d 3d20 2246 494e 4953  tate"] == "FINIS
-00001a90: 4845 4422 3a0a 2020 2020 2020 2020 2020  HED":.          
-00001aa0: 2020 6272 6561 6b0a 0a20 2020 2023 2054    break..    # T
-00001ab0: 6865 206f 7065 7261 7469 6f6e 2069 7320  he operation is 
-00001ac0: 636f 6d70 6c65 7465 640a 2020 2020 7369  completed.    si
-00001ad0: 6d75 6c61 7469 6f6e 5f64 6963 7420 3d20  mulation_dict = 
-00001ae0: 5f73 696d 756c 6174 696f 6e5f 636f 6e63  _simulation_conc
-00001af0: 6c75 6465 5f6f 7065 7261 7469 6f6e 280a  lude_operation(.
-00001b00: 2020 2020 2020 2020 6964 5f73 696d 756c          id_simul
-00001b10: 6174 696f 6e2c 206f 7065 7261 7469 6f6e  ation, operation
-00001b20: 2c20 6375 7272 656e 745f 6f70 6572 6174  , current_operat
-00001b30: 696f 6e5f 7374 6174 7573 0a20 2020 2029  ion_status.    )
-00001b40: 0a0a 2020 2020 6966 2073 696d 756c 6174  ..    if simulat
-00001b50: 696f 6e5f 6469 6374 5b22 6572 726f 725f  ion_dict["error_
-00001b60: 6d73 6722 5d20 616e 6420 7369 6d75 6c61  msg"] and simula
-00001b70: 7469 6f6e 5f64 6963 745b 2265 7272 6f72  tion_dict["error
-00001b80: 5f6d 7367 225d 2021 3d20 224e 6f6e 6522  _msg"] != "None"
-00001b90: 3a0a 2020 2020 2020 2020 706f 7465 6e74  :.        potent
-00001ba0: 6961 6c5f 6572 726f 725f 6d73 6720 3d20  ial_error_msg = 
-00001bb0: 2220 2877 6974 6820 6572 726f 7220 277b  " (with error '{
-00001bc0: 7d27 2922 2e66 6f72 6d61 7428 7369 6d75  }')".format(simu
-00001bd0: 6c61 7469 6f6e 5f64 6963 745b 2265 7272  lation_dict["err
-00001be0: 6f72 5f6d 7367 225d 290a 2020 2020 656c  or_msg"]).    el
-00001bf0: 7365 3a0a 2020 2020 2020 2020 706f 7465  se:.        pote
-00001c00: 6e74 6961 6c5f 6572 726f 725f 6d73 6720  ntial_error_msg 
-00001c10: 3d20 2222 0a20 2020 206c 6f67 6765 722e  = "".    logger.
-00001c20: 696e 666f 280a 2020 2020 2020 2020 225b  info(.        "[
-00001c30: 2b5d 2043 7572 7265 6e74 2073 696d 756c  +] Current simul
-00001c40: 6174 696f 6e20 7374 6174 7573 3a20 277b  ation status: '{
-00001c50: 7d27 7b7d 222e 666f 726d 6174 280a 2020  }'{}".format(.  
-00001c60: 2020 2020 2020 2020 2020 7369 6d75 6c61            simula
-00001c70: 7469 6f6e 5f64 6963 745b 2273 7461 7475  tion_dict["statu
-00001c80: 7322 5d2c 2070 6f74 656e 7469 616c 5f65  s"], potential_e
-00001c90: 7272 6f72 5f6d 7367 0a20 2020 2020 2020  rror_msg.       
-00001ca0: 2029 0a20 2020 2029 0a0a 2020 2020 7265   ).    )..    re
-00001cb0: 7475 726e 2069 645f 7369 6d75 6c61 7469  turn id_simulati
-00001cc0: 6f6e 0a0a 0a64 6566 205f 7369 6d75 6c61  on...def _simula
-00001cd0: 7469 6f6e 5f73 7461 7274 5f6f 7065 7261  tion_start_opera
-00001ce0: 7469 6f6e 280a 2020 2020 6d65 7468 6f64  tion(.    method
-00001cf0: 3a20 7374 722c 0a20 2020 206f 7065 7261  : str,.    opera
-00001d00: 7469 6f6e 3a20 7374 722c 0a20 2020 2023  tion: str,.    #
-00001d10: 2069 645f 7369 6d75 6c61 7469 6f6e 3a20   id_simulation: 
-00001d20: 696e 742c 0a20 2020 2075 7269 3a20 7374  int,.    uri: st
-00001d30: 722c 0a20 2020 2023 2075 7269 5f67 6574  r,.    # uri_get
-00001d40: 5f73 7461 7475 735f 6261 7365 3a20 7374  _status_base: st
-00001d50: 722c 0a20 2020 2070 6f73 745f 6461 7461  r,.    post_data
-00001d60: 3a20 4f70 7469 6f6e 616c 5b41 6e79 5d20  : Optional[Any] 
-00001d70: 3d20 4e6f 6e65 2c0a 2920 2d3e 2054 7570  = None,.) -> Tup
-00001d80: 6c65 5b72 6571 7565 7374 732e 5265 7370  le[requests.Resp
-00001d90: 6f6e 7365 2c20 7374 725d 3a0a 0a20 2020  onse, str]:..   
-00001da0: 2069 6620 6d65 7468 6f64 203d 3d20 2267   if method == "g
-00001db0: 6574 223a 0a20 2020 2020 2020 2072 6573  et":.        res
-00001dc0: 756c 7420 3d20 5f67 6574 2875 7269 290a  ult = _get(uri).
-00001dd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00001de0: 2020 6461 7461 203d 206a 736f 6e2e 6475    data = json.du
-00001df0: 6d70 7328 706f 7374 5f64 6174 6129 0a20  mps(post_data). 
-00001e00: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00001e10: 5f70 6f73 7428 7572 692c 2064 6174 613d  _post(uri, data=
-00001e20: 6461 7461 2c20 6865 6164 6572 733d 7b22  data, headers={"
-00001e30: 436f 6e74 656e 742d 5479 7065 223a 2022  Content-Type": "
-00001e40: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00001e50: 227d 290a 0a20 2020 2023 2069 6620 7265  "})..    # if re
-00001e60: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-00001e70: 2021 3d20 3230 303a 0a20 2020 2023 2020   != 200:.    #  
-00001e80: 2020 2023 2053 7065 6369 616c 2063 6173     # Special cas
-00001e90: 653a 2074 6869 7320 6f70 6572 6174 696f  e: this operatio
-00001ea0: 6e73 2069 7320 616c 7265 6164 7920 7275  ns is already ru
-00001eb0: 6e6e 696e 6720 696e 2074 6865 2049 5420  nning in the IT 
-00001ec0: 5369 6d75 6c61 7469 6f6e 2041 5049 2062  Simulation API b
-00001ed0: 6163 6b65 6e64 0a20 2020 2023 2020 2020  ackend.    #    
-00001ee0: 2023 2062 7574 2069 7320 6163 7475 616c   # but is actual
-00001ef0: 6c79 2066 696e 6973 6865 642e 2049 6e20  ly finished. In 
-00001f00: 7468 6973 2063 6173 652c 2067 6574 2069  this case, get i
-00001f10: 7473 2073 7461 7475 7320 2874 6869 7320  ts status (this 
-00001f20: 7769 6c6c 2064 656c 6574 6520 7468 6520  will delete the 
-00001f30: 7461 736b 0a20 2020 2023 2020 2020 2023  task.    #     #
-00001f40: 2074 6865 2049 5420 5369 6d75 6c61 7469   the IT Simulati
-00001f50: 6f6e 2041 5049 2062 6163 6b65 6e64 292c  on API backend),
-00001f60: 2061 6e64 2074 7279 2061 6761 696e 2e0a   and try again..
-00001f70: 2020 2020 2320 2020 2020 2320 544f 444f      #     # TODO
-00001f80: 3a20 7468 6973 2069 7320 6e6f 7420 7065  : this is not pe
-00001f90: 7266 6563 742c 2069 6e20 7468 6520 7365  rfect, in the se
-00001fa0: 6e73 6520 7468 6174 2069 7420 6973 206e  nse that it is n
-00001fb0: 6f74 2061 2067 7265 6174 2055 582e 0a20  ot a great UX.. 
-00001fc0: 2020 2023 2020 2020 2074 7279 3a0a 2020     #     try:.  
-00001fd0: 2020 2320 2020 2020 2020 2020 7265 7375    #         resu
-00001fe0: 6c74 5f67 6574 5f73 7461 7475 7320 3d20  lt_get_status = 
-00001ff0: 5f67 6574 2875 7269 5f67 6574 5f73 7461  _get(uri_get_sta
-00002000: 7475 7329 0a20 2020 2023 2020 2020 2020  tus).    #      
-00002010: 2020 2069 6620 7265 7375 6c74 5f67 6574     if result_get
-00002020: 5f73 7461 7475 732e 7374 6174 7573 5f63  _status.status_c
-00002030: 6f64 6520 3d3d 2032 3030 3a0a 2020 2020  ode == 200:.    
-00002040: 2320 2020 2020 2020 2020 2020 2020 7265  #             re
-00002050: 7375 6c74 5f67 6574 5f73 7461 7475 735f  sult_get_status_
-00002060: 6a73 6f6e 203d 2072 6573 756c 745f 6765  json = result_ge
-00002070: 745f 7374 6174 7573 2e6a 736f 6e28 290a  t_status.json().
-00002080: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00002090: 2020 6966 2028 0a20 2020 2023 2020 2020    if (.    #    
-000020a0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-000020b0: 280a 2020 2020 2320 2020 2020 2020 2020  (.    #         
-000020c0: 2020 2020 2020 2020 2020 2020 6b20 696e              k in
-000020d0: 2072 6573 756c 745f 6765 745f 7374 6174   result_get_stat
-000020e0: 7573 5f6a 736f 6e0a 2020 2020 2320 2020  us_json.    #   
+00000850: 2d2d 2d2d 2d2d 2d20 230a 0a0a 6465 6620  ------- #...def 
+00000860: 5f67 6574 2872 6f75 7465 3a20 7374 722c  _get(route: str,
+00000870: 202a 2a6b 7761 7267 733a 2041 6e79 2920   **kwargs: Any) 
+00000880: 2d3e 2072 6571 7565 7374 732e 5265 7370  -> requests.Resp
+00000890: 6f6e 7365 3a0a 2020 2020 7265 7475 726e  onse:.    return
+000008a0: 2072 6571 7565 7374 732e 6765 7428 0a20   requests.get(. 
+000008b0: 2020 2020 2020 2066 227b 6372 5f61 7069         f"{cr_api
+000008c0: 5f63 6c69 656e 745f 636f 6e66 6967 2e63  _client_config.c
+000008d0: 6f72 655f 6170 695f 7572 6c7d 7b72 6f75  ore_api_url}{rou
+000008e0: 7465 7d22 2c0a 2020 2020 2020 2020 7665  te}",.        ve
+000008f0: 7269 6679 3d63 725f 6170 695f 636c 6965  rify=cr_api_clie
+00000900: 6e74 5f63 6f6e 6669 672e 6361 6365 7274  nt_config.cacert
+00000910: 2c0a 2020 2020 2020 2020 6365 7274 3d28  ,.        cert=(
+00000920: 6372 5f61 7069 5f63 6c69 656e 745f 636f  cr_api_client_co
+00000930: 6e66 6967 2e63 6572 742c 2063 725f 6170  nfig.cert, cr_ap
+00000940: 695f 636c 6965 6e74 5f63 6f6e 6669 672e  i_client_config.
+00000950: 6b65 7929 2c0a 2020 2020 2020 2020 2a2a  key),.        **
+00000960: 6b77 6172 6773 2c0a 2020 2020 290a 0a0a  kwargs,.    )...
+00000970: 6465 6620 5f70 6f73 7428 726f 7574 653a  def _post(route:
+00000980: 2073 7472 2c20 2a2a 6b77 6172 6773 3a20   str, **kwargs: 
+00000990: 416e 7929 202d 3e20 7265 7175 6573 7473  Any) -> requests
+000009a0: 2e52 6573 706f 6e73 653a 0a20 2020 2072  .Response:.    r
+000009b0: 6574 7572 6e20 7265 7175 6573 7473 2e70  eturn requests.p
+000009c0: 6f73 7428 0a20 2020 2020 2020 2066 227b  ost(.        f"{
+000009d0: 6372 5f61 7069 5f63 6c69 656e 745f 636f  cr_api_client_co
+000009e0: 6e66 6967 2e63 6f72 655f 6170 695f 7572  nfig.core_api_ur
+000009f0: 6c7d 7b72 6f75 7465 7d22 2c0a 2020 2020  l}{route}",.    
+00000a00: 2020 2020 7665 7269 6679 3d63 725f 6170      verify=cr_ap
+00000a10: 695f 636c 6965 6e74 5f63 6f6e 6669 672e  i_client_config.
+00000a20: 6361 6365 7274 2c0a 2020 2020 2020 2020  cacert,.        
+00000a30: 6365 7274 3d28 6372 5f61 7069 5f63 6c69  cert=(cr_api_cli
+00000a40: 656e 745f 636f 6e66 6967 2e63 6572 742c  ent_config.cert,
+00000a50: 2063 725f 6170 695f 636c 6965 6e74 5f63   cr_api_client_c
+00000a60: 6f6e 6669 672e 6b65 7929 2c0a 2020 2020  onfig.key),.    
+00000a70: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
+00000a80: 2020 290a 0a0a 6465 6620 5f70 7574 2872    )...def _put(r
+00000a90: 6f75 7465 3a20 7374 722c 202a 2a6b 7761  oute: str, **kwa
+00000aa0: 7267 733a 2041 6e79 2920 2d3e 2072 6571  rgs: Any) -> req
+00000ab0: 7565 7374 732e 5265 7370 6f6e 7365 3a0a  uests.Response:.
+00000ac0: 2020 2020 7265 7475 726e 2072 6571 7565      return reque
+00000ad0: 7374 732e 7075 7428 0a20 2020 2020 2020  sts.put(.       
+00000ae0: 2066 227b 6372 5f61 7069 5f63 6c69 656e   f"{cr_api_clien
+00000af0: 745f 636f 6e66 6967 2e63 6f72 655f 6170  t_config.core_ap
+00000b00: 695f 7572 6c7d 7b72 6f75 7465 7d22 2c0a  i_url}{route}",.
+00000b10: 2020 2020 2020 2020 7665 7269 6679 3d63          verify=c
+00000b20: 725f 6170 695f 636c 6965 6e74 5f63 6f6e  r_api_client_con
+00000b30: 6669 672e 6361 6365 7274 2c0a 2020 2020  fig.cacert,.    
+00000b40: 2020 2020 6365 7274 3d28 6372 5f61 7069      cert=(cr_api
+00000b50: 5f63 6c69 656e 745f 636f 6e66 6967 2e63  _client_config.c
+00000b60: 6572 742c 2063 725f 6170 695f 636c 6965  ert, cr_api_clie
+00000b70: 6e74 5f63 6f6e 6669 672e 6b65 7929 2c0a  nt_config.key),.
+00000b80: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+00000b90: 2c0a 2020 2020 290a 0a0a 6465 6620 5f64  ,.    )...def _d
+00000ba0: 656c 6574 6528 726f 7574 653a 2073 7472  elete(route: str
+00000bb0: 2c20 2a2a 6b77 6172 6773 3a20 416e 7929  , **kwargs: Any)
+00000bc0: 202d 3e20 7265 7175 6573 7473 2e52 6573   -> requests.Res
+00000bd0: 706f 6e73 653a 0a20 2020 2072 6574 7572  ponse:.    retur
+00000be0: 6e20 7265 7175 6573 7473 2e64 656c 6574  n requests.delet
+00000bf0: 6528 0a20 2020 2020 2020 2066 227b 6372  e(.        f"{cr
+00000c00: 5f61 7069 5f63 6c69 656e 745f 636f 6e66  _api_client_conf
+00000c10: 6967 2e63 6f72 655f 6170 695f 7572 6c7d  ig.core_api_url}
+00000c20: 7b72 6f75 7465 7d22 2c0a 2020 2020 2020  {route}",.      
+00000c30: 2020 7665 7269 6679 3d63 725f 6170 695f    verify=cr_api_
+00000c40: 636c 6965 6e74 5f63 6f6e 6669 672e 6361  client_config.ca
+00000c50: 6365 7274 2c0a 2020 2020 2020 2020 6365  cert,.        ce
+00000c60: 7274 3d28 6372 5f61 7069 5f63 6c69 656e  rt=(cr_api_clien
+00000c70: 745f 636f 6e66 6967 2e63 6572 742c 2063  t_config.cert, c
+00000c80: 725f 6170 695f 636c 6965 6e74 5f63 6f6e  r_api_client_con
+00000c90: 6669 672e 6b65 7929 2c0a 2020 2020 2020  fig.key),.      
+00000ca0: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
+00000cb0: 290a 0a0a 6465 6620 5f68 616e 646c 655f  )...def _handle_
+00000cc0: 6572 726f 7228 7265 7375 6c74 3a20 7265  error(result: re
+00000cd0: 7175 6573 7473 2e52 6573 706f 6e73 652c  quests.Response,
+00000ce0: 2063 6f6e 7465 7874 5f65 7272 6f72 5f6d   context_error_m
+00000cf0: 7367 3a20 7374 7229 202d 3e20 4e6f 6e65  sg: str) -> None
+00000d00: 3a0a 2020 2020 6572 726f 725f 6d73 673a  :.    error_msg:
+00000d10: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00000d20: 204e 6f6e 650a 0a20 2020 2069 6620 7265   None..    if re
+00000d30: 7375 6c74 2e68 6561 6465 7273 2e67 6574  sult.headers.get
+00000d40: 2822 636f 6e74 656e 742d 7479 7065 2229  ("content-type")
+00000d50: 203d 3d20 2261 7070 6c69 6361 7469 6f6e   == "application
+00000d60: 2f6a 736f 6e22 3a0a 2020 2020 2020 2020  /json":.        
+00000d70: 7265 7375 6c74 5f6a 736f 6e20 3d20 7265  result_json = re
+00000d80: 7375 6c74 2e6a 736f 6e28 290a 2020 2020  sult.json().    
+00000d90: 2020 2020 6966 2022 6d65 7373 6167 6522      if "message"
+00000da0: 2069 6e20 7265 7375 6c74 5f6a 736f 6e3a   in result_json:
+00000db0: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+00000dc0: 6f72 5f6d 7367 203d 2072 6573 756c 745f  or_msg = result_
+00000dd0: 6a73 6f6e 5b22 6d65 7373 6167 6522 5d0a  json["message"].
+00000de0: 2020 2020 2020 2020 656c 6966 2022 6465          elif "de
+00000df0: 7461 696c 2220 696e 2072 6573 756c 745f  tail" in result_
+00000e00: 6a73 6f6e 3a0a 2020 2020 2020 2020 2020  json:.          
+00000e10: 2020 6572 726f 725f 6d73 6720 3d20 7265    error_msg = re
+00000e20: 7375 6c74 5f6a 736f 6e5b 2264 6574 6169  sult_json["detai
+00000e30: 6c22 5d0a 0a20 2020 2069 6620 6572 726f  l"]..    if erro
+00000e40: 725f 6d73 6720 6973 204e 6f6e 653a 0a20  r_msg is None:. 
+00000e50: 2020 2020 2020 2065 7272 6f72 5f6d 7367         error_msg
+00000e60: 203d 2072 6573 756c 742e 7465 7874 0a0a   = result.text..
+00000e70: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+00000e80: 696f 6e28 0a20 2020 2020 2020 2066 227b  ion(.        f"{
+00000e90: 636f 6e74 6578 745f 6572 726f 725f 6d73  context_error_ms
+00000ea0: 677d 2e20 220a 2020 2020 2020 2020 6622  g}. ".        f"
+00000eb0: 5374 6174 7573 2063 6f64 653a 2027 7b72  Status code: '{r
+00000ec0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
+00000ed0: 657d 272e 2022 0a20 2020 2020 2020 2066  e}'. ".        f
+00000ee0: 2245 7272 6f72 206d 6573 7361 6765 3a20  "Error message: 
+00000ef0: 277b 6572 726f 725f 6d73 677d 272e 220a  '{error_msg}'.".
+00000f00: 2020 2020 290a 0a0a 2320 4765 6e65 7261      )...# Genera
+00000f10: 7465 2061 2075 6e69 7175 6520 6173 6369  te a unique asci
+00000f20: 6920 6e61 6d65 0a64 6566 205f 6765 745f  i name.def _get_
+00000f30: 7261 6e64 6f6d 5f73 7472 696e 6728 6c65  random_string(le
+00000f40: 6e67 7468 3a20 696e 7429 202d 3e20 7374  ngth: int) -> st
+00000f50: 723a 0a20 2020 206c 6574 7465 7273 203d  r:.    letters =
+00000f60: 2073 7472 696e 672e 6173 6369 695f 6c6f   string.ascii_lo
+00000f70: 7765 7263 6173 650a 2020 2020 7265 7375  wercase.    resu
+00000f80: 6c74 5f73 7472 203d 2022 222e 6a6f 696e  lt_str = "".join
+00000f90: 2872 616e 646f 6d2e 6368 6f69 6365 286c  (random.choice(l
+00000fa0: 6574 7465 7273 2920 666f 7220 6920 696e  etters) for i in
+00000fb0: 2072 616e 6765 286c 656e 6774 6829 290a   range(length)).
+00000fc0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00000fd0: 745f 7374 720a 0a0a 6465 6620 5f73 696d  t_str...def _sim
+00000fe0: 756c 6174 696f 6e5f 6578 6563 7574 655f  ulation_execute_
+00000ff0: 6f70 6572 6174 696f 6e28 0a20 2020 206d  operation(.    m
+00001000: 6574 686f 643a 2073 7472 2c0a 2020 2020  ethod: str,.    
+00001010: 6f70 6572 6174 696f 6e3a 2073 7472 2c0a  operation: str,.
+00001020: 2020 2020 6964 5f73 696d 756c 6174 696f      id_simulatio
+00001030: 6e3a 2069 6e74 2c0a 2020 2020 6578 7065  n: int,.    expe
+00001040: 6374 6564 5f63 7572 7265 6e74 5f73 696d  cted_current_sim
+00001050: 756c 6174 696f 6e5f 7374 6174 7573 3a20  ulation_status: 
+00001060: 7374 722c 0a20 2020 206f 7074 696f 6e61  str,.    optiona
+00001070: 6c5f 7061 7261 6d31 3a20 4f70 7469 6f6e  l_param1: Option
+00001080: 616c 5b41 6e79 5d20 3d20 4e6f 6e65 2c0a  al[Any] = None,.
+00001090: 2020 2020 6f70 7469 6f6e 616c 5f70 6172      optional_par
+000010a0: 616d 323a 204f 7074 696f 6e61 6c5b 416e  am2: Optional[An
+000010b0: 795d 203d 204e 6f6e 652c 0a20 2020 2070  y] = None,.    p
+000010c0: 6f73 745f 6461 7461 3a20 4f70 7469 6f6e  ost_data: Option
+000010d0: 616c 5b41 6e79 5d20 3d20 4e6f 6e65 2c0a  al[Any] = None,.
+000010e0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2222  ) -> int:.    ""
+000010f0: 220a 2020 2020 4765 6e65 7269 6320 6d65  ".    Generic me
+00001100: 7468 6f64 2074 6f20 6c61 756e 6368 2049  thod to launch I
+00001110: 5420 5369 6d75 6c61 7469 6f6e 2041 5049  T Simulation API
+00001120: 206f 7065 7261 7469 6f6e 206f 6e20 6120   operation on a 
+00001130: 7461 7267 6574 2073 696d 756c 6174 696f  target simulatio
+00001140: 6e2e 0a0a 2020 2020 5468 6973 2066 756e  n...    This fun
+00001150: 6374 696f 6e20 5348 4f55 4c44 2062 6520  ction SHOULD be 
+00001160: 7573 6564 2074 6f20 6361 6c6c 2061 6c6c  used to call all
+00001170: 2022 6173 796e 6368 726f 6e6f 7573 2220   "asynchronous" 
+00001180: 6f70 6572 6174 696f 6e73 2065 7870 6f73  operations expos
+00001190: 6564 2062 7920 7468 650a 2020 2020 4954  ed by the.    IT
+000011a0: 2053 696d 756c 6174 696f 6e20 4150 492e   Simulation API.
+000011b0: 2054 6861 7420 6973 2c20 666f 7220 616c   That is, for al
+000011c0: 6c20 4150 4920 656e 6470 6f69 6e74 7320  l API endpoints 
+000011d0: 7468 6174 206c 6175 6e63 6820 616e 2022  that launch an "
+000011e0: 6173 796e 6368 726f 6e6f 7573 2074 6173  asynchronous tas
+000011f0: 6b22 2c0a 2020 2020 616e 6420 7768 6963  k",.    and whic
+00001200: 6820 6861 7665 2061 6e20 6173 736f 6369  h have an associ
+00001210: 6174 6564 2022 2f67 6574 5f73 7461 7475  ated "/get_statu
+00001220: 7322 2065 6e64 706f 696e 742e 0a0a 2020  s" endpoint...  
+00001230: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
+00001240: 4d55 5354 204e 4f54 2062 6520 7573 6564  MUST NOT be used
+00001250: 2066 6f72 2073 796e 6368 726f 6e6f 7573   for synchronous
+00001260: 2065 6e64 706f 696e 7473 2e0a 2020 2020   endpoints..    
+00001270: 2222 220a 0a20 2020 206c 6f67 6765 722e  """..    logger.
+00001280: 696e 666f 280a 2020 2020 2020 2020 225b  info(.        "[
+00001290: 2b5d 2047 6f69 6e67 2074 6f20 6578 6563  +] Going to exec
+000012a0: 7574 6520 6f70 6572 6174 696f 6e20 277b  ute operation '{
+000012b0: 7d27 206f 6e20 7369 6d75 6c61 7469 6f6e  }' on simulation
+000012c0: 2049 4420 277b 7d27 222e 666f 726d 6174   ID '{}'".format
+000012d0: 280a 2020 2020 2020 2020 2020 2020 6f70  (.            op
+000012e0: 6572 6174 696f 6e2c 2069 645f 7369 6d75  eration, id_simu
+000012f0: 6c61 7469 6f6e 0a20 2020 2020 2020 2029  lation.        )
+00001300: 0a20 2020 2029 0a0a 2020 2020 2320 4275  .    )..    # Bu
+00001310: 696c 6420 5552 490a 2020 2020 7572 6920  ild URI.    uri 
+00001320: 3d20 6622 2f73 696d 756c 6174 696f 6e2f  = f"/simulation/
+00001330: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d2f  {id_simulation}/
+00001340: 7b6f 7065 7261 7469 6f6e 7d22 0a20 2020  {operation}".   
+00001350: 2069 6620 6f70 7469 6f6e 616c 5f70 6172   if optional_par
+00001360: 616d 3120 6973 206e 6f74 204e 6f6e 653a  am1 is not None:
+00001370: 0a20 2020 2020 2020 2075 7269 203d 2066  .        uri = f
+00001380: 227b 7572 697d 2f7b 7374 7228 6f70 7469  "{uri}/{str(opti
+00001390: 6f6e 616c 5f70 6172 616d 3129 7d22 0a20  onal_param1)}". 
+000013a0: 2020 2069 6620 6f70 7469 6f6e 616c 5f70     if optional_p
+000013b0: 6172 616d 3220 6973 206e 6f74 204e 6f6e  aram2 is not Non
+000013c0: 653a 0a20 2020 2020 2020 2075 7269 203d  e:.        uri =
+000013d0: 2066 227b 7572 697d 2f7b 7374 7228 6f70   f"{uri}/{str(op
+000013e0: 7469 6f6e 616c 5f70 6172 616d 3229 7d22  tional_param2)}"
+000013f0: 0a0a 2020 2020 2320 5374 6172 7420 7468  ..    # Start th
+00001400: 6520 6f70 6572 6174 696f 6e0a 2020 2020  e operation.    
+00001410: 7265 7375 6c74 2c20 7461 736b 5f69 6465  result, task_ide
+00001420: 6e74 6966 6965 7220 3d20 5f73 696d 756c  ntifier = _simul
+00001430: 6174 696f 6e5f 7374 6172 745f 6f70 6572  ation_start_oper
+00001440: 6174 696f 6e28 0a20 2020 2020 2020 206d  ation(.        m
+00001450: 6574 686f 642c 206f 7065 7261 7469 6f6e  ethod, operation
+00001460: 2c20 7572 692c 2070 6f73 745f 6461 7461  , uri, post_data
+00001470: 0a20 2020 2029 0a0a 2020 2020 2320 4275  .    )..    # Bu
+00001480: 696c 6420 5552 4920 746f 2067 6574 2074  ild URI to get t
+00001490: 6865 2073 7461 7475 7320 6f66 2074 6865  he status of the
+000014a0: 2074 6173 6b0a 2020 2020 7572 695f 6765   task.    uri_ge
+000014b0: 745f 7374 6174 7573 203d 2028 0a20 2020  t_status = (.   
+000014c0: 2020 2020 2066 222f 7369 6d75 6c61 7469       f"/simulati
+000014d0: 6f6e 2f7b 6964 5f73 696d 756c 6174 696f  on/{id_simulatio
+000014e0: 6e7d 2f7b 6f70 6572 6174 696f 6e7d 2f67  n}/{operation}/g
+000014f0: 6574 5f73 7461 7475 732f 7b74 6173 6b5f  et_status/{task_
+00001500: 6964 656e 7469 6669 6572 7d22 0a20 2020  identifier}".   
+00001510: 2029 0a0a 2020 2020 2320 4861 6e64 6c65   )..    # Handle
+00001520: 2063 6c6f 6e69 6e67 2063 6173 6520 7768   cloning case wh
+00001530: 6572 6520 6120 6e65 7720 6964 5f73 696d  ere a new id_sim
+00001540: 756c 6174 696f 6e20 6f72 206e 6577 2064  ulation or new d
+00001550: 6174 6173 6574 5f69 6420 6973 2072 6574  ataset_id is ret
+00001560: 7572 6e65 640a 2020 2020 6966 206f 7065  urned.    if ope
+00001570: 7261 7469 6f6e 203d 3d20 2263 6c6f 6e65  ration == "clone
+00001580: 223a 0a20 2020 2020 2020 2069 645f 7369  ":.        id_si
+00001590: 6d75 6c61 7469 6f6e 203d 2072 6573 756c  mulation = resul
+000015a0: 742e 6a73 6f6e 2829 5b22 6964 225d 0a0a  t.json()["id"]..
+000015b0: 2020 2020 2320 5761 6974 2066 6f72 2074      # Wait for t
+000015c0: 6865 206f 7065 7261 7469 6f6e 2074 6f20  he operation to 
+000015d0: 6265 2063 6f6d 706c 6574 6564 2069 6e20  be completed in 
+000015e0: 6261 636b 656e 640a 2020 2020 6375 7272  backend.    curr
+000015f0: 656e 745f 6f70 6572 6174 696f 6e5f 7374  ent_operation_st
+00001600: 6174 7573 3a20 4469 6374 5b73 7472 2c20  atus: Dict[str, 
+00001610: 416e 795d 203d 207b 7d0a 2020 2020 6469  Any] = {}.    di
+00001620: 7370 6c61 795f 6964 7820 3d20 300a 2020  splay_idx = 0.  
+00001630: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
+00001640: 2020 2020 2020 2320 536c 6565 7020 6265        # Sleep be
+00001650: 666f 7265 206e 6578 7420 6974 6572 6174  fore next iterat
+00001660: 696f 6e0a 2020 2020 2020 2020 7469 6d65  ion.        time
+00001670: 2e73 6c65 6570 2830 2e35 290a 0a20 2020  .sleep(0.5)..   
+00001680: 2020 2020 2023 2044 6f20 6e6f 7420 6469       # Do not di
+00001690: 7370 6c61 7920 6465 6275 6720 696e 666f  splay debug info
+000016a0: 2061 7420 6561 6368 206c 6f6f 7020 6974   at each loop it
+000016b0: 6572 6169 6f6e 0a20 2020 2020 2020 2069  eraion.        i
+000016c0: 6620 6469 7370 6c61 795f 6964 7820 2520  f display_idx % 
+000016d0: 3130 203d 3d20 303a 0a20 2020 2020 2020  10 == 0:.       
+000016e0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+000016f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00001700: 2020 2220 205b 2b5d 2043 7572 7265 6e74    "  [+] Current
+00001710: 6c79 2065 7865 6375 7469 6e67 206f 7065  ly executing ope
+00001720: 7261 7469 6f6e 2027 7b7d 2720 6f6e 2022  ration '{}' on "
+00001730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001740: 2022 7369 6d75 6c61 7469 6f6e 2049 4420   "simulation ID 
+00001750: 277b 7d27 2c20 7769 7468 2074 6173 6b20  '{}', with task 
+00001760: 6964 207b 7d2e 2e2e 222e 666f 726d 6174  id {}...".format
+00001770: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00001780: 2020 2020 2020 6f70 6572 6174 696f 6e2c        operation,
+00001790: 2069 645f 7369 6d75 6c61 7469 6f6e 2c20   id_simulation, 
+000017a0: 7461 736b 5f69 6465 6e74 6966 6965 720a  task_identifier.
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017c0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+000017d0: 2020 2020 2020 2020 6469 7370 6c61 795f          display_
+000017e0: 6964 7820 2b3d 2031 0a0a 2020 2020 2020  idx += 1..      
+000017f0: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
+00001800: 7572 695f 6765 745f 7374 6174 7573 290a  uri_get_status).
+00001810: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
+00001820: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
+00001830: 2032 3030 3a0a 2020 2020 2020 2020 2020   200:.          
+00001840: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+00001850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001860: 2072 6573 756c 742c 0a20 2020 2020 2020   result,.       
+00001870: 2020 2020 2020 2020 2066 2245 7272 6f72           f"Error
+00001880: 2077 6869 6c65 2067 6574 7469 6e67 2074   while getting t
+00001890: 6865 2073 7461 7475 7320 6f66 2074 6865  he status of the
+000018a0: 206f 7065 7261 7469 6f6e 2027 7b6f 7065   operation '{ope
+000018b0: 7261 7469 6f6e 7d27 2028 7461 736b 2069  ration}' (task i
+000018c0: 6420 7b74 6173 6b5f 6964 656e 7469 6669  d {task_identifi
+000018d0: 6572 7d29 222c 0a20 2020 2020 2020 2020  er})",.         
+000018e0: 2020 2029 0a0a 2020 2020 2020 2020 6375     )..        cu
+000018f0: 7272 656e 745f 6f70 6572 6174 696f 6e5f  rrent_operation_
+00001900: 7374 6174 7573 203d 2072 6573 756c 742e  status = result.
+00001910: 6a73 6f6e 2829 0a20 2020 2020 2020 2069  json().        i
+00001920: 6620 6e6f 7420 616c 6c28 0a20 2020 2020  f not all(.     
+00001930: 2020 2020 2020 206b 2069 6e20 6375 7272         k in curr
+00001940: 656e 745f 6f70 6572 6174 696f 6e5f 7374  ent_operation_st
+00001950: 6174 7573 2066 6f72 206b 2069 6e20 5b22  atus for k in ["
+00001960: 7374 6174 6522 2c20 2265 7272 6f72 5f6d  state", "error_m
+00001970: 7367 222c 2022 7265 7375 6c74 225d 0a20  sg", "result"]. 
+00001980: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00001990: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+000019a0: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
+000019b0: 2020 2020 2020 2066 2245 7272 6f72 2077         f"Error w
+000019c0: 6869 6c65 2067 6574 7469 6e67 2074 6865  hile getting the
+000019d0: 2073 7461 7475 7320 6f66 2074 6865 206f   status of the o
+000019e0: 6e67 6f69 6e67 2027 7b6f 7065 7261 7469  ngoing '{operati
+000019f0: 6f6e 7d27 206f 7065 7261 7469 6f6e 2028  on}' operation (
+00001a00: 7461 736b 2069 6420 7b74 6173 6b5f 6964  task id {task_id
+00001a10: 656e 7469 6669 6572 7d29 3a20 7265 7475  entifier}): retu
+00001a20: 726e 6564 2069 6e66 6f72 6d61 7469 6f6e  rned information
+00001a30: 2066 726f 6d20 4150 4920 6973 206e 6f74   from API is not
+00001a40: 2077 656c 6c20 666f 726d 6564 220a 2020   well formed".  
+00001a50: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00001a60: 2020 2020 2069 6620 6375 7272 656e 745f       if current_
+00001a70: 6f70 6572 6174 696f 6e5f 7374 6174 7573  operation_status
+00001a80: 5b22 7374 6174 6522 5d20 3d3d 2022 4649  ["state"] == "FI
+00001a90: 4e49 5348 4544 223a 0a20 2020 2020 2020  NISHED":.       
+00001aa0: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
+00001ab0: 2320 5468 6520 6f70 6572 6174 696f 6e20  # The operation 
+00001ac0: 6973 2063 6f6d 706c 6574 6564 0a20 2020  is completed.   
+00001ad0: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
+00001ae0: 203d 205f 7369 6d75 6c61 7469 6f6e 5f63   = _simulation_c
+00001af0: 6f6e 636c 7564 655f 6f70 6572 6174 696f  onclude_operatio
+00001b00: 6e28 0a20 2020 2020 2020 2069 645f 7369  n(.        id_si
+00001b10: 6d75 6c61 7469 6f6e 2c20 6f70 6572 6174  mulation, operat
+00001b20: 696f 6e2c 2063 7572 7265 6e74 5f6f 7065  ion, current_ope
+00001b30: 7261 7469 6f6e 5f73 7461 7475 730a 2020  ration_status.  
+00001b40: 2020 290a 0a20 2020 2069 6620 7369 6d75    )..    if simu
+00001b50: 6c61 7469 6f6e 5f64 6963 745b 2265 7272  lation_dict["err
+00001b60: 6f72 5f6d 7367 225d 2061 6e64 2073 696d  or_msg"] and sim
+00001b70: 756c 6174 696f 6e5f 6469 6374 5b22 6572  ulation_dict["er
+00001b80: 726f 725f 6d73 6722 5d20 213d 2022 4e6f  ror_msg"] != "No
+00001b90: 6e65 223a 0a20 2020 2020 2020 2070 6f74  ne":.        pot
+00001ba0: 656e 7469 616c 5f65 7272 6f72 5f6d 7367  ential_error_msg
+00001bb0: 203d 2022 2028 7769 7468 2065 7272 6f72   = " (with error
+00001bc0: 2027 7b7d 2729 222e 666f 726d 6174 2873   '{}')".format(s
+00001bd0: 696d 756c 6174 696f 6e5f 6469 6374 5b22  imulation_dict["
+00001be0: 6572 726f 725f 6d73 6722 5d29 0a20 2020  error_msg"]).   
+00001bf0: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
+00001c00: 6f74 656e 7469 616c 5f65 7272 6f72 5f6d  otential_error_m
+00001c10: 7367 203d 2022 220a 2020 2020 6c6f 6767  sg = "".    logg
+00001c20: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+00001c30: 2022 5b2b 5d20 4375 7272 656e 7420 7369   "[+] Current si
+00001c40: 6d75 6c61 7469 6f6e 2073 7461 7475 733a  mulation status:
+00001c50: 2027 7b7d 277b 7d22 2e66 6f72 6d61 7428   '{}'{}".format(
+00001c60: 0a20 2020 2020 2020 2020 2020 2073 696d  .            sim
+00001c70: 756c 6174 696f 6e5f 6469 6374 5b22 7374  ulation_dict["st
+00001c80: 6174 7573 225d 2c20 706f 7465 6e74 6961  atus"], potentia
+00001c90: 6c5f 6572 726f 725f 6d73 670a 2020 2020  l_error_msg.    
+00001ca0: 2020 2020 290a 2020 2020 290a 0a20 2020      ).    )..   
+00001cb0: 2072 6574 7572 6e20 6964 5f73 696d 756c   return id_simul
+00001cc0: 6174 696f 6e0a 0a0a 6465 6620 5f73 696d  ation...def _sim
+00001cd0: 756c 6174 696f 6e5f 7374 6172 745f 6f70  ulation_start_op
+00001ce0: 6572 6174 696f 6e28 0a20 2020 206d 6574  eration(.    met
+00001cf0: 686f 643a 2073 7472 2c0a 2020 2020 6f70  hod: str,.    op
+00001d00: 6572 6174 696f 6e3a 2073 7472 2c0a 2020  eration: str,.  
+00001d10: 2020 2320 6964 5f73 696d 756c 6174 696f    # id_simulatio
+00001d20: 6e3a 2069 6e74 2c0a 2020 2020 7572 693a  n: int,.    uri:
+00001d30: 2073 7472 2c0a 2020 2020 2320 7572 695f   str,.    # uri_
+00001d40: 6765 745f 7374 6174 7573 5f62 6173 653a  get_status_base:
+00001d50: 2073 7472 2c0a 2020 2020 706f 7374 5f64   str,.    post_d
+00001d60: 6174 613a 204f 7074 696f 6e61 6c5b 416e  ata: Optional[An
+00001d70: 795d 203d 204e 6f6e 652c 0a29 202d 3e20  y] = None,.) -> 
+00001d80: 5475 706c 655b 7265 7175 6573 7473 2e52  Tuple[requests.R
+00001d90: 6573 706f 6e73 652c 2073 7472 5d3a 0a0a  esponse, str]:..
+00001da0: 2020 2020 6966 206d 6574 686f 6420 3d3d      if method ==
+00001db0: 2022 6765 7422 3a0a 2020 2020 2020 2020   "get":.        
+00001dc0: 7265 7375 6c74 203d 205f 6765 7428 7572  result = _get(ur
+00001dd0: 6929 0a20 2020 2065 6c73 653a 0a20 2020  i).    else:.   
+00001de0: 2020 2020 2064 6174 6120 3d20 6a73 6f6e       data = json
+00001df0: 2e64 756d 7073 2870 6f73 745f 6461 7461  .dumps(post_data
+00001e00: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
+00001e10: 203d 205f 706f 7374 2875 7269 2c20 6461   = _post(uri, da
+00001e20: 7461 3d64 6174 612c 2068 6561 6465 7273  ta=data, headers
+00001e30: 3d7b 2243 6f6e 7465 6e74 2d54 7970 6522  ={"Content-Type"
+00001e40: 3a20 2261 7070 6c69 6361 7469 6f6e 2f6a  : "application/j
+00001e50: 736f 6e22 7d29 0a0a 2020 2020 2320 6966  son"})..    # if
+00001e60: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
+00001e70: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
+00001e80: 2320 2020 2020 2320 5370 6563 6961 6c20  #     # Special 
+00001e90: 6361 7365 3a20 7468 6973 206f 7065 7261  case: this opera
+00001ea0: 7469 6f6e 7320 6973 2061 6c72 6561 6479  tions is already
+00001eb0: 2072 756e 6e69 6e67 2069 6e20 7468 6520   running in the 
+00001ec0: 4954 2053 696d 756c 6174 696f 6e20 4150  IT Simulation AP
+00001ed0: 4920 6261 636b 656e 640a 2020 2020 2320  I backend.    # 
+00001ee0: 2020 2020 2320 6275 7420 6973 2061 6374      # but is act
+00001ef0: 7561 6c6c 7920 6669 6e69 7368 6564 2e20  ually finished. 
+00001f00: 496e 2074 6869 7320 6361 7365 2c20 6765  In this case, ge
+00001f10: 7420 6974 7320 7374 6174 7573 2028 7468  t its status (th
+00001f20: 6973 2077 696c 6c20 6465 6c65 7465 2074  is will delete t
+00001f30: 6865 2074 6173 6b0a 2020 2020 2320 2020  he task.    #   
+00001f40: 2020 2320 7468 6520 4954 2053 696d 756c    # the IT Simul
+00001f50: 6174 696f 6e20 4150 4920 6261 636b 656e  ation API backen
+00001f60: 6429 2c20 616e 6420 7472 7920 6167 6169  d), and try agai
+00001f70: 6e2e 0a20 2020 2023 2020 2020 2023 2054  n..    #     # T
+00001f80: 4f44 4f3a 2074 6869 7320 6973 206e 6f74  ODO: this is not
+00001f90: 2070 6572 6665 6374 2c20 696e 2074 6865   perfect, in the
+00001fa0: 2073 656e 7365 2074 6861 7420 6974 2069   sense that it i
+00001fb0: 7320 6e6f 7420 6120 6772 6561 7420 5558  s not a great UX
+00001fc0: 2e0a 2020 2020 2320 2020 2020 7472 793a  ..    #     try:
+00001fd0: 0a20 2020 2023 2020 2020 2020 2020 2072  .    #         r
+00001fe0: 6573 756c 745f 6765 745f 7374 6174 7573  esult_get_status
+00001ff0: 203d 205f 6765 7428 7572 695f 6765 745f   = _get(uri_get_
+00002000: 7374 6174 7573 290a 2020 2020 2320 2020  status).    #   
+00002010: 2020 2020 2020 6966 2072 6573 756c 745f        if result_
+00002020: 6765 745f 7374 6174 7573 2e73 7461 7475  get_status.statu
+00002030: 735f 636f 6465 203d 3d20 3230 303a 0a20  s_code == 200:. 
+00002040: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+00002050: 2072 6573 756c 745f 6765 745f 7374 6174   result_get_stat
+00002060: 7573 5f6a 736f 6e20 3d20 7265 7375 6c74  us_json = result
+00002070: 5f67 6574 5f73 7461 7475 732e 6a73 6f6e  _get_status.json
+00002080: 2829 0a20 2020 2023 2020 2020 2020 2020  ().    #        
+00002090: 2020 2020 2069 6620 280a 2020 2020 2320       if (.    # 
+000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020b0: 616c 6c28 0a20 2020 2023 2020 2020 2020  all(.    #      
+000020c0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+000020d0: 2069 6e20 7265 7375 6c74 5f67 6574 5f73   in result_get_s
+000020e0: 7461 7475 735f 6a73 6f6e 0a20 2020 2023  tatus_json.    #
 000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002100: 2020 666f 7220 6b20 696e 205b 2273 7461    for k in ["sta
-00002110: 7465 222c 2022 7265 7375 6c74 222c 2022  te", "result", "
-00002120: 6572 726f 725f 6d73 6722 5d0a 2020 2020  error_msg"].    
-00002130: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-00002140: 2020 290a 2020 2020 2320 2020 2020 2020    ).    #       
-00002150: 2020 2020 2020 2020 2020 616e 6420 7265            and re
-00002160: 7375 6c74 5f67 6574 5f73 7461 7475 735f  sult_get_status_
-00002170: 6a73 6f6e 5b22 7374 6174 6522 5d20 3d3d  json["state"] ==
-00002180: 2022 4649 4e49 5348 4544 220a 2020 2020   "FINISHED".    
-00002190: 2320 2020 2020 2020 2020 2020 2020 293a  #             ):
-000021a0: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-000021b0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-000021c0: 726e 696e 6728 0a20 2020 2023 2020 2020  rning(.    #    
+00002100: 2020 2020 2066 6f72 206b 2069 6e20 5b22       for k in ["
+00002110: 7374 6174 6522 2c20 2272 6573 756c 7422  state", "result"
+00002120: 2c20 2265 7272 6f72 5f6d 7367 225d 0a20  , "error_msg"]. 
+00002130: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+00002140: 2020 2020 2029 0a20 2020 2023 2020 2020       ).    #    
+00002150: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00002160: 2072 6573 756c 745f 6765 745f 7374 6174   result_get_stat
+00002170: 7573 5f6a 736f 6e5b 2273 7461 7465 225d  us_json["state"]
+00002180: 203d 3d20 2246 494e 4953 4845 4422 0a20   == "FINISHED". 
+00002190: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+000021a0: 2029 3a0a 2020 2020 2320 2020 2020 2020   ):.    #       
+000021b0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+000021c0: 2e77 6172 6e69 6e67 280a 2020 2020 2320  .warning(.    # 
 000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021e0: 2022 2020 5b2b 5d20 4120 7072 6576 696f   "  [+] A previo
-000021f0: 7573 2027 7b7d 2720 6f70 6572 6174 696f  us '{}' operatio
-00002200: 6e20 7761 7320 7275 6e6e 696e 6720 666f  n was running fo
-00002210: 7220 7369 6d75 6c61 7469 6f6e 2049 4420  r simulation ID 
-00002220: 7b7d 2061 6e64 2074 6572 6d69 6e61 7465  {} and terminate
-00002230: 642c 2062 7574 2069 7473 2072 6573 756c  d, but its resul
-00002240: 7420 7761 7320 6e6f 7420 6665 7463 6865  t was not fetche
-00002250: 6420 2872 6573 756c 7420 7761 7320 7b7d  d (result was {}
-00002260: 2c20 6572 726f 7220 7761 7320 7b7d 292e  , error was {}).
-00002270: 2041 7474 656d 7074 696e 6720 7468 6520   Attempting the 
-00002280: 6f70 6572 6174 696f 6e20 6167 6169 6e2e  operation again.
-00002290: 222e 666f 726d 6174 280a 2020 2020 2320  ".format(.    # 
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022b0: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
-000022c0: 6e2c 0a20 2020 2023 2020 2020 2020 2020  n,.    #        
+000021e0: 2020 2020 2220 205b 2b5d 2041 2070 7265      "  [+] A pre
+000021f0: 7669 6f75 7320 277b 7d27 206f 7065 7261  vious '{}' opera
+00002200: 7469 6f6e 2077 6173 2072 756e 6e69 6e67  tion was running
+00002210: 2066 6f72 2073 696d 756c 6174 696f 6e20   for simulation 
+00002220: 4944 207b 7d20 616e 6420 7465 726d 696e  ID {} and termin
+00002230: 6174 6564 2c20 6275 7420 6974 7320 7265  ated, but its re
+00002240: 7375 6c74 2077 6173 206e 6f74 2066 6574  sult was not fet
+00002250: 6368 6564 2028 7265 7375 6c74 2077 6173  ched (result was
+00002260: 207b 7d2c 2065 7272 6f72 2077 6173 207b   {}, error was {
+00002270: 7d29 2e20 4174 7465 6d70 7469 6e67 2074  }). Attempting t
+00002280: 6865 206f 7065 7261 7469 6f6e 2061 6761  he operation aga
+00002290: 696e 2e22 2e66 6f72 6d61 7428 0a20 2020  in.".format(.   
+000022a0: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+000022b0: 2020 2020 2020 2020 2020 206f 7065 7261             opera
+000022c0: 7469 6f6e 2c0a 2020 2020 2320 2020 2020  tion,.    #     
 000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022e0: 2069 645f 7369 6d75 6c61 7469 6f6e 2c0a   id_simulation,.
-000022f0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00002300: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00002310: 7375 6c74 5f67 6574 5f73 7461 7475 735f  sult_get_status_
-00002320: 6a73 6f6e 5b22 7265 7375 6c74 225d 2c0a  json["result"],.
-00002330: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00002340: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00002350: 7375 6c74 5f67 6574 5f73 7461 7475 735f  sult_get_status_
-00002360: 6a73 6f6e 5b22 6572 726f 725f 6d73 6722  json["error_msg"
-00002370: 5d2c 0a20 2020 2023 2020 2020 2020 2020  ],.    #        
-00002380: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00002390: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-000023a0: 2020 2020 2029 0a20 2020 2023 2020 2020       ).    #    
-000023b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000023c0: 6d65 7468 6f64 203d 3d20 2267 6574 223a  method == "get":
-000023d0: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-000023e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000023f0: 7420 3d20 5f67 6574 2875 7269 290a 2020  t = _get(uri).  
-00002400: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-00002410: 2020 2020 656c 7365 3a0a 2020 2020 2320      else:.    # 
-00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 2020 2020 7265 7375 6c74 203d 205f 706f      result = _po
-00002440: 7374 2875 7269 290a 2020 2020 2320 2020  st(uri).    #   
-00002450: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00002460: 6f6e 3a0a 2020 2020 2320 2020 2020 2020  on:.    #       
-00002470: 2020 7061 7373 0a0a 2020 2020 6966 2072    pass..    if r
-00002480: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-00002490: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-000024a0: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-000024b0: 7265 7375 6c74 2c20 6622 4361 6e6e 6f74  result, f"Cannot
-000024c0: 2065 7865 6375 7465 206f 7065 7261 7469   execute operati
-000024d0: 6f6e 2027 7b6f 7065 7261 7469 6f6e 7d27  on '{operation}'
-000024e0: 2229 0a0a 2020 2020 2320 4765 7420 6261  ")..    # Get ba
-000024f0: 636b 2074 6865 2074 6173 6b20 6e61 6d65  ck the task name
-00002500: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
-00002510: 2020 7461 736b 5f69 6465 6e74 6966 6965    task_identifie
-00002520: 723a 2073 7472 203d 2072 6573 756c 742e  r: str = result.
-00002530: 6a73 6f6e 2829 5b22 7461 736b 5f6e 616d  json()["task_nam
-00002540: 6522 5d0a 2020 2020 6578 6365 7074 2045  e"].    except E
-00002550: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
-00002560: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00002570: 6e28 0a20 2020 2020 2020 2020 2020 2066  n(.            f
-00002580: 2243 616e 6e6f 7420 6578 6563 7574 6520  "Cannot execute 
-00002590: 6f70 6572 6174 696f 6e20 277b 6f70 6572  operation '{oper
-000025a0: 6174 696f 6e7d 273a 2049 5420 5369 6d75  ation}': IT Simu
-000025b0: 6c61 7469 6f6e 2041 5049 2064 6964 206e  lation API did n
-000025c0: 6f74 2073 656e 6420 6261 636b 2074 6865  ot send back the
-000025d0: 2074 6173 6b20 6e61 6d65 2070 726f 7065   task name prope
-000025e0: 726c 792e 2041 626f 7274 696e 672e 220a  rly. Aborting.".
-000025f0: 2020 2020 2020 2020 290a 0a20 2020 2072          )..    r
-00002600: 6574 7572 6e20 7265 7375 6c74 2c20 7461  eturn result, ta
-00002610: 736b 5f69 6465 6e74 6966 6965 720a 0a0a  sk_identifier...
-00002620: 6465 6620 5f73 696d 756c 6174 696f 6e5f  def _simulation_
-00002630: 636f 6e63 6c75 6465 5f6f 7065 7261 7469  conclude_operati
-00002640: 6f6e 280a 2020 2020 6964 5f73 696d 756c  on(.    id_simul
-00002650: 6174 696f 6e3a 2069 6e74 2c20 6f70 6572  ation: int, oper
-00002660: 6174 696f 6e3a 2073 7472 2c20 6669 6e61  ation: str, fina
-00002670: 6c5f 6f70 6572 6174 696f 6e5f 7374 6174  l_operation_stat
-00002680: 7573 3a20 4469 6374 5b73 7472 2c20 416e  us: Dict[str, An
-00002690: 795d 0a29 202d 3e20 4469 6374 5b73 7472  y].) -> Dict[str
-000026a0: 2c20 416e 795d 3a0a 2020 2020 7369 6d75  , Any]:.    simu
-000026b0: 6c61 7469 6f6e 5f64 6963 7420 3d20 6665  lation_dict = fe
-000026c0: 7463 685f 7369 6d75 6c61 7469 6f6e 2869  tch_simulation(i
-000026d0: 645f 7369 6d75 6c61 7469 6f6e 290a 2020  d_simulation).  
-000026e0: 2020 6966 2028 0a20 2020 2020 2020 2066    if (.        f
-000026f0: 696e 616c 5f6f 7065 7261 7469 6f6e 5f73  inal_operation_s
-00002700: 7461 7475 735b 2273 7461 7465 225d 2021  tatus["state"] !
-00002710: 3d20 2246 494e 4953 4845 4422 0a20 2020  = "FINISHED".   
-00002720: 2020 2020 206f 7220 6669 6e61 6c5f 6f70       or final_op
-00002730: 6572 6174 696f 6e5f 7374 6174 7573 5b22  eration_status["
-00002740: 6572 726f 725f 6d73 6722 5d20 6973 206e  error_msg"] is n
-00002750: 6f74 204e 6f6e 650a 2020 2020 293a 0a20  ot None.    ):. 
-00002760: 2020 2020 2020 2023 2053 6f6d 6574 6869         # Somethi
-00002770: 6e67 2077 656e 7420 7772 6f6e 670a 2020  ng went wrong.  
-00002780: 2020 2020 2020 2320 5261 6973 6520 616e        # Raise an
-00002790: 2065 7863 6570 7469 6f6e 2c20 6275 7420   exception, but 
-000027a0: 616c 736f 2065 6e73 7572 6520 7468 6174  also ensure that
-000027b0: 2074 6865 2073 696d 756c 6174 696f 6e20   the simulation 
-000027c0: 7374 6174 7573 2069 7320 4552 524f 520a  status is ERROR.
-000027d0: 2020 2020 2020 2020 6966 2066 696e 616c          if final
-000027e0: 5f6f 7065 7261 7469 6f6e 5f73 7461 7475  _operation_statu
-000027f0: 735b 2273 7461 7465 225d 2021 3d20 2246  s["state"] != "F
-00002800: 494e 4953 4845 4422 3a0a 2020 2020 2020  INISHED":.      
-00002810: 2020 2020 2020 2320 5368 6f75 6c64 206e        # Should n
-00002820: 6576 6572 2068 6170 7065 6e2c 206e 6f72  ever happen, nor
-00002830: 6d61 6c6c 790a 2020 2020 2020 2020 2020  mally.          
-00002840: 2020 6572 726f 725f 6d73 6720 3d20 2245    error_msg = "E
-00002850: 7272 6f72 2064 7572 696e 6720 7369 6d75  rror during simu
-00002860: 6c61 7469 6f6e 206f 7065 7261 7469 6f6e  lation operation
-00002870: 2027 7b7d 2720 6f6e 2073 696d 756c 6174   '{}' on simulat
-00002880: 696f 6e20 4944 2027 7b7d 2720 2874 6173  ion ID '{}' (tas
-00002890: 6b20 6964 207b 7d29 3a20 6f70 6572 6174  k id {}): operat
-000028a0: 696f 6e20 656e 6465 6420 756e 6578 7065  ion ended unexpe
-000028b0: 6374 6564 6c79 2e20 5468 6520 6f70 6572  ctedly. The oper
-000028c0: 6174 696f 6e20 7374 6174 7573 2069 7320  ation status is 
-000028d0: 277b 7d27 2061 6e64 2074 6865 2067 6976  '{}' and the giv
-000028e0: 656e 2065 7272 6f72 2069 7320 277b 7d27  en error is '{}'
-000028f0: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
-00002900: 2020 2020 2020 2020 2020 6f70 6572 6174            operat
-00002910: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00002920: 2020 2020 2069 645f 7369 6d75 6c61 7469       id_simulati
-00002930: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00002940: 2020 2020 6669 6e61 6c5f 6f70 6572 6174      final_operat
-00002950: 696f 6e5f 7374 6174 7573 5b22 7461 736b  ion_status["task
-00002960: 5f6e 616d 6522 5d2c 0a20 2020 2020 2020  _name"],.       
-00002970: 2020 2020 2020 2020 2066 696e 616c 5f6f           final_o
-00002980: 7065 7261 7469 6f6e 5f73 7461 7475 735b  peration_status[
-00002990: 2273 7461 7465 225d 2c0a 2020 2020 2020  "state"],.      
-000029a0: 2020 2020 2020 2020 2020 6669 6e61 6c5f            final_
-000029b0: 6f70 6572 6174 696f 6e5f 7374 6174 7573  operation_status
-000029c0: 5b22 6572 726f 725f 6d73 6722 5d2c 0a20  ["error_msg"],. 
-000029d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000029e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000029f0: 2020 2020 2020 2023 2045 7272 6f72 2064         # Error d
-00002a00: 7572 696e 6720 7468 6520 6f70 6572 6174  uring the operat
-00002a10: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00002a20: 6572 726f 725f 6d73 6720 3d20 2245 7272  error_msg = "Err
-00002a30: 6f72 2064 7572 696e 6720 7369 6d75 6c61  or during simula
-00002a40: 7469 6f6e 206f 7065 7261 7469 6f6e 2027  tion operation '
-00002a50: 7b7d 2720 6f6e 2073 696d 756c 6174 696f  {}' on simulatio
-00002a60: 6e20 4944 2027 7b7d 2720 2874 6173 6b20  n ID '{}' (task 
-00002a70: 6964 207b 7d20 293a 2072 6574 7572 6e65  id {} ): returne
-00002a80: 6420 6572 726f 7220 6d65 7373 6167 6520  d error message 
-00002a90: 6973 2027 7b7d 2722 2e66 6f72 6d61 7428  is '{}'".format(
-00002aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ab0: 206f 7065 7261 7469 6f6e 2c0a 2020 2020   operation,.    
-00002ac0: 2020 2020 2020 2020 2020 2020 6964 5f73              id_s
-00002ad0: 696d 756c 6174 696f 6e2c 0a20 2020 2020  imulation,.     
-00002ae0: 2020 2020 2020 2020 2020 2066 696e 616c             final
-00002af0: 5f6f 7065 7261 7469 6f6e 5f73 7461 7475  _operation_statu
-00002b00: 735b 2274 6173 6b5f 6e61 6d65 225d 2c0a  s["task_name"],.
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 6669 6e61 6c5f 6f70 6572 6174 696f 6e5f  final_operation_
-00002b30: 7374 6174 7573 5b22 6572 726f 725f 6d73  status["error_ms
-00002b40: 6722 5d2c 0a20 2020 2020 2020 2020 2020  g"],.           
-00002b50: 2029 0a0a 2020 2020 2020 2020 2320 5570   )..        # Up
-00002b60: 6461 7465 2073 696d 756c 6174 696f 6e20  date simulation 
-00002b70: 7374 6174 7573 2069 6620 6e65 6365 7373  status if necess
-00002b80: 6172 790a 2020 2020 2020 2020 6966 2073  ary.        if s
-00002b90: 696d 756c 6174 696f 6e5f 6469 6374 5b22  imulation_dict["
-00002ba0: 7374 6174 7573 225d 2021 3d20 2245 5252  status"] != "ERR
-00002bb0: 4f52 223a 0a20 2020 2020 2020 2020 2020  OR":.           
-00002bc0: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
-00002bd0: 5b22 7374 6174 7573 225d 203d 2022 4552  ["status"] = "ER
-00002be0: 524f 5222 0a20 2020 2020 2020 2020 2020  ROR".           
-00002bf0: 2064 6174 6120 3d20 7b22 7374 6174 7573   data = {"status
-00002c00: 223a 2022 4552 524f 5222 7d0a 2020 2020  ": "ERROR"}.    
-00002c10: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-00002c20: 2020 2020 2020 2020 2020 2020 2073 696d               sim
-00002c30: 756c 6174 696f 6e5f 6469 6374 5b22 6572  ulation_dict["er
-00002c40: 726f 725f 6d73 6722 5d20 6973 206e 6f74  ror_msg"] is not
-00002c50: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00002c60: 2020 2020 2020 616e 6420 6c65 6e28 7369        and len(si
-00002c70: 6d75 6c61 7469 6f6e 5f64 6963 745b 2265  mulation_dict["e
-00002c80: 7272 6f72 5f6d 7367 225d 2920 3e20 300a  rror_msg"]) > 0.
-00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ca0: 616e 6420 7369 6d75 6c61 7469 6f6e 5f64  and simulation_d
-00002cb0: 6963 745b 2265 7272 6f72 5f6d 7367 225d  ict["error_msg"]
-00002cc0: 2021 3d20 224e 6f6e 6522 0a20 2020 2020   != "None".     
-00002cd0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00002ce0: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
-00002cf0: 6572 726f 725f 6d73 6722 5d20 3d20 7369  error_msg"] = si
-00002d00: 6d75 6c61 7469 6f6e 5f64 6963 745b 0a20  mulation_dict[. 
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2022 6572 726f 725f 6d73 6722 0a20     "error_msg". 
-00002d30: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00002d40: 202b 2022 2e20 416e 6f74 6865 7220 6572   + ". Another er
-00002d50: 726f 7220 6f63 6375 7265 643a 207b 7d22  ror occured: {}"
-00002d60: 2e66 6f72 6d61 7428 6572 726f 725f 6d73  .format(error_ms
-00002d70: 6729 0a20 2020 2020 2020 2020 2020 2065  g).            e
-00002d80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00002d90: 2020 2020 2064 6174 615b 2265 7272 6f72       data["error
-00002da0: 5f6d 7367 225d 203d 2065 7272 6f72 5f6d  _msg"] = error_m
-00002db0: 7367 0a20 2020 2020 2020 2020 2020 2075  sg.            u
-00002dc0: 7064 6174 655f 7369 6d75 6c61 7469 6f6e  pdate_simulation
-00002dd0: 2869 645f 7369 6d75 6c61 7469 6f6e 2c20  (id_simulation, 
-00002de0: 6461 7461 290a 0a20 2020 2020 2020 2072  data)..        r
-00002df0: 6169 7365 2045 7863 6570 7469 6f6e 2865  aise Exception(e
-00002e00: 7272 6f72 5f6d 7367 290a 2020 2020 656c  rror_msg).    el
-00002e10: 7365 3a0a 2020 2020 2020 2020 2320 416c  se:.        # Al
-00002e20: 6c20 7765 6e74 2077 656c 6c0a 0a20 2020  l went well..   
-00002e30: 2020 2020 2023 2044 656c 6574 6520 7468       # Delete th
-00002e40: 6520 6572 726f 7220 6d65 7373 6167 6520  e error message 
-00002e50: 696e 2064 622c 2069 6620 6e65 6365 7373  in db, if necess
-00002e60: 6172 790a 2020 2020 2020 2020 6966 2028  ary.        if (
-00002e70: 0a20 2020 2020 2020 2020 2020 2073 696d  .            sim
-00002e80: 756c 6174 696f 6e5f 6469 6374 5b22 7374  ulation_dict["st
-00002e90: 6174 7573 225d 2021 3d20 2245 5252 4f52  atus"] != "ERROR
-00002ea0: 220a 2020 2020 2020 2020 2020 2020 616e  ".            an
-00002eb0: 6420 7369 6d75 6c61 7469 6f6e 5f64 6963  d simulation_dic
-00002ec0: 745b 2265 7272 6f72 5f6d 7367 225d 2069  t["error_msg"] i
-00002ed0: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-00002ee0: 2020 2020 2020 2061 6e64 206c 656e 2873         and len(s
-00002ef0: 696d 756c 6174 696f 6e5f 6469 6374 5b22  imulation_dict["
-00002f00: 6572 726f 725f 6d73 6722 5d29 203e 2030  error_msg"]) > 0
-00002f10: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00002f20: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
-00002f30: 5b22 6572 726f 725f 6d73 6722 5d20 213d  ["error_msg"] !=
-00002f40: 2022 4e6f 6e65 220a 2020 2020 2020 2020   "None".        
-00002f50: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00002f60: 696d 756c 6174 696f 6e5f 6469 6374 5b22  imulation_dict["
-00002f70: 6572 726f 725f 6d73 6722 5d20 3d20 224e  error_msg"] = "N
-00002f80: 6f6e 6522 0a20 2020 2020 2020 2020 2020  one".           
-00002f90: 2064 6174 6120 3d20 7b22 6572 726f 725f   data = {"error_
-00002fa0: 6d73 6722 3a20 7369 6d75 6c61 7469 6f6e  msg": simulation
-00002fb0: 5f64 6963 745b 2265 7272 6f72 5f6d 7367  _dict["error_msg
-00002fc0: 225d 7d0a 2020 2020 2020 2020 2020 2020  "]}.            
-00002fd0: 7570 6461 7465 5f73 696d 756c 6174 696f  update_simulatio
-00002fe0: 6e28 6964 5f73 696d 756c 6174 696f 6e2c  n(id_simulation,
-00002ff0: 2064 6174 6129 0a0a 2020 2020 2020 2020   data)..        
-00003000: 6966 2066 696e 616c 5f6f 7065 7261 7469  if final_operati
-00003010: 6f6e 5f73 7461 7475 735b 2272 6573 756c  on_status["resul
-00003020: 7422 5d3a 0a20 2020 2020 2020 2020 2020  t"]:.           
-00003030: 2072 6573 756c 745f 6f70 6572 6174 696f   result_operatio
-00003040: 6e20 3d20 2220 5265 7375 6c74 2069 733a  n = " Result is:
-00003050: 205c 6e7b 7d22 2e66 6f72 6d61 7428 0a20   \n{}".format(. 
-00003060: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00003070: 696e 616c 5f6f 7065 7261 7469 6f6e 5f73  inal_operation_s
-00003080: 7461 7475 735b 2272 6573 756c 7422 5d0a  tatus["result"].
-00003090: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000030a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000030b0: 2020 2020 2020 2020 7265 7375 6c74 5f6f          result_o
-000030c0: 7065 7261 7469 6f6e 203d 2022 220a 2020  peration = "".  
-000030d0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-000030e0: 6f28 0a20 2020 2020 2020 2020 2020 2022  o(.            "
-000030f0: 5b2b 5d20 4f70 6572 6174 696f 6e20 277b  [+] Operation '{
-00003100: 7d27 206f 6e20 7369 6d75 6c61 7469 6f6e  }' on simulation
-00003110: 2049 4420 277b 7d27 2028 7461 736b 2069   ID '{}' (task i
-00003120: 6420 7b7d 2920 7761 7320 636f 7272 6563  d {}) was correc
-00003130: 746c 7920 6578 6563 7574 6564 2e7b 7d22  tly executed.{}"
-00003140: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00003150: 2020 2020 2020 2020 206f 7065 7261 7469           operati
-00003160: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00003170: 2020 2020 6964 5f73 696d 756c 6174 696f      id_simulatio
-00003180: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00003190: 2020 2066 696e 616c 5f6f 7065 7261 7469     final_operati
-000031a0: 6f6e 5f73 7461 7475 735b 2274 6173 6b5f  on_status["task_
-000031b0: 6e61 6d65 225d 2c0a 2020 2020 2020 2020  name"],.        
-000031c0: 2020 2020 2020 2020 7265 7375 6c74 5f6f          result_o
-000031d0: 7065 7261 7469 6f6e 2c0a 2020 2020 2020  peration,.      
-000031e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000031f0: 290a 2020 2020 7265 7475 726e 2073 696d  ).    return sim
-00003200: 756c 6174 696f 6e5f 6469 6374 0a0a 0a64  ulation_dict...d
-00003210: 6566 205f 7661 6c69 6461 7465 5f79 616d  ef _validate_yam
-00003220: 6c5f 746f 706f 6c6f 6779 5f66 696c 6528  l_topology_file(
-00003230: 7961 6d6c 5f63 6f6e 6669 6775 7261 7469  yaml_configurati
-00003240: 6f6e 5f66 696c 653a 2073 7472 2920 2d3e  on_file: str) ->
-00003250: 204e 6f6e 653a 0a20 2020 2069 6620 6f73   None:.    if os
-00003260: 2e70 6174 682e 6578 6973 7473 2879 616d  .path.exists(yam
-00003270: 6c5f 636f 6e66 6967 7572 6174 696f 6e5f  l_configuration_
-00003280: 6669 6c65 2920 6973 206e 6f74 2054 7275  file) is not Tru
-00003290: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
-000032a0: 2045 7863 6570 7469 6f6e 280a 2020 2020   Exception(.    
-000032b0: 2020 2020 2020 2020 2254 6865 2070 726f          "The pro
-000032c0: 7669 6465 6420 5941 4d4c 2063 6f6e 6669  vided YAML confi
-000032d0: 6775 7261 7469 6f6e 2070 6174 6820 646f  guration path do
-000032e0: 6573 206e 6f74 2065 7869 7374 3a20 277b  es not exist: '{
-000032f0: 7d27 222e 666f 726d 6174 280a 2020 2020  }'".format(.    
-00003300: 2020 2020 2020 2020 2020 2020 7961 6d6c              yaml
-00003310: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f66  _configuration_f
-00003320: 696c 650a 2020 2020 2020 2020 2020 2020  ile.            
-00003330: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-00003340: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
-00003350: 6c65 2879 616d 6c5f 636f 6e66 6967 7572  le(yaml_configur
-00003360: 6174 696f 6e5f 6669 6c65 2920 6973 206e  ation_file) is n
-00003370: 6f74 2054 7275 653a 0a20 2020 2020 2020  ot True:.       
-00003380: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-00003390: 280a 2020 2020 2020 2020 2020 2020 2254  (.            "T
-000033a0: 6865 2070 726f 7669 6465 6420 5941 4d4c  he provided YAML
-000033b0: 2063 6f6e 6669 6775 7261 7469 6f6e 2070   configuration p
-000033c0: 6174 6820 6973 206e 6f74 2061 2066 696c  ath is not a fil
-000033d0: 653a 2027 7b7d 2722 2e66 6f72 6d61 7428  e: '{}'".format(
-000033e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000033f0: 2079 616d 6c5f 636f 6e66 6967 7572 6174   yaml_configurat
-00003400: 696f 6e5f 6669 6c65 0a20 2020 2020 2020  ion_file.       
-00003410: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
-00003420: 0a0a 2020 2020 6966 206f 732e 6163 6365  ..    if os.acce
-00003430: 7373 2879 616d 6c5f 636f 6e66 6967 7572  ss(yaml_configur
-00003440: 6174 696f 6e5f 6669 6c65 2c20 6f73 2e52  ation_file, os.R
-00003450: 5f4f 4b29 2069 7320 6e6f 7420 5472 7565  _OK) is not True
-00003460: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00003470: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
-00003480: 2020 2020 2020 2022 5468 6520 7072 6f76         "The prov
-00003490: 6964 6564 2059 414d 4c20 636f 6e66 6967  ided YAML config
-000034a0: 7572 6174 696f 6e20 6669 6c65 2069 7320  uration file is 
-000034b0: 6e6f 7420 7265 6164 6162 6c65 3a20 277b  not readable: '{
-000034c0: 7d27 222e 666f 726d 6174 280a 2020 2020  }'".format(.    
-000034d0: 2020 2020 2020 2020 2020 2020 7961 6d6c              yaml
-000034e0: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f66  _configuration_f
-000034f0: 696c 650a 2020 2020 2020 2020 2020 2020  ile.            
-00003500: 290a 2020 2020 2020 2020 290a 0a0a 6465  ).        )...de
-00003510: 6620 5f72 6561 645f 7961 6d6c 5f74 6f70  f _read_yaml_top
-00003520: 6f6c 6f67 795f 6669 6c65 2879 616d 6c5f  ology_file(yaml_
-00003530: 636f 6e66 6967 7572 6174 696f 6e5f 6669  configuration_fi
-00003540: 6c65 3a20 7374 7229 202d 3e20 7374 723a  le: str) -> str:
-00003550: 0a20 2020 2077 6974 6820 6f70 656e 2879  .    with open(y
-00003560: 616d 6c5f 636f 6e66 6967 7572 6174 696f  aml_configuratio
-00003570: 6e5f 6669 6c65 2c20 2272 2229 2061 7320  n_file, "r") as 
-00003580: 6664 3a0a 2020 2020 2020 2020 7961 6d6c  fd:.        yaml
-00003590: 5f63 6f6e 7465 6e74 203d 2066 642e 7265  _content = fd.re
-000035a0: 6164 2829 0a20 2020 2020 2020 2072 6574  ad().        ret
-000035b0: 7572 6e20 7961 6d6c 5f63 6f6e 7465 6e74  urn yaml_content
-000035c0: 0a0a 0a64 6566 205f 7a69 705f 7265 736f  ...def _zip_reso
-000035d0: 7572 6365 7328 7265 736f 7572 6365 735f  urces(resources_
-000035e0: 7061 7468 3a20 5061 7468 2c20 7465 6d70  path: Path, temp
-000035f0: 5f64 6972 3a20 5061 7468 2920 2d3e 2050  _dir: Path) -> P
-00003600: 6174 683a 0a20 2020 2022 2222 0a20 2020  ath:.    """.   
-00003610: 205a 6970 2061 2066 6f6c 6465 7220 696e   Zip a folder in
-00003620: 2061 6e20 6172 6368 6976 650a 2020 2020   an archive.    
-00003630: 2222 220a 2020 2020 6469 725f 6e61 6d65  """.    dir_name
-00003640: 3a20 7374 7220 3d20 6f73 2e70 6174 682e  : str = os.path.
-00003650: 6261 7365 6e61 6d65 286f 732e 7061 7468  basename(os.path
-00003660: 2e6e 6f72 6d70 6174 6828 7265 736f 7572  .normpath(resour
-00003670: 6365 735f 7061 7468 2929 0a20 2020 207a  ces_path)).    z
-00003680: 6970 5f62 6173 655f 6e61 6d65 3a20 7374  ip_base_name: st
-00003690: 7220 3d20 6f73 2e70 6174 682e 6a6f 696e  r = os.path.join
-000036a0: 2874 656d 705f 6469 722c 2064 6972 5f6e  (temp_dir, dir_n
-000036b0: 616d 6529 0a20 2020 207a 6970 5f66 6f72  ame).    zip_for
-000036c0: 6d61 743a 2073 7472 203d 2022 7a69 7022  mat: str = "zip"
-000036d0: 0a20 2020 2077 6974 6820 7368 7574 696c  .    with shutil
-000036e0: 5f6d 616b 655f 6172 6368 6976 655f 6c6f  _make_archive_lo
-000036f0: 636b 3a0a 2020 2020 2020 2020 7368 7574  ck:.        shut
-00003700: 696c 2e6d 616b 655f 6172 6368 6976 6528  il.make_archive(
-00003710: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
-00003720: 655f 6e61 6d65 3d7a 6970 5f62 6173 655f  e_name=zip_base_
-00003730: 6e61 6d65 2c20 666f 726d 6174 3d7a 6970  name, format=zip
-00003740: 5f66 6f72 6d61 742c 2072 6f6f 745f 6469  _format, root_di
-00003750: 723d 7265 736f 7572 6365 735f 7061 7468  r=resources_path
-00003760: 0a20 2020 2020 2020 2029 0a20 2020 2072  .        ).    r
-00003770: 6574 7572 6e20 227b 7d2e 7a69 7022 2e66  eturn "{}.zip".f
-00003780: 6f72 6d61 7428 7a69 705f 6261 7365 5f6e  ormat(zip_base_n
-00003790: 616d 6529 0a0a 0a23 204d 6f64 6966 7920  ame)...# Modify 
-000037a0: 7468 6520 746f 706f 6c6f 6779 2074 6f20  the topology to 
-000037b0: 6164 6420 7061 7261 6d65 7465 7273 2074  add parameters t
-000037c0: 6861 7420 6361 6e20 6265 2064 6564 7563  hat can be deduc
-000037d0: 6564 2062 790a 2320 7265 6164 696e 6720  ed by.# reading 
-000037e0: 7468 6520 746f 706f 6c6f 6779 0a64 6566  the topology.def
-000037f0: 205f 7369 6d75 5f63 7265 6174 655f 6164   _simu_create_ad
-00003800: 645f 696d 706c 6963 6974 5f74 6f70 6f5f  d_implicit_topo_
-00003810: 7061 7261 6d65 7465 7273 2874 6f70 6f6c  parameters(topol
-00003820: 6f67 793a 2041 6e79 2920 2d3e 204e 6f6e  ogy: Any) -> Non
-00003830: 653a 0a20 2020 2023 2041 6464 2061 2022  e:.    # Add a "
-00003840: 646e 7322 2070 6172 616d 6574 6572 2074  dns" parameter t
-00003850: 6f20 646f 636b 6572 206e 6f64 6573 2062  o docker nodes b
-00003860: 7920 6465 6475 6369 6e67 2069 7420 6672  y deducing it fr
-00003870: 6f6d 0a20 2020 2023 2072 6561 6469 6e67  om.    # reading
-00003880: 2074 6865 2022 6468 6370 5f6e 616d 6573   the "dhcp_names
-00003890: 6572 7665 7222 206f 6620 726f 7574 6572  erver" of router
-000038a0: 206e 6f64 6573 0a20 2020 205f 7369 6d75   nodes.    _simu
-000038b0: 5f63 7265 6174 655f 6164 645f 696d 706c  _create_add_impl
-000038c0: 6963 6974 5f64 6e73 5f70 6172 616d 6574  icit_dns_paramet
-000038d0: 6572 2874 6f70 6f6c 6f67 7929 0a0a 0a64  er(topology)...d
-000038e0: 6566 205f 7369 6d75 5f63 7265 6174 655f  ef _simu_create_
-000038f0: 6164 645f 696d 706c 6963 6974 5f64 6e73  add_implicit_dns
-00003900: 5f70 6172 616d 6574 6572 2874 6f70 6f6c  _parameter(topol
-00003910: 6f67 793a 2041 6e79 2920 2d3e 204e 6f6e  ogy: Any) -> Non
-00003920: 653a 0a20 2020 2023 204c 6973 7420 7468  e:.    # List th
-00003930: 6520 444e 5320 7365 7276 6572 7320 616e  e DNS servers an
-00003940: 6420 7468 6569 7220 7377 6974 6368 6573  d their switches
-00003950: 0a20 2020 2073 7769 7463 685f 6e61 6d65  .    switch_name
-00003960: 5f74 6f5f 646e 735f 6970 203d 2064 6963  _to_dns_ip = dic
-00003970: 7428 290a 2020 2020 666f 7220 6c69 6e6b  t().    for link
-00003980: 2069 6e20 746f 706f 6c6f 6779 5b22 6c69   in topology["li
-00003990: 6e6b 7322 5d3a 0a20 2020 2020 2020 2069  nks"]:.        i
-000039a0: 6620 2274 7970 6522 206e 6f74 2069 6e20  f "type" not in 
-000039b0: 6c69 6e6b 5b22 6e6f 6465 225d 3a0a 2020  link["node"]:.  
-000039c0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-000039d0: 7565 0a20 2020 2020 2020 2069 6620 6c69  ue.        if li
-000039e0: 6e6b 5b22 6e6f 6465 225d 5b22 7479 7065  nk["node"]["type
-000039f0: 225d 203d 3d20 2272 6f75 7465 7222 3a0a  "] == "router":.
-00003a00: 2020 2020 2020 2020 2020 2020 7061 7261              para
-00003a10: 6d73 203d 206c 696e 6b5b 2270 6172 616d  ms = link["param
-00003a20: 7322 5d0a 2020 2020 2020 2020 2020 2020  s"].            
-00003a30: 6966 2022 6468 6370 5f6e 616d 6573 6572  if "dhcp_nameser
-00003a40: 7665 7222 206e 6f74 2069 6e20 7061 7261  ver" not in para
-00003a50: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00003a60: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-00003a70: 2020 2020 2020 2020 2064 6e73 5f73 6572           dns_ser
-00003a80: 7665 725f 6970 203d 2070 6172 616d 735b  ver_ip = params[
-00003a90: 2264 6863 705f 6e61 6d65 7365 7276 6572  "dhcp_nameserver
-00003aa0: 225d 0a20 2020 2020 2020 2020 2020 2069  "].            i
-00003ab0: 6620 226e 616d 6522 206e 6f74 2069 6e20  f "name" not in 
-00003ac0: 6c69 6e6b 5b22 7377 6974 6368 225d 3a0a  link["switch"]:.
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00003af0: 2020 2020 2073 775f 6e61 6d65 203d 206c       sw_name = l
-00003b00: 696e 6b5b 2273 7769 7463 6822 5d5b 226e  ink["switch"]["n
-00003b10: 616d 6522 5d0a 2020 2020 2020 2020 2020  ame"].          
-00003b20: 2020 6966 2073 775f 6e61 6d65 206e 6f74    if sw_name not
-00003b30: 2069 6e20 7377 6974 6368 5f6e 616d 655f   in switch_name_
-00003b40: 746f 5f64 6e73 5f69 703a 0a20 2020 2020  to_dns_ip:.     
-00003b50: 2020 2020 2020 2020 2020 2073 7769 7463             switc
-00003b60: 685f 6e61 6d65 5f74 6f5f 646e 735f 6970  h_name_to_dns_ip
-00003b70: 5b73 775f 6e61 6d65 5d20 3d20 5b5d 0a20  [sw_name] = []. 
-00003b80: 2020 2020 2020 2020 2020 2073 7769 7463             switc
-00003b90: 685f 6e61 6d65 5f74 6f5f 646e 735f 6970  h_name_to_dns_ip
-00003ba0: 5b73 775f 6e61 6d65 5d2e 6170 7065 6e64  [sw_name].append
-00003bb0: 2864 6e73 5f73 6572 7665 725f 6970 290a  (dns_server_ip).
-00003bc0: 0a20 2020 2023 2041 6464 2074 6865 2073  .    # Add the s
-00003bd0: 7769 7463 6865 7320 4950 7320 746f 2074  witches IPs to t
-00003be0: 6865 2064 6f63 6b65 7220 6e6f 6465 730a  he docker nodes.
-00003bf0: 2020 2020 666f 7220 6c69 6e6b 2069 6e20      for link in 
-00003c00: 746f 706f 6c6f 6779 5b22 6c69 6e6b 7322  topology["links"
-00003c10: 5d3a 0a20 2020 2020 2020 206e 6f64 6520  ]:.        node 
-00003c20: 3d20 6c69 6e6b 5b22 6e6f 6465 225d 0a20  = link["node"]. 
-00003c30: 2020 2020 2020 2069 6620 2274 7970 6522         if "type"
-00003c40: 206e 6f74 2069 6e20 6e6f 6465 3a0a 2020   not in node:.  
-00003c50: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00003c60: 7565 0a20 2020 2020 2020 2069 6620 6e6f  ue.        if no
-00003c70: 6465 5b22 7479 7065 225d 203d 3d20 2264  de["type"] == "d
-00003c80: 6f63 6b65 7222 3a0a 2020 2020 2020 2020  ocker":.        
-00003c90: 2020 2020 7377 203d 206c 696e 6b5b 2273      sw = link["s
-00003ca0: 7769 7463 6822 5d5b 226e 616d 6522 5d0a  witch"]["name"].
-00003cb0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00003cc0: 7720 6e6f 7420 696e 206c 6973 7428 7377  w not in list(sw
-00003cd0: 6974 6368 5f6e 616d 655f 746f 5f64 6e73  itch_name_to_dns
-00003ce0: 5f69 702e 6b65 7973 2829 293a 0a20 2020  _ip.keys()):.   
-00003cf0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00003d00: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-00003d10: 2020 646e 735f 6c69 7374 203d 2073 7769    dns_list = swi
-00003d20: 7463 685f 6e61 6d65 5f74 6f5f 646e 735f  tch_name_to_dns_
-00003d30: 6970 5b73 775d 0a20 2020 2020 2020 2020  ip[sw].         
-00003d40: 2020 2069 6620 2264 6e73 2220 6e6f 7420     if "dns" not 
-00003d50: 696e 206e 6f64 653a 0a20 2020 2020 2020  in node:.       
-00003d60: 2020 2020 2020 2020 206e 6f64 655b 2264           node["d
-00003d70: 6e73 225d 203d 205b 5d0a 2020 2020 2020  ns"] = [].      
-00003d80: 2020 2020 2020 666f 7220 646e 7320 696e        for dns in
-00003d90: 2064 6e73 5f6c 6973 743a 0a20 2020 2020   dns_list:.     
-00003da0: 2020 2020 2020 2020 2020 206e 6f64 655b             node[
-00003db0: 2264 6e73 225d 2e61 7070 656e 6428 646e  "dns"].append(dn
-00003dc0: 7329 0a20 2020 2020 2020 2020 2020 2023  s).            #
-00003dd0: 2061 6464 2061 2064 6566 6175 6c74 2064   add a default d
-00003de0: 6e73 2073 6572 7665 720a 2020 2020 2020  ns server.      
-00003df0: 2020 2020 2020 6e6f 6465 5b22 646e 7322        node["dns"
-00003e00: 5d2e 6170 7065 6e64 2822 312e 312e 312e  ].append("1.1.1.
-00003e10: 3122 290a 2020 2020 2020 2020 2020 2020  1").            
-00003e20: 2320 456e 7375 7265 2075 6e69 6369 7479  # Ensure unicity
-00003e30: 2061 6e64 206f 7264 6572 696e 672c 2066   and ordering, f
-00003e40: 726f 6d20 7079 7468 6f6e 2033 2e37 2b2c  rom python 3.7+,
-00003e50: 2062 6563 6175 7365 2064 6963 7420 6973   because dict is
-00003e60: 206f 7264 6572 6564 3a0a 2020 2020 2020   ordered:.      
-00003e70: 2020 2020 2020 6e6f 6465 5b22 646e 7322        node["dns"
-00003e80: 5d20 3d20 6c69 7374 2864 6963 742e 6672  ] = list(dict.fr
-00003e90: 6f6d 6b65 7973 286e 6f64 655b 2264 6e73  omkeys(node["dns
-00003ea0: 225d 2929 0a0a 0a64 6566 205f 5f76 616c  "]))...def __val
-00003eb0: 6964 6174 655f 7265 736f 7572 6365 735f  idate_resources_
-00003ec0: 7061 7468 280a 2020 2020 7265 736f 7572  path(.    resour
-00003ed0: 6365 735f 7061 7468 3a20 7374 722c 2072  ces_path: str, r
-00003ee0: 6169 7365 5f65 7863 6570 7469 6f6e 3a20  aise_exception: 
-00003ef0: 626f 6f6c 203d 2054 7275 650a 2920 2d3e  bool = True.) ->
-00003f00: 2062 6f6f 6c3a 0a20 2020 2023 2045 7869   bool:.    # Exi
-00003f10: 7374 7320 3f0a 2020 2020 6966 206e 6f74  sts ?.    if not
-00003f20: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
-00003f30: 7265 736f 7572 6365 735f 7061 7468 293a  resources_path):
-00003f40: 0a20 2020 2020 2020 2069 6620 7261 6973  .        if rais
-00003f50: 655f 6578 6365 7074 696f 6e3a 0a20 2020  e_exception:.   
-00003f60: 2020 2020 2020 2020 2072 6169 7365 2046           raise F
-00003f70: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
-00003f80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00003f90: 2020 6627 5468 6520 7072 6f76 6964 6564    f'The provided
-00003fa0: 2072 6573 6f75 7263 6573 2070 6174 6820   resources path 
-00003fb0: 646f 6573 206e 6f74 2065 7869 7374 3a20  does not exist: 
-00003fc0: 227b 7265 736f 7572 6365 735f 7061 7468  "{resources_path
-00003fd0: 7d22 270a 2020 2020 2020 2020 2020 2020  }"'.            
-00003fe0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00003ff0: 2046 616c 7365 0a20 2020 2023 2044 6972   False.    # Dir
-00004000: 6563 746f 7279 203f 0a20 2020 2069 6620  ectory ?.    if 
-00004010: 6e6f 7420 6f73 2e70 6174 682e 6973 6469  not os.path.isdi
-00004020: 7228 7265 736f 7572 6365 735f 7061 7468  r(resources_path
-00004030: 293a 0a20 2020 2020 2020 2069 6620 7261  ):.        if ra
-00004040: 6973 655f 6578 6365 7074 696f 6e3a 0a20  ise_exception:. 
-00004050: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00004060: 204e 6f74 4144 6972 6563 746f 7279 4572   NotADirectoryEr
-00004070: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00004080: 2020 2020 2066 2754 6865 2070 726f 7669       f'The provi
-00004090: 6465 6420 7265 736f 7572 6365 7320 7061  ded resources pa
-000040a0: 7468 2069 7320 6e6f 7420 6120 6469 7265  th is not a dire
-000040b0: 6374 6f72 793a 2022 7b72 6573 6f75 7263  ctory: "{resourc
-000040c0: 6573 5f70 6174 687d 2227 0a20 2020 2020  es_path}"'.     
-000040d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000040e0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-000040f0: 2020 2320 456d 7074 7920 3f0a 2020 2020    # Empty ?.    
-00004100: 6669 6c65 7320 3d20 6f73 2e6c 6973 7464  files = os.listd
-00004110: 6972 2872 6573 6f75 7263 6573 5f70 6174  ir(resources_pat
-00004120: 6829 0a20 2020 2069 6620 6c65 6e28 6669  h).    if len(fi
-00004130: 6c65 7329 203d 3d20 303a 0a20 2020 2020  les) == 0:.     
-00004140: 2020 2069 6620 7261 6973 655f 6578 6365     if raise_exce
-00004150: 7074 696f 6e3a 0a20 2020 2020 2020 2020  ption:.         
-00004160: 2020 2072 6169 7365 204f 5345 7272 6f72     raise OSError
-00004170: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004180: 2020 6627 5468 6520 7072 6f76 6964 6564    f'The provided
-00004190: 2072 6573 6f75 7263 6573 2070 6174 6820   resources path 
-000041a0: 6973 2061 6e20 656d 7074 7920 6469 7265  is an empty dire
-000041b0: 6374 6f72 793a 2022 7b72 6573 6f75 7263  ctory: "{resourc
-000041c0: 6573 5f70 6174 687d 2227 0a20 2020 2020  es_path}"'.     
-000041d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000041e0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-000041f0: 2020 2320 5265 6164 6162 6c65 203f 0a20    # Readable ?. 
-00004200: 2020 2066 6f72 2066 696c 655f 6e61 6d65     for file_name
-00004210: 2069 6e20 6669 6c65 733a 0a20 2020 2020   in files:.     
-00004220: 2020 2066 696c 655f 7061 7468 203d 206f     file_path = o
-00004230: 732e 7061 7468 2e6a 6f69 6e28 7265 736f  s.path.join(reso
-00004240: 7572 6365 735f 7061 7468 2c20 6669 6c65  urces_path, file
-00004250: 5f6e 616d 6529 0a20 2020 2020 2020 2069  _name).        i
-00004260: 6620 6e6f 7420 6f73 2e61 6363 6573 7328  f not os.access(
-00004270: 6669 6c65 5f70 6174 682c 206f 732e 525f  file_path, os.R_
-00004280: 4f4b 293a 0a20 2020 2020 2020 2020 2020  OK):.           
-00004290: 2069 6620 7261 6973 655f 6578 6365 7074   if raise_except
-000042a0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-000042b0: 2020 2020 2072 6169 7365 2050 6572 6d69       raise Permi
-000042c0: 7373 696f 6e45 7272 6f72 280a 2020 2020  ssionError(.    
+000022e0: 2020 2020 6964 5f73 696d 756c 6174 696f      id_simulatio
+000022f0: 6e2c 0a20 2020 2023 2020 2020 2020 2020  n,.    #        
+00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002310: 2072 6573 756c 745f 6765 745f 7374 6174   result_get_stat
+00002320: 7573 5f6a 736f 6e5b 2272 6573 756c 7422  us_json["result"
+00002330: 5d2c 0a20 2020 2023 2020 2020 2020 2020  ],.    #        
+00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002350: 2072 6573 756c 745f 6765 745f 7374 6174   result_get_stat
+00002360: 7573 5f6a 736f 6e5b 2265 7272 6f72 5f6d  us_json["error_m
+00002370: 7367 225d 2c0a 2020 2020 2320 2020 2020  sg"],.    #     
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 290a 2020 2020 2320 2020 2020 2020 2020  ).    #         
+000023a0: 2020 2020 2020 2020 290a 2020 2020 2320          ).    # 
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 6966 206d 6574 686f 6420 3d3d 2022 6765  if method == "ge
+000023d0: 7422 3a0a 2020 2020 2320 2020 2020 2020  t":.    #       
+000023e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000023f0: 7375 6c74 203d 205f 6765 7428 7572 6929  sult = _get(uri)
+00002400: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
+00002410: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00002420: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+00002430: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00002440: 5f70 6f73 7428 7572 6929 0a20 2020 2023  _post(uri).    #
+00002450: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+00002460: 7074 696f 6e3a 0a20 2020 2023 2020 2020  ption:.    #    
+00002470: 2020 2020 2070 6173 730a 0a20 2020 2069       pass..    i
+00002480: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
+00002490: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
+000024a0: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
+000024b0: 6f72 2872 6573 756c 742c 2066 2243 616e  or(result, f"Can
+000024c0: 6e6f 7420 6578 6563 7574 6520 6f70 6572  not execute oper
+000024d0: 6174 696f 6e20 277b 6f70 6572 6174 696f  ation '{operatio
+000024e0: 6e7d 2722 290a 0a20 2020 2023 2047 6574  n}'")..    # Get
+000024f0: 2062 6163 6b20 7468 6520 7461 736b 206e   back the task n
+00002500: 616d 650a 2020 2020 7472 793a 0a20 2020  ame.    try:.   
+00002510: 2020 2020 2074 6173 6b5f 6964 656e 7469       task_identi
+00002520: 6669 6572 3a20 7374 7220 3d20 7265 7375  fier: str = resu
+00002530: 6c74 2e6a 736f 6e28 295b 2274 6173 6b5f  lt.json()["task_
+00002540: 6e61 6d65 225d 0a20 2020 2065 7863 6570  name"].    excep
+00002550: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
+00002560: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00002570: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00002580: 2020 6622 4361 6e6e 6f74 2065 7865 6375    f"Cannot execu
+00002590: 7465 206f 7065 7261 7469 6f6e 2027 7b6f  te operation '{o
+000025a0: 7065 7261 7469 6f6e 7d27 3a20 4954 2053  peration}': IT S
+000025b0: 696d 756c 6174 696f 6e20 4150 4920 6469  imulation API di
+000025c0: 6420 6e6f 7420 7365 6e64 2062 6163 6b20  d not send back 
+000025d0: 7468 6520 7461 736b 206e 616d 6520 7072  the task name pr
+000025e0: 6f70 6572 6c79 2e20 4162 6f72 7469 6e67  operly. Aborting
+000025f0: 2e22 0a20 2020 2020 2020 2029 0a0a 2020  .".        )..  
+00002600: 2020 7265 7475 726e 2072 6573 756c 742c    return result,
+00002610: 2074 6173 6b5f 6964 656e 7469 6669 6572   task_identifier
+00002620: 0a0a 0a64 6566 205f 7369 6d75 6c61 7469  ...def _simulati
+00002630: 6f6e 5f63 6f6e 636c 7564 655f 6f70 6572  on_conclude_oper
+00002640: 6174 696f 6e28 0a20 2020 2069 645f 7369  ation(.    id_si
+00002650: 6d75 6c61 7469 6f6e 3a20 696e 742c 206f  mulation: int, o
+00002660: 7065 7261 7469 6f6e 3a20 7374 722c 2066  peration: str, f
+00002670: 696e 616c 5f6f 7065 7261 7469 6f6e 5f73  inal_operation_s
+00002680: 7461 7475 733a 2044 6963 745b 7374 722c  tatus: Dict[str,
+00002690: 2041 6e79 5d0a 2920 2d3e 2044 6963 745b   Any].) -> Dict[
+000026a0: 7374 722c 2041 6e79 5d3a 0a20 2020 2073  str, Any]:.    s
+000026b0: 696d 756c 6174 696f 6e5f 6469 6374 203d  imulation_dict =
+000026c0: 2066 6574 6368 5f73 696d 756c 6174 696f   fetch_simulatio
+000026d0: 6e28 6964 5f73 696d 756c 6174 696f 6e29  n(id_simulation)
+000026e0: 0a20 2020 2069 6620 280a 2020 2020 2020  .    if (.      
+000026f0: 2020 6669 6e61 6c5f 6f70 6572 6174 696f    final_operatio
+00002700: 6e5f 7374 6174 7573 5b22 7374 6174 6522  n_status["state"
+00002710: 5d20 213d 2022 4649 4e49 5348 4544 220a  ] != "FINISHED".
+00002720: 2020 2020 2020 2020 6f72 2066 696e 616c          or final
+00002730: 5f6f 7065 7261 7469 6f6e 5f73 7461 7475  _operation_statu
+00002740: 735b 2265 7272 6f72 5f6d 7367 225d 2069  s["error_msg"] i
+00002750: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2029  s not None.    )
+00002760: 3a0a 2020 2020 2020 2020 2320 536f 6d65  :.        # Some
+00002770: 7468 696e 6720 7765 6e74 2077 726f 6e67  thing went wrong
+00002780: 0a20 2020 2020 2020 2023 2052 6169 7365  .        # Raise
+00002790: 2061 6e20 6578 6365 7074 696f 6e2c 2062   an exception, b
+000027a0: 7574 2061 6c73 6f20 656e 7375 7265 2074  ut also ensure t
+000027b0: 6861 7420 7468 6520 7369 6d75 6c61 7469  hat the simulati
+000027c0: 6f6e 2073 7461 7475 7320 6973 2045 5252  on status is ERR
+000027d0: 4f52 0a20 2020 2020 2020 2069 6620 6669  OR.        if fi
+000027e0: 6e61 6c5f 6f70 6572 6174 696f 6e5f 7374  nal_operation_st
+000027f0: 6174 7573 5b22 7374 6174 6522 5d20 213d  atus["state"] !=
+00002800: 2022 4649 4e49 5348 4544 223a 0a20 2020   "FINISHED":.   
+00002810: 2020 2020 2020 2020 2023 2053 686f 756c           # Shoul
+00002820: 6420 6e65 7665 7220 6861 7070 656e 2c20  d never happen, 
+00002830: 6e6f 726d 616c 6c79 0a20 2020 2020 2020  normally.       
+00002840: 2020 2020 2065 7272 6f72 5f6d 7367 203d       error_msg =
+00002850: 2022 4572 726f 7220 6475 7269 6e67 2073   "Error during s
+00002860: 696d 756c 6174 696f 6e20 6f70 6572 6174  imulation operat
+00002870: 696f 6e20 277b 7d27 206f 6e20 7369 6d75  ion '{}' on simu
+00002880: 6c61 7469 6f6e 2049 4420 277b 7d27 2028  lation ID '{}' (
+00002890: 7461 736b 2069 6420 7b7d 293a 206f 7065  task id {}): ope
+000028a0: 7261 7469 6f6e 2065 6e64 6564 2075 6e65  ration ended une
+000028b0: 7870 6563 7465 646c 792e 2054 6865 206f  xpectedly. The o
+000028c0: 7065 7261 7469 6f6e 2073 7461 7475 7320  peration status 
+000028d0: 6973 2027 7b7d 2720 616e 6420 7468 6520  is '{}' and the 
+000028e0: 6769 7665 6e20 6572 726f 7220 6973 2027  given error is '
+000028f0: 7b7d 2722 2e66 6f72 6d61 7428 0a20 2020  {}'".format(.   
+00002900: 2020 2020 2020 2020 2020 2020 206f 7065               ope
+00002910: 7261 7469 6f6e 2c0a 2020 2020 2020 2020  ration,.        
+00002920: 2020 2020 2020 2020 6964 5f73 696d 756c          id_simul
+00002930: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
+00002940: 2020 2020 2020 2066 696e 616c 5f6f 7065         final_ope
+00002950: 7261 7469 6f6e 5f73 7461 7475 735b 2274  ration_status["t
+00002960: 6173 6b5f 6e61 6d65 225d 2c0a 2020 2020  ask_name"],.    
+00002970: 2020 2020 2020 2020 2020 2020 6669 6e61              fina
+00002980: 6c5f 6f70 6572 6174 696f 6e5f 7374 6174  l_operation_stat
+00002990: 7573 5b22 7374 6174 6522 5d2c 0a20 2020  us["state"],.   
+000029a0: 2020 2020 2020 2020 2020 2020 2066 696e               fin
+000029b0: 616c 5f6f 7065 7261 7469 6f6e 5f73 7461  al_operation_sta
+000029c0: 7475 735b 2265 7272 6f72 5f6d 7367 225d  tus["error_msg"]
+000029d0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+000029e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000029f0: 2020 2020 2020 2020 2020 2320 4572 726f            # Erro
+00002a00: 7220 6475 7269 6e67 2074 6865 206f 7065  r during the ope
+00002a10: 7261 7469 6f6e 0a20 2020 2020 2020 2020  ration.         
+00002a20: 2020 2065 7272 6f72 5f6d 7367 203d 2022     error_msg = "
+00002a30: 4572 726f 7220 6475 7269 6e67 2073 696d  Error during sim
+00002a40: 756c 6174 696f 6e20 6f70 6572 6174 696f  ulation operatio
+00002a50: 6e20 277b 7d27 206f 6e20 7369 6d75 6c61  n '{}' on simula
+00002a60: 7469 6f6e 2049 4420 277b 7d27 2028 7461  tion ID '{}' (ta
+00002a70: 736b 2069 6420 7b7d 2029 3a20 7265 7475  sk id {} ): retu
+00002a80: 726e 6564 2065 7272 6f72 206d 6573 7361  rned error messa
+00002a90: 6765 2069 7320 277b 7d27 222e 666f 726d  ge is '{}'".form
+00002aa0: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00002ab0: 2020 2020 6f70 6572 6174 696f 6e2c 0a20      operation,. 
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002ad0: 645f 7369 6d75 6c61 7469 6f6e 2c0a 2020  d_simulation,.  
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00002af0: 6e61 6c5f 6f70 6572 6174 696f 6e5f 7374  nal_operation_st
+00002b00: 6174 7573 5b22 7461 736b 5f6e 616d 6522  atus["task_name"
+00002b10: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00002b20: 2020 2066 696e 616c 5f6f 7065 7261 7469     final_operati
+00002b30: 6f6e 5f73 7461 7475 735b 2265 7272 6f72  on_status["error
+00002b40: 5f6d 7367 225d 2c0a 2020 2020 2020 2020  _msg"],.        
+00002b50: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+00002b60: 2055 7064 6174 6520 7369 6d75 6c61 7469   Update simulati
+00002b70: 6f6e 2073 7461 7475 7320 6966 206e 6563  on status if nec
+00002b80: 6573 7361 7279 0a20 2020 2020 2020 2069  essary.        i
+00002b90: 6620 7369 6d75 6c61 7469 6f6e 5f64 6963  f simulation_dic
+00002ba0: 745b 2273 7461 7475 7322 5d20 213d 2022  t["status"] != "
+00002bb0: 4552 524f 5222 3a0a 2020 2020 2020 2020  ERROR":.        
+00002bc0: 2020 2020 7369 6d75 6c61 7469 6f6e 5f64      simulation_d
+00002bd0: 6963 745b 2273 7461 7475 7322 5d20 3d20  ict["status"] = 
+00002be0: 2245 5252 4f52 220a 2020 2020 2020 2020  "ERROR".        
+00002bf0: 2020 2020 6461 7461 203d 207b 2273 7461      data = {"sta
+00002c00: 7475 7322 3a20 2245 5252 4f52 227d 0a20  tus": "ERROR"}. 
+00002c10: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 7369 6d75 6c61 7469 6f6e 5f64 6963 745b  simulation_dict[
+00002c40: 2265 7272 6f72 5f6d 7367 225d 2069 7320  "error_msg"] is 
+00002c50: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+00002c60: 2020 2020 2020 2020 2061 6e64 206c 656e           and len
+00002c70: 2873 696d 756c 6174 696f 6e5f 6469 6374  (simulation_dict
+00002c80: 5b22 6572 726f 725f 6d73 6722 5d29 203e  ["error_msg"]) >
+00002c90: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
+00002ca0: 2020 2061 6e64 2073 696d 756c 6174 696f     and simulatio
+00002cb0: 6e5f 6469 6374 5b22 6572 726f 725f 6d73  n_dict["error_ms
+00002cc0: 6722 5d20 213d 2022 4e6f 6e65 220a 2020  g"] != "None".  
+00002cd0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00002ce0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00002cf0: 615b 2265 7272 6f72 5f6d 7367 225d 203d  a["error_msg"] =
+00002d00: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
+00002d10: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00002d20: 2020 2020 2020 2265 7272 6f72 5f6d 7367        "error_msg
+00002d30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00002d40: 2020 5d20 2b20 222e 2041 6e6f 7468 6572    ] + ". Another
+00002d50: 2065 7272 6f72 206f 6363 7572 6564 3a20   error occured: 
+00002d60: 7b7d 222e 666f 726d 6174 2865 7272 6f72  {}".format(error
+00002d70: 5f6d 7367 290a 2020 2020 2020 2020 2020  _msg).          
+00002d80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00002d90: 2020 2020 2020 2020 6461 7461 5b22 6572          data["er
+00002da0: 726f 725f 6d73 6722 5d20 3d20 6572 726f  ror_msg"] = erro
+00002db0: 725f 6d73 670a 2020 2020 2020 2020 2020  r_msg.          
+00002dc0: 2020 7570 6461 7465 5f73 696d 756c 6174    update_simulat
+00002dd0: 696f 6e28 6964 5f73 696d 756c 6174 696f  ion(id_simulatio
+00002de0: 6e2c 2064 6174 6129 0a0a 2020 2020 2020  n, data)..      
+00002df0: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+00002e00: 6e28 6572 726f 725f 6d73 6729 0a20 2020  n(error_msg).   
+00002e10: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
+00002e20: 2041 6c6c 2077 656e 7420 7765 6c6c 0a0a   All went well..
+00002e30: 2020 2020 2020 2020 2320 4465 6c65 7465          # Delete
+00002e40: 2074 6865 2065 7272 6f72 206d 6573 7361   the error messa
+00002e50: 6765 2069 6e20 6462 2c20 6966 206e 6563  ge in db, if nec
+00002e60: 6573 7361 7279 0a20 2020 2020 2020 2069  essary.        i
+00002e70: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00002e80: 7369 6d75 6c61 7469 6f6e 5f64 6963 745b  simulation_dict[
+00002e90: 2273 7461 7475 7322 5d20 213d 2022 4552  "status"] != "ER
+00002ea0: 524f 5222 0a20 2020 2020 2020 2020 2020  ROR".           
+00002eb0: 2061 6e64 2073 696d 756c 6174 696f 6e5f   and simulation_
+00002ec0: 6469 6374 5b22 6572 726f 725f 6d73 6722  dict["error_msg"
+00002ed0: 5d20 6973 206e 6f74 204e 6f6e 650a 2020  ] is not None.  
+00002ee0: 2020 2020 2020 2020 2020 616e 6420 6c65            and le
+00002ef0: 6e28 7369 6d75 6c61 7469 6f6e 5f64 6963  n(simulation_dic
+00002f00: 745b 2265 7272 6f72 5f6d 7367 225d 2920  t["error_msg"]) 
+00002f10: 3e20 300a 2020 2020 2020 2020 2020 2020  > 0.            
+00002f20: 616e 6420 7369 6d75 6c61 7469 6f6e 5f64  and simulation_d
+00002f30: 6963 745b 2265 7272 6f72 5f6d 7367 225d  ict["error_msg"]
+00002f40: 2021 3d20 224e 6f6e 6522 0a20 2020 2020   != "None".     
+00002f50: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00002f60: 2020 7369 6d75 6c61 7469 6f6e 5f64 6963    simulation_dic
+00002f70: 745b 2265 7272 6f72 5f6d 7367 225d 203d  t["error_msg"] =
+00002f80: 2022 4e6f 6e65 220a 2020 2020 2020 2020   "None".        
+00002f90: 2020 2020 6461 7461 203d 207b 2265 7272      data = {"err
+00002fa0: 6f72 5f6d 7367 223a 2073 696d 756c 6174  or_msg": simulat
+00002fb0: 696f 6e5f 6469 6374 5b22 6572 726f 725f  ion_dict["error_
+00002fc0: 6d73 6722 5d7d 0a20 2020 2020 2020 2020  msg"]}.         
+00002fd0: 2020 2075 7064 6174 655f 7369 6d75 6c61     update_simula
+00002fe0: 7469 6f6e 2869 645f 7369 6d75 6c61 7469  tion(id_simulati
+00002ff0: 6f6e 2c20 6461 7461 290a 0a20 2020 2020  on, data)..     
+00003000: 2020 2069 6620 6669 6e61 6c5f 6f70 6572     if final_oper
+00003010: 6174 696f 6e5f 7374 6174 7573 5b22 7265  ation_status["re
+00003020: 7375 6c74 225d 3a0a 2020 2020 2020 2020  sult"]:.        
+00003030: 2020 2020 7265 7375 6c74 5f6f 7065 7261      result_opera
+00003040: 7469 6f6e 203d 2022 2052 6573 756c 7420  tion = " Result 
+00003050: 6973 3a5c 6e7b 7d22 2e66 6f72 6d61 7428  is:\n{}".format(
+00003060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003070: 2066 696e 616c 5f6f 7065 7261 7469 6f6e   final_operation
+00003080: 5f73 7461 7475 735b 2272 6573 756c 7422  _status["result"
+00003090: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
+000030a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000030b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000030c0: 5f6f 7065 7261 7469 6f6e 203d 2022 220a  _operation = "".
+000030d0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+000030e0: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+000030f0: 2022 5b2b 5d20 4f70 6572 6174 696f 6e20   "[+] Operation 
+00003100: 277b 7d27 206f 6e20 7369 6d75 6c61 7469  '{}' on simulati
+00003110: 6f6e 2049 4420 277b 7d27 2028 7461 736b  on ID '{}' (task
+00003120: 2069 6420 7b7d 2920 7761 7320 636f 7272   id {}) was corr
+00003130: 6563 746c 7920 6578 6563 7574 6564 2e7b  ectly executed.{
+00003140: 7d22 2e66 6f72 6d61 7428 0a20 2020 2020  }".format(.     
+00003150: 2020 2020 2020 2020 2020 206f 7065 7261             opera
+00003160: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+00003170: 2020 2020 2020 6964 5f73 696d 756c 6174        id_simulat
+00003180: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00003190: 2020 2020 2066 696e 616c 5f6f 7065 7261       final_opera
+000031a0: 7469 6f6e 5f73 7461 7475 735b 2274 6173  tion_status["tas
+000031b0: 6b5f 6e61 6d65 225d 2c0a 2020 2020 2020  k_name"],.      
+000031c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000031d0: 5f6f 7065 7261 7469 6f6e 2c0a 2020 2020  _operation,.    
+000031e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000031f0: 2020 290a 2020 2020 7265 7475 726e 2073    ).    return s
+00003200: 696d 756c 6174 696f 6e5f 6469 6374 0a0a  imulation_dict..
+00003210: 0a64 6566 205f 7661 6c69 6461 7465 5f79  .def _validate_y
+00003220: 616d 6c5f 746f 706f 6c6f 6779 5f66 696c  aml_topology_fil
+00003230: 6528 7961 6d6c 5f63 6f6e 6669 6775 7261  e(yaml_configura
+00003240: 7469 6f6e 5f66 696c 653a 2073 7472 2920  tion_file: str) 
+00003250: 2d3e 204e 6f6e 653a 0a20 2020 2069 6620  -> None:.    if 
+00003260: 6f73 2e70 6174 682e 6578 6973 7473 2879  os.path.exists(y
+00003270: 616d 6c5f 636f 6e66 6967 7572 6174 696f  aml_configuratio
+00003280: 6e5f 6669 6c65 2920 6973 206e 6f74 2054  n_file) is not T
+00003290: 7275 653a 0a20 2020 2020 2020 2072 6169  rue:.        rai
+000032a0: 7365 2045 7863 6570 7469 6f6e 280a 2020  se Exception(.  
+000032b0: 2020 2020 2020 2020 2020 2254 6865 2070            "The p
+000032c0: 726f 7669 6465 6420 5941 4d4c 2063 6f6e  rovided YAML con
+000032d0: 6669 6775 7261 7469 6f6e 2070 6174 6820  figuration path 
+000032e0: 646f 6573 206e 6f74 2065 7869 7374 3a20  does not exist: 
+000032f0: 277b 7d27 222e 666f 726d 6174 280a 2020  '{}'".format(.  
+00003300: 2020 2020 2020 2020 2020 2020 2020 7961                ya
+00003310: 6d6c 5f63 6f6e 6669 6775 7261 7469 6f6e  ml_configuration
+00003320: 5f66 696c 650a 2020 2020 2020 2020 2020  _file.          
+00003330: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
+00003340: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
+00003350: 6669 6c65 2879 616d 6c5f 636f 6e66 6967  file(yaml_config
+00003360: 7572 6174 696f 6e5f 6669 6c65 2920 6973  uration_file) is
+00003370: 206e 6f74 2054 7275 653a 0a20 2020 2020   not True:.     
+00003380: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+00003390: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+000033a0: 2254 6865 2070 726f 7669 6465 6420 5941  "The provided YA
+000033b0: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+000033c0: 2070 6174 6820 6973 206e 6f74 2061 2066   path is not a f
+000033d0: 696c 653a 2027 7b7d 2722 2e66 6f72 6d61  ile: '{}'".forma
+000033e0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+000033f0: 2020 2079 616d 6c5f 636f 6e66 6967 7572     yaml_configur
+00003400: 6174 696f 6e5f 6669 6c65 0a20 2020 2020  ation_file.     
+00003410: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00003420: 2029 0a0a 2020 2020 6966 206f 732e 6163   )..    if os.ac
+00003430: 6365 7373 2879 616d 6c5f 636f 6e66 6967  cess(yaml_config
+00003440: 7572 6174 696f 6e5f 6669 6c65 2c20 6f73  uration_file, os
+00003450: 2e52 5f4f 4b29 2069 7320 6e6f 7420 5472  .R_OK) is not Tr
+00003460: 7565 3a0a 2020 2020 2020 2020 7261 6973  ue:.        rais
+00003470: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
+00003480: 2020 2020 2020 2020 2022 5468 6520 7072           "The pr
+00003490: 6f76 6964 6564 2059 414d 4c20 636f 6e66  ovided YAML conf
+000034a0: 6967 7572 6174 696f 6e20 6669 6c65 2069  iguration file i
+000034b0: 7320 6e6f 7420 7265 6164 6162 6c65 3a20  s not readable: 
+000034c0: 277b 7d27 222e 666f 726d 6174 280a 2020  '{}'".format(.  
+000034d0: 2020 2020 2020 2020 2020 2020 2020 7961                ya
+000034e0: 6d6c 5f63 6f6e 6669 6775 7261 7469 6f6e  ml_configuration
+000034f0: 5f66 696c 650a 2020 2020 2020 2020 2020  _file.          
+00003500: 2020 290a 2020 2020 2020 2020 290a 0a0a    ).        )...
+00003510: 6465 6620 5f72 6561 645f 7961 6d6c 5f74  def _read_yaml_t
+00003520: 6f70 6f6c 6f67 795f 6669 6c65 2879 616d  opology_file(yam
+00003530: 6c5f 636f 6e66 6967 7572 6174 696f 6e5f  l_configuration_
+00003540: 6669 6c65 3a20 7374 7229 202d 3e20 7374  file: str) -> st
+00003550: 723a 0a20 2020 2077 6974 6820 6f70 656e  r:.    with open
+00003560: 2879 616d 6c5f 636f 6e66 6967 7572 6174  (yaml_configurat
+00003570: 696f 6e5f 6669 6c65 2c20 2272 2229 2061  ion_file, "r") a
+00003580: 7320 6664 3a0a 2020 2020 2020 2020 7961  s fd:.        ya
+00003590: 6d6c 5f63 6f6e 7465 6e74 203d 2066 642e  ml_content = fd.
+000035a0: 7265 6164 2829 0a20 2020 2020 2020 2072  read().        r
+000035b0: 6574 7572 6e20 7961 6d6c 5f63 6f6e 7465  eturn yaml_conte
+000035c0: 6e74 0a0a 0a64 6566 205f 7a69 705f 7265  nt...def _zip_re
+000035d0: 736f 7572 6365 7328 7265 736f 7572 6365  sources(resource
+000035e0: 735f 7061 7468 3a20 5061 7468 2c20 7465  s_path: Path, te
+000035f0: 6d70 5f64 6972 3a20 5061 7468 2920 2d3e  mp_dir: Path) ->
+00003600: 2050 6174 683a 0a20 2020 2022 2222 0a20   Path:.    """. 
+00003610: 2020 205a 6970 2061 2066 6f6c 6465 7220     Zip a folder 
+00003620: 696e 2061 6e20 6172 6368 6976 650a 2020  in an archive.  
+00003630: 2020 2222 220a 2020 2020 6469 725f 6e61    """.    dir_na
+00003640: 6d65 3a20 7374 7220 3d20 6f73 2e70 6174  me: str = os.pat
+00003650: 682e 6261 7365 6e61 6d65 286f 732e 7061  h.basename(os.pa
+00003660: 7468 2e6e 6f72 6d70 6174 6828 7265 736f  th.normpath(reso
+00003670: 7572 6365 735f 7061 7468 2929 0a20 2020  urces_path)).   
+00003680: 207a 6970 5f62 6173 655f 6e61 6d65 3a20   zip_base_name: 
+00003690: 7374 7220 3d20 6f73 2e70 6174 682e 6a6f  str = os.path.jo
+000036a0: 696e 2874 656d 705f 6469 722c 2064 6972  in(temp_dir, dir
+000036b0: 5f6e 616d 6529 0a20 2020 207a 6970 5f66  _name).    zip_f
+000036c0: 6f72 6d61 743a 2073 7472 203d 2022 7a69  ormat: str = "zi
+000036d0: 7022 0a20 2020 2077 6974 6820 7368 7574  p".    with shut
+000036e0: 696c 5f6d 616b 655f 6172 6368 6976 655f  il_make_archive_
+000036f0: 6c6f 636b 3a0a 2020 2020 2020 2020 7368  lock:.        sh
+00003700: 7574 696c 2e6d 616b 655f 6172 6368 6976  util.make_archiv
+00003710: 6528 0a20 2020 2020 2020 2020 2020 2062  e(.            b
+00003720: 6173 655f 6e61 6d65 3d7a 6970 5f62 6173  ase_name=zip_bas
+00003730: 655f 6e61 6d65 2c20 666f 726d 6174 3d7a  e_name, format=z
+00003740: 6970 5f66 6f72 6d61 742c 2072 6f6f 745f  ip_format, root_
+00003750: 6469 723d 7265 736f 7572 6365 735f 7061  dir=resources_pa
+00003760: 7468 0a20 2020 2020 2020 2029 0a20 2020  th.        ).   
+00003770: 2072 6574 7572 6e20 227b 7d2e 7a69 7022   return "{}.zip"
+00003780: 2e66 6f72 6d61 7428 7a69 705f 6261 7365  .format(zip_base
+00003790: 5f6e 616d 6529 0a0a 0a23 204d 6f64 6966  _name)...# Modif
+000037a0: 7920 7468 6520 746f 706f 6c6f 6779 2074  y the topology t
+000037b0: 6f20 6164 6420 7061 7261 6d65 7465 7273  o add parameters
+000037c0: 2074 6861 7420 6361 6e20 6265 2064 6564   that can be ded
+000037d0: 7563 6564 2062 790a 2320 7265 6164 696e  uced by.# readin
+000037e0: 6720 7468 6520 746f 706f 6c6f 6779 0a64  g the topology.d
+000037f0: 6566 205f 7369 6d75 5f63 7265 6174 655f  ef _simu_create_
+00003800: 6164 645f 696d 706c 6963 6974 5f74 6f70  add_implicit_top
+00003810: 6f5f 7061 7261 6d65 7465 7273 2874 6f70  o_parameters(top
+00003820: 6f6c 6f67 793a 2041 6e79 2920 2d3e 204e  ology: Any) -> N
+00003830: 6f6e 653a 0a20 2020 2023 2041 6464 2061  one:.    # Add a
+00003840: 2022 646e 7322 2070 6172 616d 6574 6572   "dns" parameter
+00003850: 2074 6f20 646f 636b 6572 206e 6f64 6573   to docker nodes
+00003860: 2062 7920 6465 6475 6369 6e67 2069 7420   by deducing it 
+00003870: 6672 6f6d 0a20 2020 2023 2072 6561 6469  from.    # readi
+00003880: 6e67 2074 6865 2022 6468 6370 5f6e 616d  ng the "dhcp_nam
+00003890: 6573 6572 7665 7222 206f 6620 726f 7574  eserver" of rout
+000038a0: 6572 206e 6f64 6573 0a20 2020 205f 7369  er nodes.    _si
+000038b0: 6d75 5f63 7265 6174 655f 6164 645f 696d  mu_create_add_im
+000038c0: 706c 6963 6974 5f64 6e73 5f70 6172 616d  plicit_dns_param
+000038d0: 6574 6572 2874 6f70 6f6c 6f67 7929 0a0a  eter(topology)..
+000038e0: 0a64 6566 205f 7369 6d75 5f63 7265 6174  .def _simu_creat
+000038f0: 655f 6164 645f 696d 706c 6963 6974 5f64  e_add_implicit_d
+00003900: 6e73 5f70 6172 616d 6574 6572 2874 6f70  ns_parameter(top
+00003910: 6f6c 6f67 793a 2041 6e79 2920 2d3e 204e  ology: Any) -> N
+00003920: 6f6e 653a 0a20 2020 2023 204c 6973 7420  one:.    # List 
+00003930: 7468 6520 444e 5320 7365 7276 6572 7320  the DNS servers 
+00003940: 616e 6420 7468 6569 7220 7377 6974 6368  and their switch
+00003950: 6573 0a20 2020 2073 7769 7463 685f 6e61  es.    switch_na
+00003960: 6d65 5f74 6f5f 646e 735f 6970 203d 2064  me_to_dns_ip = d
+00003970: 6963 7428 290a 2020 2020 666f 7220 6c69  ict().    for li
+00003980: 6e6b 2069 6e20 746f 706f 6c6f 6779 5b22  nk in topology["
+00003990: 6c69 6e6b 7322 5d3a 0a20 2020 2020 2020  links"]:.       
+000039a0: 2069 6620 2274 7970 6522 206e 6f74 2069   if "type" not i
+000039b0: 6e20 6c69 6e6b 5b22 6e6f 6465 225d 3a0a  n link["node"]:.
+000039c0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000039d0: 696e 7565 0a20 2020 2020 2020 2069 6620  inue.        if 
+000039e0: 6c69 6e6b 5b22 6e6f 6465 225d 5b22 7479  link["node"]["ty
+000039f0: 7065 225d 203d 3d20 2272 6f75 7465 7222  pe"] == "router"
+00003a00: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00003a10: 7261 6d73 203d 206c 696e 6b5b 2270 6172  rams = link["par
+00003a20: 616d 7322 5d0a 2020 2020 2020 2020 2020  ams"].          
+00003a30: 2020 6966 2022 6468 6370 5f6e 616d 6573    if "dhcp_names
+00003a40: 6572 7665 7222 206e 6f74 2069 6e20 7061  erver" not in pa
+00003a50: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
+00003a60: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00003a70: 2020 2020 2020 2020 2020 2064 6e73 5f73             dns_s
+00003a80: 6572 7665 725f 6970 203d 2070 6172 616d  erver_ip = param
+00003a90: 735b 2264 6863 705f 6e61 6d65 7365 7276  s["dhcp_nameserv
+00003aa0: 6572 225d 0a20 2020 2020 2020 2020 2020  er"].           
+00003ab0: 2069 6620 226e 616d 6522 206e 6f74 2069   if "name" not i
+00003ac0: 6e20 6c69 6e6b 5b22 7377 6974 6368 225d  n link["switch"]
+00003ad0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003ae0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00003af0: 2020 2020 2020 2073 775f 6e61 6d65 203d         sw_name =
+00003b00: 206c 696e 6b5b 2273 7769 7463 6822 5d5b   link["switch"][
+00003b10: 226e 616d 6522 5d0a 2020 2020 2020 2020  "name"].        
+00003b20: 2020 2020 6966 2073 775f 6e61 6d65 206e      if sw_name n
+00003b30: 6f74 2069 6e20 7377 6974 6368 5f6e 616d  ot in switch_nam
+00003b40: 655f 746f 5f64 6e73 5f69 703a 0a20 2020  e_to_dns_ip:.   
+00003b50: 2020 2020 2020 2020 2020 2020 2073 7769               swi
+00003b60: 7463 685f 6e61 6d65 5f74 6f5f 646e 735f  tch_name_to_dns_
+00003b70: 6970 5b73 775f 6e61 6d65 5d20 3d20 5b5d  ip[sw_name] = []
+00003b80: 0a20 2020 2020 2020 2020 2020 2073 7769  .            swi
+00003b90: 7463 685f 6e61 6d65 5f74 6f5f 646e 735f  tch_name_to_dns_
+00003ba0: 6970 5b73 775f 6e61 6d65 5d2e 6170 7065  ip[sw_name].appe
+00003bb0: 6e64 2864 6e73 5f73 6572 7665 725f 6970  nd(dns_server_ip
+00003bc0: 290a 0a20 2020 2023 2041 6464 2074 6865  )..    # Add the
+00003bd0: 2073 7769 7463 6865 7320 4950 7320 746f   switches IPs to
+00003be0: 2074 6865 2064 6f63 6b65 7220 6e6f 6465   the docker node
+00003bf0: 730a 2020 2020 666f 7220 6c69 6e6b 2069  s.    for link i
+00003c00: 6e20 746f 706f 6c6f 6779 5b22 6c69 6e6b  n topology["link
+00003c10: 7322 5d3a 0a20 2020 2020 2020 206e 6f64  s"]:.        nod
+00003c20: 6520 3d20 6c69 6e6b 5b22 6e6f 6465 225d  e = link["node"]
+00003c30: 0a20 2020 2020 2020 2069 6620 2274 7970  .        if "typ
+00003c40: 6522 206e 6f74 2069 6e20 6e6f 6465 3a0a  e" not in node:.
+00003c50: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00003c60: 696e 7565 0a20 2020 2020 2020 2069 6620  inue.        if 
+00003c70: 6e6f 6465 5b22 7479 7065 225d 203d 3d20  node["type"] == 
+00003c80: 2264 6f63 6b65 7222 3a0a 2020 2020 2020  "docker":.      
+00003c90: 2020 2020 2020 7377 203d 206c 696e 6b5b        sw = link[
+00003ca0: 2273 7769 7463 6822 5d5b 226e 616d 6522  "switch"]["name"
+00003cb0: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+00003cc0: 2073 7720 6e6f 7420 696e 206c 6973 7428   sw not in list(
+00003cd0: 7377 6974 6368 5f6e 616d 655f 746f 5f64  switch_name_to_d
+00003ce0: 6e73 5f69 702e 6b65 7973 2829 293a 0a20  ns_ip.keys()):. 
+00003cf0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00003d00: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00003d10: 2020 2020 646e 735f 6c69 7374 203d 2073      dns_list = s
+00003d20: 7769 7463 685f 6e61 6d65 5f74 6f5f 646e  witch_name_to_dn
+00003d30: 735f 6970 5b73 775d 0a20 2020 2020 2020  s_ip[sw].       
+00003d40: 2020 2020 2069 6620 2264 6e73 2220 6e6f       if "dns" no
+00003d50: 7420 696e 206e 6f64 653a 0a20 2020 2020  t in node:.     
+00003d60: 2020 2020 2020 2020 2020 206e 6f64 655b             node[
+00003d70: 2264 6e73 225d 203d 205b 5d0a 2020 2020  "dns"] = [].    
+00003d80: 2020 2020 2020 2020 666f 7220 646e 7320          for dns 
+00003d90: 696e 2064 6e73 5f6c 6973 743a 0a20 2020  in dns_list:.   
+00003da0: 2020 2020 2020 2020 2020 2020 206e 6f64               nod
+00003db0: 655b 2264 6e73 225d 2e61 7070 656e 6428  e["dns"].append(
+00003dc0: 646e 7329 0a20 2020 2020 2020 2020 2020  dns).           
+00003dd0: 2023 2061 6464 2061 2064 6566 6175 6c74   # add a default
+00003de0: 2064 6e73 2073 6572 7665 720a 2020 2020   dns server.    
+00003df0: 2020 2020 2020 2020 6e6f 6465 5b22 646e          node["dn
+00003e00: 7322 5d2e 6170 7065 6e64 2822 312e 312e  s"].append("1.1.
+00003e10: 312e 3122 290a 2020 2020 2020 2020 2020  1.1").          
+00003e20: 2020 2320 456e 7375 7265 2075 6e69 6369    # Ensure unici
+00003e30: 7479 2061 6e64 206f 7264 6572 696e 672c  ty and ordering,
+00003e40: 2066 726f 6d20 7079 7468 6f6e 2033 2e37   from python 3.7
+00003e50: 2b2c 2062 6563 6175 7365 2064 6963 7420  +, because dict 
+00003e60: 6973 206f 7264 6572 6564 3a0a 2020 2020  is ordered:.    
+00003e70: 2020 2020 2020 2020 6e6f 6465 5b22 646e          node["dn
+00003e80: 7322 5d20 3d20 6c69 7374 2864 6963 742e  s"] = list(dict.
+00003e90: 6672 6f6d 6b65 7973 286e 6f64 655b 2264  fromkeys(node["d
+00003ea0: 6e73 225d 2929 0a0a 0a64 6566 205f 5f76  ns"]))...def __v
+00003eb0: 616c 6964 6174 655f 7265 736f 7572 6365  alidate_resource
+00003ec0: 735f 7061 7468 280a 2020 2020 7265 736f  s_path(.    reso
+00003ed0: 7572 6365 735f 7061 7468 3a20 5061 7468  urces_path: Path
+00003ee0: 2c20 7261 6973 655f 6578 6365 7074 696f  , raise_exceptio
+00003ef0: 6e3a 2062 6f6f 6c20 3d20 5472 7565 0a29  n: bool = True.)
+00003f00: 202d 3e20 626f 6f6c 3a0a 2020 2020 2320   -> bool:.    # 
+00003f10: 4578 6973 7473 203f 0a20 2020 2069 6620  Exists ?.    if 
+00003f20: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
+00003f30: 7473 2872 6573 6f75 7263 6573 5f70 6174  ts(resources_pat
+00003f40: 6829 3a0a 2020 2020 2020 2020 6966 2072  h):.        if r
+00003f50: 6169 7365 5f65 7863 6570 7469 6f6e 3a0a  aise_exception:.
+00003f60: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00003f70: 6520 4669 6c65 4e6f 7446 6f75 6e64 4572  e FileNotFoundEr
+00003f80: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00003f90: 2020 2020 2066 2754 6865 2070 726f 7669       f'The provi
+00003fa0: 6465 6420 7265 736f 7572 6365 7320 7061  ded resources pa
+00003fb0: 7468 2064 6f65 7320 6e6f 7420 6578 6973  th does not exis
+00003fc0: 743a 2022 7b72 6573 6f75 7263 6573 5f70  t: "{resources_p
+00003fd0: 6174 687d 2227 0a20 2020 2020 2020 2020  ath}"'.         
+00003fe0: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
+00003ff0: 7572 6e20 4661 6c73 650a 2020 2020 2320  urn False.    # 
+00004000: 4469 7265 6374 6f72 7920 3f0a 2020 2020  Directory ?.    
+00004010: 6966 206e 6f74 206f 732e 7061 7468 2e69  if not os.path.i
+00004020: 7364 6972 2872 6573 6f75 7263 6573 5f70  sdir(resources_p
+00004030: 6174 6829 3a0a 2020 2020 2020 2020 6966  ath):.        if
+00004040: 2072 6169 7365 5f65 7863 6570 7469 6f6e   raise_exception
+00004050: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00004060: 6973 6520 4e6f 7441 4469 7265 6374 6f72  ise NotADirector
+00004070: 7945 7272 6f72 280a 2020 2020 2020 2020  yError(.        
+00004080: 2020 2020 2020 2020 6627 5468 6520 7072          f'The pr
+00004090: 6f76 6964 6564 2072 6573 6f75 7263 6573  ovided resources
+000040a0: 2070 6174 6820 6973 206e 6f74 2061 2064   path is not a d
+000040b0: 6972 6563 746f 7279 3a20 227b 7265 736f  irectory: "{reso
+000040c0: 7572 6365 735f 7061 7468 7d22 270a 2020  urces_path}"'.  
+000040d0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000040e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000040f0: 0a20 2020 2023 2045 6d70 7479 203f 0a20  .    # Empty ?. 
+00004100: 2020 2066 696c 6573 203d 206f 732e 6c69     files = os.li
+00004110: 7374 6469 7228 7265 736f 7572 6365 735f  stdir(resources_
+00004120: 7061 7468 290a 2020 2020 6966 206c 656e  path).    if len
+00004130: 2866 696c 6573 2920 3d3d 2030 3a0a 2020  (files) == 0:.  
+00004140: 2020 2020 2020 6966 2072 6169 7365 5f65        if raise_e
+00004150: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
+00004160: 2020 2020 2020 7261 6973 6520 4f53 4572        raise OSEr
+00004170: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00004180: 2020 2020 2066 2754 6865 2070 726f 7669       f'The provi
+00004190: 6465 6420 7265 736f 7572 6365 7320 7061  ded resources pa
+000041a0: 7468 2069 7320 616e 2065 6d70 7479 2064  th is an empty d
+000041b0: 6972 6563 746f 7279 3a20 227b 7265 736f  irectory: "{reso
+000041c0: 7572 6365 735f 7061 7468 7d22 270a 2020  urces_path}"'.  
+000041d0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000041e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000041f0: 0a20 2020 2023 2052 6561 6461 626c 6520  .    # Readable 
+00004200: 3f0a 2020 2020 666f 7220 6669 6c65 5f6e  ?.    for file_n
+00004210: 616d 6520 696e 2066 696c 6573 3a0a 2020  ame in files:.  
+00004220: 2020 2020 2020 6669 6c65 5f70 6174 6820        file_path 
+00004230: 3d20 6f73 2e70 6174 682e 6a6f 696e 2872  = os.path.join(r
+00004240: 6573 6f75 7263 6573 5f70 6174 682c 2066  esources_path, f
+00004250: 696c 655f 6e61 6d65 290a 2020 2020 2020  ile_name).      
+00004260: 2020 6966 206e 6f74 206f 732e 6163 6365    if not os.acce
+00004270: 7373 2866 696c 655f 7061 7468 2c20 6f73  ss(file_path, os
+00004280: 2e52 5f4f 4b29 3a0a 2020 2020 2020 2020  .R_OK):.        
+00004290: 2020 2020 6966 2072 6169 7365 5f65 7863      if raise_exc
+000042a0: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
+000042b0: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
+000042c0: 726d 6973 7369 6f6e 4572 726f 7228 0a20  rmissionError(. 
 000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042e0: 6627 5468 6520 7072 6f76 6964 6564 2072  f'The provided r
-000042f0: 6573 6f75 7263 6573 2070 6174 6820 636f  esources path co
-00004300: 6e74 6169 6e73 2075 6e72 6561 6461 626c  ntains unreadabl
-00004310: 6520 6669 6c65 733a 2022 7b72 6573 6f75  e files: "{resou
-00004320: 7263 6573 5f70 6174 687d 2227 0a20 2020  rces_path}"'.   
-00004330: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00004340: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004350: 6e20 4661 6c73 650a 2020 2020 7265 7475  n False.    retu
-00004360: 726e 2054 7275 650a 0a0a 6465 6620 5f6e  rn True...def _n
-00004370: 6f72 6d61 6c69 7a65 5f73 696d 756c 6174  ormalize_simulat
-00004380: 696f 6e5f 7265 736f 7572 6365 7328 0a20  ion_resources(. 
-00004390: 2020 2074 6f70 6f6c 6f67 795f 636f 6e74     topology_cont
-000043a0: 656e 743a 2044 6963 745b 7374 722c 2041  ent: Dict[str, A
-000043b0: 6e79 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ny] = None,.    
-000043c0: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
-000043d0: 6573 5f70 6174 6873 3a20 4f70 7469 6f6e  es_paths: Option
-000043e0: 616c 5b4c 6973 745b 5061 7468 5d5d 203d  al[List[Path]] =
-000043f0: 204e 6f6e 652c 0a29 202d 3e20 5475 706c   None,.) -> Tupl
-00004400: 655b 696e 742c 204c 6973 745b 7374 725d  e[int, List[str]
-00004410: 5d3a 0a20 2020 2022 2222 4372 6561 7465  ]:.    """Create
-00004420: 2061 206e 6577 2073 696d 756c 6174 696f   a new simulatio
-00004430: 6e20 6d6f 6465 6c20 696e 2064 6174 6162  n model in datab
-00004440: 6173 6520 6261 7365 6420 6f6e 2074 6865  ase based on the
-00004450: 2070 726f 7669 6465 6420 746f 706f 6c6f   provided topolo
-00004460: 6779 2c20 616c 6f6e 6720 7769 7468 206f  gy, along with o
-00004470: 7074 696f 6e61 6c20 7265 736f 7572 6365  ptional resource
-00004480: 2066 696c 6573 2e0a 0a20 2020 203a 7265   files...    :re
-00004490: 7475 726e 3a20 4120 7475 706c 6520 636f  turn: A tuple co
-000044a0: 6e74 6169 6e69 6e67 2074 6865 2049 4420  ntaining the ID 
-000044b0: 6f66 2074 6865 2063 7265 6174 6564 2073  of the created s
-000044c0: 696d 756c 6174 696f 6e2c 2061 6e64 2074  imulation, and t
-000044d0: 6865 206e 6577 206e 6f64 6573 206f 6620  he new nodes of 
-000044e0: 7468 6520 7369 6d75 6c61 7469 6f6e 2e0a  the simulation..
-000044f0: 2020 2020 3a72 7479 7065 3a20 3a63 6c61      :rtype: :cla
-00004500: 7373 3a60 5475 706c 655b 696e 742c 204c  ss:`Tuple[int, L
-00004510: 6973 745b 7374 725d 5d60 0a0a 2020 2020  ist[str]]`..    
-00004520: 3a70 6172 616d 2074 6f70 6f6c 6f67 795f  :param topology_
-00004530: 636f 6e74 656e 743a 2041 2064 6963 7420  content: A dict 
-00004540: 636f 6e74 6169 6e69 6e67 2074 6865 206e  containing the n
-00004550: 6f64 6573 2061 6e64 206e 6574 776f 726b  odes and network
-00004560: 2074 6f70 6f6c 6f67 7920 746f 2063 7265   topology to cre
-00004570: 6174 652e 0a20 2020 203a 7479 7065 2074  ate..    :type t
-00004580: 6f70 6f6c 6f67 795f 6669 6c65 3a20 3a63  opology_file: :c
-00004590: 6c61 7373 3a60 6469 6374 600a 2020 2020  lass:`dict`.    
-000045a0: 3a70 6172 616d 2074 6f70 6f6c 6f67 795f  :param topology_
-000045b0: 7265 736f 7572 6365 735f 7061 7468 733a  resources_paths:
-000045c0: 2054 6865 2070 6174 6820 746f 2072 6573   The path to res
-000045d0: 6f75 7263 6573 2074 6861 7420 7769 6c6c  ources that will
-000045e0: 2062 6520 7075 7368 6564 2069 6e74 6f20   be pushed into 
-000045f0: 636f 6d70 6174 6962 6c65 206e 6f64 6573  compatible nodes
-00004600: 2e0a 2020 2020 3a74 7970 6520 746f 706f  ..    :type topo
-00004610: 6c6f 6779 5f72 6573 6f75 7263 6573 5f70  logy_resources_p
-00004620: 6174 6873 3a20 3a63 6c61 7373 3a60 6c69  aths: :class:`li
-00004630: 7374 602c 206f 7074 696f 6e61 6c0a 0a20  st`, optional.. 
-00004640: 2020 2022 2222 0a0a 2020 2020 6966 2022     """..    if "
-00004650: 6e61 6d65 2220 6e6f 7420 696e 2074 6f70  name" not in top
-00004660: 6f6c 6f67 795f 636f 6e74 656e 743a 0a20  ology_content:. 
-00004670: 2020 2020 2020 206e 616d 6520 3d20 2254         name = "T
-00004680: 6f70 6f6c 6f67 7922 0a20 2020 2065 6c73  opology".    els
-00004690: 653a 0a20 2020 2020 2020 206e 616d 6520  e:.        name 
-000046a0: 3d20 746f 706f 6c6f 6779 5f63 6f6e 7465  = topology_conte
-000046b0: 6e74 5b22 6e61 6d65 225d 0a0a 2020 2020  nt["name"]..    
-000046c0: 6966 2022 6e6f 6465 7322 206e 6f74 2069  if "nodes" not i
-000046d0: 6e20 746f 706f 6c6f 6779 5f63 6f6e 7465  n topology_conte
-000046e0: 6e74 3a0a 2020 2020 2020 2020 7261 6973  nt:.        rais
-000046f0: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
-00004700: 2020 2020 2020 2020 2022 5468 6572 6520           "There 
-00004710: 7368 6f75 6c64 2062 6520 6120 276e 6f64  should be a 'nod
-00004720: 6573 2720 7374 7275 6374 7572 6520 696e  es' structure in
-00004730: 2074 6865 2059 414d 4c20 636f 6e66 6967   the YAML config
-00004740: 7572 6174 696f 6e20 6669 6c65 220a 2020  uration file".  
-00004750: 2020 2020 2020 290a 0a20 2020 2069 6620        )..    if 
-00004760: 226c 696e 6b73 2220 6e6f 7420 696e 2074  "links" not in t
-00004770: 6f70 6f6c 6f67 795f 636f 6e74 656e 743a  opology_content:
-00004780: 0a20 2020 2020 2020 2072 6169 7365 2045  .        raise E
-00004790: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
-000047a0: 2020 2020 2020 2254 6865 7265 2073 686f        "There sho
-000047b0: 756c 6420 6265 2061 2027 6c69 6e6b 7327  uld be a 'links'
-000047c0: 2073 7472 7563 7475 7265 2069 6e20 7468   structure in th
-000047d0: 6520 5941 4d4c 2063 6f6e 6669 6775 7261  e YAML configura
-000047e0: 7469 6f6e 2066 696c 6522 0a20 2020 2020  tion file".     
-000047f0: 2020 2029 0a0a 2020 2020 7265 7175 6972     )..    requir
-00004800: 6564 203d 205b 2273 7769 7463 6822 2c20  ed = ["switch", 
-00004810: 226e 6f64 6522 2c20 2270 6172 616d 7322  "node", "params"
-00004820: 5d0a 2020 2020 666f 7220 6c69 6e6b 2069  ].    for link i
-00004830: 6e20 746f 706f 6c6f 6779 5f63 6f6e 7465  n topology_conte
-00004840: 6e74 5b22 6c69 6e6b 7322 5d3a 0a20 2020  nt["links"]:.   
-00004850: 2020 2020 2066 6f72 2072 6571 2069 6e20       for req in 
-00004860: 7265 7175 6972 6564 3a0a 2020 2020 2020  required:.      
-00004870: 2020 2020 2020 6966 2072 6571 206e 6f74        if req not
-00004880: 2069 6e20 6c69 6e6b 3a0a 2020 2020 2020   in link:.      
-00004890: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000048a0: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
-000048b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000048c0: 2254 6865 7265 2073 686f 756c 6420 6265  "There should be
-000048d0: 2061 2027 7b72 6571 7d27 2070 6172 616d   a '{req}' param
-000048e0: 6574 6572 2066 6f72 2065 7665 7279 2069  eter for every i
-000048f0: 7465 6d20 6f66 2027 6c69 6e6b 7327 2069  tem of 'links' i
-00004900: 6e20 7468 6520 5941 4d4c 2063 6f6e 6669  n the YAML confi
-00004910: 6775 7261 7469 6f6e 2066 696c 6522 0a20  guration file". 
-00004920: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00004930: 0a0a 2020 2020 5f73 696d 755f 6372 6561  ..    _simu_crea
-00004940: 7465 5f61 6464 5f69 6d70 6c69 6369 745f  te_add_implicit_
-00004950: 746f 706f 5f70 6172 616d 6574 6572 7328  topo_parameters(
-00004960: 746f 706f 6c6f 6779 5f63 6f6e 7465 6e74  topology_content
-00004970: 290a 0a20 2020 2073 696d 756c 6174 696f  )..    simulatio
-00004980: 6e5f 6469 6374 203d 207b 226e 616d 6522  n_dict = {"name"
-00004990: 3a20 6e61 6d65 2c20 226e 6574 776f 726b  : name, "network
-000049a0: 223a 2074 6f70 6f6c 6f67 795f 636f 6e74  ": topology_cont
-000049b0: 656e 742c 2022 7265 736f 7572 6365 735f  ent, "resources_
-000049c0: 7061 7468 7322 3a20 5b5d 7d0a 0a20 2020  paths": []}..   
-000049d0: 2023 204e 6f72 6d61 6c69 7a65 2074 6865   # Normalize the
-000049e0: 2072 6573 6f75 7263 6573 2070 6174 6873   resources paths
-000049f0: 0a20 2020 2069 6620 746f 706f 6c6f 6779  .    if topology
-00004a00: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
-00004a10: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00004a20: 2020 746f 706f 6c6f 6779 5f72 6573 6f75    topology_resou
-00004a30: 7263 6573 5f70 6174 6873 203d 205b 5d0a  rces_paths = [].
-00004a40: 0a20 2020 206e 6f72 6d61 6c69 7a65 645f  .    normalized_
-00004a50: 7061 7468 7320 3d20 5b5d 0a20 2020 2066  paths = [].    f
-00004a60: 6f72 2072 6573 6f75 7263 6520 696e 2074  or resource in t
-00004a70: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
-00004a80: 735f 7061 7468 733a 0a20 2020 2020 2020  s_paths:.       
-00004a90: 2072 6573 6f75 7263 6520 3d20 6f73 2e70   resource = os.p
-00004aa0: 6174 682e 6e6f 726d 7061 7468 2872 6573  ath.normpath(res
-00004ab0: 6f75 7263 6529 0a20 2020 2020 2020 2023  ource).        #
-00004ac0: 2052 656d 6f76 696e 6720 7472 6169 6c69   Removing traili
-00004ad0: 6e67 2073 6c61 7368 6573 2062 6563 6175  ng slashes becau
-00004ae0: 7365 2074 6865 7920 6172 6520 6967 6e6f  se they are igno
-00004af0: 7265 6420 6279 205a 6970 4669 6c65 0a20  red by ZipFile. 
-00004b00: 2020 2020 2020 2069 6620 7265 736f 7572         if resour
-00004b10: 6365 2e65 6e64 7377 6974 6828 222f 2229  ce.endswith("/")
-00004b20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00004b30: 736f 7572 6365 203d 2072 6573 6f75 7263  source = resourc
-00004b40: 655b 3a3a 2d31 5d0a 2020 2020 2020 2020  e[::-1].        
-00004b50: 6e6f 726d 616c 697a 6564 5f70 6174 6873  normalized_paths
-00004b60: 2e61 7070 656e 6428 7265 736f 7572 6365  .append(resource
-00004b70: 290a 2020 2020 746f 706f 6c6f 6779 5f72  ).    topology_r
-00004b80: 6573 6f75 7263 6573 5f70 6174 6873 203d  esources_paths =
-00004b90: 206e 6f72 6d61 6c69 7a65 645f 7061 7468   normalized_path
-00004ba0: 730a 0a20 2020 2023 2056 6572 6966 7920  s..    # Verify 
-00004bb0: 7468 6174 2077 6520 646f 206e 6f74 2068  that we do not h
-00004bc0: 6176 6520 7468 6520 7361 6d65 2072 6573  ave the same res
-00004bd0: 6f75 7263 6573 2070 6174 6820 696e 2074  ources path in t
-00004be0: 6865 206c 6973 740a 2020 2020 6966 206c  he list.    if l
-00004bf0: 656e 2873 6574 2874 6f70 6f6c 6f67 795f  en(set(topology_
-00004c00: 7265 736f 7572 6365 735f 7061 7468 7329  resources_paths)
-00004c10: 2920 213d 206c 656e 2874 6f70 6f6c 6f67  ) != len(topolog
-00004c20: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
-00004c30: 7329 3a0a 2020 2020 2020 2020 7261 6973  s):.        rais
-00004c40: 6520 4578 6365 7074 696f 6e28 2249 6465  e Exception("Ide
-00004c50: 6e74 6963 616c 2072 6573 6f75 7263 6573  ntical resources
-00004c60: 2070 6174 6873 2068 6176 6520 6265 656e   paths have been
-00004c70: 2067 6976 656e 2229 0a0a 2020 2020 666f   given")..    fo
-00004c80: 7220 7265 736f 7572 6365 2069 6e20 746f  r resource in to
-00004c90: 706f 6c6f 6779 5f72 6573 6f75 7263 6573  pology_resources
-00004ca0: 5f70 6174 6873 3a0a 2020 2020 2020 2020  _paths:.        
-00004cb0: 2320 5661 6c69 6461 7465 2072 6573 6f75  # Validate resou
-00004cc0: 7263 6573 2070 6174 680a 2020 2020 2020  rces path.      
-00004cd0: 2020 5f5f 7661 6c69 6461 7465 5f72 6573    __validate_res
-00004ce0: 6f75 7263 6573 5f70 6174 6828 7265 736f  ources_path(reso
-00004cf0: 7572 6365 2920 2023 2072 6169 7365 2061  urce)  # raise a
-00004d00: 6e20 6578 6365 7074 696f 6e20 6966 2069  n exception if i
-00004d10: 6e76 616c 6964 0a20 2020 2020 2020 2023  nvalid.        #
-00004d20: 2074 616b 6520 7468 6520 6162 736f 6c75   take the absolu
-00004d30: 7465 2070 6174 680a 2020 2020 2020 2020  te path.        
-00004d40: 7369 6d75 6c61 7469 6f6e 5f64 6963 745b  simulation_dict[
-00004d50: 2272 6573 6f75 7263 6573 5f70 6174 6873  "resources_paths
-00004d60: 225d 2e61 7070 656e 6428 6f73 2e70 6174  "].append(os.pat
-00004d70: 682e 6162 7370 6174 6828 7265 736f 7572  h.abspath(resour
-00004d80: 6365 2929 0a0a 2020 2020 7265 7475 726e  ce))..    return
-00004d90: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
-00004da0: 0a0a 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  ...# -----------
-00004db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
-00004df0: 230a 2320 4150 4920 6865 6c70 6572 730a  #.# API helpers.
-00004e00: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  # --------------
-00004e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2023 0a0a  ------------ #..
-00004e50: 0a23 2323 0a23 2053 696d 756c 6174 696f  .###.# Simulatio
-00004e60: 6e20 6865 6c70 6572 730a 2323 230a 0a0a  n helpers.###...
-00004e70: 6465 6620 6372 6561 7465 5f73 696d 756c  def create_simul
-00004e80: 6174 696f 6e28 0a20 2020 2074 6f70 6f6c  ation(.    topol
-00004e90: 6f67 795f 636f 6e74 656e 743a 2044 6963  ogy_content: Dic
-00004ea0: 745b 7374 722c 2041 6e79 5d20 3d20 4e6f  t[str, Any] = No
-00004eb0: 6e65 2c0a 2020 2020 746f 706f 6c6f 6779  ne,.    topology
-00004ec0: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
-00004ed0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00004ee0: 5061 7468 5d5d 203d 204e 6f6e 652c 0a20  Path]] = None,. 
-00004ef0: 2020 2061 6c6c 6f63 6174 696f 6e5f 7374     allocation_st
-00004f00: 7261 7465 6779 3a20 4f70 7469 6f6e 616c  rategy: Optional
-00004f10: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2920  [str] = None,.) 
-00004f20: 2d3e 2054 7570 6c65 5b69 6e74 2c20 4c69  -> Tuple[int, Li
-00004f30: 7374 5b73 7472 5d5d 3a0a 2020 2020 2222  st[str]]:.    ""
-00004f40: 2243 7265 6174 6520 6120 6e65 7720 7369  "Create a new si
-00004f50: 6d75 6c61 7469 6f6e 206d 6f64 656c 2069  mulation model i
-00004f60: 6e20 6461 7461 6261 7365 2062 6173 6564  n database based
-00004f70: 206f 6e20 7468 6520 7072 6f76 6964 6564   on the provided
-00004f80: 2074 6f70 6f6c 6f67 792c 2061 6c6f 6e67   topology, along
-00004f90: 2077 6974 6820 6f70 7469 6f6e 616c 2072   with optional r
-00004fa0: 6573 6f75 7263 6520 6669 6c65 732e 0a0a  esource files...
-00004fb0: 2020 2020 3a72 6574 7572 6e3a 2041 2074      :return: A t
-00004fc0: 7570 6c65 2063 6f6e 7461 696e 696e 6720  uple containing 
-00004fd0: 7468 6520 4944 206f 6620 7468 6520 6372  the ID of the cr
-00004fe0: 6561 7465 6420 7369 6d75 6c61 7469 6f6e  eated simulation
-00004ff0: 2c20 616e 6420 7468 6520 6e65 7720 6e6f  , and the new no
-00005000: 6465 7320 6f66 2074 6865 2073 696d 756c  des of the simul
-00005010: 6174 696f 6e2e 0a20 2020 203a 7274 7970  ation..    :rtyp
-00005020: 653a 203a 636c 6173 733a 6054 7570 6c65  e: :class:`Tuple
-00005030: 5b69 6e74 2c20 4c69 7374 5b73 7472 5d5d  [int, List[str]]
-00005040: 600a 0a20 2020 203a 7061 7261 6d20 746f  `..    :param to
-00005050: 706f 6c6f 6779 5f63 6f6e 7465 6e74 3a20  pology_content: 
-00005060: 4120 6469 6374 2063 6f6e 7461 696e 696e  A dict containin
-00005070: 6720 7468 6520 6e6f 6465 7320 616e 6420  g the nodes and 
-00005080: 6e65 7477 6f72 6b20 746f 706f 6c6f 6779  network topology
-00005090: 2074 6f20 6372 6561 7465 2e0a 2020 2020   to create..    
-000050a0: 3a74 7970 6520 746f 706f 6c6f 6779 5f66  :type topology_f
-000050b0: 696c 653a 203a 636c 6173 733a 6064 6963  ile: :class:`dic
-000050c0: 7460 0a20 2020 203a 7061 7261 6d20 746f  t`.    :param to
-000050d0: 706f 6c6f 6779 5f72 6573 6f75 7263 6573  pology_resources
-000050e0: 5f70 6174 6873 3a20 5468 6520 7061 7468  _paths: The path
-000050f0: 2074 6f20 7265 736f 7572 6365 7320 7468   to resources th
-00005100: 6174 2077 696c 6c20 6265 2070 7573 6865  at will be pushe
-00005110: 6420 696e 746f 2063 6f6d 7061 7469 626c  d into compatibl
-00005120: 6520 6e6f 6465 732e 0a20 2020 203a 7479  e nodes..    :ty
-00005130: 7065 2074 6f70 6f6c 6f67 795f 7265 736f  pe topology_reso
-00005140: 7572 6365 735f 7061 7468 733a 203a 636c  urces_paths: :cl
-00005150: 6173 733a 606c 6973 7460 2c20 6f70 7469  ass:`list`, opti
-00005160: 6f6e 616c 0a20 2020 203a 7061 7261 6d20  onal.    :param 
-00005170: 616c 6c6f 6361 7469 6f6e 5f73 7472 6174  allocation_strat
-00005180: 6567 793a 204e 616d 6520 6f66 2074 6865  egy: Name of the
-00005190: 2061 6c6c 6f63 6174 696f 6e20 7374 7261   allocation stra
-000051a0: 7465 6779 2074 6f20 7573 6520 746f 2061  tegy to use to a
-000051b0: 6c6c 6f63 6174 6520 6e6f 6465 7320 746f  llocate nodes to
-000051c0: 2063 6f6d 7075 7465 2073 6572 7665 7273   compute servers
-000051d0: 2e0a 2020 2020 3a74 7970 6520 616c 6c6f  ..    :type allo
-000051e0: 6361 7469 6f6e 5f73 7472 6174 6567 793a  cation_strategy:
-000051f0: 203a 636c 6173 733a 6073 7472 602c 206f   :class:`str`, o
-00005200: 7074 696f 6e61 6c0a 0a20 2020 2022 2222  ptional..    """
-00005210: 0a0a 2020 2020 7369 6d75 6c61 7469 6f6e  ..    simulation
-00005220: 5f64 6963 7420 3d20 5f6e 6f72 6d61 6c69  _dict = _normali
-00005230: 7a65 5f73 696d 756c 6174 696f 6e5f 7265  ze_simulation_re
-00005240: 736f 7572 6365 7328 0a20 2020 2020 2020  sources(.       
-00005250: 2074 6f70 6f6c 6f67 795f 636f 6e74 656e   topology_conten
-00005260: 743d 746f 706f 6c6f 6779 5f63 6f6e 7465  t=topology_conte
-00005270: 6e74 2c0a 2020 2020 2020 2020 746f 706f  nt,.        topo
-00005280: 6c6f 6779 5f72 6573 6f75 7263 6573 5f70  logy_resources_p
-00005290: 6174 6873 3d74 6f70 6f6c 6f67 795f 7265  aths=topology_re
-000052a0: 736f 7572 6365 735f 7061 7468 732c 0a20  sources_paths,. 
-000052b0: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
-000052c0: 205f 6372 6561 7465 5f6f 725f 6578 7465   _create_or_exte
-000052d0: 6e64 5f73 696d 756c 6174 696f 6e28 0a20  nd_simulation(. 
-000052e0: 2020 2020 2020 2073 696d 756c 6174 696f         simulatio
-000052f0: 6e5f 6469 6374 3d73 696d 756c 6174 696f  n_dict=simulatio
-00005300: 6e5f 6469 6374 2c20 616c 6c6f 6361 7469  n_dict, allocati
-00005310: 6f6e 5f73 7472 6174 6567 793d 616c 6c6f  on_strategy=allo
-00005320: 6361 7469 6f6e 5f73 7472 6174 6567 790a  cation_strategy.
-00005330: 2020 2020 290a 0a0a 6465 6620 6578 7465      )...def exte
-00005340: 6e64 5f73 696d 756c 6174 696f 6e28 0a20  nd_simulation(. 
-00005350: 2020 2074 6f70 6f6c 6f67 795f 636f 6e74     topology_cont
-00005360: 656e 743a 2044 6963 745b 7374 722c 2041  ent: Dict[str, A
-00005370: 6e79 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ny] = None,.    
-00005380: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
-00005390: 6573 5f70 6174 6873 3a20 4f70 7469 6f6e  es_paths: Option
-000053a0: 616c 5b4c 6973 745b 5061 7468 5d5d 203d  al[List[Path]] =
-000053b0: 204e 6f6e 652c 0a20 2020 2061 6c6c 6f63   None,.    alloc
-000053c0: 6174 696f 6e5f 7374 7261 7465 6779 3a20  ation_strategy: 
-000053d0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-000053e0: 4e6f 6e65 2c0a 2020 2020 6964 5f73 696d  None,.    id_sim
-000053f0: 756c 6174 696f 6e3a 2069 6e74 203d 204e  ulation: int = N
-00005400: 6f6e 652c 0a29 202d 3e20 5475 706c 655b  one,.) -> Tuple[
-00005410: 696e 742c 204c 6973 745b 7374 725d 5d3a  int, List[str]]:
-00005420: 0a20 2020 2022 2222 4578 7465 6e64 2061  .    """Extend a
-00005430: 6e20 6578 6973 7469 6e67 2073 696d 756c  n existing simul
-00005440: 6174 696f 6e20 6d6f 6465 6c20 696e 2064  ation model in d
-00005450: 6174 6162 6173 6520 6261 7365 6420 6f6e  atabase based on
-00005460: 2074 6865 2070 726f 7669 6465 6420 746f   the provided to
-00005470: 706f 6c6f 6779 2c20 616c 6f6e 6720 7769  pology, along wi
-00005480: 7468 206f 7074 696f 6e61 6c20 7265 736f  th optional reso
-00005490: 7572 6365 2066 696c 6573 2e0a 0a20 2020  urce files...   
-000054a0: 203a 7265 7475 726e 3a20 4120 7475 706c   :return: A tupl
-000054b0: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
-000054c0: 2049 4420 6f66 2074 6865 2063 7265 6174   ID of the creat
-000054d0: 6564 2073 696d 756c 6174 696f 6e2c 2061  ed simulation, a
-000054e0: 6e64 2074 6865 206e 6577 206e 6f64 6573  nd the new nodes
-000054f0: 206f 6620 7468 6520 7369 6d75 6c61 7469   of the simulati
-00005500: 6f6e 2e0a 2020 2020 3a72 7479 7065 3a20  on..    :rtype: 
-00005510: 3a63 6c61 7373 3a60 5475 706c 655b 696e  :class:`Tuple[in
-00005520: 742c 204c 6973 745b 7374 725d 5d60 0a0a  t, List[str]]`..
-00005530: 2020 2020 3a70 6172 616d 2074 6f70 6f6c      :param topol
-00005540: 6f67 795f 636f 6e74 656e 743a 2041 2064  ogy_content: A d
-00005550: 6963 7420 636f 6e74 6169 6e69 6e67 2074  ict containing t
-00005560: 6865 206e 6f64 6573 2061 6e64 206e 6574  he nodes and net
-00005570: 776f 726b 2074 6f70 6f6c 6f67 7920 746f  work topology to
-00005580: 2063 7265 6174 652e 0a20 2020 203a 7479   create..    :ty
-00005590: 7065 2074 6f70 6f6c 6f67 795f 6669 6c65  pe topology_file
-000055a0: 3a20 3a63 6c61 7373 3a60 6469 6374 600a  : :class:`dict`.
-000055b0: 2020 2020 3a70 6172 616d 2074 6f70 6f6c      :param topol
-000055c0: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
-000055d0: 7468 733a 2054 6865 2070 6174 6820 746f  ths: The path to
-000055e0: 2072 6573 6f75 7263 6573 2074 6861 7420   resources that 
-000055f0: 7769 6c6c 2062 6520 7075 7368 6564 2069  will be pushed i
-00005600: 6e74 6f20 636f 6d70 6174 6962 6c65 206e  nto compatible n
-00005610: 6f64 6573 2e0a 2020 2020 3a74 7970 6520  odes..    :type 
-00005620: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
-00005630: 6573 5f70 6174 6873 3a20 3a63 6c61 7373  es_paths: :class
-00005640: 3a60 6c69 7374 602c 206f 7074 696f 6e61  :`list`, optiona
-00005650: 6c0a 2020 2020 3a70 6172 616d 2061 6c6c  l.    :param all
-00005660: 6f63 6174 696f 6e5f 7374 7261 7465 6779  ocation_strategy
-00005670: 3a20 4e61 6d65 206f 6620 7468 6520 616c  : Name of the al
-00005680: 6c6f 6361 7469 6f6e 2073 7472 6174 6567  location strateg
-00005690: 7920 746f 2075 7365 2074 6f20 616c 6c6f  y to use to allo
-000056a0: 6361 7465 206e 6f64 6573 2074 6f20 636f  cate nodes to co
-000056b0: 6d70 7574 6520 7365 7276 6572 732e 0a20  mpute servers.. 
-000056c0: 2020 203a 7479 7065 2061 6c6c 6f63 6174     :type allocat
-000056d0: 696f 6e5f 7374 7261 7465 6779 3a20 3a63  ion_strategy: :c
-000056e0: 6c61 7373 3a60 7374 7260 2c20 6f70 7469  lass:`str`, opti
-000056f0: 6f6e 616c 0a20 2020 203a 7061 7261 6d20  onal.    :param 
-00005700: 6964 5f73 696d 756c 6174 696f 6e3a 2054  id_simulation: T
-00005710: 6865 2073 696d 756c 6174 696f 6e20 4944  he simulation ID
-00005720: 2c20 7768 656e 2065 7874 656e 6469 6e67  , when extending
-00005730: 2061 6e20 6578 6973 7469 6e67 2073 696d   an existing sim
-00005740: 756c 6174 696f 6e20 7769 7468 206e 6577  ulation with new
-00005750: 206e 6f64 6573 2061 6e64 206c 696e 6b73   nodes and links
-00005760: 2e0a 2020 2020 3a74 7970 6520 6964 5f73  ..    :type id_s
-00005770: 696d 756c 6174 696f 6e3a 203a 636c 6173  imulation: :clas
-00005780: 733a 6069 6e74 602c 206f 7074 696f 6e61  s:`int`, optiona
-00005790: 6c0a 0a20 2020 2022 2222 0a0a 2020 2020  l..    """..    
-000057a0: 7369 6d75 6c61 7469 6f6e 5f64 6963 7420  simulation_dict 
-000057b0: 3d20 5f6e 6f72 6d61 6c69 7a65 5f73 696d  = _normalize_sim
-000057c0: 756c 6174 696f 6e5f 7265 736f 7572 6365  ulation_resource
-000057d0: 7328 0a20 2020 2020 2020 2074 6f70 6f6c  s(.        topol
-000057e0: 6f67 795f 636f 6e74 656e 743d 746f 706f  ogy_content=topo
-000057f0: 6c6f 6779 5f63 6f6e 7465 6e74 2c0a 2020  logy_content,.  
-00005800: 2020 2020 2020 746f 706f 6c6f 6779 5f72        topology_r
-00005810: 6573 6f75 7263 6573 5f70 6174 6873 3d74  esources_paths=t
-00005820: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
-00005830: 735f 7061 7468 732c 0a20 2020 2029 0a0a  s_paths,.    )..
-00005840: 2020 2020 7265 7475 726e 205f 6372 6561      return _crea
-00005850: 7465 5f6f 725f 6578 7465 6e64 5f73 696d  te_or_extend_sim
-00005860: 756c 6174 696f 6e28 0a20 2020 2020 2020  ulation(.       
-00005870: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
-00005880: 3d73 696d 756c 6174 696f 6e5f 6469 6374  =simulation_dict
-00005890: 2c0a 2020 2020 2020 2020 6964 5f73 696d  ,.        id_sim
-000058a0: 756c 6174 696f 6e3d 6964 5f73 696d 756c  ulation=id_simul
-000058b0: 6174 696f 6e2c 0a20 2020 2020 2020 2061  ation,.        a
-000058c0: 6c6c 6f63 6174 696f 6e5f 7374 7261 7465  llocation_strate
-000058d0: 6779 3d61 6c6c 6f63 6174 696f 6e5f 7374  gy=allocation_st
-000058e0: 7261 7465 6779 2c0a 2020 2020 290a 0a0a  rategy,.    )...
-000058f0: 6465 6620 6372 6561 7465 5f73 696d 756c  def create_simul
-00005900: 6174 696f 6e5f 6672 6f6d 5f74 6f70 6f6c  ation_from_topol
-00005910: 6f67 7928 0a20 2020 2074 6f70 6f6c 6f67  ogy(.    topolog
-00005920: 795f 6669 6c65 3a20 7374 7220 3d20 4e6f  y_file: str = No
-00005930: 6e65 2c0a 2020 2020 746f 706f 6c6f 6779  ne,.    topology
-00005940: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
-00005950: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00005960: 5061 7468 5d5d 203d 204e 6f6e 652c 0a20  Path]] = None,. 
-00005970: 2020 2061 6c6c 6f63 6174 696f 6e5f 7374     allocation_st
-00005980: 7261 7465 6779 3a20 4f70 7469 6f6e 616c  rategy: Optional
-00005990: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2920  [str] = None,.) 
-000059a0: 2d3e 2054 7570 6c65 5b69 6e74 2c20 4c69  -> Tuple[int, Li
-000059b0: 7374 5b73 7472 5d5d 3a0a 2020 2020 2222  st[str]]:.    ""
-000059c0: 2243 7265 6174 6520 6120 6e65 7720 7369  "Create a new si
-000059d0: 6d75 6c61 7469 6f6e 206d 6f64 656c 2069  mulation model i
-000059e0: 6e20 6461 7461 6261 7365 2062 6173 6564  n database based
-000059f0: 206f 6e20 7468 6520 7072 6f76 6964 6564   on the provided
-00005a00: 2074 6f70 6f6c 6f67 7920 6669 6c65 2c20   topology file, 
-00005a10: 616c 6f6e 6720 7769 7468 206f 7074 696f  along with optio
-00005a20: 6e61 6c20 7265 736f 7572 6365 2066 696c  nal resource fil
-00005a30: 6573 2e0a 0a20 2020 203a 7265 7475 726e  es...    :return
-00005a40: 3a20 4120 7475 706c 6520 636f 6e74 6169  : A tuple contai
-00005a50: 6e69 6e67 2074 6865 2049 4420 6f66 2074  ning the ID of t
-00005a60: 6865 2063 7265 6174 6564 2073 696d 756c  he created simul
-00005a70: 6174 696f 6e2c 2061 6e64 2074 6865 206e  ation, and the n
-00005a80: 6577 206e 6f64 6573 206f 6620 7468 6520  ew nodes of the 
-00005a90: 7369 6d75 6c61 7469 6f6e 2e0a 2020 2020  simulation..    
-00005aa0: 3a72 7479 7065 3a20 3a63 6c61 7373 3a60  :rtype: :class:`
-00005ab0: 5475 706c 655b 696e 742c 204c 6973 745b  Tuple[int, List[
-00005ac0: 7374 725d 5d60 0a0a 2020 2020 3a70 6172  str]]`..    :par
-00005ad0: 616d 2074 6f70 6f6c 6f67 795f 6669 6c65  am topology_file
-00005ae0: 3a20 5468 6520 7061 7468 2074 6f20 6120  : The path to a 
-00005af0: 746f 706f 6c6f 6779 2066 696c 6520 636f  topology file co
-00005b00: 6e74 6169 6e69 6e67 2074 6865 206e 6f64  ntaining the nod
-00005b10: 6573 2061 6e64 206e 6574 776f 726b 2074  es and network t
-00005b20: 6f70 6f6c 6f67 7920 746f 2063 7265 6174  opology to creat
-00005b30: 652e 0a20 2020 203a 7479 7065 2074 6f70  e..    :type top
-00005b40: 6f6c 6f67 795f 6669 6c65 3a20 3a63 6c61  ology_file: :cla
-00005b50: 7373 3a60 7374 7260 0a20 2020 203a 7061  ss:`str`.    :pa
-00005b60: 7261 6d20 746f 706f 6c6f 6779 5f72 6573  ram topology_res
-00005b70: 6f75 7263 6573 5f70 6174 6873 3a20 5468  ources_paths: Th
-00005b80: 6520 7061 7468 2074 6f20 7265 736f 7572  e path to resour
-00005b90: 6365 7320 7468 6174 2077 696c 6c20 6265  ces that will be
-00005ba0: 2070 7573 6865 6420 696e 746f 2063 6f6d   pushed into com
-00005bb0: 7061 7469 626c 6520 6e6f 6465 732e 0a20  patible nodes.. 
-00005bc0: 2020 203a 7479 7065 2074 6f70 6f6c 6f67     :type topolog
-00005bd0: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
-00005be0: 733a 203a 636c 6173 733a 6073 7472 602c  s: :class:`str`,
-00005bf0: 206f 7074 696f 6e61 6c0a 2020 2020 3a70   optional.    :p
-00005c00: 6172 616d 2061 6c6c 6f63 6174 696f 6e5f  aram allocation_
-00005c10: 7374 7261 7465 6779 3a20 4e61 6d65 206f  strategy: Name o
-00005c20: 6620 7468 6520 616c 6c6f 6361 7469 6f6e  f the allocation
-00005c30: 2073 7472 6174 6567 7920 746f 2075 7365   strategy to use
-00005c40: 2074 6f20 616c 6c6f 6361 7465 206e 6f64   to allocate nod
-00005c50: 6573 2074 6f20 636f 6d70 7574 6520 7365  es to compute se
-00005c60: 7276 6572 732e 0a20 2020 203a 7479 7065  rvers..    :type
-00005c70: 2061 6c6c 6f63 6174 696f 6e5f 7374 7261   allocation_stra
-00005c80: 7465 6779 3a20 3a63 6c61 7373 3a60 7374  tegy: :class:`st
-00005c90: 7260 2c20 6f70 7469 6f6e 616c 0a0a 2020  r`, optional..  
-00005ca0: 2020 3e3e 3e20 6672 6f6d 2063 725f 6170    >>> from cr_ap
-00005cb0: 695f 636c 6965 6e74 2069 6d70 6f72 7420  i_client import 
-00005cc0: 636f 7265 5f61 7069 0a20 2020 203e 3e3e  core_api.    >>>
-00005cd0: 2063 6f72 655f 6170 692e 7265 7365 7428   core_api.reset(
-00005ce0: 290a 2020 2020 3e3e 3e20 636f 7265 5f61  ).    >>> core_a
-00005cf0: 7069 2e63 7265 6174 655f 7369 6d75 6c61  pi.create_simula
-00005d00: 7469 6f6e 5f66 726f 6d5f 746f 706f 6c6f  tion_from_topolo
-00005d10: 6779 2822 6461 7461 2f74 6f70 6f6c 6f67  gy("data/topolog
-00005d20: 6965 732f 746f 706f 6c6f 6779 2d31 2d63  ies/topology-1-c
-00005d30: 6c69 656e 742e 7961 6d6c 2229 0a20 2020  lient.yaml").   
-00005d40: 2031 0a0a 2020 2020 2222 220a 0a20 2020   1..    """..   
-00005d50: 2069 6620 746f 706f 6c6f 6779 5f72 6573   if topology_res
-00005d60: 6f75 7263 6573 5f70 6174 6873 2069 7320  ources_paths is 
-00005d70: 4e6f 6e65 3a0a 2020 2020 2020 2020 746f  None:.        to
-00005d80: 706f 6c6f 6779 5f72 6573 6f75 7263 6573  pology_resources
-00005d90: 5f70 6174 6873 203d 205b 5d0a 0a20 2020  _paths = []..   
-00005da0: 2023 2043 7265 6174 6520 6120 6e65 7720   # Create a new 
-00005db0: 7369 6d75 6c61 7469 6f6e 206d 6f64 656c  simulation model
-00005dc0: 2069 6e20 6461 7461 6261 7365 2062 6173   in database bas
-00005dd0: 6564 206f 6e20 7468 6520 7072 6f76 6964  ed on the provid
-00005de0: 6564 2074 6f70 6f6c 6f67 7920 6669 6c65  ed topology file
-00005df0: 2070 6174 682e 2222 220a 2020 2020 6966   path.""".    if
-00005e00: 2074 6f70 6f6c 6f67 795f 6669 6c65 2069   topology_file i
-00005e10: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00005e20: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
-00005e30: 2241 6e20 746f 706f 6c6f 6779 2066 696c  "An topology fil
-00005e40: 6520 6973 2072 6571 7569 7265 6422 290a  e is required").
-00005e50: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
-00005e60: 5941 4d4c 2063 6f6e 6669 6775 7261 7469  YAML configurati
-00005e70: 6f6e 2066 696c 650a 2020 2020 5f76 616c  on file.    _val
-00005e80: 6964 6174 655f 7961 6d6c 5f74 6f70 6f6c  idate_yaml_topol
-00005e90: 6f67 795f 6669 6c65 2874 6f70 6f6c 6f67  ogy_file(topolog
-00005ea0: 795f 6669 6c65 290a 0a20 2020 2023 204f  y_file)..    # O
-00005eb0: 7065 6e20 616e 6420 7265 6164 2059 414d  pen and read YAM
-00005ec0: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
-00005ed0: 6669 6c65 0a20 2020 2079 616d 6c5f 636f  file.    yaml_co
-00005ee0: 6e74 656e 7420 3d20 5f72 6561 645f 7961  ntent = _read_ya
-00005ef0: 6d6c 5f74 6f70 6f6c 6f67 795f 6669 6c65  ml_topology_file
-00005f00: 2874 6f70 6f6c 6f67 795f 6669 6c65 290a  (topology_file).
-00005f10: 0a20 2020 2023 2050 6172 7365 2059 414d  .    # Parse YAM
-00005f20: 4c20 636f 6e66 6967 7572 6174 696f 6e0a  L configuration.
-00005f30: 2020 2020 2320 5765 2075 7365 2072 7561      # We use rua
-00005f40: 6d65 6c2e 7961 6d6c 2062 6563 6175 7365  mel.yaml because
-00005f50: 2069 7420 6b65 6570 7320 616e 6368 6f72   it keeps anchor
-00005f60: 7320 616e 640a 2020 2020 2320 616c 6961  s and.    # alia
-00005f70: 7365 7320 696e 206d 656d 6f72 792e 2049  ses in memory. I
-00005f80: 7420 6973 2076 6572 7920 636f 6e76 656e  t is very conven
-00005f90: 6965 6e74 2077 6865 6e20 7468 6520 7369  ient when the si
-00005fa0: 6d75 6c61 7469 6f6e 0a20 2020 2023 2069  mulation.    # i
-00005fb0: 7320 7374 6f72 6564 2f66 6574 6368 6564  s stored/fetched
-00005fc0: 2028 7265 6665 7265 6e63 6573 2061 7265   (references are
-00005fd0: 206b 6570 7421 290a 2020 2020 6c6f 6164   kept!).    load
-00005fe0: 6572 203d 2059 414d 4c28 7479 703d 2272  er = YAML(typ="r
-00005ff0: 7422 290a 2020 2020 746f 706f 6c6f 6779  t").    topology
-00006000: 5f63 6f6e 7465 6e74 203d 206c 6f61 6465  _content = loade
-00006010: 722e 6c6f 6164 2879 616d 6c5f 636f 6e74  r.load(yaml_cont
-00006020: 656e 7429 0a0a 2020 2020 2320 4164 6420  ent)..    # Add 
-00006030: 6120 6465 6661 756c 7420 7265 736f 7572  a default resour
-00006040: 6365 7320 6469 7265 6374 6f72 7920 6966  ces directory if
-00006050: 2069 7420 6578 6973 7473 2e0a 2020 2020   it exists..    
-00006060: 2320 4966 2074 6865 2074 6f70 6f6c 6f67  # If the topolog
-00006070: 7920 6973 2022 7061 7468 2f74 6f2f 746f  y is "path/to/to
-00006080: 706f 2e79 616d 6c22 2c20 7468 6520 6465  po.yaml", the de
-00006090: 6661 756c 7420 7265 736f 7572 6365 7320  fault resources 
-000060a0: 6469 7265 6374 6f72 7920 6973 2022 7061  directory is "pa
-000060b0: 7468 2f74 6f2f 7265 736f 7572 6365 7322  th/to/resources"
-000060c0: 2e0a 2020 2020 6465 6661 756c 745f 7265  ..    default_re
-000060d0: 736f 7572 6365 735f 7061 7468 203d 206f  sources_path = o
-000060e0: 732e 7061 7468 2e6a 6f69 6e28 6f73 2e70  s.path.join(os.p
-000060f0: 6174 682e 6469 726e 616d 6528 746f 706f  ath.dirname(topo
-00006100: 6c6f 6779 5f66 696c 6529 2c20 2272 6573  logy_file), "res
-00006110: 6f75 7263 6573 2229 0a20 2020 2064 6566  ources").    def
-00006120: 6175 6c74 5f72 6573 6f75 7263 6573 5f70  ault_resources_p
-00006130: 6174 6820 3d20 6f73 2e70 6174 682e 6e6f  ath = os.path.no
-00006140: 726d 7061 7468 2864 6566 6175 6c74 5f72  rmpath(default_r
-00006150: 6573 6f75 7263 6573 5f70 6174 6829 0a20  esources_path). 
-00006160: 2020 2069 6620 5f5f 7661 6c69 6461 7465     if __validate
-00006170: 5f72 6573 6f75 7263 6573 5f70 6174 6828  _resources_path(
-00006180: 6465 6661 756c 745f 7265 736f 7572 6365  default_resource
-00006190: 735f 7061 7468 2c20 4661 6c73 6529 3a0a  s_path, False):.
-000061a0: 2020 2020 2020 2020 6966 2064 6566 6175          if defau
-000061b0: 6c74 5f72 6573 6f75 7263 6573 5f70 6174  lt_resources_pat
-000061c0: 6820 6e6f 7420 696e 2074 6f70 6f6c 6f67  h not in topolog
-000061d0: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
-000061e0: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-000061f0: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
-00006200: 735f 7061 7468 732e 6170 7065 6e64 2864  s_paths.append(d
-00006210: 6566 6175 6c74 5f72 6573 6f75 7263 6573  efault_resources
-00006220: 5f70 6174 6829 0a0a 2020 2020 7265 7475  _path)..    retu
-00006230: 726e 2063 7265 6174 655f 7369 6d75 6c61  rn create_simula
-00006240: 7469 6f6e 280a 2020 2020 2020 2020 746f  tion(.        to
-00006250: 706f 6c6f 6779 5f63 6f6e 7465 6e74 3d74  pology_content=t
-00006260: 6f70 6f6c 6f67 795f 636f 6e74 656e 742c  opology_content,
-00006270: 0a20 2020 2020 2020 2074 6f70 6f6c 6f67  .        topolog
-00006280: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
-00006290: 733d 746f 706f 6c6f 6779 5f72 6573 6f75  s=topology_resou
-000062a0: 7263 6573 5f70 6174 6873 2c0a 2020 2020  rces_paths,.    
-000062b0: 2020 2020 616c 6c6f 6361 7469 6f6e 5f73      allocation_s
-000062c0: 7472 6174 6567 793d 616c 6c6f 6361 7469  trategy=allocati
-000062d0: 6f6e 5f73 7472 6174 6567 792c 0a20 2020  on_strategy,.   
-000062e0: 2029 0a0a 0a64 6566 2065 7874 656e 645f   )...def extend_
-000062f0: 7369 6d75 6c61 7469 6f6e 5f66 726f 6d5f  simulation_from_
-00006300: 746f 706f 6c6f 6779 280a 2020 2020 746f  topology(.    to
-00006310: 706f 6c6f 6779 5f66 696c 653a 2073 7472  pology_file: str
-00006320: 203d 204e 6f6e 652c 0a20 2020 2074 6f70   = None,.    top
-00006330: 6f6c 6f67 795f 7265 736f 7572 6365 735f  ology_resources_
-00006340: 7061 7468 733a 204f 7074 696f 6e61 6c5b  paths: Optional[
-00006350: 4c69 7374 5b50 6174 685d 5d20 3d20 4e6f  List[Path]] = No
-00006360: 6e65 2c0a 2020 2020 616c 6c6f 6361 7469  ne,.    allocati
-00006370: 6f6e 5f73 7472 6174 6567 793a 204f 7074  on_strategy: Opt
-00006380: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00006390: 652c 0a20 2020 2069 645f 7369 6d75 6c61  e,.    id_simula
-000063a0: 7469 6f6e 3a20 696e 7420 3d20 4e6f 6e65  tion: int = None
-000063b0: 2c0a 2920 2d3e 2054 7570 6c65 5b69 6e74  ,.) -> Tuple[int
-000063c0: 2c20 4c69 7374 5b73 7472 5d5d 3a0a 2020  , List[str]]:.  
-000063d0: 2020 2222 2245 7874 656e 6420 616e 2065    """Extend an e
-000063e0: 7869 7374 696e 6720 7369 6d75 6c61 7469  xisting simulati
-000063f0: 6f6e 206d 6f64 656c 2069 6e20 6461 7461  on model in data
-00006400: 6261 7365 2062 6173 6564 206f 6e20 7468  base based on th
-00006410: 6520 7072 6f76 6964 6564 2074 6f70 6f6c  e provided topol
-00006420: 6f67 7920 6669 6c65 2c20 616c 6f6e 6720  ogy file, along 
-00006430: 7769 7468 206f 7074 696f 6e61 6c20 7265  with optional re
-00006440: 736f 7572 6365 2066 696c 6573 2e0a 0a20  source files... 
-00006450: 2020 203a 7265 7475 726e 3a20 4120 7475     :return: A tu
-00006460: 706c 6520 636f 6e74 6169 6e69 6e67 2074  ple containing t
-00006470: 6865 2049 4420 6f66 2074 6865 2063 7265  he ID of the cre
-00006480: 6174 6564 2073 696d 756c 6174 696f 6e2c  ated simulation,
-00006490: 2061 6e64 2074 6865 206e 6577 206e 6f64   and the new nod
-000064a0: 6573 206f 6620 7468 6520 7369 6d75 6c61  es of the simula
-000064b0: 7469 6f6e 2e0a 2020 2020 3a72 7479 7065  tion..    :rtype
-000064c0: 3a20 3a63 6c61 7373 3a60 5475 706c 655b  : :class:`Tuple[
-000064d0: 696e 742c 204c 6973 745b 7374 725d 5d60  int, List[str]]`
-000064e0: 0a0a 2020 2020 3a70 6172 616d 2074 6f70  ..    :param top
-000064f0: 6f6c 6f67 795f 6669 6c65 3a20 5468 6520  ology_file: The 
-00006500: 7061 7468 2074 6f20 6120 746f 706f 6c6f  path to a topolo
-00006510: 6779 2066 696c 6520 636f 6e74 6169 6e69  gy file containi
-00006520: 6e67 2074 6865 206e 6f64 6573 2061 6e64  ng the nodes and
-00006530: 206e 6574 776f 726b 2074 6f70 6f6c 6f67   network topolog
-00006540: 7920 746f 2063 7265 6174 652e 0a20 2020  y to create..   
-00006550: 203a 7479 7065 2074 6f70 6f6c 6f67 795f   :type topology_
-00006560: 6669 6c65 3a20 3a63 6c61 7373 3a60 7374  file: :class:`st
-00006570: 7260 0a20 2020 203a 7061 7261 6d20 746f  r`.    :param to
-00006580: 706f 6c6f 6779 5f72 6573 6f75 7263 6573  pology_resources
-00006590: 5f70 6174 6873 3a20 5468 6520 7061 7468  _paths: The path
-000065a0: 2074 6f20 7265 736f 7572 6365 7320 7468   to resources th
-000065b0: 6174 2077 696c 6c20 6265 2070 7573 6865  at will be pushe
-000065c0: 6420 696e 746f 2063 6f6d 7061 7469 626c  d into compatibl
-000065d0: 6520 6e6f 6465 732e 0a20 2020 203a 7479  e nodes..    :ty
-000065e0: 7065 2074 6f70 6f6c 6f67 795f 7265 736f  pe topology_reso
-000065f0: 7572 6365 735f 7061 7468 733a 203a 636c  urces_paths: :cl
-00006600: 6173 733a 6073 7472 602c 206f 7074 696f  ass:`str`, optio
-00006610: 6e61 6c0a 2020 2020 3a70 6172 616d 2061  nal.    :param a
-00006620: 6c6c 6f63 6174 696f 6e5f 7374 7261 7465  llocation_strate
-00006630: 6779 3a20 4e61 6d65 206f 6620 7468 6520  gy: Name of the 
-00006640: 616c 6c6f 6361 7469 6f6e 2073 7472 6174  allocation strat
-00006650: 6567 7920 746f 2075 7365 2074 6f20 616c  egy to use to al
-00006660: 6c6f 6361 7465 206e 6f64 6573 2074 6f20  locate nodes to 
-00006670: 636f 6d70 7574 6520 7365 7276 6572 732e  compute servers.
-00006680: 0a20 2020 203a 7479 7065 2061 6c6c 6f63  .    :type alloc
-00006690: 6174 696f 6e5f 7374 7261 7465 6779 3a20  ation_strategy: 
-000066a0: 3a63 6c61 7373 3a60 7374 7260 2c20 6f70  :class:`str`, op
-000066b0: 7469 6f6e 616c 0a20 2020 203a 7061 7261  tional.    :para
-000066c0: 6d20 6964 5f73 696d 756c 6174 696f 6e3a  m id_simulation:
-000066d0: 2054 6865 2073 696d 756c 6174 696f 6e20   The simulation 
-000066e0: 4944 2c20 7768 656e 2065 7874 656e 6469  ID, when extendi
-000066f0: 6e67 2061 6e20 6578 6973 7469 6e67 2073  ng an existing s
-00006700: 696d 756c 6174 696f 6e20 7769 7468 206e  imulation with n
-00006710: 6577 206e 6f64 6573 2061 6e64 206c 696e  ew nodes and lin
-00006720: 6b73 2e0a 2020 2020 3a74 7970 6520 6964  ks..    :type id
-00006730: 5f73 696d 756c 6174 696f 6e3a 203a 636c  _simulation: :cl
-00006740: 6173 733a 6069 6e74 602c 206f 7074 696f  ass:`int`, optio
-00006750: 6e61 6c0a 2020 2020 2222 220a 2020 2020  nal.    """.    
-00006760: 6966 2074 6f70 6f6c 6f67 795f 7265 736f  if topology_reso
-00006770: 7572 6365 735f 7061 7468 7320 6973 204e  urces_paths is N
-00006780: 6f6e 653a 0a20 2020 2020 2020 2074 6f70  one:.        top
-00006790: 6f6c 6f67 795f 7265 736f 7572 6365 735f  ology_resources_
-000067a0: 7061 7468 7320 3d20 5b5d 0a0a 2020 2020  paths = []..    
-000067b0: 2320 4372 6561 7465 2061 206e 6577 2073  # Create a new s
-000067c0: 696d 756c 6174 696f 6e20 6d6f 6465 6c20  imulation model 
-000067d0: 696e 2064 6174 6162 6173 6520 6261 7365  in database base
-000067e0: 6420 6f6e 2074 6865 2070 726f 7669 6465  d on the provide
-000067f0: 6420 746f 706f 6c6f 6779 2066 696c 6520  d topology file 
-00006800: 7061 7468 2e22 2222 0a20 2020 2069 6620  path.""".    if 
-00006810: 746f 706f 6c6f 6779 5f66 696c 6520 6973  topology_file is
-00006820: 204e 6f6e 653a 0a20 2020 2020 2020 2072   None:.        r
-00006830: 6169 7365 2045 7863 6570 7469 6f6e 2822  aise Exception("
-00006840: 416e 2074 6f70 6f6c 6f67 7920 6669 6c65  An topology file
-00006850: 2069 7320 7265 7175 6972 6564 2229 0a0a   is required")..
-00006860: 2020 2020 2320 5661 6c69 6461 7465 2059      # Validate Y
-00006870: 414d 4c20 636f 6e66 6967 7572 6174 696f  AML configuratio
-00006880: 6e20 6669 6c65 0a20 2020 205f 7661 6c69  n file.    _vali
-00006890: 6461 7465 5f79 616d 6c5f 746f 706f 6c6f  date_yaml_topolo
-000068a0: 6779 5f66 696c 6528 746f 706f 6c6f 6779  gy_file(topology
-000068b0: 5f66 696c 6529 0a0a 2020 2020 2320 4f70  _file)..    # Op
-000068c0: 656e 2061 6e64 2072 6561 6420 5941 4d4c  en and read YAML
-000068d0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-000068e0: 696c 650a 2020 2020 7961 6d6c 5f63 6f6e  ile.    yaml_con
-000068f0: 7465 6e74 203d 205f 7265 6164 5f79 616d  tent = _read_yam
-00006900: 6c5f 746f 706f 6c6f 6779 5f66 696c 6528  l_topology_file(
-00006910: 746f 706f 6c6f 6779 5f66 696c 6529 0a0a  topology_file)..
-00006920: 2020 2020 2320 5061 7273 6520 5941 4d4c      # Parse YAML
-00006930: 2063 6f6e 6669 6775 7261 7469 6f6e 0a20   configuration. 
-00006940: 2020 2023 2057 6520 7573 6520 7275 616d     # We use ruam
-00006950: 656c 2e79 616d 6c20 6265 6361 7573 6520  el.yaml because 
-00006960: 6974 206b 6565 7073 2061 6e63 686f 7273  it keeps anchors
-00006970: 2061 6e64 0a20 2020 2023 2061 6c69 6173   and.    # alias
-00006980: 6573 2069 6e20 6d65 6d6f 7279 2e20 4974  es in memory. It
-00006990: 2069 7320 7665 7279 2063 6f6e 7665 6e69   is very conveni
-000069a0: 656e 7420 7768 656e 2074 6865 2073 696d  ent when the sim
-000069b0: 756c 6174 696f 6e0a 2020 2020 2320 6973  ulation.    # is
-000069c0: 2073 746f 7265 642f 6665 7463 6865 6420   stored/fetched 
-000069d0: 2872 6566 6572 656e 6365 7320 6172 6520  (references are 
-000069e0: 6b65 7074 2129 0a20 2020 206c 6f61 6465  kept!).    loade
-000069f0: 7220 3d20 5941 4d4c 2874 7970 3d22 7274  r = YAML(typ="rt
-00006a00: 2229 0a20 2020 2074 6f70 6f6c 6f67 795f  ").    topology_
-00006a10: 636f 6e74 656e 7420 3d20 6c6f 6164 6572  content = loader
-00006a20: 2e6c 6f61 6428 7961 6d6c 5f63 6f6e 7465  .load(yaml_conte
-00006a30: 6e74 290a 0a20 2020 2023 2041 6464 2061  nt)..    # Add a
-00006a40: 2064 6566 6175 6c74 2072 6573 6f75 7263   default resourc
-00006a50: 6573 2064 6972 6563 746f 7279 2069 6620  es directory if 
-00006a60: 6974 2065 7869 7374 732e 0a20 2020 2023  it exists..    #
-00006a70: 2049 6620 7468 6520 746f 706f 6c6f 6779   If the topology
-00006a80: 2069 7320 2270 6174 682f 746f 2f74 6f70   is "path/to/top
-00006a90: 6f2e 7961 6d6c 222c 2074 6865 2064 6566  o.yaml", the def
-00006aa0: 6175 6c74 2072 6573 6f75 7263 6573 2064  ault resources d
-00006ab0: 6972 6563 746f 7279 2069 7320 2270 6174  irectory is "pat
-00006ac0: 682f 746f 2f72 6573 6f75 7263 6573 222e  h/to/resources".
-00006ad0: 0a20 2020 2064 6566 6175 6c74 5f72 6573  .    default_res
-00006ae0: 6f75 7263 6573 5f70 6174 6820 3d20 6f73  ources_path = os
-00006af0: 2e70 6174 682e 6a6f 696e 286f 732e 7061  .path.join(os.pa
-00006b00: 7468 2e64 6972 6e61 6d65 2874 6f70 6f6c  th.dirname(topol
-00006b10: 6f67 795f 6669 6c65 292c 2022 7265 736f  ogy_file), "reso
-00006b20: 7572 6365 7322 290a 2020 2020 6465 6661  urces").    defa
-00006b30: 756c 745f 7265 736f 7572 6365 735f 7061  ult_resources_pa
-00006b40: 7468 203d 206f 732e 7061 7468 2e6e 6f72  th = os.path.nor
-00006b50: 6d70 6174 6828 6465 6661 756c 745f 7265  mpath(default_re
-00006b60: 736f 7572 6365 735f 7061 7468 290a 2020  sources_path).  
-00006b70: 2020 6966 205f 5f76 616c 6964 6174 655f    if __validate_
-00006b80: 7265 736f 7572 6365 735f 7061 7468 2864  resources_path(d
-00006b90: 6566 6175 6c74 5f72 6573 6f75 7263 6573  efault_resources
-00006ba0: 5f70 6174 682c 2046 616c 7365 293a 0a20  _path, False):. 
-00006bb0: 2020 2020 2020 2069 6620 6465 6661 756c         if defaul
-00006bc0: 745f 7265 736f 7572 6365 735f 7061 7468  t_resources_path
-00006bd0: 206e 6f74 2069 6e20 746f 706f 6c6f 6779   not in topology
-00006be0: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
-00006bf0: 3a0a 2020 2020 2020 2020 2020 2020 746f  :.            to
-00006c00: 706f 6c6f 6779 5f72 6573 6f75 7263 6573  pology_resources
-00006c10: 5f70 6174 6873 2e61 7070 656e 6428 6465  _paths.append(de
-00006c20: 6661 756c 745f 7265 736f 7572 6365 735f  fault_resources_
-00006c30: 7061 7468 290a 0a20 2020 2072 6574 7572  path)..    retur
-00006c40: 6e20 6578 7465 6e64 5f73 696d 756c 6174  n extend_simulat
-00006c50: 696f 6e28 0a20 2020 2020 2020 2074 6f70  ion(.        top
-00006c60: 6f6c 6f67 795f 636f 6e74 656e 743d 746f  ology_content=to
-00006c70: 706f 6c6f 6779 5f63 6f6e 7465 6e74 2c0a  pology_content,.
-00006c80: 2020 2020 2020 2020 746f 706f 6c6f 6779          topology
-00006c90: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
-00006ca0: 3d74 6f70 6f6c 6f67 795f 7265 736f 7572  =topology_resour
-00006cb0: 6365 735f 7061 7468 732c 0a20 2020 2020  ces_paths,.     
-00006cc0: 2020 2061 6c6c 6f63 6174 696f 6e5f 7374     allocation_st
-00006cd0: 7261 7465 6779 3d61 6c6c 6f63 6174 696f  rategy=allocatio
-00006ce0: 6e5f 7374 7261 7465 6779 2c0a 2020 2020  n_strategy,.    
-00006cf0: 2020 2020 6964 5f73 696d 756c 6174 696f      id_simulatio
-00006d00: 6e3d 6964 5f73 696d 756c 6174 696f 6e2c  n=id_simulation,
-00006d10: 0a20 2020 2029 0a0a 0a64 6566 2063 7265  .    )...def cre
-00006d20: 6174 655f 7369 6d75 6c61 7469 6f6e 5f66  ate_simulation_f
-00006d30: 726f 6d5f 6261 7365 626f 7828 0a20 2020  rom_basebox(.   
-00006d40: 2062 6173 6562 6f78 5f69 643a 2073 7472   basebox_id: str
-00006d50: 2c0a 2020 2020 6164 645f 696e 7465 726e  ,.    add_intern
-00006d60: 6574 3a20 626f 6f6c 203d 2046 616c 7365  et: bool = False
-00006d70: 2c0a 2020 2020 6164 645f 686f 7374 3a20  ,.    add_host: 
-00006d80: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00006d90: 2020 616c 6c6f 6361 7469 6f6e 5f73 7472    allocation_str
-00006da0: 6174 6567 793a 204f 7074 696f 6e61 6c5b  ategy: Optional[
-00006db0: 7374 725d 203d 204e 6f6e 652c 0a29 202d  str] = None,.) -
-00006dc0: 3e20 696e 743a 0a20 2020 2022 2222 4372  > int:.    """Cr
-00006dd0: 6561 7465 2061 206e 6577 2073 696d 756c  eate a new simul
-00006de0: 6174 696f 6e20 6d6f 6465 6c20 696e 2064  ation model in d
-00006df0: 6174 6162 6173 6520 6261 7365 6420 6f6e  atabase based on
-00006e00: 2074 6865 2070 726f 7669 6465 6420 6261   the provided ba
-00006e10: 7365 626f 7820 6964 2c20 7769 7468 0a20  sebox id, with. 
-00006e20: 2020 206f 7074 696f 6e61 6c20 696e 7465     optional inte
-00006e30: 726e 6574 2061 6e64 2f6f 7220 686f 7374  rnet and/or host
-00006e40: 2063 6f6e 6e65 6374 6976 6974 792e 0a0a   connectivity...
-00006e50: 2020 2020 2222 220a 0a20 2020 2069 6620      """..    if 
-00006e60: 6261 7365 626f 785f 6964 2069 7320 4e6f  basebox_id is No
-00006e70: 6e65 3a0a 2020 2020 2020 2020 7261 6973  ne:.        rais
-00006e80: 6520 4578 6365 7074 696f 6e28 2241 2062  e Exception("A b
-00006e90: 6173 6562 6f78 2049 4420 6973 2072 6571  asebox ID is req
-00006ea0: 7569 7265 6422 290a 0a20 2020 2023 2043  uired")..    # C
-00006eb0: 7265 6174 6520 616e 2074 6f70 6f6c 6f67  reate an topolog
-00006ec0: 7920 7769 7468 2074 6865 2070 726f 7669  y with the provi
-00006ed0: 6465 6420 6261 7365 626f 7820 4944 0a20  ded basebox ID. 
-00006ee0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00006ef0: 6261 7365 626f 7820 3d20 6665 7463 685f  basebox = fetch_
-00006f00: 6261 7365 626f 7828 6261 7365 626f 785f  basebox(basebox_
-00006f10: 6964 290a 2020 2020 6578 6365 7074 2045  id).    except E
-00006f20: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
-00006f30: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00006f40: 6e28 0a20 2020 2020 2020 2020 2020 2066  n(.            f
-00006f50: 2243 616e 6e6f 7420 6669 6e64 2062 6173  "Cannot find bas
-00006f60: 6562 6f78 2069 6e20 6461 7461 6261 7365  ebox in database
-00006f70: 2066 726f 6d20 6261 7365 626f 7820 4944   from basebox ID
-00006f80: 2027 7b62 6173 6562 6f78 5f69 647d 2722   '{basebox_id}'"
-00006f90: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00006fa0: 6e6f 6465 5f6e 616d 6520 3d20 5f67 6574  node_name = _get
-00006fb0: 5f72 616e 646f 6d5f 7374 7269 6e67 2831  _random_string(1
-00006fc0: 3029 0a20 2020 2072 6f6c 6520 3d20 6261  0).    role = ba
-00006fd0: 7365 626f 785b 2272 6f6c 6522 5d0a 2020  sebox["role"].  
-00006fe0: 2020 6e62 5f70 726f 6320 3d20 6261 7365    nb_proc = base
-00006ff0: 626f 785b 226e 625f 7072 6f63 225d 0a20  box["nb_proc"]. 
-00007000: 2020 206d 656d 6f72 795f 7369 7a65 203d     memory_size =
-00007010: 2062 6173 6562 6f78 5b22 6d65 6d6f 7279   basebox["memory
-00007020: 5f73 697a 6522 5d0a 0a20 2020 2079 616d  _size"]..    yam
-00007030: 6c5f 636f 6e74 656e 7420 3d20 6622 2222  l_content = f"""
-00007040: 2d2d 2d0a 6e61 6d65 3a20 227b 6261 7365  ---.name: "{base
-00007050: 626f 785f 6964 7d22 0a6e 6f64 6573 3a0a  box_id}".nodes:.
-00007060: 0a20 202d 2026 7377 6974 6368 0a20 2020  .  - &switch.   
-00007070: 2074 7970 653a 2073 7769 7463 680a 2020   type: switch.  
-00007080: 2020 6e61 6d65 3a20 2273 7769 7463 6822    name: "switch"
-00007090: 0a0a 2020 2d20 2663 6c69 656e 740a 2020  ..  - &client.  
-000070a0: 2020 7479 7065 3a20 7669 7274 7561 6c5f    type: virtual_
-000070b0: 6d61 6368 696e 650a 2020 2020 6e61 6d65  machine.    name
-000070c0: 3a20 227b 6e6f 6465 5f6e 616d 657d 220a  : "{node_name}".
-000070d0: 2020 2020 6261 7365 626f 785f 6964 3a20      basebox_id: 
-000070e0: 227b 6261 7365 626f 785f 6964 7d22 0a20  "{basebox_id}". 
-000070f0: 2020 206e 625f 7072 6f63 3a20 7b6e 625f     nb_proc: {nb_
-00007100: 7072 6f63 7d0a 2020 2020 6d65 6d6f 7279  proc}.    memory
-00007110: 5f73 697a 653a 207b 6d65 6d6f 7279 5f73  _size: {memory_s
-00007120: 697a 657d 0a20 2020 2072 6f6c 6573 3a20  ize}.    roles: 
-00007130: 5b22 7b72 6f6c 657d 225d 0a22 2222 0a0a  ["{role}"]."""..
-00007140: 2020 2020 6966 2061 6464 5f68 6f73 743a      if add_host:
-00007150: 0a20 2020 2020 2020 2079 616d 6c5f 636f  .        yaml_co
-00007160: 6e74 656e 7420 2b3d 2022 2222 0a20 202d  ntent += """.  -
-00007170: 2026 686f 7374 5f6d 6163 6869 6e65 0a20   &host_machine. 
-00007180: 2020 2074 7970 653a 2068 6f73 745f 6d61     type: host_ma
-00007190: 6368 696e 650a 2020 2020 6e61 6d65 3a20  chine.    name: 
-000071a0: 2268 6f73 7422 0a22 2222 0a0a 2020 2020  "host"."""..    
-000071b0: 6966 2061 6464 5f69 6e74 6572 6e65 743a  if add_internet:
-000071c0: 0a20 2020 2020 2020 2023 2061 6464 2064  .        # add d
-000071d0: 6566 6175 6c74 2072 6f75 7465 2074 6f20  efault route to 
-000071e0: 6761 7465 7761 792c 2061 2067 6174 6577  gateway, a gatew
-000071f0: 6179 2061 6e64 2061 2073 7769 7463 6820  ay and a switch 
-00007200: 746f 2070 6c75 6720 7468 6520 6761 7465  to plug the gate
-00007210: 7761 7920 616e 6420 7468 6520 726f 7574  way and the rout
-00007220: 6572 0a20 2020 2020 2020 2079 616d 6c5f  er.        yaml_
-00007230: 636f 6e74 656e 7420 2b3d 2022 2222 0a20  content += """. 
-00007240: 202d 2026 726f 7574 6572 0a20 2020 2074   - &router.    t
-00007250: 7970 653a 2072 6f75 7465 720a 2020 2020  ype: router.    
-00007260: 6e61 6d65 3a20 2272 6f75 7465 7222 0a20  name: "router". 
-00007270: 2020 2072 6f75 7465 733a 0a20 2020 2020     routes:.     
-00007280: 202d 2022 302e 302e 302e 302f 3020 2d3e   - "0.0.0.0/0 ->
-00007290: 2031 3932 2e31 3638 2e32 332e 3222 0a0a   192.168.23.2"..
-000072a0: 2020 2d20 2673 7769 7463 685f 696e 7465    - &switch_inte
-000072b0: 726e 6574 0a20 2020 2074 7970 653a 2073  rnet.    type: s
-000072c0: 7769 7463 680a 2020 2020 6e61 6d65 3a20  witch.    name: 
-000072d0: 2273 7769 7463 6849 6e74 6572 6e65 7422  "switchInternet"
-000072e0: 0a0a 2020 2d20 2670 6879 7369 6361 6c5f  ..  - &physical_
-000072f0: 6761 7465 7761 790a 2020 2020 7479 7065  gateway.    type
-00007300: 3a20 7068 7973 6963 616c 5f67 6174 6577  : physical_gatew
-00007310: 6179 0a20 2020 206e 616d 653a 2022 7068  ay.    name: "ph
-00007320: 7973 6963 616c 4761 7465 7761 7922 0a22  ysicalGateway"."
-00007330: 2222 0a20 2020 2065 6c73 653a 0a20 2020  "".    else:.   
-00007340: 2020 2020 2079 616d 6c5f 636f 6e74 656e       yaml_conten
-00007350: 7420 2b3d 2022 2222 0a20 202d 2026 726f  t += """.  - &ro
-00007360: 7574 6572 0a20 2020 2074 7970 653a 2072  uter.    type: r
-00007370: 6f75 7465 720a 2020 2020 6e61 6d65 3a20  outer.    name: 
-00007380: 2272 6f75 7465 7222 0a22 2222 0a0a 2020  "router"."""..  
-00007390: 2020 7961 6d6c 5f63 6f6e 7465 6e74 202b    yaml_content +
-000073a0: 3d20 2222 220a 6c69 6e6b 733a 0a0a 2020  = """.links:..  
-000073b0: 2d20 7377 6974 6368 3a20 2a73 7769 7463  - switch: *switc
-000073c0: 680a 2020 2020 6e6f 6465 3a20 2a72 6f75  h.    node: *rou
-000073d0: 7465 720a 2020 2020 7061 7261 6d73 3a0a  ter.    params:.
-000073e0: 2020 2020 2020 6970 3a20 2231 3932 2e31        ip: "192.1
-000073f0: 3638 2e32 2e31 2f32 3422 0a20 2020 2020  68.2.1/24".     
-00007400: 2064 6863 705f 6e61 6d65 7365 7276 6572   dhcp_nameserver
-00007410: 3a20 2238 2e38 2e38 2e38 220a 0a20 202d  : "8.8.8.8"..  -
-00007420: 2073 7769 7463 683a 202a 7377 6974 6368   switch: *switch
-00007430: 0a20 2020 206e 6f64 653a 202a 636c 6965  .    node: *clie
-00007440: 6e74 0a20 2020 2070 6172 616d 733a 0a20  nt.    params:. 
-00007450: 2020 2020 2069 703a 2022 3139 322e 3136       ip: "192.16
-00007460: 382e 322e 322f 3234 220a 2222 220a 0a20  8.2.2/24".""".. 
-00007470: 2020 2069 6620 6164 645f 686f 7374 3a0a     if add_host:.
-00007480: 2020 2020 2020 2020 7961 6d6c 5f63 6f6e          yaml_con
-00007490: 7465 6e74 202b 3d20 2222 220a 2020 2d20  tent += """.  - 
-000074a0: 7377 6974 6368 3a20 2a73 7769 7463 680a  switch: *switch.
-000074b0: 2020 2020 6e6f 6465 3a20 2a68 6f73 745f      node: *host_
-000074c0: 6d61 6368 696e 650a 2020 2020 7061 7261  machine.    para
-000074d0: 6d73 3a0a 2020 2020 2020 6970 3a20 2231  ms:.      ip: "1
-000074e0: 3932 2e31 3638 2e32 2e33 2f32 3422 0a22  92.168.2.3/24"."
-000074f0: 2222 0a0a 2020 2020 6966 2061 6464 5f69  ""..    if add_i
-00007500: 6e74 6572 6e65 743a 0a20 2020 2020 2020  nternet:.       
-00007510: 2079 616d 6c5f 636f 6e74 656e 7420 2b3d   yaml_content +=
-00007520: 2022 2222 0a20 202d 2073 7769 7463 683a   """.  - switch:
-00007530: 202a 7377 6974 6368 5f69 6e74 6572 6e65   *switch_interne
-00007540: 740a 2020 2020 6e6f 6465 3a20 2a72 6f75  t.    node: *rou
-00007550: 7465 720a 2020 2020 7061 7261 6d73 3a0a  ter.    params:.
-00007560: 2020 2020 2020 6970 3a20 2231 3932 2e31        ip: "192.1
-00007570: 3638 2e32 332e 312f 3234 220a 0a20 202d  68.23.1/24"..  -
-00007580: 2073 7769 7463 683a 202a 7377 6974 6368   switch: *switch
-00007590: 5f69 6e74 6572 6e65 740a 2020 2020 6e6f  _internet.    no
-000075a0: 6465 3a20 2a70 6879 7369 6361 6c5f 6761  de: *physical_ga
-000075b0: 7465 7761 790a 2020 2020 7061 7261 6d73  teway.    params
-000075c0: 3a0a 2020 2020 2020 6970 3a20 2231 3932  :.      ip: "192
-000075d0: 2e31 3638 2e32 332e 322f 3234 220a 2222  .168.23.2/24".""
-000075e0: 220a 0a20 2020 206c 6f61 6465 7220 3d20  "..    loader = 
-000075f0: 5941 4d4c 2874 7970 3d22 7274 2229 0a20  YAML(typ="rt"). 
-00007600: 2020 2074 6f70 6f6c 6f67 795f 636f 6e74     topology_cont
-00007610: 656e 7420 3d20 6c6f 6164 6572 2e6c 6f61  ent = loader.loa
-00007620: 6428 7961 6d6c 5f63 6f6e 7465 6e74 290a  d(yaml_content).
-00007630: 0a20 2020 2072 6574 7572 6e20 6372 6561  .    return crea
-00007640: 7465 5f73 696d 756c 6174 696f 6e28 0a20  te_simulation(. 
-00007650: 2020 2020 2020 2074 6f70 6f6c 6f67 795f         topology_
-00007660: 636f 6e74 656e 743d 746f 706f 6c6f 6779  content=topology
-00007670: 5f63 6f6e 7465 6e74 2c0a 2020 2020 2020  _content,.      
-00007680: 2020 616c 6c6f 6361 7469 6f6e 5f73 7472    allocation_str
-00007690: 6174 6567 793d 616c 6c6f 6361 7469 6f6e  ategy=allocation
-000076a0: 5f73 7472 6174 6567 792c 0a20 2020 2029  _strategy,.    )
-000076b0: 0a0a 0a64 6566 2065 7874 656e 645f 7369  ...def extend_si
-000076c0: 6d75 6c61 7469 6f6e 5f66 726f 6d5f 6261  mulation_from_ba
-000076d0: 7365 626f 7828 0a20 2020 2062 6173 6562  sebox(.    baseb
-000076e0: 6f78 5f69 643a 2073 7472 2c0a 2020 2020  ox_id: str,.    
-000076f0: 7377 6974 6368 5f6e 616d 653a 2073 7472  switch_name: str
-00007700: 2c0a 2020 2020 616c 6c6f 6361 7469 6f6e  ,.    allocation
-00007710: 5f73 7472 6174 6567 793a 204f 7074 696f  _strategy: Optio
-00007720: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00007730: 0a20 2020 2069 645f 7369 6d75 6c61 7469  .    id_simulati
-00007740: 6f6e 3a20 696e 7420 3d20 4e6f 6e65 2c0a  on: int = None,.
-00007750: 2920 2d3e 2069 6e74 3a0a 2020 2020 2222  ) -> int:.    ""
-00007760: 2245 7874 656e 6420 616e 2065 7869 7374  "Extend an exist
-00007770: 696e 6720 7369 6d75 6c61 7469 6f6e 206d  ing simulation m
-00007780: 6f64 656c 2069 6e20 6461 7461 6261 7365  odel in database
-00007790: 2062 6173 6564 206f 6e20 7468 650a 2020   based on the.  
-000077a0: 2020 7072 6f76 6964 6564 2062 6173 6562    provided baseb
-000077b0: 6f78 2069 642c 2061 6e64 2070 6c75 6720  ox id, and plug 
-000077c0: 7468 6520 6e65 7720 6e6f 6465 206f 6620  the new node of 
-000077d0: 7468 6520 7370 6563 6966 6564 2073 7769  the specifed swi
-000077e0: 7463 682e 0a0a 2020 2020 2222 220a 0a20  tch...    """.. 
-000077f0: 2020 2069 6620 6261 7365 626f 785f 6964     if basebox_id
-00007800: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00007810: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00007820: 6e28 2241 2062 6173 6562 6f78 2049 4420  n("A basebox ID 
-00007830: 6973 2072 6571 7569 7265 6422 290a 0a20  is required").. 
-00007840: 2020 2023 2043 7265 6174 6520 616e 2074     # Create an t
-00007850: 6f70 6f6c 6f67 7920 7769 7468 2074 6865  opology with the
-00007860: 2070 726f 7669 6465 6420 6261 7365 626f   provided basebo
-00007870: 7820 4944 0a20 2020 2074 7279 3a0a 2020  x ID.    try:.  
-00007880: 2020 2020 2020 6261 7365 626f 7820 3d20        basebox = 
-00007890: 6665 7463 685f 6261 7365 626f 7828 6261  fetch_basebox(ba
-000078a0: 7365 626f 785f 6964 290a 2020 2020 6578  sebox_id).    ex
-000078b0: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
-000078c0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
-000078d0: 6365 7074 696f 6e28 0a20 2020 2020 2020  ception(.       
-000078e0: 2020 2020 2066 2243 616e 6e6f 7420 6669       f"Cannot fi
-000078f0: 6e64 2062 6173 6562 6f78 2069 6e20 6461  nd basebox in da
-00007900: 7461 6261 7365 2066 726f 6d20 6261 7365  tabase from base
-00007910: 626f 7820 4944 2027 7b62 6173 6562 6f78  box ID '{basebox
-00007920: 5f69 647d 2722 0a20 2020 2020 2020 2029  _id}'".        )
-00007930: 0a0a 2020 2020 6e6f 6465 5f6e 616d 6520  ..    node_name 
-00007940: 3d20 5f67 6574 5f72 616e 646f 6d5f 7374  = _get_random_st
-00007950: 7269 6e67 2831 3029 0a20 2020 2072 6f6c  ring(10).    rol
-00007960: 6520 3d20 6261 7365 626f 785b 2272 6f6c  e = basebox["rol
-00007970: 6522 5d0a 2020 2020 6e62 5f70 726f 6320  e"].    nb_proc 
-00007980: 3d20 6261 7365 626f 785b 226e 625f 7072  = basebox["nb_pr
-00007990: 6f63 225d 0a20 2020 206d 656d 6f72 795f  oc"].    memory_
-000079a0: 7369 7a65 203d 2062 6173 6562 6f78 5b22  size = basebox["
-000079b0: 6d65 6d6f 7279 5f73 697a 6522 5d0a 0a20  memory_size"].. 
-000079c0: 2020 2074 6f70 6f6c 6f67 795f 636f 6e74     topology_cont
-000079d0: 656e 7420 3d20 7b0a 2020 2020 2020 2020  ent = {.        
-000079e0: 226e 6f64 6573 223a 205b 0a20 2020 2020  "nodes": [.     
-000079f0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00007a00: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00007a10: 2022 7669 7274 7561 6c5f 6d61 6368 696e   "virtual_machin
-00007a20: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00007a30: 2020 2020 226e 616d 6522 3a20 6e6f 6465      "name": node
-00007a40: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-00007a50: 2020 2020 2020 2022 6261 7365 626f 785f         "basebox_
-00007a60: 6964 223a 2062 6173 6562 6f78 5f69 642c  id": basebox_id,
-00007a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007a80: 2022 6e62 5f70 726f 6322 3a20 6e62 5f70   "nb_proc": nb_p
-00007a90: 726f 632c 0a20 2020 2020 2020 2020 2020  roc,.           
-00007aa0: 2020 2020 2022 6d65 6d6f 7279 5f73 697a       "memory_siz
-00007ab0: 6522 3a20 6d65 6d6f 7279 5f73 697a 652c  e": memory_size,
-00007ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007ad0: 2022 726f 6c65 7322 3a20 5b72 6f6c 655d   "roles": [role]
-00007ae0: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
-00007af0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00007b00: 2020 2022 6c69 6e6b 7322 3a20 5b0a 2020     "links": [.  
-00007b10: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00007b20: 2020 2020 2020 2020 2020 2020 2273 7769              "swi
-00007b30: 7463 6822 3a20 7b22 7479 7065 223a 2022  tch": {"type": "
-00007b40: 7377 6974 6368 222c 2022 6e61 6d65 223a  switch", "name":
-00007b50: 2073 7769 7463 685f 6e61 6d65 7d2c 0a20   switch_name},. 
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007b70: 6e6f 6465 223a 207b 0a20 2020 2020 2020  node": {.       
-00007b80: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-00007b90: 7065 223a 2022 7669 7274 7561 6c5f 6d61  pe": "virtual_ma
-00007ba0: 6368 696e 6522 2c0a 2020 2020 2020 2020  chine",.        
-00007bb0: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-00007bc0: 6522 3a20 6e6f 6465 5f6e 616d 652c 0a20  e": node_name,. 
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00007be0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007bf0: 2020 2270 6172 616d 7322 3a20 7b7d 2c20    "params": {}, 
-00007c00: 2023 2044 796e 616d 6963 2049 5020 6164   # Dynamic IP ad
-00007c10: 6472 6573 730a 2020 2020 2020 2020 2020  dress.          
-00007c20: 2020 7d0a 2020 2020 2020 2020 5d2c 0a20    }.        ],. 
-00007c30: 2020 207d 0a0a 2020 2020 7265 7475 726e     }..    return
-00007c40: 2065 7874 656e 645f 7369 6d75 6c61 7469   extend_simulati
-00007c50: 6f6e 280a 2020 2020 2020 2020 746f 706f  on(.        topo
-00007c60: 6c6f 6779 5f63 6f6e 7465 6e74 3d74 6f70  logy_content=top
-00007c70: 6f6c 6f67 795f 636f 6e74 656e 742c 0a20  ology_content,. 
-00007c80: 2020 2020 2020 2061 6c6c 6f63 6174 696f         allocatio
-00007c90: 6e5f 7374 7261 7465 6779 3d61 6c6c 6f63  n_strategy=alloc
-00007ca0: 6174 696f 6e5f 7374 7261 7465 6779 2c0a  ation_strategy,.
-00007cb0: 2020 2020 2020 2020 6964 5f73 696d 756c          id_simul
-00007cc0: 6174 696f 6e3d 6964 5f73 696d 756c 6174  ation=id_simulat
-00007cd0: 696f 6e2c 0a20 2020 2029 0a0a 0a23 2323  ion,.    )...###
-00007ce0: 0a23 2054 6f70 6f6c 6f67 7920 6865 6c70  .# Topology help
-00007cf0: 6572 730a 2323 230a 0a0a 6465 6620 746f  ers.###...def to
-00007d00: 706f 6c6f 6779 5f66 696c 655f 6164 645f  pology_file_add_
-00007d10: 7765 6273 6974 6573 280a 2020 2020 746f  websites(.    to
-00007d20: 706f 6c6f 6779 5f66 696c 653a 2073 7472  pology_file: str
-00007d30: 2c20 7765 6273 6974 6573 3a20 4c69 7374  , websites: List
-00007d40: 5b73 7472 5d2c 2073 7769 7463 685f 6e61  [str], switch_na
-00007d50: 6d65 3a20 7374 720a 2920 2d3e 2073 7472  me: str.) -> str
-00007d60: 3a0a 2020 2020 2222 2241 6464 2064 6f63  :.    """Add doc
-00007d70: 6b65 7220 7765 6273 6974 6573 206e 6f64  ker websites nod
-00007d80: 6520 746f 2061 2067 6976 656e 2074 6f70  e to a given top
-00007d90: 6f6c 6f67 792c 2061 6e64 2072 6574 7572  ology, and retur
-00007da0: 6e20 7468 6520 7570 6461 7465 6420 746f  n the updated to
-00007db0: 706f 6c6f 6779 2e22 2222 0a0a 2020 2020  pology."""..    
-00007dc0: 2320 5661 6c69 6461 7465 2059 414d 4c20  # Validate YAML 
-00007dd0: 746f 706f 6c6f 6779 2066 696c 650a 2020  topology file.  
-00007de0: 2020 5f76 616c 6964 6174 655f 7961 6d6c    _validate_yaml
-00007df0: 5f74 6f70 6f6c 6f67 795f 6669 6c65 2874  _topology_file(t
-00007e00: 6f70 6f6c 6f67 795f 6669 6c65 290a 0a20  opology_file).. 
-00007e10: 2020 2023 204f 7065 6e20 616e 6420 7265     # Open and re
-00007e20: 6164 2059 414d 4c20 746f 706f 6c6f 6779  ad YAML topology
-00007e30: 2066 696c 650a 2020 2020 746f 706f 6c6f   file.    topolo
-00007e40: 6779 5f79 616d 6c20 3d20 5f72 6561 645f  gy_yaml = _read_
-00007e50: 7961 6d6c 5f74 6f70 6f6c 6f67 795f 6669  yaml_topology_fi
-00007e60: 6c65 2874 6f70 6f6c 6f67 795f 6669 6c65  le(topology_file
-00007e70: 290a 0a20 2020 2023 2055 7064 6174 6520  )..    # Update 
-00007e80: 746f 706f 6c6f 6779 2077 6974 6820 7468  topology with th
-00007e90: 6520 4150 490a 2020 2020 746f 706f 6c6f  e API.    topolo
-00007ea0: 6779 5f79 616d 6c20 3d20 746f 706f 6c6f  gy_yaml = topolo
-00007eb0: 6779 5f61 6464 5f77 6562 7369 7465 7328  gy_add_websites(
-00007ec0: 746f 706f 6c6f 6779 5f79 616d 6c2c 2077  topology_yaml, w
-00007ed0: 6562 7369 7465 732c 2073 7769 7463 685f  ebsites, switch_
-00007ee0: 6e61 6d65 290a 0a20 2020 2072 6574 7572  name)..    retur
-00007ef0: 6e20 746f 706f 6c6f 6779 5f79 616d 6c0a  n topology_yaml.
-00007f00: 0a0a 6465 6620 746f 706f 6c6f 6779 5f66  ..def topology_f
-00007f10: 696c 655f 6164 645f 6467 6128 0a20 2020  ile_add_dga(.   
-00007f20: 2074 6f70 6f6c 6f67 795f 6669 6c65 3a20   topology_file: 
-00007f30: 7374 722c 0a20 2020 2061 6c67 6f72 6974  str,.    algorit
-00007f40: 686d 3a20 7374 722c 0a20 2020 2073 7769  hm: str,.    swi
-00007f50: 7463 685f 6e61 6d65 3a20 7374 722c 0a20  tch_name: str,. 
-00007f60: 2020 206e 756d 6265 723a 2069 6e74 2c0a     number: int,.
-00007f70: 2020 2020 7265 736f 7572 6365 735f 6469      resources_di
-00007f80: 723a 2073 7472 2c0a 2920 2d3e 2028 7374  r: str,.) -> (st
-00007f90: 722c 204c 6973 745b 7374 725d 293a 0a20  r, List[str]):. 
-00007fa0: 2020 2022 2222 4164 6420 646f 636b 6572     """Add docker
-00007fb0: 2065 6d70 7479 2077 6562 7369 7465 7320   empty websites 
-00007fc0: 6e6f 6465 2077 6974 6820 4447 4120 746f  node with DGA to
-00007fd0: 2061 2067 6976 656e 2074 6f70 6f6c 6f67   a given topolog
-00007fe0: 792c 2061 6e64 2072 6574 7572 6e20 7468  y, and return th
-00007ff0: 6520 7570 6461 7465 6420 746f 706f 6c6f  e updated topolo
-00008000: 6779 2e22 2222 0a0a 2020 2020 2320 5661  gy."""..    # Va
-00008010: 6c69 6461 7465 0a0a 2020 2020 2320 5661  lidate..    # Va
-00008020: 6c69 6461 7465 2059 414d 4c20 746f 706f  lidate YAML topo
-00008030: 6c6f 6779 2066 696c 650a 2020 2020 5f76  logy file.    _v
-00008040: 616c 6964 6174 655f 7961 6d6c 5f74 6f70  alidate_yaml_top
-00008050: 6f6c 6f67 795f 6669 6c65 2874 6f70 6f6c  ology_file(topol
-00008060: 6f67 795f 6669 6c65 290a 0a20 2020 2023  ogy_file)..    #
-00008070: 204f 7065 6e20 616e 6420 7265 6164 2059   Open and read Y
-00008080: 414d 4c20 746f 706f 6c6f 6779 2066 696c  AML topology fil
-00008090: 650a 2020 2020 746f 706f 6c6f 6779 5f79  e.    topology_y
-000080a0: 616d 6c20 3d20 5f72 6561 645f 7961 6d6c  aml = _read_yaml
-000080b0: 5f74 6f70 6f6c 6f67 795f 6669 6c65 2874  _topology_file(t
-000080c0: 6f70 6f6c 6f67 795f 6669 6c65 290a 0a20  opology_file).. 
-000080d0: 2020 2023 2055 7064 6174 6520 746f 706f     # Update topo
-000080e0: 6c6f 6779 2077 6974 6820 7468 6520 4150  logy with the AP
-000080f0: 490a 2020 2020 2874 6f70 6f6c 6f67 795f  I.    (topology_
-00008100: 7961 6d6c 2c20 646f 6d61 696e 7329 203d  yaml, domains) =
-00008110: 2074 6f70 6f6c 6f67 795f 6164 645f 6467   topology_add_dg
-00008120: 6128 0a20 2020 2020 2020 2074 6f70 6f6c  a(.        topol
-00008130: 6f67 795f 7961 6d6c 2c20 616c 676f 7269  ogy_yaml, algori
-00008140: 7468 6d2c 2073 7769 7463 685f 6e61 6d65  thm, switch_name
-00008150: 2c20 6e75 6d62 6572 2c20 7265 736f 7572  , number, resour
-00008160: 6365 735f 6469 720a 2020 2020 290a 0a20  ces_dir.    ).. 
-00008170: 2020 2072 6574 7572 6e20 746f 706f 6c6f     return topolo
-00008180: 6779 5f79 616d 6c2c 2064 6f6d 6169 6e73  gy_yaml, domains
-00008190: 0a0a 0a64 6566 2074 6f70 6f6c 6f67 795f  ...def topology_
-000081a0: 6669 6c65 5f61 6464 5f64 6e73 5f73 6572  file_add_dns_ser
-000081b0: 7665 7228 0a20 2020 2074 6f70 6f6c 6f67  ver(.    topolog
-000081c0: 795f 6669 6c65 3a20 7374 722c 0a20 2020  y_file: str,.   
-000081d0: 2073 7769 7463 685f 6e61 6d65 3a20 7374   switch_name: st
-000081e0: 722c 0a20 2020 2072 6573 6f75 7263 6573  r,.    resources
-000081f0: 5f64 6972 3a20 7374 722c 0a29 202d 3e20  _dir: str,.) -> 
-00008200: 2873 7472 2c20 7374 7229 3a0a 2020 2020  (str, str):.    
-00008210: 2222 2241 6464 2061 2044 4e53 2073 6572  """Add a DNS ser
-00008220: 7665 7220 746f 2061 2059 414d 4c20 746f  ver to a YAML to
-00008230: 706f 6c6f 6779 2e0a 2020 2020 5265 7475  pology..    Retu
-00008240: 726e 7320 7468 6520 7570 6461 7465 6420  rns the updated 
-00008250: 746f 706f 6c6f 6779 2061 6e64 2074 6865  topology and the
-00008260: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
-00008270: 444e 5320 636f 6e66 6967 7572 6174 696f  DNS configuratio
-00008280: 6e20 6669 6c65 2e22 2222 0a0a 2020 2020  n file."""..    
-00008290: 2320 5661 6c69 6461 7465 0a0a 2020 2020  # Validate..    
-000082a0: 2320 5661 6c69 6461 7465 2059 414d 4c20  # Validate YAML 
-000082b0: 746f 706f 6c6f 6779 2066 696c 650a 2020  topology file.  
-000082c0: 2020 5f76 616c 6964 6174 655f 7961 6d6c    _validate_yaml
-000082d0: 5f74 6f70 6f6c 6f67 795f 6669 6c65 2874  _topology_file(t
-000082e0: 6f70 6f6c 6f67 795f 6669 6c65 290a 0a20  opology_file).. 
-000082f0: 2020 2023 204f 7065 6e20 616e 6420 7265     # Open and re
-00008300: 6164 2059 414d 4c20 746f 706f 6c6f 6779  ad YAML topology
-00008310: 2066 696c 650a 2020 2020 746f 706f 6c6f   file.    topolo
-00008320: 6779 5f79 616d 6c20 3d20 5f72 6561 645f  gy_yaml = _read_
-00008330: 7961 6d6c 5f74 6f70 6f6c 6f67 795f 6669  yaml_topology_fi
-00008340: 6c65 2874 6f70 6f6c 6f67 795f 6669 6c65  le(topology_file
-00008350: 290a 0a20 2020 2023 2055 7064 6174 6520  )..    # Update 
-00008360: 746f 706f 6c6f 6779 2077 6974 6820 7468  topology with th
-00008370: 6520 4150 490a 2020 2020 2874 6f70 6f6c  e API.    (topol
-00008380: 6f67 795f 7961 6d6c 2c20 646e 735f 636f  ogy_yaml, dns_co
-00008390: 6e66 5f63 6f6e 7465 6e74 2920 3d20 746f  nf_content) = to
-000083a0: 706f 6c6f 6779 5f61 6464 5f64 6e73 5f73  pology_add_dns_s
-000083b0: 6572 7665 7228 0a20 2020 2020 2020 2074  erver(.        t
-000083c0: 6f70 6f6c 6f67 795f 7961 6d6c 2c20 7377  opology_yaml, sw
-000083d0: 6974 6368 5f6e 616d 652c 2072 6573 6f75  itch_name, resou
-000083e0: 7263 6573 5f64 6972 0a20 2020 2029 0a0a  rces_dir.    )..
-000083f0: 2020 2020 7265 7475 726e 2074 6f70 6f6c      return topol
-00008400: 6f67 795f 7961 6d6c 2c20 646e 735f 636f  ogy_yaml, dns_co
-00008410: 6e66 5f63 6f6e 7465 6e74 0a0a 0a23 2323  nf_content...###
-00008420: 0a23 2042 6173 6562 6f78 2068 656c 7065  .# Basebox helpe
-00008430: 7273 0a23 2323 0a0a 0a64 6566 205f 7261  rs.###...def _ra
-00008440: 6973 655f 6572 726f 725f 6d73 6728 7265  ise_error_msg(re
-00008450: 7375 6c74 3a20 6469 6374 2920 2d3e 204e  sult: dict) -> N
-00008460: 6f6e 653a 0a20 2020 2022 2222 0a20 2020  one:.    """.   
-00008470: 2052 6169 7365 2061 6e20 6572 726f 7220   Raise an error 
-00008480: 6d65 7373 6167 6520 6966 2061 2074 6173  message if a tas
-00008490: 6b20 2865 6720 7468 6520 6261 7365 626f  k (eg the basebo
-000084a0: 7820 7665 7269 6669 6361 7469 6f6e 2920  x verification) 
-000084b0: 6661 696c 6564 0a20 2020 203a 7061 7261  failed.    :para
-000084c0: 6d20 7265 7375 6c74 3a20 7468 6520 7265  m result: the re
-000084d0: 7375 6c74 206f 6620 7468 6520 7461 736b  sult of the task
-000084e0: 0a20 2020 203a 7265 7475 726e 3a20 4e6f  .    :return: No
-000084f0: 6e65 0a20 2020 2022 2222 0a20 2020 2065  ne.    """.    e
-00008500: 7272 6f72 5f6d 7367 203d 2022 4e6f 2065  rror_msg = "No e
-00008510: 7272 6f72 206d 6573 7361 6765 2072 6574  rror message ret
-00008520: 7572 6e65 6422 0a20 2020 2069 6620 2272  urned".    if "r
-00008530: 6573 756c 7422 2069 6e20 7265 7375 6c74  esult" in result
-00008540: 3a0a 2020 2020 2020 2020 6966 2022 6572  :.        if "er
-00008550: 726f 725f 6d73 6722 2069 6e20 7265 7375  ror_msg" in resu
-00008560: 6c74 5b22 7265 7375 6c74 225d 3a0a 2020  lt["result"]:.  
-00008570: 2020 2020 2020 2020 2020 6572 726f 725f            error_
-00008580: 6d73 6720 3d20 7265 7375 6c74 5b22 7265  msg = result["re
-00008590: 7375 6c74 225d 5b22 6572 726f 725f 6d73  sult"]["error_ms
-000085a0: 6722 5d0a 2020 2020 2020 2020 7261 6973  g"].        rais
-000085b0: 6520 4578 6365 7074 696f 6e28 6572 726f  e Exception(erro
-000085c0: 725f 6d73 6729 0a20 2020 2065 6c73 653a  r_msg).    else:
-000085d0: 0a20 2020 2020 2020 2072 6169 7365 2045  .        raise E
-000085e0: 7863 6570 7469 6f6e 2866 224e 6f20 2772  xception(f"No 'r
-000085f0: 6573 756c 7427 206b 6579 2069 6e20 7265  esult' key in re
-00008600: 7375 6c74 3a20 7b72 6573 756c 747d 2229  sult: {result}")
-00008610: 0a0a 0a64 6566 205f 5f62 6173 6562 6f78  ...def __basebox
-00008620: 6573 5f76 6572 6966 6963 6174 696f 6e5f  es_verification_
-00008630: 7761 6974 5f75 6e74 696c 5f63 6f6d 706c  wait_until_compl
-00008640: 6574 6528 0a20 2020 2074 6173 6b5f 6964  ete(.    task_id
-00008650: 3a20 7374 722c 206c 6f67 5f73 7566 6669  : str, log_suffi
-00008660: 783a 2073 7472 203d 204e 6f6e 652c 2074  x: str = None, t
-00008670: 696d 656f 7574 3a20 696e 7420 3d20 3336  imeout: int = 36
-00008680: 3030 0a29 202d 3e20 6469 6374 3a0a 2020  00.) -> dict:.  
-00008690: 2020 2222 220a 2020 2020 5761 6974 2075    """.    Wait u
-000086a0: 6e74 696c 2074 6865 2076 6572 6966 6963  ntil the verific
-000086b0: 6174 696f 6e20 7461 736b 2072 6570 7265  ation task repre
-000086c0: 7365 6e74 696e 6720 6279 2069 7473 2069  senting by its i
-000086d0: 6420 6973 2063 6f6d 706c 6574 6564 0a20  d is completed. 
-000086e0: 2020 203a 7061 7261 6d20 7461 736b 5f69     :param task_i
-000086f0: 643a 2074 6865 2074 6173 6b20 6964 0a20  d: the task id. 
-00008700: 2020 203a 7061 7261 6d20 6c6f 675f 7375     :param log_su
-00008710: 6666 6978 3a20 7768 6174 2074 6f20 696e  ffix: what to in
-00008720: 7365 7274 2069 6e74 6f20 7468 6520 6c6f  sert into the lo
-00008730: 670a 2020 2020 3a70 6172 616d 2074 696d  g.    :param tim
-00008740: 656f 7574 3a20 7468 6520 7469 6d65 6f75  eout: the timeou
-00008750: 7420 746f 2073 746f 7020 7468 6520 7461  t to stop the ta
-00008760: 736b 0a20 2020 203a 7265 7475 726e 3a20  sk.    :return: 
-00008770: 7468 6520 7265 7375 6c74 206f 6620 7468  the result of th
-00008780: 6520 6261 7365 626f 7820 7665 7269 6669  e basebox verifi
-00008790: 6361 7469 6f6e 0a20 2020 2022 2222 0a0a  cation.    """..
-000087a0: 2020 2020 7374 6172 745f 7469 6d65 203d      start_time =
-000087b0: 2074 696d 652e 7469 6d65 2829 0a0a 2020   time.time()..  
-000087c0: 2020 6669 6e69 7368 6564 203d 2046 616c    finished = Fal
-000087d0: 7365 0a20 2020 2077 6869 6c65 206e 6f74  se.    while not
-000087e0: 2028 6669 6e69 7368 6564 206f 7220 2874   (finished or (t
-000087f0: 696d 652e 7469 6d65 2829 202d 2073 7461  ime.time() - sta
-00008800: 7274 5f74 696d 6529 203e 2074 696d 656f  rt_time) > timeo
-00008810: 7574 293a 0a20 2020 2020 2020 2074 696d  ut):.        tim
-00008820: 652e 736c 6565 7028 3229 0a20 2020 2020  e.sleep(2).     
-00008830: 2020 2063 7572 7265 6e74 5f74 696d 6520     current_time 
-00008840: 3d20 7469 6d65 2e74 696d 6528 290a 2020  = time.time().  
-00008850: 2020 2020 2020 656c 6170 7365 6420 3d20        elapsed = 
-00008860: 696e 7428 6375 7272 656e 745f 7469 6d65  int(current_time
-00008870: 202d 2073 7461 7274 5f74 696d 6529 0a20   - start_time). 
-00008880: 2020 2020 2020 2069 6620 6c6f 675f 7375         if log_su
-00008890: 6666 6978 2069 7320 6e6f 7420 4e6f 6e65  ffix is not None
-000088a0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-000088b0: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
-000088c0: 2020 2020 2020 2020 2020 2066 2220 2020             f"   
-000088d0: 5b2b 5d20 4375 7272 656e 746c 7920 7665  [+] Currently ve
-000088e0: 7269 6679 696e 6720 7b6c 6f67 5f73 7566  rifying {log_suf
-000088f0: 6669 787d 2066 6f72 207b 656c 6170 7365  fix} for {elapse
-00008900: 647d 2073 6563 6f6e 6473 2028 7469 6d65  d} seconds (time
-00008910: 6f75 7420 6174 207b 7469 6d65 6f75 747d  out at {timeout}
-00008920: 2073 6563 6f6e 6473 2922 0a20 2020 2020   seconds)".     
-00008930: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00008940: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00008950: 2020 206c 6f67 6765 722e 696e 666f 280a     logger.info(.
-00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008970: 6622 2020 205b 2b5d 2043 7572 7265 6e74  f"   [+] Current
-00008980: 6c79 2072 756e 6e69 6e67 2074 6865 2076  ly running the v
-00008990: 6572 6966 6963 6174 696f 6e20 666f 7220  erification for 
-000089a0: 7b65 6c61 7073 6564 7d20 7365 636f 6e64  {elapsed} second
-000089b0: 7322 0a20 2020 2020 2020 2020 2020 2029  s".            )
-000089c0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-000089d0: 203d 205f 706f 7374 2822 2f62 6173 6562   = _post("/baseb
-000089e0: 6f78 2f73 7461 7475 735f 7665 7269 6679  ox/status_verify
-000089f0: 222c 2064 6174 613d 7b22 7461 736b 5f69  ", data={"task_i
-00008a00: 6422 3a20 7461 736b 5f69 647d 290a 2020  d": task_id}).  
-00008a10: 2020 2020 2020 7265 7375 6c74 2e72 6169        result.rai
-00008a20: 7365 5f66 6f72 5f73 7461 7475 7328 290a  se_for_status().
-00008a30: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00008a40: 2072 6573 756c 742e 6a73 6f6e 2829 0a0a   result.json()..
-00008a50: 2020 2020 2020 2020 6966 2022 7374 6174          if "stat
-00008a60: 7573 2220 696e 2072 6573 756c 743a 0a20  us" in result:. 
-00008a70: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00008a80: 6e74 5f73 7461 7475 7320 3d20 7265 7375  nt_status = resu
-00008a90: 6c74 5b22 7374 6174 7573 225d 0a0a 2020  lt["status"]..  
-00008aa0: 2020 2020 2020 2020 2020 6966 2063 7572            if cur
-00008ab0: 7265 6e74 5f73 7461 7475 7320 3d3d 2022  rent_status == "
-00008ac0: 4552 524f 5222 3a0a 2020 2020 2020 2020  ERROR":.        
-00008ad0: 2020 2020 2020 2020 6572 726f 725f 6d65          error_me
-00008ae0: 7373 6167 6520 3d20 7265 7375 6c74 5b22  ssage = result["
-00008af0: 6572 726f 725f 6d73 6722 5d0a 2020 2020  error_msg"].    
-00008b00: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00008b10: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
-00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b30: 2066 2245 7272 6f72 2064 7572 696e 6720   f"Error during 
-00008b40: 7665 7269 6669 6361 7469 6f6e 206f 7065  verification ope
-00008b50: 7261 7469 6f6e 3a20 277b 6572 726f 725f  ration: '{error_
-00008b60: 6d65 7373 6167 657d 2722 0a20 2020 2020  message}'".     
-00008b70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00008b80: 2020 2020 2020 2020 2065 6c69 6620 6375           elif cu
-00008b90: 7272 656e 745f 7374 6174 7573 203d 3d20  rrent_status == 
-00008ba0: 2246 494e 4953 4845 4422 3a0a 2020 2020  "FINISHED":.    
-00008bb0: 2020 2020 2020 2020 2020 2020 6669 6e69              fini
-00008bc0: 7368 6564 203d 2054 7275 650a 0a20 2020  shed = True..   
-00008bd0: 2069 6620 6e6f 7420 6669 6e69 7368 6564   if not finished
-00008be0: 3a0a 2020 2020 2020 2020 6572 726f 725f  :.        error_
-00008bf0: 6d73 6720 3d20 6622 5b2d 5d20 556e 6162  msg = f"[-] Unab
-00008c00: 6c65 2074 6f20 7465 726d 696e 6174 6520  le to terminate 
-00008c10: 6f70 6572 6174 696f 6e20 6265 666f 7265  operation before
-00008c20: 2074 696d 656f 7574 206f 6620 7b74 696d   timeout of {tim
-00008c30: 656f 7574 7d20 7365 636f 6e64 732e 2053  eout} seconds. S
-00008c40: 746f 7070 696e 6720 6f70 6572 6174 696f  topping operatio
-00008c50: 6e2e 220a 2020 2020 2020 2020 7265 7375  n.".        resu
-00008c60: 6c74 203d 2076 6572 6966 795f 6261 7365  lt = verify_base
-00008c70: 626f 785f 7374 6f70 2874 6173 6b5f 6964  box_stop(task_id
-00008c80: 290a 2020 2020 2020 2020 7374 6f70 7065  ).        stoppe
-00008c90: 6420 3d20 7265 7375 6c74 5b22 7374 6174  d = result["stat
-00008ca0: 7573 225d 203d 3d20 2253 544f 5050 4544  us"] == "STOPPED
-00008cb0: 220a 2020 2020 2020 2020 6966 2073 746f  ".        if sto
-00008cc0: 7070 6564 3a0a 2020 2020 2020 2020 2020  pped:.          
-00008cd0: 2020 7265 7375 6c74 5b22 7265 7375 6c74    result["result
-00008ce0: 225d 203d 2064 6963 7428 290a 2020 2020  "] = dict().    
-00008cf0: 2020 2020 2020 2020 7265 7375 6c74 5b22          result["
-00008d00: 7265 7375 6c74 225d 5b22 6572 726f 725f  result"]["error_
-00008d10: 6d73 6722 5d20 3d20 6572 726f 725f 6d73  msg"] = error_ms
-00008d20: 670a 2020 2020 2020 2020 2020 2020 7265  g.            re
-00008d30: 7475 726e 2072 6573 756c 740a 2020 2020  turn result.    
-00008d40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008d50: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
-00008d60: 7074 696f 6e28 2255 6e61 626c 6520 746f  ption("Unable to
-00008d70: 2073 746f 7020 7665 7269 6669 6361 7469   stop verificati
-00008d80: 6f6e 2074 6173 6b22 290a 0a20 2020 2072  on task")..    r
-00008d90: 6573 756c 7420 3d20 5f70 6f73 7428 222f  esult = _post("/
-00008da0: 6261 7365 626f 782f 7265 7375 6c74 5f76  basebox/result_v
-00008db0: 6572 6966 7922 2c20 6461 7461 3d7b 2274  erify", data={"t
-00008dc0: 6173 6b5f 6964 223a 2074 6173 6b5f 6964  ask_id": task_id
-00008dd0: 7d29 0a20 2020 2072 6573 756c 742e 7261  }).    result.ra
-00008de0: 6973 655f 666f 725f 7374 6174 7573 2829  ise_for_status()
-00008df0: 0a20 2020 2072 6573 756c 7420 3d20 7265  .    result = re
-00008e00: 7375 6c74 2e6a 736f 6e28 290a 0a20 2020  sult.json()..   
-00008e10: 2073 7563 6365 7373 203d 2072 6573 756c   success = resul
-00008e20: 745b 2273 7461 7475 7322 5d20 3d3d 2022  t["status"] == "
-00008e30: 4649 4e49 5348 4544 2220 616e 6420 7265  FINISHED" and re
-00008e40: 7375 6c74 5b22 7265 7375 6c74 225d 5b22  sult["result"]["
-00008e50: 7375 6363 6573 7322 5d20 6973 2054 7275  success"] is Tru
-00008e60: 650a 0a20 2020 2069 6620 6e6f 7420 7375  e..    if not su
-00008e70: 6363 6573 733a 0a20 2020 2020 2020 2065  ccess:.        e
-00008e80: 7272 6f72 5f6d 7367 203d 2072 6573 756c  rror_msg = resul
-00008e90: 745b 2272 6573 756c 7422 5d5b 2265 7272  t["result"]["err
-00008ea0: 6f72 5f6d 7367 225d 0a20 2020 2020 2020  or_msg"].       
-00008eb0: 206c 6f67 6765 722e 6572 726f 7228 0a20   logger.error(. 
-00008ec0: 2020 2020 2020 2020 2020 2066 225b 2d5d             f"[-]
-00008ed0: 2054 6865 2062 6173 6562 6f78 2076 6572   The basebox ver
-00008ee0: 6966 6963 6174 696f 6e20 7761 7320 6578  ification was ex
-00008ef0: 6563 7574 6564 2077 6974 6820 6572 726f  ecuted with erro
-00008f00: 723a 207b 6572 726f 725f 6d73 677d 220a  r: {error_msg}".
-00008f10: 2020 2020 2020 2020 290a 0a20 2020 2072          )..    r
-00008f20: 6574 7572 6e20 7265 7375 6c74 0a0a 0a64  eturn result...d
-00008f30: 6566 205f 5f77 6169 745f 666f 725f 7468  ef __wait_for_th
-00008f40: 655f 6f70 6572 6174 696f 6e5f 746f 5f73  e_operation_to_s
-00008f50: 7461 7274 2874 6173 6b5f 6964 3a20 7374  tart(task_id: st
-00008f60: 7229 202d 3e20 626f 6f6c 3a0a 2020 2020  r) -> bool:.    
-00008f70: 2222 220a 2020 2020 5761 6974 2066 6f72  """.    Wait for
-00008f80: 2061 2074 6173 6b20 746f 2073 7461 7274   a task to start
-00008f90: 0a20 2020 203a 7061 7261 6d20 7461 736b  .    :param task
-00008fa0: 5f69 643a 2074 6865 2074 6173 6b20 6964  _id: the task id
-00008fb0: 0a20 2020 203a 7265 7475 726e 3a20 4973  .    :return: Is
-00008fc0: 2074 6865 2074 6173 6b20 7275 6e6e 696e   the task runnin
-00008fd0: 670a 2020 2020 2222 220a 0a20 2020 2072  g.    """..    r
-00008fe0: 756e 6e69 6e67 203d 2046 616c 7365 0a20  unning = False. 
-00008ff0: 2020 2074 696d 656f 7574 203d 2031 300a     timeout = 10.
-00009000: 2020 2020 7374 6172 745f 7469 6d65 203d      start_time =
-00009010: 2074 696d 652e 7469 6d65 2829 0a20 2020   time.time().   
-00009020: 2077 6869 6c65 206e 6f74 2028 7275 6e6e   while not (runn
-00009030: 696e 6720 6f72 2028 7469 6d65 2e74 696d  ing or (time.tim
-00009040: 6528 2920 2d20 7374 6172 745f 7469 6d65  e() - start_time
-00009050: 2920 3e20 7469 6d65 6f75 7429 3a0a 2020  ) > timeout):.  
-00009060: 2020 2020 2020 7265 7375 6c74 203d 205f        result = _
-00009070: 706f 7374 2822 2f62 6173 6562 6f78 2f73  post("/basebox/s
-00009080: 7461 7475 735f 7665 7269 6679 222c 2064  tatus_verify", d
-00009090: 6174 613d 7b22 7461 736b 5f69 6422 3a20  ata={"task_id": 
-000090a0: 7461 736b 5f69 647d 290a 2020 2020 2020  task_id}).      
-000090b0: 2020 7265 7375 6c74 2e72 6169 7365 5f66    result.raise_f
-000090c0: 6f72 5f73 7461 7475 7328 290a 2020 2020  or_status().    
-000090d0: 2020 2020 7265 7375 6c74 203d 2072 6573      result = res
-000090e0: 756c 742e 6a73 6f6e 2829 0a20 2020 2020  ult.json().     
-000090f0: 2020 2072 756e 6e69 6e67 203d 2072 6573     running = res
+000042e0: 2020 2066 2754 6865 2070 726f 7669 6465     f'The provide
+000042f0: 6420 7265 736f 7572 6365 7320 7061 7468  d resources path
+00004300: 2063 6f6e 7461 696e 7320 756e 7265 6164   contains unread
+00004310: 6162 6c65 2066 696c 6573 3a20 227b 7265  able files: "{re
+00004320: 736f 7572 6365 735f 7061 7468 7d22 270a  sources_path}"'.
+00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004340: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00004350: 7475 726e 2046 616c 7365 0a20 2020 2072  turn False.    r
+00004360: 6574 7572 6e20 5472 7565 0a0a 0a64 6566  eturn True...def
+00004370: 205f 6e6f 726d 616c 697a 655f 7369 6d75   _normalize_simu
+00004380: 6c61 7469 6f6e 5f72 6573 6f75 7263 655f  lation_resource_
+00004390: 7061 7468 7328 0a20 2020 2074 6f70 6f6c  paths(.    topol
+000043a0: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
+000043b0: 7468 733a 204f 7074 696f 6e61 6c5b 4c69  ths: Optional[Li
+000043c0: 7374 5b50 6174 685d 5d20 3d20 4e6f 6e65  st[Path]] = None
+000043d0: 2c0a 2920 2d3e 204c 6973 745b 5061 7468  ,.) -> List[Path
+000043e0: 5d3a 0a20 2020 2022 2222 4e6f 726d 616c  ]:.    """Normal
+000043f0: 697a 6520 7369 6d75 6c61 7469 6f6e 2072  ize simulation r
+00004400: 6573 6f75 7263 6520 7061 7468 732e 2e0a  esource paths...
+00004410: 0a20 2020 203a 7265 7475 726e 3a20 5468  .    :return: Th
+00004420: 6520 6e6f 726d 616c 697a 6564 2070 6174  e normalized pat
+00004430: 6873 2e0a 2020 2020 3a72 7479 7065 3a20  hs..    :rtype: 
+00004440: 3a63 6c61 7373 3a60 4c69 7374 5b73 7472  :class:`List[str
+00004450: 5d60 0a0a 2020 2020 3a70 6172 616d 2074  ]`..    :param t
+00004460: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
+00004470: 735f 7061 7468 733a 2054 6865 2070 6174  s_paths: The pat
+00004480: 6820 746f 2072 6573 6f75 7263 6573 2074  h to resources t
+00004490: 6861 7420 7769 6c6c 2062 6520 7075 7368  hat will be push
+000044a0: 6564 2069 6e74 6f20 636f 6d70 6174 6962  ed into compatib
+000044b0: 6c65 206e 6f64 6573 2e0a 2020 2020 3a74  le nodes..    :t
+000044c0: 7970 6520 746f 706f 6c6f 6779 5f72 6573  ype topology_res
+000044d0: 6f75 7263 6573 5f70 6174 6873 3a20 3a63  ources_paths: :c
+000044e0: 6c61 7373 3a60 6c69 7374 602c 206f 7074  lass:`list`, opt
+000044f0: 696f 6e61 6c0a 0a20 2020 2022 2222 0a20  ional..    """. 
+00004500: 2020 2069 6620 746f 706f 6c6f 6779 5f72     if topology_r
+00004510: 6573 6f75 7263 6573 5f70 6174 6873 2069  esources_paths i
+00004520: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00004530: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
+00004540: 6573 5f70 6174 6873 203d 205b 5d0a 0a20  es_paths = [].. 
+00004550: 2020 206e 6f72 6d61 6c69 7a65 645f 7061     normalized_pa
+00004560: 7468 7320 3d20 5b5d 0a20 2020 2066 6f72  ths = [].    for
+00004570: 2072 6573 6f75 7263 6520 696e 2074 6f70   resource in top
+00004580: 6f6c 6f67 795f 7265 736f 7572 6365 735f  ology_resources_
+00004590: 7061 7468 733a 0a20 2020 2020 2020 2072  paths:.        r
+000045a0: 6573 6f75 7263 6520 3d20 6f73 2e70 6174  esource = os.pat
+000045b0: 682e 6e6f 726d 7061 7468 2872 6573 6f75  h.normpath(resou
+000045c0: 7263 6529 0a20 2020 2020 2020 2023 2052  rce).        # R
+000045d0: 656d 6f76 696e 6720 7472 6169 6c69 6e67  emoving trailing
+000045e0: 2073 6c61 7368 6573 2062 6563 6175 7365   slashes because
+000045f0: 2074 6865 7920 6172 6520 6967 6e6f 7265   they are ignore
+00004600: 6420 6279 205a 6970 4669 6c65 0a20 2020  d by ZipFile.   
+00004610: 2020 2020 2069 6620 7265 736f 7572 6365       if resource
+00004620: 2e65 6e64 7377 6974 6828 222f 2229 3a0a  .endswith("/"):.
+00004630: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+00004640: 7572 6365 203d 2072 6573 6f75 7263 655b  urce = resource[
+00004650: 3a3a 2d31 5d0a 2020 2020 2020 2020 6e6f  ::-1].        no
+00004660: 726d 616c 697a 6564 5f70 6174 6873 2e61  rmalized_paths.a
+00004670: 7070 656e 6428 7265 736f 7572 6365 290a  ppend(resource).
+00004680: 2020 2020 746f 706f 6c6f 6779 5f72 6573      topology_res
+00004690: 6f75 7263 6573 5f70 6174 6873 203d 206e  ources_paths = n
+000046a0: 6f72 6d61 6c69 7a65 645f 7061 7468 730a  ormalized_paths.
+000046b0: 0a20 2020 2072 6574 7572 6e20 746f 706f  .    return topo
+000046c0: 6c6f 6779 5f72 6573 6f75 7263 6573 5f70  logy_resources_p
+000046d0: 6174 6873 0a0a 0a64 6566 205f 6e6f 726d  aths...def _norm
+000046e0: 616c 697a 655f 7369 6d75 6c61 7469 6f6e  alize_simulation
+000046f0: 5f72 6573 6f75 7263 6573 280a 2020 2020  _resources(.    
+00004700: 746f 706f 6c6f 6779 5f63 6f6e 7465 6e74  topology_content
+00004710: 3a20 4469 6374 5b73 7472 2c20 416e 795d  : Dict[str, Any]
+00004720: 203d 204e 6f6e 652c 0a20 2020 2074 6f70   = None,.    top
+00004730: 6f6c 6f67 795f 7265 736f 7572 6365 735f  ology_resources_
+00004740: 7061 7468 733a 204f 7074 696f 6e61 6c5b  paths: Optional[
+00004750: 4c69 7374 5b50 6174 685d 5d20 3d20 4e6f  List[Path]] = No
+00004760: 6e65 2c0a 2920 2d3e 2044 6963 745b 7374  ne,.) -> Dict[st
+00004770: 722c 2041 6e79 5d3a 0a20 2020 2022 2222  r, Any]:.    """
+00004780: 4372 6561 7465 2061 206e 6577 2073 696d  Create a new sim
+00004790: 756c 6174 696f 6e20 6d6f 6465 6c20 696e  ulation model in
+000047a0: 2064 6174 6162 6173 6520 6261 7365 6420   database based 
+000047b0: 6f6e 2074 6865 2070 726f 7669 6465 6420  on the provided 
+000047c0: 746f 706f 6c6f 6779 2c20 616c 6f6e 6720  topology, along 
+000047d0: 7769 7468 206f 7074 696f 6e61 6c20 7265  with optional re
+000047e0: 736f 7572 6365 2066 696c 6573 2e0a 0a20  source files... 
+000047f0: 2020 203a 7265 7475 726e 3a20 4120 7475     :return: A tu
+00004800: 706c 6520 636f 6e74 6169 6e69 6e67 2074  ple containing t
+00004810: 6865 2049 4420 6f66 2074 6865 2063 7265  he ID of the cre
+00004820: 6174 6564 2073 696d 756c 6174 696f 6e2c  ated simulation,
+00004830: 2061 6e64 2074 6865 206e 6577 206e 6f64   and the new nod
+00004840: 6573 206f 6620 7468 6520 7369 6d75 6c61  es of the simula
+00004850: 7469 6f6e 2e0a 2020 2020 3a72 7479 7065  tion..    :rtype
+00004860: 3a20 3a63 6c61 7373 3a60 5475 706c 655b  : :class:`Tuple[
+00004870: 696e 742c 204c 6973 745b 7374 725d 5d60  int, List[str]]`
+00004880: 0a0a 2020 2020 3a70 6172 616d 2074 6f70  ..    :param top
+00004890: 6f6c 6f67 795f 636f 6e74 656e 743a 2041  ology_content: A
+000048a0: 2064 6963 7420 636f 6e74 6169 6e69 6e67   dict containing
+000048b0: 2074 6865 206e 6f64 6573 2061 6e64 206e   the nodes and n
+000048c0: 6574 776f 726b 2074 6f70 6f6c 6f67 7920  etwork topology 
+000048d0: 746f 2063 7265 6174 652e 0a20 2020 203a  to create..    :
+000048e0: 7479 7065 2074 6f70 6f6c 6f67 795f 6669  type topology_fi
+000048f0: 6c65 3a20 3a63 6c61 7373 3a60 6469 6374  le: :class:`dict
+00004900: 600a 2020 2020 3a70 6172 616d 2074 6f70  `.    :param top
+00004910: 6f6c 6f67 795f 7265 736f 7572 6365 735f  ology_resources_
+00004920: 7061 7468 733a 2054 6865 2070 6174 6820  paths: The path 
+00004930: 746f 2072 6573 6f75 7263 6573 2074 6861  to resources tha
+00004940: 7420 7769 6c6c 2062 6520 7075 7368 6564  t will be pushed
+00004950: 2069 6e74 6f20 636f 6d70 6174 6962 6c65   into compatible
+00004960: 206e 6f64 6573 2e0a 2020 2020 3a74 7970   nodes..    :typ
+00004970: 6520 746f 706f 6c6f 6779 5f72 6573 6f75  e topology_resou
+00004980: 7263 6573 5f70 6174 6873 3a20 3a63 6c61  rces_paths: :cla
+00004990: 7373 3a60 6c69 7374 602c 206f 7074 696f  ss:`list`, optio
+000049a0: 6e61 6c0a 0a20 2020 2022 2222 0a0a 2020  nal..    """..  
+000049b0: 2020 6966 2022 6e61 6d65 2220 6e6f 7420    if "name" not 
+000049c0: 696e 2074 6f70 6f6c 6f67 795f 636f 6e74  in topology_cont
+000049d0: 656e 743a 0a20 2020 2020 2020 206e 616d  ent:.        nam
+000049e0: 6520 3d20 2254 6f70 6f6c 6f67 7922 0a20  e = "Topology". 
+000049f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00004a00: 206e 616d 6520 3d20 746f 706f 6c6f 6779   name = topology
+00004a10: 5f63 6f6e 7465 6e74 5b22 6e61 6d65 225d  _content["name"]
+00004a20: 0a0a 2020 2020 6966 2022 6e6f 6465 7322  ..    if "nodes"
+00004a30: 206e 6f74 2069 6e20 746f 706f 6c6f 6779   not in topology
+00004a40: 5f63 6f6e 7465 6e74 3a0a 2020 2020 2020  _content:.      
+00004a50: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+00004a60: 6e28 0a20 2020 2020 2020 2020 2020 2022  n(.            "
+00004a70: 5468 6572 6520 7368 6f75 6c64 2062 6520  There should be 
+00004a80: 6120 276e 6f64 6573 2720 7374 7275 6374  a 'nodes' struct
+00004a90: 7572 6520 696e 2074 6865 2059 414d 4c20  ure in the YAML 
+00004aa0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00004ab0: 6c65 220a 2020 2020 2020 2020 290a 0a20  le".        ).. 
+00004ac0: 2020 2069 6620 226c 696e 6b73 2220 6e6f     if "links" no
+00004ad0: 7420 696e 2074 6f70 6f6c 6f67 795f 636f  t in topology_co
+00004ae0: 6e74 656e 743a 0a20 2020 2020 2020 2072  ntent:.        r
+00004af0: 6169 7365 2045 7863 6570 7469 6f6e 280a  aise Exception(.
+00004b00: 2020 2020 2020 2020 2020 2020 2254 6865              "The
+00004b10: 7265 2073 686f 756c 6420 6265 2061 2027  re should be a '
+00004b20: 6c69 6e6b 7327 2073 7472 7563 7475 7265  links' structure
+00004b30: 2069 6e20 7468 6520 5941 4d4c 2063 6f6e   in the YAML con
+00004b40: 6669 6775 7261 7469 6f6e 2066 696c 6522  figuration file"
+00004b50: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00004b60: 7265 7175 6972 6564 203d 205b 2273 7769  required = ["swi
+00004b70: 7463 6822 2c20 226e 6f64 6522 2c20 2270  tch", "node", "p
+00004b80: 6172 616d 7322 5d0a 2020 2020 666f 7220  arams"].    for 
+00004b90: 6c69 6e6b 2069 6e20 746f 706f 6c6f 6779  link in topology
+00004ba0: 5f63 6f6e 7465 6e74 5b22 6c69 6e6b 7322  _content["links"
+00004bb0: 5d3a 0a20 2020 2020 2020 2066 6f72 2072  ]:.        for r
+00004bc0: 6571 2069 6e20 7265 7175 6972 6564 3a0a  eq in required:.
+00004bd0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00004be0: 6571 206e 6f74 2069 6e20 6c69 6e6b 3a0a  eq not in link:.
+00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c00: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+00004c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004c20: 2020 2020 2066 2254 6865 7265 2073 686f       f"There sho
+00004c30: 756c 6420 6265 2061 2027 7b72 6571 7d27  uld be a '{req}'
+00004c40: 2070 6172 616d 6574 6572 2066 6f72 2065   parameter for e
+00004c50: 7665 7279 2069 7465 6d20 6f66 2027 6c69  very item of 'li
+00004c60: 6e6b 7327 2069 6e20 7468 6520 5941 4d4c  nks' in the YAML
+00004c70: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00004c80: 696c 6522 0a20 2020 2020 2020 2020 2020  ile".           
+00004c90: 2020 2020 2029 0a0a 2020 2020 5f73 696d       )..    _sim
+00004ca0: 755f 6372 6561 7465 5f61 6464 5f69 6d70  u_create_add_imp
+00004cb0: 6c69 6369 745f 746f 706f 5f70 6172 616d  licit_topo_param
+00004cc0: 6574 6572 7328 746f 706f 6c6f 6779 5f63  eters(topology_c
+00004cd0: 6f6e 7465 6e74 290a 0a20 2020 2073 696d  ontent)..    sim
+00004ce0: 756c 6174 696f 6e5f 6469 6374 203d 207b  ulation_dict = {
+00004cf0: 226e 616d 6522 3a20 6e61 6d65 2c20 226e  "name": name, "n
+00004d00: 6574 776f 726b 223a 2074 6f70 6f6c 6f67  etwork": topolog
+00004d10: 795f 636f 6e74 656e 742c 2022 7265 736f  y_content, "reso
+00004d20: 7572 6365 735f 7061 7468 7322 3a20 5b5d  urces_paths": []
+00004d30: 7d0a 0a20 2020 2023 204e 6f72 6d61 6c69  }..    # Normali
+00004d40: 7a65 2074 6865 2072 6573 6f75 7263 6573  ze the resources
+00004d50: 2070 6174 6873 0a20 2020 2074 6f70 6f6c   paths.    topol
+00004d60: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
+00004d70: 7468 7320 3d20 5f6e 6f72 6d61 6c69 7a65  ths = _normalize
+00004d80: 5f73 696d 756c 6174 696f 6e5f 7265 736f  _simulation_reso
+00004d90: 7572 6365 5f70 6174 6873 280a 2020 2020  urce_paths(.    
+00004da0: 2020 2020 746f 706f 6c6f 6779 5f72 6573      topology_res
+00004db0: 6f75 7263 6573 5f70 6174 6873 0a20 2020  ources_paths.   
+00004dc0: 2029 0a0a 2020 2020 2320 5665 7269 6679   )..    # Verify
+00004dd0: 2074 6861 7420 7765 2064 6f20 6e6f 7420   that we do not 
+00004de0: 6861 7665 2074 6865 2073 616d 6520 7265  have the same re
+00004df0: 736f 7572 6365 7320 7061 7468 2069 6e20  sources path in 
+00004e00: 7468 6520 6c69 7374 0a20 2020 2069 6620  the list.    if 
+00004e10: 6c65 6e28 7365 7428 746f 706f 6c6f 6779  len(set(topology
+00004e20: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
+00004e30: 2929 2021 3d20 6c65 6e28 746f 706f 6c6f  )) != len(topolo
+00004e40: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
+00004e50: 6873 293a 0a20 2020 2020 2020 2072 6169  hs):.        rai
+00004e60: 7365 2045 7863 6570 7469 6f6e 2822 4964  se Exception("Id
+00004e70: 656e 7469 6361 6c20 7265 736f 7572 6365  entical resource
+00004e80: 7320 7061 7468 7320 6861 7665 2062 6565  s paths have bee
+00004e90: 6e20 6769 7665 6e22 290a 0a20 2020 2066  n given")..    f
+00004ea0: 6f72 2072 6573 6f75 7263 6520 696e 2074  or resource in t
+00004eb0: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
+00004ec0: 735f 7061 7468 733a 0a20 2020 2020 2020  s_paths:.       
+00004ed0: 2023 2056 616c 6964 6174 6520 7265 736f   # Validate reso
+00004ee0: 7572 6365 7320 7061 7468 0a20 2020 2020  urces path.     
+00004ef0: 2020 205f 5f76 616c 6964 6174 655f 7265     __validate_re
+00004f00: 736f 7572 6365 735f 7061 7468 2872 6573  sources_path(res
+00004f10: 6f75 7263 6529 2020 2320 7261 6973 6520  ource)  # raise 
+00004f20: 616e 2065 7863 6570 7469 6f6e 2069 6620  an exception if 
+00004f30: 696e 7661 6c69 640a 2020 2020 2020 2020  invalid.        
+00004f40: 2320 7461 6b65 2074 6865 2061 6273 6f6c  # take the absol
+00004f50: 7574 6520 7061 7468 0a20 2020 2020 2020  ute path.       
+00004f60: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
+00004f70: 5b22 7265 736f 7572 6365 735f 7061 7468  ["resources_path
+00004f80: 7322 5d2e 6170 7065 6e64 286f 732e 7061  s"].append(os.pa
+00004f90: 7468 2e61 6273 7061 7468 2872 6573 6f75  th.abspath(resou
+00004fa0: 7263 6529 290a 0a20 2020 2072 6574 7572  rce))..    retur
+00004fb0: 6e20 7369 6d75 6c61 7469 6f6e 5f64 6963  n simulation_dic
+00004fc0: 740a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  t...# ----------
+00004fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005010: 2023 0a23 2041 5049 2068 656c 7065 7273   #.# API helpers
+00005020: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .# -------------
+00005030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 230a  ------------- #.
+00005070: 0a0a 2323 230a 2320 5369 6d75 6c61 7469  ..###.# Simulati
+00005080: 6f6e 2068 656c 7065 7273 0a23 2323 0a0a  on helpers.###..
+00005090: 0a64 6566 2063 7265 6174 655f 7369 6d75  .def create_simu
+000050a0: 6c61 7469 6f6e 280a 2020 2020 746f 706f  lation(.    topo
+000050b0: 6c6f 6779 5f63 6f6e 7465 6e74 3a20 4469  logy_content: Di
+000050c0: 6374 5b73 7472 2c20 416e 795d 203d 204e  ct[str, Any] = N
+000050d0: 6f6e 652c 0a20 2020 2074 6f70 6f6c 6f67  one,.    topolog
+000050e0: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
+000050f0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+00005100: 5b50 6174 685d 5d20 3d20 4e6f 6e65 2c0a  [Path]] = None,.
+00005110: 2020 2020 616c 6c6f 6361 7469 6f6e 5f73      allocation_s
+00005120: 7472 6174 6567 793a 204f 7074 696f 6e61  trategy: Optiona
+00005130: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
+00005140: 202d 3e20 5475 706c 655b 696e 742c 204c   -> Tuple[int, L
+00005150: 6973 745b 7374 725d 5d3a 0a20 2020 2022  ist[str]]:.    "
+00005160: 2222 4372 6561 7465 2061 206e 6577 2073  ""Create a new s
+00005170: 696d 756c 6174 696f 6e20 6d6f 6465 6c20  imulation model 
+00005180: 696e 2064 6174 6162 6173 6520 6261 7365  in database base
+00005190: 6420 6f6e 2074 6865 2070 726f 7669 6465  d on the provide
+000051a0: 6420 746f 706f 6c6f 6779 2c20 616c 6f6e  d topology, alon
+000051b0: 6720 7769 7468 206f 7074 696f 6e61 6c20  g with optional 
+000051c0: 7265 736f 7572 6365 2066 696c 6573 2e0a  resource files..
+000051d0: 0a20 2020 203a 7265 7475 726e 3a20 4120  .    :return: A 
+000051e0: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
+000051f0: 2074 6865 2049 4420 6f66 2074 6865 2063   the ID of the c
+00005200: 7265 6174 6564 2073 696d 756c 6174 696f  reated simulatio
+00005210: 6e2c 2061 6e64 2074 6865 206e 6577 206e  n, and the new n
+00005220: 6f64 6573 206f 6620 7468 6520 7369 6d75  odes of the simu
+00005230: 6c61 7469 6f6e 2e0a 2020 2020 3a72 7479  lation..    :rty
+00005240: 7065 3a20 3a63 6c61 7373 3a60 5475 706c  pe: :class:`Tupl
+00005250: 655b 696e 742c 204c 6973 745b 7374 725d  e[int, List[str]
+00005260: 5d60 0a0a 2020 2020 3a70 6172 616d 2074  ]`..    :param t
+00005270: 6f70 6f6c 6f67 795f 636f 6e74 656e 743a  opology_content:
+00005280: 2041 2064 6963 7420 636f 6e74 6169 6e69   A dict containi
+00005290: 6e67 2074 6865 206e 6f64 6573 2061 6e64  ng the nodes and
+000052a0: 206e 6574 776f 726b 2074 6f70 6f6c 6f67   network topolog
+000052b0: 7920 746f 2063 7265 6174 652e 0a20 2020  y to create..   
+000052c0: 203a 7479 7065 2074 6f70 6f6c 6f67 795f   :type topology_
+000052d0: 6669 6c65 3a20 3a63 6c61 7373 3a60 6469  file: :class:`di
+000052e0: 6374 600a 2020 2020 3a70 6172 616d 2074  ct`.    :param t
+000052f0: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
+00005300: 735f 7061 7468 733a 2054 6865 2070 6174  s_paths: The pat
+00005310: 6820 746f 2072 6573 6f75 7263 6573 2074  h to resources t
+00005320: 6861 7420 7769 6c6c 2062 6520 7075 7368  hat will be push
+00005330: 6564 2069 6e74 6f20 636f 6d70 6174 6962  ed into compatib
+00005340: 6c65 206e 6f64 6573 2e0a 2020 2020 3a74  le nodes..    :t
+00005350: 7970 6520 746f 706f 6c6f 6779 5f72 6573  ype topology_res
+00005360: 6f75 7263 6573 5f70 6174 6873 3a20 3a63  ources_paths: :c
+00005370: 6c61 7373 3a60 6c69 7374 602c 206f 7074  lass:`list`, opt
+00005380: 696f 6e61 6c0a 2020 2020 3a70 6172 616d  ional.    :param
+00005390: 2061 6c6c 6f63 6174 696f 6e5f 7374 7261   allocation_stra
+000053a0: 7465 6779 3a20 4e61 6d65 206f 6620 7468  tegy: Name of th
+000053b0: 6520 616c 6c6f 6361 7469 6f6e 2073 7472  e allocation str
+000053c0: 6174 6567 7920 746f 2075 7365 2074 6f20  ategy to use to 
+000053d0: 616c 6c6f 6361 7465 206e 6f64 6573 2074  allocate nodes t
+000053e0: 6f20 636f 6d70 7574 6520 7365 7276 6572  o compute server
+000053f0: 732e 0a20 2020 203a 7479 7065 2061 6c6c  s..    :type all
+00005400: 6f63 6174 696f 6e5f 7374 7261 7465 6779  ocation_strategy
+00005410: 3a20 3a63 6c61 7373 3a60 7374 7260 2c20  : :class:`str`, 
+00005420: 6f70 7469 6f6e 616c 0a0a 2020 2020 2222  optional..    ""
+00005430: 220a 0a20 2020 2073 696d 756c 6174 696f  "..    simulatio
+00005440: 6e5f 6469 6374 203d 205f 6e6f 726d 616c  n_dict = _normal
+00005450: 697a 655f 7369 6d75 6c61 7469 6f6e 5f72  ize_simulation_r
+00005460: 6573 6f75 7263 6573 280a 2020 2020 2020  esources(.      
+00005470: 2020 746f 706f 6c6f 6779 5f63 6f6e 7465    topology_conte
+00005480: 6e74 3d74 6f70 6f6c 6f67 795f 636f 6e74  nt=topology_cont
+00005490: 656e 742c 0a20 2020 2020 2020 2074 6f70  ent,.        top
+000054a0: 6f6c 6f67 795f 7265 736f 7572 6365 735f  ology_resources_
+000054b0: 7061 7468 733d 746f 706f 6c6f 6779 5f72  paths=topology_r
+000054c0: 6573 6f75 7263 6573 5f70 6174 6873 2c0a  esources_paths,.
+000054d0: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
+000054e0: 6e20 5f63 7265 6174 655f 6f72 5f65 7874  n _create_or_ext
+000054f0: 656e 645f 7369 6d75 6c61 7469 6f6e 280a  end_simulation(.
+00005500: 2020 2020 2020 2020 7369 6d75 6c61 7469          simulati
+00005510: 6f6e 5f64 6963 743d 7369 6d75 6c61 7469  on_dict=simulati
+00005520: 6f6e 5f64 6963 742c 2061 6c6c 6f63 6174  on_dict, allocat
+00005530: 696f 6e5f 7374 7261 7465 6779 3d61 6c6c  ion_strategy=all
+00005540: 6f63 6174 696f 6e5f 7374 7261 7465 6779  ocation_strategy
+00005550: 0a20 2020 2029 0a0a 0a64 6566 2065 7874  .    )...def ext
+00005560: 656e 645f 7369 6d75 6c61 7469 6f6e 280a  end_simulation(.
+00005570: 2020 2020 746f 706f 6c6f 6779 5f63 6f6e      topology_con
+00005580: 7465 6e74 3a20 4469 6374 5b73 7472 2c20  tent: Dict[str, 
+00005590: 416e 795d 203d 204e 6f6e 652c 0a20 2020  Any] = None,.   
+000055a0: 2074 6f70 6f6c 6f67 795f 7265 736f 7572   topology_resour
+000055b0: 6365 735f 7061 7468 733a 204f 7074 696f  ces_paths: Optio
+000055c0: 6e61 6c5b 4c69 7374 5b50 6174 685d 5d20  nal[List[Path]] 
+000055d0: 3d20 4e6f 6e65 2c0a 2020 2020 616c 6c6f  = None,.    allo
+000055e0: 6361 7469 6f6e 5f73 7472 6174 6567 793a  cation_strategy:
+000055f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00005600: 204e 6f6e 652c 0a20 2020 2069 645f 7369   None,.    id_si
+00005610: 6d75 6c61 7469 6f6e 3a20 696e 7420 3d20  mulation: int = 
+00005620: 4e6f 6e65 2c0a 2920 2d3e 2054 7570 6c65  None,.) -> Tuple
+00005630: 5b69 6e74 2c20 4c69 7374 5b73 7472 5d5d  [int, List[str]]
+00005640: 3a0a 2020 2020 2222 2245 7874 656e 6420  :.    """Extend 
+00005650: 616e 2065 7869 7374 696e 6720 7369 6d75  an existing simu
+00005660: 6c61 7469 6f6e 206d 6f64 656c 2069 6e20  lation model in 
+00005670: 6461 7461 6261 7365 2062 6173 6564 206f  database based o
+00005680: 6e20 7468 6520 7072 6f76 6964 6564 2074  n the provided t
+00005690: 6f70 6f6c 6f67 792c 2061 6c6f 6e67 2077  opology, along w
+000056a0: 6974 6820 6f70 7469 6f6e 616c 2072 6573  ith optional res
+000056b0: 6f75 7263 6520 6669 6c65 732e 0a0a 2020  ource files...  
+000056c0: 2020 3a72 6574 7572 6e3a 2041 2074 7570    :return: A tup
+000056d0: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
+000056e0: 6520 4944 206f 6620 7468 6520 6372 6561  e ID of the crea
+000056f0: 7465 6420 7369 6d75 6c61 7469 6f6e 2c20  ted simulation, 
+00005700: 616e 6420 7468 6520 6e65 7720 6e6f 6465  and the new node
+00005710: 7320 6f66 2074 6865 2073 696d 756c 6174  s of the simulat
+00005720: 696f 6e2e 0a20 2020 203a 7274 7970 653a  ion..    :rtype:
+00005730: 203a 636c 6173 733a 6054 7570 6c65 5b69   :class:`Tuple[i
+00005740: 6e74 2c20 4c69 7374 5b73 7472 5d5d 600a  nt, List[str]]`.
+00005750: 0a20 2020 203a 7061 7261 6d20 746f 706f  .    :param topo
+00005760: 6c6f 6779 5f63 6f6e 7465 6e74 3a20 4120  logy_content: A 
+00005770: 6469 6374 2063 6f6e 7461 696e 696e 6720  dict containing 
+00005780: 7468 6520 6e6f 6465 7320 616e 6420 6e65  the nodes and ne
+00005790: 7477 6f72 6b20 746f 706f 6c6f 6779 2074  twork topology t
+000057a0: 6f20 6372 6561 7465 2e0a 2020 2020 3a74  o create..    :t
+000057b0: 7970 6520 746f 706f 6c6f 6779 5f66 696c  ype topology_fil
+000057c0: 653a 203a 636c 6173 733a 6064 6963 7460  e: :class:`dict`
+000057d0: 0a20 2020 203a 7061 7261 6d20 746f 706f  .    :param topo
+000057e0: 6c6f 6779 5f72 6573 6f75 7263 6573 5f70  logy_resources_p
+000057f0: 6174 6873 3a20 5468 6520 7061 7468 2074  aths: The path t
+00005800: 6f20 7265 736f 7572 6365 7320 7468 6174  o resources that
+00005810: 2077 696c 6c20 6265 2070 7573 6865 6420   will be pushed 
+00005820: 696e 746f 2063 6f6d 7061 7469 626c 6520  into compatible 
+00005830: 6e6f 6465 732e 0a20 2020 203a 7479 7065  nodes..    :type
+00005840: 2074 6f70 6f6c 6f67 795f 7265 736f 7572   topology_resour
+00005850: 6365 735f 7061 7468 733a 203a 636c 6173  ces_paths: :clas
+00005860: 733a 606c 6973 7460 2c20 6f70 7469 6f6e  s:`list`, option
+00005870: 616c 0a20 2020 203a 7061 7261 6d20 616c  al.    :param al
+00005880: 6c6f 6361 7469 6f6e 5f73 7472 6174 6567  location_strateg
+00005890: 793a 204e 616d 6520 6f66 2074 6865 2061  y: Name of the a
+000058a0: 6c6c 6f63 6174 696f 6e20 7374 7261 7465  llocation strate
+000058b0: 6779 2074 6f20 7573 6520 746f 2061 6c6c  gy to use to all
+000058c0: 6f63 6174 6520 6e6f 6465 7320 746f 2063  ocate nodes to c
+000058d0: 6f6d 7075 7465 2073 6572 7665 7273 2e0a  ompute servers..
+000058e0: 2020 2020 3a74 7970 6520 616c 6c6f 6361      :type alloca
+000058f0: 7469 6f6e 5f73 7472 6174 6567 793a 203a  tion_strategy: :
+00005900: 636c 6173 733a 6073 7472 602c 206f 7074  class:`str`, opt
+00005910: 696f 6e61 6c0a 2020 2020 3a70 6172 616d  ional.    :param
+00005920: 2069 645f 7369 6d75 6c61 7469 6f6e 3a20   id_simulation: 
+00005930: 5468 6520 7369 6d75 6c61 7469 6f6e 2049  The simulation I
+00005940: 442c 2077 6865 6e20 6578 7465 6e64 696e  D, when extendin
+00005950: 6720 616e 2065 7869 7374 696e 6720 7369  g an existing si
+00005960: 6d75 6c61 7469 6f6e 2077 6974 6820 6e65  mulation with ne
+00005970: 7720 6e6f 6465 7320 616e 6420 6c69 6e6b  w nodes and link
+00005980: 732e 0a20 2020 203a 7479 7065 2069 645f  s..    :type id_
+00005990: 7369 6d75 6c61 7469 6f6e 3a20 3a63 6c61  simulation: :cla
+000059a0: 7373 3a60 696e 7460 2c20 6f70 7469 6f6e  ss:`int`, option
+000059b0: 616c 0a0a 2020 2020 2222 220a 0a20 2020  al..    """..   
+000059c0: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
+000059d0: 203d 205f 6e6f 726d 616c 697a 655f 7369   = _normalize_si
+000059e0: 6d75 6c61 7469 6f6e 5f72 6573 6f75 7263  mulation_resourc
+000059f0: 6573 280a 2020 2020 2020 2020 746f 706f  es(.        topo
+00005a00: 6c6f 6779 5f63 6f6e 7465 6e74 3d74 6f70  logy_content=top
+00005a10: 6f6c 6f67 795f 636f 6e74 656e 742c 0a20  ology_content,. 
+00005a20: 2020 2020 2020 2074 6f70 6f6c 6f67 795f         topology_
+00005a30: 7265 736f 7572 6365 735f 7061 7468 733d  resources_paths=
+00005a40: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
+00005a50: 6573 5f70 6174 6873 2c0a 2020 2020 290a  es_paths,.    ).
+00005a60: 0a20 2020 2072 6574 7572 6e20 5f63 7265  .    return _cre
+00005a70: 6174 655f 6f72 5f65 7874 656e 645f 7369  ate_or_extend_si
+00005a80: 6d75 6c61 7469 6f6e 280a 2020 2020 2020  mulation(.      
+00005a90: 2020 7369 6d75 6c61 7469 6f6e 5f64 6963    simulation_dic
+00005aa0: 743d 7369 6d75 6c61 7469 6f6e 5f64 6963  t=simulation_dic
+00005ab0: 742c 0a20 2020 2020 2020 2069 645f 7369  t,.        id_si
+00005ac0: 6d75 6c61 7469 6f6e 3d69 645f 7369 6d75  mulation=id_simu
+00005ad0: 6c61 7469 6f6e 2c0a 2020 2020 2020 2020  lation,.        
+00005ae0: 616c 6c6f 6361 7469 6f6e 5f73 7472 6174  allocation_strat
+00005af0: 6567 793d 616c 6c6f 6361 7469 6f6e 5f73  egy=allocation_s
+00005b00: 7472 6174 6567 792c 0a20 2020 2029 0a0a  trategy,.    )..
+00005b10: 0a64 6566 2063 7265 6174 655f 7369 6d75  .def create_simu
+00005b20: 6c61 7469 6f6e 5f66 726f 6d5f 746f 706f  lation_from_topo
+00005b30: 6c6f 6779 280a 2020 2020 746f 706f 6c6f  logy(.    topolo
+00005b40: 6779 5f66 696c 653a 2073 7472 203d 204e  gy_file: str = N
+00005b50: 6f6e 652c 0a20 2020 2074 6f70 6f6c 6f67  one,.    topolog
+00005b60: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
+00005b70: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+00005b80: 5b50 6174 685d 5d20 3d20 4e6f 6e65 2c0a  [Path]] = None,.
+00005b90: 2020 2020 616c 6c6f 6361 7469 6f6e 5f73      allocation_s
+00005ba0: 7472 6174 6567 793a 204f 7074 696f 6e61  trategy: Optiona
+00005bb0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
+00005bc0: 202d 3e20 5475 706c 655b 696e 742c 204c   -> Tuple[int, L
+00005bd0: 6973 745b 7374 725d 5d3a 0a20 2020 2022  ist[str]]:.    "
+00005be0: 2222 4372 6561 7465 2061 206e 6577 2073  ""Create a new s
+00005bf0: 696d 756c 6174 696f 6e20 6d6f 6465 6c20  imulation model 
+00005c00: 696e 2064 6174 6162 6173 6520 6261 7365  in database base
+00005c10: 6420 6f6e 2074 6865 2070 726f 7669 6465  d on the provide
+00005c20: 6420 746f 706f 6c6f 6779 2066 696c 652c  d topology file,
+00005c30: 2061 6c6f 6e67 2077 6974 6820 6f70 7469   along with opti
+00005c40: 6f6e 616c 2072 6573 6f75 7263 6520 6669  onal resource fi
+00005c50: 6c65 732e 0a0a 2020 2020 3a72 6574 7572  les...    :retur
+00005c60: 6e3a 2041 2074 7570 6c65 2063 6f6e 7461  n: A tuple conta
+00005c70: 696e 696e 6720 7468 6520 4944 206f 6620  ining the ID of 
+00005c80: 7468 6520 6372 6561 7465 6420 7369 6d75  the created simu
+00005c90: 6c61 7469 6f6e 2c20 616e 6420 7468 6520  lation, and the 
+00005ca0: 6e65 7720 6e6f 6465 7320 6f66 2074 6865  new nodes of the
+00005cb0: 2073 696d 756c 6174 696f 6e2e 0a20 2020   simulation..   
+00005cc0: 203a 7274 7970 653a 203a 636c 6173 733a   :rtype: :class:
+00005cd0: 6054 7570 6c65 5b69 6e74 2c20 4c69 7374  `Tuple[int, List
+00005ce0: 5b73 7472 5d5d 600a 0a20 2020 203a 7061  [str]]`..    :pa
+00005cf0: 7261 6d20 746f 706f 6c6f 6779 5f66 696c  ram topology_fil
+00005d00: 653a 2054 6865 2070 6174 6820 746f 2061  e: The path to a
+00005d10: 2074 6f70 6f6c 6f67 7920 6669 6c65 2063   topology file c
+00005d20: 6f6e 7461 696e 696e 6720 7468 6520 6e6f  ontaining the no
+00005d30: 6465 7320 616e 6420 6e65 7477 6f72 6b20  des and network 
+00005d40: 746f 706f 6c6f 6779 2074 6f20 6372 6561  topology to crea
+00005d50: 7465 2e0a 2020 2020 3a74 7970 6520 746f  te..    :type to
+00005d60: 706f 6c6f 6779 5f66 696c 653a 203a 636c  pology_file: :cl
+00005d70: 6173 733a 6073 7472 600a 2020 2020 3a70  ass:`str`.    :p
+00005d80: 6172 616d 2074 6f70 6f6c 6f67 795f 7265  aram topology_re
+00005d90: 736f 7572 6365 735f 7061 7468 733a 2054  sources_paths: T
+00005da0: 6865 2070 6174 6820 746f 2072 6573 6f75  he path to resou
+00005db0: 7263 6573 2074 6861 7420 7769 6c6c 2062  rces that will b
+00005dc0: 6520 7075 7368 6564 2069 6e74 6f20 636f  e pushed into co
+00005dd0: 6d70 6174 6962 6c65 206e 6f64 6573 2e0a  mpatible nodes..
+00005de0: 2020 2020 3a74 7970 6520 746f 706f 6c6f      :type topolo
+00005df0: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
+00005e00: 6873 3a20 3a63 6c61 7373 3a60 7374 7260  hs: :class:`str`
+00005e10: 2c20 6f70 7469 6f6e 616c 0a20 2020 203a  , optional.    :
+00005e20: 7061 7261 6d20 616c 6c6f 6361 7469 6f6e  param allocation
+00005e30: 5f73 7472 6174 6567 793a 204e 616d 6520  _strategy: Name 
+00005e40: 6f66 2074 6865 2061 6c6c 6f63 6174 696f  of the allocatio
+00005e50: 6e20 7374 7261 7465 6779 2074 6f20 7573  n strategy to us
+00005e60: 6520 746f 2061 6c6c 6f63 6174 6520 6e6f  e to allocate no
+00005e70: 6465 7320 746f 2063 6f6d 7075 7465 2073  des to compute s
+00005e80: 6572 7665 7273 2e0a 2020 2020 3a74 7970  ervers..    :typ
+00005e90: 6520 616c 6c6f 6361 7469 6f6e 5f73 7472  e allocation_str
+00005ea0: 6174 6567 793a 203a 636c 6173 733a 6073  ategy: :class:`s
+00005eb0: 7472 602c 206f 7074 696f 6e61 6c0a 0a20  tr`, optional.. 
+00005ec0: 2020 203e 3e3e 2066 726f 6d20 6372 5f61     >>> from cr_a
+00005ed0: 7069 5f63 6c69 656e 7420 696d 706f 7274  pi_client import
+00005ee0: 2063 6f72 655f 6170 690a 2020 2020 3e3e   core_api.    >>
+00005ef0: 3e20 636f 7265 5f61 7069 2e72 6573 6574  > core_api.reset
+00005f00: 2829 0a20 2020 2027 436f 6d70 7574 6520  ().    'Compute 
+00005f10: 696e 6672 6173 7472 7563 7475 7265 2073  infrastructure s
+00005f20: 7563 6365 7373 6675 6c6c 7920 7265 7365  uccessfully rese
+00005f30: 7427 0a20 2020 203e 3e3e 2063 6f72 655f  t'.    >>> core_
+00005f40: 6170 692e 6372 6561 7465 5f73 696d 756c  api.create_simul
+00005f50: 6174 696f 6e5f 6672 6f6d 5f74 6f70 6f6c  ation_from_topol
+00005f60: 6f67 7928 2264 6174 612f 746f 706f 6c6f  ogy("data/topolo
+00005f70: 6769 6573 2f74 6f70 6f6c 6f67 792d 312d  gies/topology-1-
+00005f80: 636c 6965 6e74 2e79 616d 6c22 290a 2020  client.yaml").  
+00005f90: 2020 2831 2c20 5b27 434c 4945 4e54 3127    (1, ['CLIENT1'
+00005fa0: 2c20 2752 6f75 7465 7231 272c 2027 5377  , 'Router1', 'Sw
+00005fb0: 6974 6368 3127 5d29 0a0a 2020 2020 2222  itch1'])..    ""
+00005fc0: 220a 0a20 2020 2069 6620 746f 706f 6c6f  "..    if topolo
+00005fd0: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
+00005fe0: 6873 2069 7320 4e6f 6e65 3a0a 2020 2020  hs is None:.    
+00005ff0: 2020 2020 746f 706f 6c6f 6779 5f72 6573      topology_res
+00006000: 6f75 7263 6573 5f70 6174 6873 203d 205b  ources_paths = [
+00006010: 5d0a 0a20 2020 2023 2043 7265 6174 6520  ]..    # Create 
+00006020: 6120 6e65 7720 7369 6d75 6c61 7469 6f6e  a new simulation
+00006030: 206d 6f64 656c 2069 6e20 6461 7461 6261   model in databa
+00006040: 7365 2062 6173 6564 206f 6e20 7468 6520  se based on the 
+00006050: 7072 6f76 6964 6564 2074 6f70 6f6c 6f67  provided topolog
+00006060: 7920 6669 6c65 2070 6174 682e 2222 220a  y file path.""".
+00006070: 2020 2020 6966 2074 6f70 6f6c 6f67 795f      if topology_
+00006080: 6669 6c65 2069 7320 4e6f 6e65 3a0a 2020  file is None:.  
+00006090: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+000060a0: 7074 696f 6e28 2241 6e20 746f 706f 6c6f  ption("An topolo
+000060b0: 6779 2066 696c 6520 6973 2072 6571 7569  gy file is requi
+000060c0: 7265 6422 290a 0a20 2020 2023 2056 616c  red")..    # Val
+000060d0: 6964 6174 6520 5941 4d4c 2063 6f6e 6669  idate YAML confi
+000060e0: 6775 7261 7469 6f6e 2066 696c 650a 2020  guration file.  
+000060f0: 2020 5f76 616c 6964 6174 655f 7961 6d6c    _validate_yaml
+00006100: 5f74 6f70 6f6c 6f67 795f 6669 6c65 2874  _topology_file(t
+00006110: 6f70 6f6c 6f67 795f 6669 6c65 290a 0a20  opology_file).. 
+00006120: 2020 2023 204f 7065 6e20 616e 6420 7265     # Open and re
+00006130: 6164 2059 414d 4c20 636f 6e66 6967 7572  ad YAML configur
+00006140: 6174 696f 6e20 6669 6c65 0a20 2020 2079  ation file.    y
+00006150: 616d 6c5f 636f 6e74 656e 7420 3d20 5f72  aml_content = _r
+00006160: 6561 645f 7961 6d6c 5f74 6f70 6f6c 6f67  ead_yaml_topolog
+00006170: 795f 6669 6c65 2874 6f70 6f6c 6f67 795f  y_file(topology_
+00006180: 6669 6c65 290a 0a20 2020 2023 2050 6172  file)..    # Par
+00006190: 7365 2059 414d 4c20 636f 6e66 6967 7572  se YAML configur
+000061a0: 6174 696f 6e0a 2020 2020 2320 5765 2075  ation.    # We u
+000061b0: 7365 2072 7561 6d65 6c2e 7961 6d6c 2062  se ruamel.yaml b
+000061c0: 6563 6175 7365 2069 7420 6b65 6570 7320  ecause it keeps 
+000061d0: 616e 6368 6f72 7320 616e 640a 2020 2020  anchors and.    
+000061e0: 2320 616c 6961 7365 7320 696e 206d 656d  # aliases in mem
+000061f0: 6f72 792e 2049 7420 6973 2076 6572 7920  ory. It is very 
+00006200: 636f 6e76 656e 6965 6e74 2077 6865 6e20  convenient when 
+00006210: 7468 6520 7369 6d75 6c61 7469 6f6e 0a20  the simulation. 
+00006220: 2020 2023 2069 7320 7374 6f72 6564 2f66     # is stored/f
+00006230: 6574 6368 6564 2028 7265 6665 7265 6e63  etched (referenc
+00006240: 6573 2061 7265 206b 6570 7421 290a 2020  es are kept!).  
+00006250: 2020 6c6f 6164 6572 203d 2059 414d 4c28    loader = YAML(
+00006260: 7479 703d 2272 7422 290a 2020 2020 746f  typ="rt").    to
+00006270: 706f 6c6f 6779 5f63 6f6e 7465 6e74 203d  pology_content =
+00006280: 206c 6f61 6465 722e 6c6f 6164 2879 616d   loader.load(yam
+00006290: 6c5f 636f 6e74 656e 7429 0a0a 2020 2020  l_content)..    
+000062a0: 2320 4164 6420 6120 6465 6661 756c 7420  # Add a default 
+000062b0: 7265 736f 7572 6365 7320 6469 7265 6374  resources direct
+000062c0: 6f72 7920 6966 2069 7420 6578 6973 7473  ory if it exists
+000062d0: 2e0a 2020 2020 2320 4966 2074 6865 2074  ..    # If the t
+000062e0: 6f70 6f6c 6f67 7920 6973 2022 7061 7468  opology is "path
+000062f0: 2f74 6f2f 746f 706f 2e79 616d 6c22 2c20  /to/topo.yaml", 
+00006300: 7468 6520 6465 6661 756c 7420 7265 736f  the default reso
+00006310: 7572 6365 7320 6469 7265 6374 6f72 7920  urces directory 
+00006320: 6973 2022 7061 7468 2f74 6f2f 7265 736f  is "path/to/reso
+00006330: 7572 6365 7322 2e0a 2020 2020 746f 706f  urces"..    topo
+00006340: 6c6f 6779 5f72 6573 6f75 7263 6573 5f70  logy_resources_p
+00006350: 6174 6873 203d 205f 6e6f 726d 616c 697a  aths = _normaliz
+00006360: 655f 7369 6d75 6c61 7469 6f6e 5f72 6573  e_simulation_res
+00006370: 6f75 7263 655f 7061 7468 7328 0a20 2020  ource_paths(.   
+00006380: 2020 2020 2074 6f70 6f6c 6f67 795f 7265       topology_re
+00006390: 736f 7572 6365 735f 7061 7468 730a 2020  sources_paths.  
+000063a0: 2020 290a 2020 2020 6465 6661 756c 745f    ).    default_
+000063b0: 7265 736f 7572 6365 735f 7061 7468 203d  resources_path =
+000063c0: 206f 732e 7061 7468 2e6a 6f69 6e28 6f73   os.path.join(os
+000063d0: 2e70 6174 682e 6469 726e 616d 6528 746f  .path.dirname(to
+000063e0: 706f 6c6f 6779 5f66 696c 6529 2c20 2272  pology_file), "r
+000063f0: 6573 6f75 7263 6573 2229 0a20 2020 2064  esources").    d
+00006400: 6566 6175 6c74 5f72 6573 6f75 7263 6573  efault_resources
+00006410: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+00006420: 6e6f 726d 7061 7468 2864 6566 6175 6c74  normpath(default
+00006430: 5f72 6573 6f75 7263 6573 5f70 6174 6829  _resources_path)
+00006440: 0a20 2020 2069 6620 5f5f 7661 6c69 6461  .    if __valida
+00006450: 7465 5f72 6573 6f75 7263 6573 5f70 6174  te_resources_pat
+00006460: 6828 6465 6661 756c 745f 7265 736f 7572  h(default_resour
+00006470: 6365 735f 7061 7468 2c20 4661 6c73 6529  ces_path, False)
+00006480: 3a0a 2020 2020 2020 2020 6966 2064 6566  :.        if def
+00006490: 6175 6c74 5f72 6573 6f75 7263 6573 5f70  ault_resources_p
+000064a0: 6174 6820 6e6f 7420 696e 2074 6f70 6f6c  ath not in topol
+000064b0: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
+000064c0: 7468 733a 0a20 2020 2020 2020 2020 2020  ths:.           
+000064d0: 2074 6f70 6f6c 6f67 795f 7265 736f 7572   topology_resour
+000064e0: 6365 735f 7061 7468 732e 6170 7065 6e64  ces_paths.append
+000064f0: 2864 6566 6175 6c74 5f72 6573 6f75 7263  (default_resourc
+00006500: 6573 5f70 6174 6829 0a0a 2020 2020 7265  es_path)..    re
+00006510: 7475 726e 2063 7265 6174 655f 7369 6d75  turn create_simu
+00006520: 6c61 7469 6f6e 280a 2020 2020 2020 2020  lation(.        
+00006530: 746f 706f 6c6f 6779 5f63 6f6e 7465 6e74  topology_content
+00006540: 3d74 6f70 6f6c 6f67 795f 636f 6e74 656e  =topology_conten
+00006550: 742c 0a20 2020 2020 2020 2074 6f70 6f6c  t,.        topol
+00006560: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
+00006570: 7468 733d 746f 706f 6c6f 6779 5f72 6573  ths=topology_res
+00006580: 6f75 7263 6573 5f70 6174 6873 2c0a 2020  ources_paths,.  
+00006590: 2020 2020 2020 616c 6c6f 6361 7469 6f6e        allocation
+000065a0: 5f73 7472 6174 6567 793d 616c 6c6f 6361  _strategy=alloca
+000065b0: 7469 6f6e 5f73 7472 6174 6567 792c 0a20  tion_strategy,. 
+000065c0: 2020 2029 0a0a 0a64 6566 2065 7874 656e     )...def exten
+000065d0: 645f 7369 6d75 6c61 7469 6f6e 5f66 726f  d_simulation_fro
+000065e0: 6d5f 746f 706f 6c6f 6779 280a 2020 2020  m_topology(.    
+000065f0: 746f 706f 6c6f 6779 5f66 696c 653a 2073  topology_file: s
+00006600: 7472 203d 204e 6f6e 652c 0a20 2020 2074  tr = None,.    t
+00006610: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
+00006620: 735f 7061 7468 733a 204f 7074 696f 6e61  s_paths: Optiona
+00006630: 6c5b 4c69 7374 5b50 6174 685d 5d20 3d20  l[List[Path]] = 
+00006640: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 6361  None,.    alloca
+00006650: 7469 6f6e 5f73 7472 6174 6567 793a 204f  tion_strategy: O
+00006660: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00006670: 6f6e 652c 0a20 2020 2069 645f 7369 6d75  one,.    id_simu
+00006680: 6c61 7469 6f6e 3a20 696e 7420 3d20 4e6f  lation: int = No
+00006690: 6e65 2c0a 2920 2d3e 2054 7570 6c65 5b69  ne,.) -> Tuple[i
+000066a0: 6e74 2c20 4c69 7374 5b73 7472 5d5d 3a0a  nt, List[str]]:.
+000066b0: 2020 2020 2222 2245 7874 656e 6420 616e      """Extend an
+000066c0: 2065 7869 7374 696e 6720 7369 6d75 6c61   existing simula
+000066d0: 7469 6f6e 206d 6f64 656c 2069 6e20 6461  tion model in da
+000066e0: 7461 6261 7365 2062 6173 6564 206f 6e20  tabase based on 
+000066f0: 7468 6520 7072 6f76 6964 6564 2074 6f70  the provided top
+00006700: 6f6c 6f67 7920 6669 6c65 2c20 616c 6f6e  ology file, alon
+00006710: 6720 7769 7468 206f 7074 696f 6e61 6c20  g with optional 
+00006720: 7265 736f 7572 6365 2066 696c 6573 2e0a  resource files..
+00006730: 0a20 2020 203a 7265 7475 726e 3a20 4120  .    :return: A 
+00006740: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
+00006750: 2074 6865 2049 4420 6f66 2074 6865 2063   the ID of the c
+00006760: 7265 6174 6564 2073 696d 756c 6174 696f  reated simulatio
+00006770: 6e2c 2061 6e64 2074 6865 206e 6577 206e  n, and the new n
+00006780: 6f64 6573 206f 6620 7468 6520 7369 6d75  odes of the simu
+00006790: 6c61 7469 6f6e 2e0a 2020 2020 3a72 7479  lation..    :rty
+000067a0: 7065 3a20 3a63 6c61 7373 3a60 5475 706c  pe: :class:`Tupl
+000067b0: 655b 696e 742c 204c 6973 745b 7374 725d  e[int, List[str]
+000067c0: 5d60 0a0a 2020 2020 3a70 6172 616d 2074  ]`..    :param t
+000067d0: 6f70 6f6c 6f67 795f 6669 6c65 3a20 5468  opology_file: Th
+000067e0: 6520 7061 7468 2074 6f20 6120 746f 706f  e path to a topo
+000067f0: 6c6f 6779 2066 696c 6520 636f 6e74 6169  logy file contai
+00006800: 6e69 6e67 2074 6865 206e 6f64 6573 2061  ning the nodes a
+00006810: 6e64 206e 6574 776f 726b 2074 6f70 6f6c  nd network topol
+00006820: 6f67 7920 746f 2063 7265 6174 652e 0a20  ogy to create.. 
+00006830: 2020 203a 7479 7065 2074 6f70 6f6c 6f67     :type topolog
+00006840: 795f 6669 6c65 3a20 3a63 6c61 7373 3a60  y_file: :class:`
+00006850: 7374 7260 0a20 2020 203a 7061 7261 6d20  str`.    :param 
+00006860: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
+00006870: 6573 5f70 6174 6873 3a20 5468 6520 7061  es_paths: The pa
+00006880: 7468 2074 6f20 7265 736f 7572 6365 7320  th to resources 
+00006890: 7468 6174 2077 696c 6c20 6265 2070 7573  that will be pus
+000068a0: 6865 6420 696e 746f 2063 6f6d 7061 7469  hed into compati
+000068b0: 626c 6520 6e6f 6465 732e 0a20 2020 203a  ble nodes..    :
+000068c0: 7479 7065 2074 6f70 6f6c 6f67 795f 7265  type topology_re
+000068d0: 736f 7572 6365 735f 7061 7468 733a 203a  sources_paths: :
+000068e0: 636c 6173 733a 6073 7472 602c 206f 7074  class:`str`, opt
+000068f0: 696f 6e61 6c0a 2020 2020 3a70 6172 616d  ional.    :param
+00006900: 2061 6c6c 6f63 6174 696f 6e5f 7374 7261   allocation_stra
+00006910: 7465 6779 3a20 4e61 6d65 206f 6620 7468  tegy: Name of th
+00006920: 6520 616c 6c6f 6361 7469 6f6e 2073 7472  e allocation str
+00006930: 6174 6567 7920 746f 2075 7365 2074 6f20  ategy to use to 
+00006940: 616c 6c6f 6361 7465 206e 6f64 6573 2074  allocate nodes t
+00006950: 6f20 636f 6d70 7574 6520 7365 7276 6572  o compute server
+00006960: 732e 0a20 2020 203a 7479 7065 2061 6c6c  s..    :type all
+00006970: 6f63 6174 696f 6e5f 7374 7261 7465 6779  ocation_strategy
+00006980: 3a20 3a63 6c61 7373 3a60 7374 7260 2c20  : :class:`str`, 
+00006990: 6f70 7469 6f6e 616c 0a20 2020 203a 7061  optional.    :pa
+000069a0: 7261 6d20 6964 5f73 696d 756c 6174 696f  ram id_simulatio
+000069b0: 6e3a 2054 6865 2073 696d 756c 6174 696f  n: The simulatio
+000069c0: 6e20 4944 2c20 7768 656e 2065 7874 656e  n ID, when exten
+000069d0: 6469 6e67 2061 6e20 6578 6973 7469 6e67  ding an existing
+000069e0: 2073 696d 756c 6174 696f 6e20 7769 7468   simulation with
+000069f0: 206e 6577 206e 6f64 6573 2061 6e64 206c   new nodes and l
+00006a00: 696e 6b73 2e0a 2020 2020 3a74 7970 6520  inks..    :type 
+00006a10: 6964 5f73 696d 756c 6174 696f 6e3a 203a  id_simulation: :
+00006a20: 636c 6173 733a 6069 6e74 602c 206f 7074  class:`int`, opt
+00006a30: 696f 6e61 6c0a 2020 2020 2222 220a 2020  ional.    """.  
+00006a40: 2020 6966 2074 6f70 6f6c 6f67 795f 7265    if topology_re
+00006a50: 736f 7572 6365 735f 7061 7468 7320 6973  sources_paths is
+00006a60: 204e 6f6e 653a 0a20 2020 2020 2020 2074   None:.        t
+00006a70: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
+00006a80: 735f 7061 7468 7320 3d20 5b5d 0a0a 2020  s_paths = []..  
+00006a90: 2020 2320 4372 6561 7465 2061 206e 6577    # Create a new
+00006aa0: 2073 696d 756c 6174 696f 6e20 6d6f 6465   simulation mode
+00006ab0: 6c20 696e 2064 6174 6162 6173 6520 6261  l in database ba
+00006ac0: 7365 6420 6f6e 2074 6865 2070 726f 7669  sed on the provi
+00006ad0: 6465 6420 746f 706f 6c6f 6779 2066 696c  ded topology fil
+00006ae0: 6520 7061 7468 2e22 2222 0a20 2020 2069  e path.""".    i
+00006af0: 6620 746f 706f 6c6f 6779 5f66 696c 6520  f topology_file 
+00006b00: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00006b10: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+00006b20: 2822 416e 2074 6f70 6f6c 6f67 7920 6669  ("An topology fi
+00006b30: 6c65 2069 7320 7265 7175 6972 6564 2229  le is required")
+00006b40: 0a0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
+00006b50: 2059 414d 4c20 636f 6e66 6967 7572 6174   YAML configurat
+00006b60: 696f 6e20 6669 6c65 0a20 2020 205f 7661  ion file.    _va
+00006b70: 6c69 6461 7465 5f79 616d 6c5f 746f 706f  lidate_yaml_topo
+00006b80: 6c6f 6779 5f66 696c 6528 746f 706f 6c6f  logy_file(topolo
+00006b90: 6779 5f66 696c 6529 0a0a 2020 2020 2320  gy_file)..    # 
+00006ba0: 4f70 656e 2061 6e64 2072 6561 6420 5941  Open and read YA
+00006bb0: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+00006bc0: 2066 696c 650a 2020 2020 7961 6d6c 5f63   file.    yaml_c
+00006bd0: 6f6e 7465 6e74 203d 205f 7265 6164 5f79  ontent = _read_y
+00006be0: 616d 6c5f 746f 706f 6c6f 6779 5f66 696c  aml_topology_fil
+00006bf0: 6528 746f 706f 6c6f 6779 5f66 696c 6529  e(topology_file)
+00006c00: 0a0a 2020 2020 2320 5061 7273 6520 5941  ..    # Parse YA
+00006c10: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+00006c20: 0a20 2020 2023 2057 6520 7573 6520 7275  .    # We use ru
+00006c30: 616d 656c 2e79 616d 6c20 6265 6361 7573  amel.yaml becaus
+00006c40: 6520 6974 206b 6565 7073 2061 6e63 686f  e it keeps ancho
+00006c50: 7273 2061 6e64 0a20 2020 2023 2061 6c69  rs and.    # ali
+00006c60: 6173 6573 2069 6e20 6d65 6d6f 7279 2e20  ases in memory. 
+00006c70: 4974 2069 7320 7665 7279 2063 6f6e 7665  It is very conve
+00006c80: 6e69 656e 7420 7768 656e 2074 6865 2073  nient when the s
+00006c90: 696d 756c 6174 696f 6e0a 2020 2020 2320  imulation.    # 
+00006ca0: 6973 2073 746f 7265 642f 6665 7463 6865  is stored/fetche
+00006cb0: 6420 2872 6566 6572 656e 6365 7320 6172  d (references ar
+00006cc0: 6520 6b65 7074 2129 0a20 2020 206c 6f61  e kept!).    loa
+00006cd0: 6465 7220 3d20 5941 4d4c 2874 7970 3d22  der = YAML(typ="
+00006ce0: 7274 2229 0a20 2020 2074 6f70 6f6c 6f67  rt").    topolog
+00006cf0: 795f 636f 6e74 656e 7420 3d20 6c6f 6164  y_content = load
+00006d00: 6572 2e6c 6f61 6428 7961 6d6c 5f63 6f6e  er.load(yaml_con
+00006d10: 7465 6e74 290a 0a20 2020 2023 2041 6464  tent)..    # Add
+00006d20: 2061 2064 6566 6175 6c74 2072 6573 6f75   a default resou
+00006d30: 7263 6573 2064 6972 6563 746f 7279 2069  rces directory i
+00006d40: 6620 6974 2065 7869 7374 732e 0a20 2020  f it exists..   
+00006d50: 2023 2049 6620 7468 6520 746f 706f 6c6f   # If the topolo
+00006d60: 6779 2069 7320 2270 6174 682f 746f 2f74  gy is "path/to/t
+00006d70: 6f70 6f2e 7961 6d6c 222c 2074 6865 2064  opo.yaml", the d
+00006d80: 6566 6175 6c74 2072 6573 6f75 7263 6573  efault resources
+00006d90: 2064 6972 6563 746f 7279 2069 7320 2270   directory is "p
+00006da0: 6174 682f 746f 2f72 6573 6f75 7263 6573  ath/to/resources
+00006db0: 222e 0a20 2020 2064 6566 6175 6c74 5f72  "..    default_r
+00006dc0: 6573 6f75 7263 6573 5f70 6174 6820 3d20  esources_path = 
+00006dd0: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
+00006de0: 7061 7468 2e64 6972 6e61 6d65 2874 6f70  path.dirname(top
+00006df0: 6f6c 6f67 795f 6669 6c65 292c 2022 7265  ology_file), "re
+00006e00: 736f 7572 6365 7322 290a 2020 2020 6465  sources").    de
+00006e10: 6661 756c 745f 7265 736f 7572 6365 735f  fault_resources_
+00006e20: 7061 7468 203d 206f 732e 7061 7468 2e6e  path = os.path.n
+00006e30: 6f72 6d70 6174 6828 6465 6661 756c 745f  ormpath(default_
+00006e40: 7265 736f 7572 6365 735f 7061 7468 290a  resources_path).
+00006e50: 2020 2020 6966 205f 5f76 616c 6964 6174      if __validat
+00006e60: 655f 7265 736f 7572 6365 735f 7061 7468  e_resources_path
+00006e70: 2864 6566 6175 6c74 5f72 6573 6f75 7263  (default_resourc
+00006e80: 6573 5f70 6174 682c 2046 616c 7365 293a  es_path, False):
+00006e90: 0a20 2020 2020 2020 2069 6620 6465 6661  .        if defa
+00006ea0: 756c 745f 7265 736f 7572 6365 735f 7061  ult_resources_pa
+00006eb0: 7468 206e 6f74 2069 6e20 746f 706f 6c6f  th not in topolo
+00006ec0: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
+00006ed0: 6873 3a0a 2020 2020 2020 2020 2020 2020  hs:.            
+00006ee0: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
+00006ef0: 6573 5f70 6174 6873 2e61 7070 656e 6428  es_paths.append(
+00006f00: 6465 6661 756c 745f 7265 736f 7572 6365  default_resource
+00006f10: 735f 7061 7468 290a 0a20 2020 2072 6574  s_path)..    ret
+00006f20: 7572 6e20 6578 7465 6e64 5f73 696d 756c  urn extend_simul
+00006f30: 6174 696f 6e28 0a20 2020 2020 2020 2074  ation(.        t
+00006f40: 6f70 6f6c 6f67 795f 636f 6e74 656e 743d  opology_content=
+00006f50: 746f 706f 6c6f 6779 5f63 6f6e 7465 6e74  topology_content
+00006f60: 2c0a 2020 2020 2020 2020 746f 706f 6c6f  ,.        topolo
+00006f70: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
+00006f80: 6873 3d74 6f70 6f6c 6f67 795f 7265 736f  hs=topology_reso
+00006f90: 7572 6365 735f 7061 7468 732c 0a20 2020  urces_paths,.   
+00006fa0: 2020 2020 2061 6c6c 6f63 6174 696f 6e5f       allocation_
+00006fb0: 7374 7261 7465 6779 3d61 6c6c 6f63 6174  strategy=allocat
+00006fc0: 696f 6e5f 7374 7261 7465 6779 2c0a 2020  ion_strategy,.  
+00006fd0: 2020 2020 2020 6964 5f73 696d 756c 6174        id_simulat
+00006fe0: 696f 6e3d 6964 5f73 696d 756c 6174 696f  ion=id_simulatio
+00006ff0: 6e2c 0a20 2020 2029 0a0a 0a64 6566 2063  n,.    )...def c
+00007000: 7265 6174 655f 7369 6d75 6c61 7469 6f6e  reate_simulation
+00007010: 5f66 726f 6d5f 6261 7365 626f 7828 0a20  _from_basebox(. 
+00007020: 2020 2062 6173 6562 6f78 5f69 643a 2073     basebox_id: s
+00007030: 7472 2c0a 2020 2020 6164 645f 696e 7465  tr,.    add_inte
+00007040: 726e 6574 3a20 626f 6f6c 203d 2046 616c  rnet: bool = Fal
+00007050: 7365 2c0a 2020 2020 6164 645f 686f 7374  se,.    add_host
+00007060: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00007070: 2020 2020 616c 6c6f 6361 7469 6f6e 5f73      allocation_s
+00007080: 7472 6174 6567 793a 204f 7074 696f 6e61  trategy: Optiona
+00007090: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
+000070a0: 202d 3e20 696e 743a 0a20 2020 2022 2222   -> int:.    """
+000070b0: 4372 6561 7465 2061 206e 6577 2073 696d  Create a new sim
+000070c0: 756c 6174 696f 6e20 6d6f 6465 6c20 696e  ulation model in
+000070d0: 2064 6174 6162 6173 6520 6261 7365 6420   database based 
+000070e0: 6f6e 2074 6865 2070 726f 7669 6465 6420  on the provided 
+000070f0: 6261 7365 626f 7820 6964 2c20 7769 7468  basebox id, with
+00007100: 0a20 2020 206f 7074 696f 6e61 6c20 696e  .    optional in
+00007110: 7465 726e 6574 2061 6e64 2f6f 7220 686f  ternet and/or ho
+00007120: 7374 2063 6f6e 6e65 6374 6976 6974 792e  st connectivity.
+00007130: 0a0a 2020 2020 2222 220a 0a20 2020 2069  ..    """..    i
+00007140: 6620 6261 7365 626f 785f 6964 2069 7320  f basebox_id is 
+00007150: 4e6f 6e65 3a0a 2020 2020 2020 2020 7261  None:.        ra
+00007160: 6973 6520 4578 6365 7074 696f 6e28 2241  ise Exception("A
+00007170: 2062 6173 6562 6f78 2049 4420 6973 2072   basebox ID is r
+00007180: 6571 7569 7265 6422 290a 0a20 2020 2023  equired")..    #
+00007190: 2043 7265 6174 6520 616e 2074 6f70 6f6c   Create an topol
+000071a0: 6f67 7920 7769 7468 2074 6865 2070 726f  ogy with the pro
+000071b0: 7669 6465 6420 6261 7365 626f 7820 4944  vided basebox ID
+000071c0: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
+000071d0: 2020 6261 7365 626f 7820 3d20 6665 7463    basebox = fetc
+000071e0: 685f 6261 7365 626f 7828 6261 7365 626f  h_basebox(basebo
+000071f0: 785f 6964 290a 2020 2020 6578 6365 7074  x_id).    except
+00007200: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
+00007210: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+00007220: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00007230: 2066 2243 616e 6e6f 7420 6669 6e64 2062   f"Cannot find b
+00007240: 6173 6562 6f78 2069 6e20 6461 7461 6261  asebox in databa
+00007250: 7365 2066 726f 6d20 6261 7365 626f 7820  se from basebox 
+00007260: 4944 2027 7b62 6173 6562 6f78 5f69 647d  ID '{basebox_id}
+00007270: 2722 0a20 2020 2020 2020 2029 0a0a 2020  '".        )..  
+00007280: 2020 6e6f 6465 5f6e 616d 6520 3d20 5f67    node_name = _g
+00007290: 6574 5f72 616e 646f 6d5f 7374 7269 6e67  et_random_string
+000072a0: 2831 3029 0a20 2020 2072 6f6c 6520 3d20  (10).    role = 
+000072b0: 6261 7365 626f 785b 2272 6f6c 6522 5d0a  basebox["role"].
+000072c0: 2020 2020 6e62 5f70 726f 6320 3d20 6261      nb_proc = ba
+000072d0: 7365 626f 785b 226e 625f 7072 6f63 225d  sebox["nb_proc"]
+000072e0: 0a20 2020 206d 656d 6f72 795f 7369 7a65  .    memory_size
+000072f0: 203d 2062 6173 6562 6f78 5b22 6d65 6d6f   = basebox["memo
+00007300: 7279 5f73 697a 6522 5d0a 0a20 2020 2079  ry_size"]..    y
+00007310: 616d 6c5f 636f 6e74 656e 7420 3d20 6622  aml_content = f"
+00007320: 2222 2d2d 2d0a 6e61 6d65 3a20 227b 6261  ""---.name: "{ba
+00007330: 7365 626f 785f 6964 7d22 0a6e 6f64 6573  sebox_id}".nodes
+00007340: 3a0a 0a20 202d 2026 7377 6974 6368 0a20  :..  - &switch. 
+00007350: 2020 2074 7970 653a 2073 7769 7463 680a     type: switch.
+00007360: 2020 2020 6e61 6d65 3a20 2273 7769 7463      name: "switc
+00007370: 6822 0a0a 2020 2d20 2663 6c69 656e 740a  h"..  - &client.
+00007380: 2020 2020 7479 7065 3a20 7669 7274 7561      type: virtua
+00007390: 6c5f 6d61 6368 696e 650a 2020 2020 6e61  l_machine.    na
+000073a0: 6d65 3a20 227b 6e6f 6465 5f6e 616d 657d  me: "{node_name}
+000073b0: 220a 2020 2020 6261 7365 626f 785f 6964  ".    basebox_id
+000073c0: 3a20 227b 6261 7365 626f 785f 6964 7d22  : "{basebox_id}"
+000073d0: 0a20 2020 206e 625f 7072 6f63 3a20 7b6e  .    nb_proc: {n
+000073e0: 625f 7072 6f63 7d0a 2020 2020 6d65 6d6f  b_proc}.    memo
+000073f0: 7279 5f73 697a 653a 207b 6d65 6d6f 7279  ry_size: {memory
+00007400: 5f73 697a 657d 0a20 2020 2072 6f6c 6573  _size}.    roles
+00007410: 3a20 5b22 7b72 6f6c 657d 225d 0a22 2222  : ["{role}"]."""
+00007420: 0a0a 2020 2020 6966 2061 6464 5f68 6f73  ..    if add_hos
+00007430: 743a 0a20 2020 2020 2020 2079 616d 6c5f  t:.        yaml_
+00007440: 636f 6e74 656e 7420 2b3d 2022 2222 0a20  content += """. 
+00007450: 202d 2026 686f 7374 5f6d 6163 6869 6e65   - &host_machine
+00007460: 0a20 2020 2074 7970 653a 2068 6f73 745f  .    type: host_
+00007470: 6d61 6368 696e 650a 2020 2020 6e61 6d65  machine.    name
+00007480: 3a20 2268 6f73 7422 0a22 2222 0a0a 2020  : "host"."""..  
+00007490: 2020 6966 2061 6464 5f69 6e74 6572 6e65    if add_interne
+000074a0: 743a 0a20 2020 2020 2020 2023 2061 6464  t:.        # add
+000074b0: 2064 6566 6175 6c74 2072 6f75 7465 2074   default route t
+000074c0: 6f20 6761 7465 7761 792c 2061 2067 6174  o gateway, a gat
+000074d0: 6577 6179 2061 6e64 2061 2073 7769 7463  eway and a switc
+000074e0: 6820 746f 2070 6c75 6720 7468 6520 6761  h to plug the ga
+000074f0: 7465 7761 7920 616e 6420 7468 6520 726f  teway and the ro
+00007500: 7574 6572 0a20 2020 2020 2020 2079 616d  uter.        yam
+00007510: 6c5f 636f 6e74 656e 7420 2b3d 2022 2222  l_content += """
+00007520: 0a20 202d 2026 726f 7574 6572 0a20 2020  .  - &router.   
+00007530: 2074 7970 653a 2072 6f75 7465 720a 2020   type: router.  
+00007540: 2020 6e61 6d65 3a20 2272 6f75 7465 7222    name: "router"
+00007550: 0a20 2020 2072 6f75 7465 733a 0a20 2020  .    routes:.   
+00007560: 2020 202d 2022 302e 302e 302e 302f 3020     - "0.0.0.0/0 
+00007570: 2d3e 2031 3932 2e31 3638 2e32 332e 3222  -> 192.168.23.2"
+00007580: 0a0a 2020 2d20 2673 7769 7463 685f 696e  ..  - &switch_in
+00007590: 7465 726e 6574 0a20 2020 2074 7970 653a  ternet.    type:
+000075a0: 2073 7769 7463 680a 2020 2020 6e61 6d65   switch.    name
+000075b0: 3a20 2273 7769 7463 6849 6e74 6572 6e65  : "switchInterne
+000075c0: 7422 0a0a 2020 2d20 2670 6879 7369 6361  t"..  - &physica
+000075d0: 6c5f 6761 7465 7761 790a 2020 2020 7479  l_gateway.    ty
+000075e0: 7065 3a20 7068 7973 6963 616c 5f67 6174  pe: physical_gat
+000075f0: 6577 6179 0a20 2020 206e 616d 653a 2022  eway.    name: "
+00007600: 7068 7973 6963 616c 4761 7465 7761 7922  physicalGateway"
+00007610: 0a22 2222 0a20 2020 2065 6c73 653a 0a20  .""".    else:. 
+00007620: 2020 2020 2020 2079 616d 6c5f 636f 6e74         yaml_cont
+00007630: 656e 7420 2b3d 2022 2222 0a20 202d 2026  ent += """.  - &
+00007640: 726f 7574 6572 0a20 2020 2074 7970 653a  router.    type:
+00007650: 2072 6f75 7465 720a 2020 2020 6e61 6d65   router.    name
+00007660: 3a20 2272 6f75 7465 7222 0a22 2222 0a0a  : "router"."""..
+00007670: 2020 2020 7961 6d6c 5f63 6f6e 7465 6e74      yaml_content
+00007680: 202b 3d20 2222 220a 6c69 6e6b 733a 0a0a   += """.links:..
+00007690: 2020 2d20 7377 6974 6368 3a20 2a73 7769    - switch: *swi
+000076a0: 7463 680a 2020 2020 6e6f 6465 3a20 2a72  tch.    node: *r
+000076b0: 6f75 7465 720a 2020 2020 7061 7261 6d73  outer.    params
+000076c0: 3a0a 2020 2020 2020 6970 3a20 2231 3932  :.      ip: "192
+000076d0: 2e31 3638 2e32 2e31 2f32 3422 0a20 2020  .168.2.1/24".   
+000076e0: 2020 2064 6863 705f 6e61 6d65 7365 7276     dhcp_nameserv
+000076f0: 6572 3a20 2238 2e38 2e38 2e38 220a 0a20  er: "8.8.8.8".. 
+00007700: 202d 2073 7769 7463 683a 202a 7377 6974   - switch: *swit
+00007710: 6368 0a20 2020 206e 6f64 653a 202a 636c  ch.    node: *cl
+00007720: 6965 6e74 0a20 2020 2070 6172 616d 733a  ient.    params:
+00007730: 0a20 2020 2020 2069 703a 2022 3139 322e  .      ip: "192.
+00007740: 3136 382e 322e 322f 3234 220a 2222 220a  168.2.2/24".""".
+00007750: 0a20 2020 2069 6620 6164 645f 686f 7374  .    if add_host
+00007760: 3a0a 2020 2020 2020 2020 7961 6d6c 5f63  :.        yaml_c
+00007770: 6f6e 7465 6e74 202b 3d20 2222 220a 2020  ontent += """.  
+00007780: 2d20 7377 6974 6368 3a20 2a73 7769 7463  - switch: *switc
+00007790: 680a 2020 2020 6e6f 6465 3a20 2a68 6f73  h.    node: *hos
+000077a0: 745f 6d61 6368 696e 650a 2020 2020 7061  t_machine.    pa
+000077b0: 7261 6d73 3a0a 2020 2020 2020 6970 3a20  rams:.      ip: 
+000077c0: 2231 3932 2e31 3638 2e32 2e33 2f32 3422  "192.168.2.3/24"
+000077d0: 0a22 2222 0a0a 2020 2020 6966 2061 6464  ."""..    if add
+000077e0: 5f69 6e74 6572 6e65 743a 0a20 2020 2020  _internet:.     
+000077f0: 2020 2079 616d 6c5f 636f 6e74 656e 7420     yaml_content 
+00007800: 2b3d 2022 2222 0a20 202d 2073 7769 7463  += """.  - switc
+00007810: 683a 202a 7377 6974 6368 5f69 6e74 6572  h: *switch_inter
+00007820: 6e65 740a 2020 2020 6e6f 6465 3a20 2a72  net.    node: *r
+00007830: 6f75 7465 720a 2020 2020 7061 7261 6d73  outer.    params
+00007840: 3a0a 2020 2020 2020 6970 3a20 2231 3932  :.      ip: "192
+00007850: 2e31 3638 2e32 332e 312f 3234 220a 0a20  .168.23.1/24".. 
+00007860: 202d 2073 7769 7463 683a 202a 7377 6974   - switch: *swit
+00007870: 6368 5f69 6e74 6572 6e65 740a 2020 2020  ch_internet.    
+00007880: 6e6f 6465 3a20 2a70 6879 7369 6361 6c5f  node: *physical_
+00007890: 6761 7465 7761 790a 2020 2020 7061 7261  gateway.    para
+000078a0: 6d73 3a0a 2020 2020 2020 6970 3a20 2231  ms:.      ip: "1
+000078b0: 3932 2e31 3638 2e32 332e 322f 3234 220a  92.168.23.2/24".
+000078c0: 2222 220a 0a20 2020 206c 6f61 6465 7220  """..    loader 
+000078d0: 3d20 5941 4d4c 2874 7970 3d22 7274 2229  = YAML(typ="rt")
+000078e0: 0a20 2020 2074 6f70 6f6c 6f67 795f 636f  .    topology_co
+000078f0: 6e74 656e 7420 3d20 6c6f 6164 6572 2e6c  ntent = loader.l
+00007900: 6f61 6428 7961 6d6c 5f63 6f6e 7465 6e74  oad(yaml_content
+00007910: 290a 0a20 2020 2072 6574 7572 6e20 6372  )..    return cr
+00007920: 6561 7465 5f73 696d 756c 6174 696f 6e28  eate_simulation(
+00007930: 0a20 2020 2020 2020 2074 6f70 6f6c 6f67  .        topolog
+00007940: 795f 636f 6e74 656e 743d 746f 706f 6c6f  y_content=topolo
+00007950: 6779 5f63 6f6e 7465 6e74 2c0a 2020 2020  gy_content,.    
+00007960: 2020 2020 616c 6c6f 6361 7469 6f6e 5f73      allocation_s
+00007970: 7472 6174 6567 793d 616c 6c6f 6361 7469  trategy=allocati
+00007980: 6f6e 5f73 7472 6174 6567 792c 0a20 2020  on_strategy,.   
+00007990: 2029 0a0a 0a64 6566 2065 7874 656e 645f   )...def extend_
+000079a0: 7369 6d75 6c61 7469 6f6e 5f66 726f 6d5f  simulation_from_
+000079b0: 6261 7365 626f 7828 0a20 2020 2062 6173  basebox(.    bas
+000079c0: 6562 6f78 5f69 643a 2073 7472 2c0a 2020  ebox_id: str,.  
+000079d0: 2020 7377 6974 6368 5f6e 616d 653a 2073    switch_name: s
+000079e0: 7472 2c0a 2020 2020 616c 6c6f 6361 7469  tr,.    allocati
+000079f0: 6f6e 5f73 7472 6174 6567 793a 204f 7074  on_strategy: Opt
+00007a00: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00007a10: 652c 0a20 2020 2069 645f 7369 6d75 6c61  e,.    id_simula
+00007a20: 7469 6f6e 3a20 696e 7420 3d20 4e6f 6e65  tion: int = None
+00007a30: 2c0a 2920 2d3e 2069 6e74 3a0a 2020 2020  ,.) -> int:.    
+00007a40: 2222 2245 7874 656e 6420 616e 2065 7869  """Extend an exi
+00007a50: 7374 696e 6720 7369 6d75 6c61 7469 6f6e  sting simulation
+00007a60: 206d 6f64 656c 2069 6e20 6461 7461 6261   model in databa
+00007a70: 7365 2062 6173 6564 206f 6e20 7468 650a  se based on the.
+00007a80: 2020 2020 7072 6f76 6964 6564 2062 6173      provided bas
+00007a90: 6562 6f78 2069 642c 2061 6e64 2070 6c75  ebox id, and plu
+00007aa0: 6720 7468 6520 6e65 7720 6e6f 6465 206f  g the new node o
+00007ab0: 6620 7468 6520 7370 6563 6966 6564 2073  f the specifed s
+00007ac0: 7769 7463 682e 0a0a 2020 2020 2222 220a  witch...    """.
+00007ad0: 0a20 2020 2069 6620 6261 7365 626f 785f  .    if basebox_
+00007ae0: 6964 2069 7320 4e6f 6e65 3a0a 2020 2020  id is None:.    
+00007af0: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+00007b00: 696f 6e28 2241 2062 6173 6562 6f78 2049  ion("A basebox I
+00007b10: 4420 6973 2072 6571 7569 7265 6422 290a  D is required").
+00007b20: 0a20 2020 2023 2043 7265 6174 6520 616e  .    # Create an
+00007b30: 2074 6f70 6f6c 6f67 7920 7769 7468 2074   topology with t
+00007b40: 6865 2070 726f 7669 6465 6420 6261 7365  he provided base
+00007b50: 626f 7820 4944 0a20 2020 2074 7279 3a0a  box ID.    try:.
+00007b60: 2020 2020 2020 2020 6261 7365 626f 7820          basebox 
+00007b70: 3d20 6665 7463 685f 6261 7365 626f 7828  = fetch_basebox(
+00007b80: 6261 7365 626f 785f 6964 290a 2020 2020  basebox_id).    
+00007b90: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00007ba0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00007bb0: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
+00007bc0: 2020 2020 2020 2066 2243 616e 6e6f 7420         f"Cannot 
+00007bd0: 6669 6e64 2062 6173 6562 6f78 2069 6e20  find basebox in 
+00007be0: 6461 7461 6261 7365 2066 726f 6d20 6261  database from ba
+00007bf0: 7365 626f 7820 4944 2027 7b62 6173 6562  sebox ID '{baseb
+00007c00: 6f78 5f69 647d 2722 0a20 2020 2020 2020  ox_id}'".       
+00007c10: 2029 0a0a 2020 2020 6e6f 6465 5f6e 616d   )..    node_nam
+00007c20: 6520 3d20 5f67 6574 5f72 616e 646f 6d5f  e = _get_random_
+00007c30: 7374 7269 6e67 2831 3029 0a20 2020 2072  string(10).    r
+00007c40: 6f6c 6520 3d20 6261 7365 626f 785b 2272  ole = basebox["r
+00007c50: 6f6c 6522 5d0a 2020 2020 6e62 5f70 726f  ole"].    nb_pro
+00007c60: 6320 3d20 6261 7365 626f 785b 226e 625f  c = basebox["nb_
+00007c70: 7072 6f63 225d 0a20 2020 206d 656d 6f72  proc"].    memor
+00007c80: 795f 7369 7a65 203d 2062 6173 6562 6f78  y_size = basebox
+00007c90: 5b22 6d65 6d6f 7279 5f73 697a 6522 5d0a  ["memory_size"].
+00007ca0: 0a20 2020 2074 6f70 6f6c 6f67 795f 636f  .    topology_co
+00007cb0: 6e74 656e 7420 3d20 7b0a 2020 2020 2020  ntent = {.      
+00007cc0: 2020 226e 6f64 6573 223a 205b 0a20 2020    "nodes": [.   
+00007cd0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00007ce0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00007cf0: 223a 2022 7669 7274 7561 6c5f 6d61 6368  ": "virtual_mach
+00007d00: 696e 6522 2c0a 2020 2020 2020 2020 2020  ine",.          
+00007d10: 2020 2020 2020 226e 616d 6522 3a20 6e6f        "name": no
+00007d20: 6465 5f6e 616d 652c 0a20 2020 2020 2020  de_name,.       
+00007d30: 2020 2020 2020 2020 2022 6261 7365 626f           "basebo
+00007d40: 785f 6964 223a 2062 6173 6562 6f78 5f69  x_id": basebox_i
+00007d50: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00007d60: 2020 2022 6e62 5f70 726f 6322 3a20 6e62     "nb_proc": nb
+00007d70: 5f70 726f 632c 0a20 2020 2020 2020 2020  _proc,.         
+00007d80: 2020 2020 2020 2022 6d65 6d6f 7279 5f73         "memory_s
+00007d90: 697a 6522 3a20 6d65 6d6f 7279 5f73 697a  ize": memory_siz
+00007da0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00007db0: 2020 2022 726f 6c65 7322 3a20 5b72 6f6c     "roles": [rol
+00007dc0: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
+00007dd0: 7d0a 2020 2020 2020 2020 5d2c 0a20 2020  }.        ],.   
+00007de0: 2020 2020 2022 6c69 6e6b 7322 3a20 5b0a       "links": [.
+00007df0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00007e00: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00007e10: 7769 7463 6822 3a20 7b22 7479 7065 223a  witch": {"type":
+00007e20: 2022 7377 6974 6368 222c 2022 6e61 6d65   "switch", "name
+00007e30: 223a 2073 7769 7463 685f 6e61 6d65 7d2c  ": switch_name},
+00007e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007e50: 2022 6e6f 6465 223a 207b 0a20 2020 2020   "node": {.     
+00007e60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007e70: 7479 7065 223a 2022 7669 7274 7561 6c5f  type": "virtual_
+00007e80: 6d61 6368 696e 6522 2c0a 2020 2020 2020  machine",.      
+00007e90: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00007ea0: 616d 6522 3a20 6e6f 6465 5f6e 616d 652c  ame": node_name,
+00007eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007ec0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00007ed0: 2020 2020 2270 6172 616d 7322 3a20 7b7d      "params": {}
+00007ee0: 2c20 2023 2044 796e 616d 6963 2049 5020  ,  # Dynamic IP 
+00007ef0: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
+00007f00: 2020 2020 7d0a 2020 2020 2020 2020 5d2c      }.        ],
+00007f10: 0a20 2020 207d 0a0a 2020 2020 7265 7475  .    }..    retu
+00007f20: 726e 2065 7874 656e 645f 7369 6d75 6c61  rn extend_simula
+00007f30: 7469 6f6e 280a 2020 2020 2020 2020 746f  tion(.        to
+00007f40: 706f 6c6f 6779 5f63 6f6e 7465 6e74 3d74  pology_content=t
+00007f50: 6f70 6f6c 6f67 795f 636f 6e74 656e 742c  opology_content,
+00007f60: 0a20 2020 2020 2020 2061 6c6c 6f63 6174  .        allocat
+00007f70: 696f 6e5f 7374 7261 7465 6779 3d61 6c6c  ion_strategy=all
+00007f80: 6f63 6174 696f 6e5f 7374 7261 7465 6779  ocation_strategy
+00007f90: 2c0a 2020 2020 2020 2020 6964 5f73 696d  ,.        id_sim
+00007fa0: 756c 6174 696f 6e3d 6964 5f73 696d 756c  ulation=id_simul
+00007fb0: 6174 696f 6e2c 0a20 2020 2029 0a0a 0a23  ation,.    )...#
+00007fc0: 2323 0a23 2054 6f70 6f6c 6f67 7920 6865  ##.# Topology he
+00007fd0: 6c70 6572 730a 2323 230a 0a0a 6465 6620  lpers.###...def 
+00007fe0: 746f 706f 6c6f 6779 5f66 696c 655f 6164  topology_file_ad
+00007ff0: 645f 7765 6273 6974 6573 280a 2020 2020  d_websites(.    
+00008000: 746f 706f 6c6f 6779 5f66 696c 653a 2073  topology_file: s
+00008010: 7472 2c20 7765 6273 6974 6573 3a20 4c69  tr, websites: Li
+00008020: 7374 5b73 7472 5d2c 2073 7769 7463 685f  st[str], switch_
+00008030: 6e61 6d65 3a20 7374 720a 2920 2d3e 2073  name: str.) -> s
+00008040: 7472 3a0a 2020 2020 2222 2241 6464 2064  tr:.    """Add d
+00008050: 6f63 6b65 7220 7765 6273 6974 6573 206e  ocker websites n
+00008060: 6f64 6520 746f 2061 2067 6976 656e 2074  ode to a given t
+00008070: 6f70 6f6c 6f67 792c 2061 6e64 2072 6574  opology, and ret
+00008080: 7572 6e20 7468 6520 7570 6461 7465 6420  urn the updated 
+00008090: 746f 706f 6c6f 6779 2e22 2222 0a0a 2020  topology."""..  
+000080a0: 2020 2320 5661 6c69 6461 7465 2059 414d    # Validate YAM
+000080b0: 4c20 746f 706f 6c6f 6779 2066 696c 650a  L topology file.
+000080c0: 2020 2020 5f76 616c 6964 6174 655f 7961      _validate_ya
+000080d0: 6d6c 5f74 6f70 6f6c 6f67 795f 6669 6c65  ml_topology_file
+000080e0: 2874 6f70 6f6c 6f67 795f 6669 6c65 290a  (topology_file).
+000080f0: 0a20 2020 2023 204f 7065 6e20 616e 6420  .    # Open and 
+00008100: 7265 6164 2059 414d 4c20 746f 706f 6c6f  read YAML topolo
+00008110: 6779 2066 696c 650a 2020 2020 746f 706f  gy file.    topo
+00008120: 6c6f 6779 5f79 616d 6c20 3d20 5f72 6561  logy_yaml = _rea
+00008130: 645f 7961 6d6c 5f74 6f70 6f6c 6f67 795f  d_yaml_topology_
+00008140: 6669 6c65 2874 6f70 6f6c 6f67 795f 6669  file(topology_fi
+00008150: 6c65 290a 0a20 2020 2023 2055 7064 6174  le)..    # Updat
+00008160: 6520 746f 706f 6c6f 6779 2077 6974 6820  e topology with 
+00008170: 7468 6520 4150 490a 2020 2020 746f 706f  the API.    topo
+00008180: 6c6f 6779 5f79 616d 6c20 3d20 746f 706f  logy_yaml = topo
+00008190: 6c6f 6779 5f61 6464 5f77 6562 7369 7465  logy_add_website
+000081a0: 7328 746f 706f 6c6f 6779 5f79 616d 6c2c  s(topology_yaml,
+000081b0: 2077 6562 7369 7465 732c 2073 7769 7463   websites, switc
+000081c0: 685f 6e61 6d65 290a 0a20 2020 2072 6574  h_name)..    ret
+000081d0: 7572 6e20 746f 706f 6c6f 6779 5f79 616d  urn topology_yam
+000081e0: 6c0a 0a0a 6465 6620 746f 706f 6c6f 6779  l...def topology
+000081f0: 5f66 696c 655f 6164 645f 6467 6128 0a20  _file_add_dga(. 
+00008200: 2020 2074 6f70 6f6c 6f67 795f 6669 6c65     topology_file
+00008210: 3a20 7374 722c 0a20 2020 2061 6c67 6f72  : str,.    algor
+00008220: 6974 686d 3a20 7374 722c 0a20 2020 2073  ithm: str,.    s
+00008230: 7769 7463 685f 6e61 6d65 3a20 7374 722c  witch_name: str,
+00008240: 0a20 2020 206e 756d 6265 723a 2069 6e74  .    number: int
+00008250: 2c0a 2020 2020 7265 736f 7572 6365 735f  ,.    resources_
+00008260: 6469 723a 2073 7472 2c0a 2920 2d3e 2028  dir: str,.) -> (
+00008270: 7374 722c 204c 6973 745b 7374 725d 293a  str, List[str]):
+00008280: 0a20 2020 2022 2222 4164 6420 646f 636b  .    """Add dock
+00008290: 6572 2065 6d70 7479 2077 6562 7369 7465  er empty website
+000082a0: 7320 6e6f 6465 2077 6974 6820 4447 4120  s node with DGA 
+000082b0: 746f 2061 2067 6976 656e 2074 6f70 6f6c  to a given topol
+000082c0: 6f67 792c 2061 6e64 2072 6574 7572 6e20  ogy, and return 
+000082d0: 7468 6520 7570 6461 7465 6420 746f 706f  the updated topo
+000082e0: 6c6f 6779 2e22 2222 0a0a 2020 2020 2320  logy."""..    # 
+000082f0: 5661 6c69 6461 7465 0a0a 2020 2020 2320  Validate..    # 
+00008300: 5661 6c69 6461 7465 2059 414d 4c20 746f  Validate YAML to
+00008310: 706f 6c6f 6779 2066 696c 650a 2020 2020  pology file.    
+00008320: 5f76 616c 6964 6174 655f 7961 6d6c 5f74  _validate_yaml_t
+00008330: 6f70 6f6c 6f67 795f 6669 6c65 2874 6f70  opology_file(top
+00008340: 6f6c 6f67 795f 6669 6c65 290a 0a20 2020  ology_file)..   
+00008350: 2023 204f 7065 6e20 616e 6420 7265 6164   # Open and read
+00008360: 2059 414d 4c20 746f 706f 6c6f 6779 2066   YAML topology f
+00008370: 696c 650a 2020 2020 746f 706f 6c6f 6779  ile.    topology
+00008380: 5f79 616d 6c20 3d20 5f72 6561 645f 7961  _yaml = _read_ya
+00008390: 6d6c 5f74 6f70 6f6c 6f67 795f 6669 6c65  ml_topology_file
+000083a0: 2874 6f70 6f6c 6f67 795f 6669 6c65 290a  (topology_file).
+000083b0: 0a20 2020 2023 2055 7064 6174 6520 746f  .    # Update to
+000083c0: 706f 6c6f 6779 2077 6974 6820 7468 6520  pology with the 
+000083d0: 4150 490a 2020 2020 2874 6f70 6f6c 6f67  API.    (topolog
+000083e0: 795f 7961 6d6c 2c20 646f 6d61 696e 7329  y_yaml, domains)
+000083f0: 203d 2074 6f70 6f6c 6f67 795f 6164 645f   = topology_add_
+00008400: 6467 6128 0a20 2020 2020 2020 2074 6f70  dga(.        top
+00008410: 6f6c 6f67 795f 7961 6d6c 2c20 616c 676f  ology_yaml, algo
+00008420: 7269 7468 6d2c 2073 7769 7463 685f 6e61  rithm, switch_na
+00008430: 6d65 2c20 6e75 6d62 6572 2c20 7265 736f  me, number, reso
+00008440: 7572 6365 735f 6469 720a 2020 2020 290a  urces_dir.    ).
+00008450: 0a20 2020 2072 6574 7572 6e20 746f 706f  .    return topo
+00008460: 6c6f 6779 5f79 616d 6c2c 2064 6f6d 6169  logy_yaml, domai
+00008470: 6e73 0a0a 0a64 6566 2074 6f70 6f6c 6f67  ns...def topolog
+00008480: 795f 6669 6c65 5f61 6464 5f64 6e73 5f73  y_file_add_dns_s
+00008490: 6572 7665 7228 0a20 2020 2074 6f70 6f6c  erver(.    topol
+000084a0: 6f67 795f 6669 6c65 3a20 7374 722c 0a20  ogy_file: str,. 
+000084b0: 2020 2073 7769 7463 685f 6e61 6d65 3a20     switch_name: 
+000084c0: 7374 722c 0a20 2020 2072 6573 6f75 7263  str,.    resourc
+000084d0: 6573 5f64 6972 3a20 7374 722c 0a29 202d  es_dir: str,.) -
+000084e0: 3e20 2873 7472 2c20 7374 7229 3a0a 2020  > (str, str):.  
+000084f0: 2020 2222 2241 6464 2061 2044 4e53 2073    """Add a DNS s
+00008500: 6572 7665 7220 746f 2061 2059 414d 4c20  erver to a YAML 
+00008510: 746f 706f 6c6f 6779 2e0a 2020 2020 5265  topology..    Re
+00008520: 7475 726e 7320 7468 6520 7570 6461 7465  turns the update
+00008530: 6420 746f 706f 6c6f 6779 2061 6e64 2074  d topology and t
+00008540: 6865 2063 6f6e 7465 6e74 206f 6620 7468  he content of th
+00008550: 6520 444e 5320 636f 6e66 6967 7572 6174  e DNS configurat
+00008560: 696f 6e20 6669 6c65 2e22 2222 0a0a 2020  ion file."""..  
+00008570: 2020 2320 5661 6c69 6461 7465 0a0a 2020    # Validate..  
+00008580: 2020 2320 5661 6c69 6461 7465 2059 414d    # Validate YAM
+00008590: 4c20 746f 706f 6c6f 6779 2066 696c 650a  L topology file.
+000085a0: 2020 2020 5f76 616c 6964 6174 655f 7961      _validate_ya
+000085b0: 6d6c 5f74 6f70 6f6c 6f67 795f 6669 6c65  ml_topology_file
+000085c0: 2874 6f70 6f6c 6f67 795f 6669 6c65 290a  (topology_file).
+000085d0: 0a20 2020 2023 204f 7065 6e20 616e 6420  .    # Open and 
+000085e0: 7265 6164 2059 414d 4c20 746f 706f 6c6f  read YAML topolo
+000085f0: 6779 2066 696c 650a 2020 2020 746f 706f  gy file.    topo
+00008600: 6c6f 6779 5f79 616d 6c20 3d20 5f72 6561  logy_yaml = _rea
+00008610: 645f 7961 6d6c 5f74 6f70 6f6c 6f67 795f  d_yaml_topology_
+00008620: 6669 6c65 2874 6f70 6f6c 6f67 795f 6669  file(topology_fi
+00008630: 6c65 290a 0a20 2020 2023 2055 7064 6174  le)..    # Updat
+00008640: 6520 746f 706f 6c6f 6779 2077 6974 6820  e topology with 
+00008650: 7468 6520 4150 490a 2020 2020 2874 6f70  the API.    (top
+00008660: 6f6c 6f67 795f 7961 6d6c 2c20 646e 735f  ology_yaml, dns_
+00008670: 636f 6e66 5f63 6f6e 7465 6e74 2920 3d20  conf_content) = 
+00008680: 746f 706f 6c6f 6779 5f61 6464 5f64 6e73  topology_add_dns
+00008690: 5f73 6572 7665 7228 0a20 2020 2020 2020  _server(.       
+000086a0: 2074 6f70 6f6c 6f67 795f 7961 6d6c 2c20   topology_yaml, 
+000086b0: 7377 6974 6368 5f6e 616d 652c 2072 6573  switch_name, res
+000086c0: 6f75 7263 6573 5f64 6972 0a20 2020 2029  ources_dir.    )
+000086d0: 0a0a 2020 2020 7265 7475 726e 2074 6f70  ..    return top
+000086e0: 6f6c 6f67 795f 7961 6d6c 2c20 646e 735f  ology_yaml, dns_
+000086f0: 636f 6e66 5f63 6f6e 7465 6e74 0a0a 0a23  conf_content...#
+00008700: 2323 0a23 2042 6173 6562 6f78 2068 656c  ##.# Basebox hel
+00008710: 7065 7273 0a23 2323 0a0a 0a64 6566 205f  pers.###...def _
+00008720: 7261 6973 655f 6572 726f 725f 6d73 6728  raise_error_msg(
+00008730: 7265 7375 6c74 3a20 6469 6374 2920 2d3e  result: dict) ->
+00008740: 204e 6f6e 653a 0a20 2020 2022 2222 0a20   None:.    """. 
+00008750: 2020 2052 6169 7365 2061 6e20 6572 726f     Raise an erro
+00008760: 7220 6d65 7373 6167 6520 6966 2061 2074  r message if a t
+00008770: 6173 6b20 2865 6720 7468 6520 6261 7365  ask (eg the base
+00008780: 626f 7820 7665 7269 6669 6361 7469 6f6e  box verification
+00008790: 2920 6661 696c 6564 0a20 2020 203a 7061  ) failed.    :pa
+000087a0: 7261 6d20 7265 7375 6c74 3a20 7468 6520  ram result: the 
+000087b0: 7265 7375 6c74 206f 6620 7468 6520 7461  result of the ta
+000087c0: 736b 0a20 2020 203a 7265 7475 726e 3a20  sk.    :return: 
+000087d0: 4e6f 6e65 0a20 2020 2022 2222 0a20 2020  None.    """.   
+000087e0: 2065 7272 6f72 5f6d 7367 203d 2022 4e6f   error_msg = "No
+000087f0: 2065 7272 6f72 206d 6573 7361 6765 2072   error message r
+00008800: 6574 7572 6e65 6422 0a20 2020 2069 6620  eturned".    if 
+00008810: 2272 6573 756c 7422 2069 6e20 7265 7375  "result" in resu
+00008820: 6c74 3a0a 2020 2020 2020 2020 6966 2022  lt:.        if "
+00008830: 6572 726f 725f 6d73 6722 2069 6e20 7265  error_msg" in re
+00008840: 7375 6c74 5b22 7265 7375 6c74 225d 3a0a  sult["result"]:.
+00008850: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+00008860: 725f 6d73 6720 3d20 7265 7375 6c74 5b22  r_msg = result["
+00008870: 7265 7375 6c74 225d 5b22 6572 726f 725f  result"]["error_
+00008880: 6d73 6722 5d0a 2020 2020 2020 2020 7261  msg"].        ra
+00008890: 6973 6520 4578 6365 7074 696f 6e28 6572  ise Exception(er
+000088a0: 726f 725f 6d73 6729 0a20 2020 2065 6c73  ror_msg).    els
+000088b0: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
+000088c0: 2045 7863 6570 7469 6f6e 2866 224e 6f20   Exception(f"No 
+000088d0: 2772 6573 756c 7427 206b 6579 2069 6e20  'result' key in 
+000088e0: 7265 7375 6c74 3a20 7b72 6573 756c 747d  result: {result}
+000088f0: 2229 0a0a 0a64 6566 205f 5f62 6173 6562  ")...def __baseb
+00008900: 6f78 6573 5f76 6572 6966 6963 6174 696f  oxes_verificatio
+00008910: 6e5f 7761 6974 5f75 6e74 696c 5f63 6f6d  n_wait_until_com
+00008920: 706c 6574 6528 0a20 2020 2074 6173 6b5f  plete(.    task_
+00008930: 6964 3a20 7374 722c 206c 6f67 5f73 7566  id: str, log_suf
+00008940: 6669 783a 2073 7472 203d 204e 6f6e 652c  fix: str = None,
+00008950: 2074 696d 656f 7574 3a20 696e 7420 3d20   timeout: int = 
+00008960: 3336 3030 0a29 202d 3e20 6469 6374 3a0a  3600.) -> dict:.
+00008970: 2020 2020 2222 220a 2020 2020 5761 6974      """.    Wait
+00008980: 2075 6e74 696c 2074 6865 2076 6572 6966   until the verif
+00008990: 6963 6174 696f 6e20 7461 736b 2072 6570  ication task rep
+000089a0: 7265 7365 6e74 696e 6720 6279 2069 7473  resenting by its
+000089b0: 2069 6420 6973 2063 6f6d 706c 6574 6564   id is completed
+000089c0: 0a20 2020 203a 7061 7261 6d20 7461 736b  .    :param task
+000089d0: 5f69 643a 2074 6865 2074 6173 6b20 6964  _id: the task id
+000089e0: 0a20 2020 203a 7061 7261 6d20 6c6f 675f  .    :param log_
+000089f0: 7375 6666 6978 3a20 7768 6174 2074 6f20  suffix: what to 
+00008a00: 696e 7365 7274 2069 6e74 6f20 7468 6520  insert into the 
+00008a10: 6c6f 670a 2020 2020 3a70 6172 616d 2074  log.    :param t
+00008a20: 696d 656f 7574 3a20 7468 6520 7469 6d65  imeout: the time
+00008a30: 6f75 7420 746f 2073 746f 7020 7468 6520  out to stop the 
+00008a40: 7461 736b 0a20 2020 203a 7265 7475 726e  task.    :return
+00008a50: 3a20 7468 6520 7265 7375 6c74 206f 6620  : the result of 
+00008a60: 7468 6520 6261 7365 626f 7820 7665 7269  the basebox veri
+00008a70: 6669 6361 7469 6f6e 0a20 2020 2022 2222  fication.    """
+00008a80: 0a0a 2020 2020 7374 6172 745f 7469 6d65  ..    start_time
+00008a90: 203d 2074 696d 652e 7469 6d65 2829 0a0a   = time.time()..
+00008aa0: 2020 2020 6669 6e69 7368 6564 203d 2046      finished = F
+00008ab0: 616c 7365 0a20 2020 2077 6869 6c65 206e  alse.    while n
+00008ac0: 6f74 2028 6669 6e69 7368 6564 206f 7220  ot (finished or 
+00008ad0: 2874 696d 652e 7469 6d65 2829 202d 2073  (time.time() - s
+00008ae0: 7461 7274 5f74 696d 6529 203e 2074 696d  tart_time) > tim
+00008af0: 656f 7574 293a 0a20 2020 2020 2020 2074  eout):.        t
+00008b00: 696d 652e 736c 6565 7028 3229 0a20 2020  ime.sleep(2).   
+00008b10: 2020 2020 2063 7572 7265 6e74 5f74 696d       current_tim
+00008b20: 6520 3d20 7469 6d65 2e74 696d 6528 290a  e = time.time().
+00008b30: 2020 2020 2020 2020 656c 6170 7365 6420          elapsed 
+00008b40: 3d20 696e 7428 6375 7272 656e 745f 7469  = int(current_ti
+00008b50: 6d65 202d 2073 7461 7274 5f74 696d 6529  me - start_time)
+00008b60: 0a20 2020 2020 2020 2069 6620 6c6f 675f  .        if log_
+00008b70: 7375 6666 6978 2069 7320 6e6f 7420 4e6f  suffix is not No
+00008b80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00008b90: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+00008ba0: 2020 2020 2020 2020 2020 2020 2066 2220               f" 
+00008bb0: 2020 5b2b 5d20 4375 7272 656e 746c 7920    [+] Currently 
+00008bc0: 7665 7269 6679 696e 6720 7b6c 6f67 5f73  verifying {log_s
+00008bd0: 7566 6669 787d 2066 6f72 207b 656c 6170  uffix} for {elap
+00008be0: 7365 647d 2073 6563 6f6e 6473 2028 7469  sed} seconds (ti
+00008bf0: 6d65 6f75 7420 6174 207b 7469 6d65 6f75  meout at {timeou
+00008c00: 747d 2073 6563 6f6e 6473 2922 0a20 2020  t} seconds)".   
+00008c10: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00008c20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00008c30: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+00008c40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008c50: 2020 6622 2020 205b 2b5d 2043 7572 7265    f"   [+] Curre
+00008c60: 6e74 6c79 2072 756e 6e69 6e67 2074 6865  ntly running the
+00008c70: 2076 6572 6966 6963 6174 696f 6e20 666f   verification fo
+00008c80: 7220 7b65 6c61 7073 6564 7d20 7365 636f  r {elapsed} seco
+00008c90: 6e64 7322 0a20 2020 2020 2020 2020 2020  nds".           
+00008ca0: 2029 0a0a 2020 2020 2020 2020 7265 7375   )..        resu
+00008cb0: 6c74 203d 205f 706f 7374 2822 2f62 6173  lt = _post("/bas
+00008cc0: 6562 6f78 2f73 7461 7475 735f 7665 7269  ebox/status_veri
+00008cd0: 6679 222c 2064 6174 613d 7b22 7461 736b  fy", data={"task
+00008ce0: 5f69 6422 3a20 7461 736b 5f69 647d 290a  _id": task_id}).
+00008cf0: 2020 2020 2020 2020 7265 7375 6c74 2e72          result.r
+00008d00: 6169 7365 5f66 6f72 5f73 7461 7475 7328  aise_for_status(
+00008d10: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
+00008d20: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
+00008d30: 0a0a 2020 2020 2020 2020 6966 2022 7374  ..        if "st
+00008d40: 6174 7573 2220 696e 2072 6573 756c 743a  atus" in result:
+00008d50: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
+00008d60: 7265 6e74 5f73 7461 7475 7320 3d20 7265  rent_status = re
+00008d70: 7375 6c74 5b22 7374 6174 7573 225d 0a0a  sult["status"]..
+00008d80: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00008d90: 7572 7265 6e74 5f73 7461 7475 7320 3d3d  urrent_status ==
+00008da0: 2022 4552 524f 5222 3a0a 2020 2020 2020   "ERROR":.      
+00008db0: 2020 2020 2020 2020 2020 6572 726f 725f            error_
+00008dc0: 6d65 7373 6167 6520 3d20 7265 7375 6c74  message = result
+00008dd0: 5b22 6572 726f 725f 6d73 6722 5d0a 2020  ["error_msg"].  
+00008de0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00008df0: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
+00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e10: 2020 2066 2245 7272 6f72 2064 7572 696e     f"Error durin
+00008e20: 6720 7665 7269 6669 6361 7469 6f6e 206f  g verification o
+00008e30: 7065 7261 7469 6f6e 3a20 277b 6572 726f  peration: '{erro
+00008e40: 725f 6d65 7373 6167 657d 2722 0a20 2020  r_message}'".   
+00008e50: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00008e60: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00008e70: 6375 7272 656e 745f 7374 6174 7573 203d  current_status =
+00008e80: 3d20 2246 494e 4953 4845 4422 3a0a 2020  = "FINISHED":.  
+00008e90: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00008ea0: 6e69 7368 6564 203d 2054 7275 650a 0a20  nished = True.. 
+00008eb0: 2020 2069 6620 6e6f 7420 6669 6e69 7368     if not finish
+00008ec0: 6564 3a0a 2020 2020 2020 2020 6572 726f  ed:.        erro
+00008ed0: 725f 6d73 6720 3d20 6622 5b2d 5d20 556e  r_msg = f"[-] Un
+00008ee0: 6162 6c65 2074 6f20 7465 726d 696e 6174  able to terminat
+00008ef0: 6520 6f70 6572 6174 696f 6e20 6265 666f  e operation befo
+00008f00: 7265 2074 696d 656f 7574 206f 6620 7b74  re timeout of {t
+00008f10: 696d 656f 7574 7d20 7365 636f 6e64 732e  imeout} seconds.
+00008f20: 2053 746f 7070 696e 6720 6f70 6572 6174   Stopping operat
+00008f30: 696f 6e2e 220a 2020 2020 2020 2020 7265  ion.".        re
+00008f40: 7375 6c74 203d 2076 6572 6966 795f 6261  sult = verify_ba
+00008f50: 7365 626f 785f 7374 6f70 2874 6173 6b5f  sebox_stop(task_
+00008f60: 6964 290a 2020 2020 2020 2020 7374 6f70  id).        stop
+00008f70: 7065 6420 3d20 7265 7375 6c74 5b22 7374  ped = result["st
+00008f80: 6174 7573 225d 203d 3d20 2253 544f 5050  atus"] == "STOPP
+00008f90: 4544 220a 2020 2020 2020 2020 6966 2073  ED".        if s
+00008fa0: 746f 7070 6564 3a0a 2020 2020 2020 2020  topped:.        
+00008fb0: 2020 2020 7265 7375 6c74 5b22 7265 7375      result["resu
+00008fc0: 6c74 225d 203d 2064 6963 7428 290a 2020  lt"] = dict().  
+00008fd0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00008fe0: 5b22 7265 7375 6c74 225d 5b22 6572 726f  ["result"]["erro
+00008ff0: 725f 6d73 6722 5d20 3d20 6572 726f 725f  r_msg"] = error_
+00009000: 6d73 670a 2020 2020 2020 2020 2020 2020  msg.            
+00009010: 7265 7475 726e 2072 6573 756c 740a 2020  return result.  
+00009020: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009030: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+00009040: 6365 7074 696f 6e28 2255 6e61 626c 6520  ception("Unable 
+00009050: 746f 2073 746f 7020 7665 7269 6669 6361  to stop verifica
+00009060: 7469 6f6e 2074 6173 6b22 290a 0a20 2020  tion task")..   
+00009070: 2072 6573 756c 7420 3d20 5f70 6f73 7428   result = _post(
+00009080: 222f 6261 7365 626f 782f 7265 7375 6c74  "/basebox/result
+00009090: 5f76 6572 6966 7922 2c20 6461 7461 3d7b  _verify", data={
+000090a0: 2274 6173 6b5f 6964 223a 2074 6173 6b5f  "task_id": task_
+000090b0: 6964 7d29 0a20 2020 2072 6573 756c 742e  id}).    result.
+000090c0: 7261 6973 655f 666f 725f 7374 6174 7573  raise_for_status
+000090d0: 2829 0a20 2020 2072 6573 756c 7420 3d20  ().    result = 
+000090e0: 7265 7375 6c74 2e6a 736f 6e28 290a 0a20  result.json().. 
+000090f0: 2020 2073 7563 6365 7373 203d 2072 6573     success = res
 00009100: 756c 745b 2273 7461 7475 7322 5d20 3d3d  ult["status"] ==
-00009110: 2022 5255 4e4e 494e 4722 0a20 2020 2020   "RUNNING".     
-00009120: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
-00009130: 0a0a 2020 2020 6966 206e 6f74 2072 756e  ..    if not run
-00009140: 6e69 6e67 3a0a 2020 2020 2020 2020 6c6f  ning:.        lo
-00009150: 6767 6572 2e65 7272 6f72 280a 2020 2020  gger.error(.    
-00009160: 2020 2020 2020 2020 6622 5b2d 5d20 556e          f"[-] Un
-00009170: 6162 6c65 2074 6f20 7374 6172 7420 6f70  able to start op
-00009180: 6572 6174 696f 6e20 6265 666f 7265 2074  eration before t
-00009190: 696d 656f 7574 206f 6620 7b74 696d 656f  imeout of {timeo
-000091a0: 7574 7d20 7365 636f 6e64 7322 0a20 2020  ut} seconds".   
-000091b0: 2020 2020 2029 0a0a 2020 2020 7265 7475       )..    retu
-000091c0: 726e 2072 756e 6e69 6e67 0a0a 0a64 6566  rn running...def
-000091d0: 205f 5f68 616e 646c 655f 7761 6974 280a   __handle_wait(.
-000091e0: 2020 2020 7761 6974 3a20 626f 6f6c 2c20      wait: bool, 
-000091f0: 7461 736b 5f69 643a 2073 7472 2c20 6c6f  task_id: str, lo
-00009200: 675f 7375 6666 6978 3a20 7374 722c 2074  g_suffix: str, t
-00009210: 696d 656f 7574 3a20 696e 7420 3d20 3336  imeout: int = 36
-00009220: 3030 0a29 202d 3e20 626f 6f6c 3a0a 2020  00.) -> bool:.  
-00009230: 2020 2222 220a 0a20 2020 203a 7061 7261    """..    :para
-00009240: 6d20 7761 6974 3a20 5761 6974 2066 6f72  m wait: Wait for
-00009250: 2074 6865 206f 7065 7261 7469 6f6e 2074   the operation t
-00009260: 6f20 6265 2063 6f6d 706c 6574 6564 2069  o be completed i
-00009270: 6e20 6261 636b 656e 640a 2020 2020 3a70  n backend.    :p
-00009280: 6172 616d 2074 6173 6b5f 6964 3a20 7468  aram task_id: th
-00009290: 6520 7461 736b 2069 640a 2020 2020 3a70  e task id.    :p
-000092a0: 6172 616d 206c 6f67 5f73 7566 6669 783a  aram log_suffix:
-000092b0: 2074 6865 2073 7472 696e 6720 746f 2062   the string to b
-000092c0: 6520 696e 7365 7274 6564 2069 6e20 7468  e inserted in th
-000092d0: 6520 6c6f 670a 2020 2020 3a70 6172 616d  e log.    :param
-000092e0: 2074 696d 656f 7574 3a20 7468 6520 7469   timeout: the ti
-000092f0: 6d65 206c 696d 6974 2062 6566 6f72 6520  me limit before 
-00009300: 7374 6f70 7069 6e67 2074 6865 2074 6173  stopping the tas
-00009310: 6b0a 2020 2020 3a72 6574 7572 6e3a 2074  k.    :return: t
-00009320: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
-00009330: 2076 6572 6966 6963 6174 696f 6e0a 2020   verification.  
-00009340: 2020 2222 220a 2020 2020 7375 6363 6573    """.    succes
-00009350: 7320 3d20 5472 7565 0a0a 2020 2020 6966  s = True..    if
-00009360: 2077 6169 743a 0a20 2020 2020 2020 2023   wait:.        #
-00009370: 2057 6169 7420 666f 7220 7468 6520 6f70   Wait for the op
-00009380: 6572 6174 696f 6e20 746f 2062 6520 636f  eration to be co
-00009390: 6d70 6c65 7465 6420 696e 2062 6163 6b65  mpleted in backe
-000093a0: 6e64 0a0a 2020 2020 2020 2020 7265 7375  nd..        resu
-000093b0: 6c74 203d 205f 5f62 6173 6562 6f78 6573  lt = __baseboxes
-000093c0: 5f76 6572 6966 6963 6174 696f 6e5f 7761  _verification_wa
-000093d0: 6974 5f75 6e74 696c 5f63 6f6d 706c 6574  it_until_complet
-000093e0: 6528 0a20 2020 2020 2020 2020 2020 2074  e(.            t
-000093f0: 6173 6b5f 6964 3d74 6173 6b5f 6964 2c20  ask_id=task_id, 
-00009400: 6c6f 675f 7375 6666 6978 3d6c 6f67 5f73  log_suffix=log_s
-00009410: 7566 6669 782c 2074 696d 656f 7574 3d74  uffix, timeout=t
-00009420: 696d 656f 7574 0a20 2020 2020 2020 2029  imeout.        )
-00009430: 0a0a 2020 2020 2020 2020 6669 6e69 7368  ..        finish
-00009440: 6564 203d 2022 7374 6174 7573 2220 696e  ed = "status" in
-00009450: 2072 6573 756c 7420 616e 6420 7265 7375   result and resu
-00009460: 6c74 5b22 7374 6174 7573 225d 203d 3d20  lt["status"] == 
-00009470: 2246 494e 4953 4845 4422 0a20 2020 2020  "FINISHED".     
-00009480: 2020 2073 7563 6365 7373 203d 2066 696e     success = fin
-00009490: 6973 6865 640a 0a20 2020 2020 2020 2069  ished..        i
-000094a0: 6620 7375 6363 6573 733a 0a20 2020 2020  f success:.     
-000094b0: 2020 2020 2020 2069 6620 2272 6573 756c         if "resul
-000094c0: 7422 2069 6e20 7265 7375 6c74 3a0a 2020  t" in result:.  
-000094d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000094e0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-000094f0: 2020 2020 2069 6620 6e6f 7420 7375 6363       if not succ
-00009500: 6573 733a 0a20 2020 2020 2020 2020 2020  ess:.           
-00009510: 205f 7261 6973 655f 6572 726f 725f 6d73   _raise_error_ms
-00009520: 6728 7265 7375 6c74 290a 0a20 2020 2065  g(result)..    e
-00009530: 6c73 653a 0a20 2020 2020 2020 2023 2077  lse:.        # w
-00009540: 6169 7420 666f 7220 7468 6520 6f70 6572  ait for the oper
-00009550: 6174 696f 6e20 746f 2073 7461 7274 0a20  ation to start. 
-00009560: 2020 2020 2020 2072 756e 6e69 6e67 203d         running =
-00009570: 205f 5f77 6169 745f 666f 725f 7468 655f   __wait_for_the_
-00009580: 6f70 6572 6174 696f 6e5f 746f 5f73 7461  operation_to_sta
-00009590: 7274 2874 6173 6b5f 6964 290a 0a20 2020  rt(task_id)..   
-000095a0: 2020 2020 2069 6620 6e6f 7420 7275 6e6e       if not runn
-000095b0: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-000095c0: 2073 7563 6365 7373 203d 2046 616c 7365   success = False
-000095d0: 0a0a 2020 2020 7265 7475 726e 2073 7563  ..    return suc
-000095e0: 6365 7373 0a0a 0a23 202d 2d2d 2d2d 2d2d  cess...# -------
-000095f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009630: 2d2d 2d20 230a 2320 436f 7265 2041 5049  --- #.# Core API
-00009640: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .# -------------
-00009650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 230a  ------------- #.
-00009690: 0a0a 6465 6620 6765 745f 7665 7273 696f  ..def get_versio
-000096a0: 6e28 2920 2d3e 2073 7472 3a0a 2020 2020  n() -> str:.    
-000096b0: 2222 2252 6574 7572 6e20 436f 7265 2041  """Return Core A
-000096c0: 5049 2076 6572 7369 6f6e 2e22 2222 0a0a  PI version."""..
-000096d0: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
-000096e0: 7428 222f 7369 6d75 6c61 7469 6f6e 2f76  t("/simulation/v
-000096f0: 6572 7369 6f6e 2229 0a0a 2020 2020 6966  ersion")..    if
-00009700: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-00009710: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-00009720: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-00009730: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
-00009740: 7420 7265 7472 6965 7665 2043 6f72 6520  t retrieve Core 
-00009750: 4150 4920 7665 7273 696f 6e22 290a 0a20  API version").. 
-00009760: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00009770: 2e6a 736f 6e28 290a 0a0a 6465 6620 7265  .json()...def re
-00009780: 7365 7428 6465 6c65 7465 5f63 6f6d 7075  set(delete_compu
-00009790: 7465 5f73 6572 7665 7273 3a20 626f 6f6c  te_servers: bool
-000097a0: 203d 2046 616c 7365 2920 2d3e 2041 6e79   = False) -> Any
-000097b0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-000097c0: 7365 7420 7468 6520 4954 2053 696d 756c  set the IT Simul
-000097d0: 6174 696f 6e20 696e 6672 6173 7472 7563  ation infrastruc
-000097e0: 7475 7265 0a0a 2020 2020 5468 6973 2068  ture..    This h
-000097f0: 6173 2074 6865 2066 6f6c 6c6f 7769 6e67  as the following
-00009800: 2065 6666 6563 743a 0a20 2020 202d 2063   effect:.    - c
-00009810: 6c65 616e 2074 6865 2064 6174 6162 6173  lean the databas
-00009820: 6520 616e 6420 7265 2d70 6f70 756c 6174  e and re-populat
-00009830: 6520 6974 2077 6974 6820 7374 6174 6963  e it with static
-00009840: 2069 6e66 6f20 2862 6173 6562 6f78 6573   info (baseboxes
-00009850: 2c20 726f 6c65 732e 2e2e 290a 2020 2020  , roles...).    
-00009860: 2d20 6279 2064 6566 6175 742c 2074 6865  - by defaut, the
-00009870: 2074 6162 6c65 206f 6620 636f 6d70 7574   table of comput
-00009880: 6520 7365 7276 6572 7320 6973 206b 6570  e servers is kep
-00009890: 742c 2062 7574 2060 6465 6c65 7465 5f63  t, but `delete_c
-000098a0: 6f6d 7075 7465 5f73 6572 7665 7273 3d54  ompute_servers=T
-000098b0: 7275 6560 2063 6861 6e67 6573 2074 6861  rue` changes tha
-000098c0: 7420 6265 6861 7669 6f72 0a20 2020 202d  t behavior.    -
-000098d0: 2072 6573 6574 2074 6865 2073 696d 756c   reset the simul
-000098e0: 6174 696f 6e20 6d61 6e61 6765 720a 2020  ation manager.  
-000098f0: 2020 2d20 7265 7365 7420 7468 6520 636f    - reset the co
-00009900: 6d70 7574 6520 7365 7276 6572 7320 2873  mpute servers (s
-00009910: 746f 7020 564d 7320 616e 6420 646f 636b  top VMs and dock
-00009920: 6572 732c 2072 6573 6574 206e 6574 776f  ers, reset netwo
-00009930: 726b 732c 202e 2e2e 290a 2020 2020 2222  rks, ...).    ""
-00009940: 220a 2020 2020 7061 7261 6d73 203d 207b  ".    params = {
-00009950: 7d0a 2020 2020 6966 2064 656c 6574 655f  }.    if delete_
-00009960: 636f 6d70 7574 655f 7365 7276 6572 733a  compute_servers:
-00009970: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00009980: 3d20 7b22 6465 6c65 7465 5f63 6f6d 7075  = {"delete_compu
-00009990: 7465 5f73 6572 7665 7273 5f66 726f 6d5f  te_servers_from_
-000099a0: 6462 223a 2064 656c 6574 655f 636f 6d70  db": delete_comp
-000099b0: 7574 655f 7365 7276 6572 737d 0a0a 2020  ute_servers}..  
-000099c0: 2020 7265 7375 6c74 203d 205f 6465 6c65    result = _dele
-000099d0: 7465 2822 2f73 696d 756c 6174 696f 6e2f  te("/simulation/
-000099e0: 636f 6d70 7574 655f 696e 6672 6173 7472  compute_infrastr
-000099f0: 7563 7475 7265 5f72 6573 6574 222c 2070  ucture_reset", p
-00009a00: 6172 616d 733d 7061 7261 6d73 290a 0a20  arams=params).. 
-00009a10: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-00009a20: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-00009a30: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-00009a40: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-00009a50: 4361 6e6e 6f74 2072 6573 6574 2073 696d  Cannot reset sim
-00009a60: 756c 6174 696f 6e20 696e 6672 6173 7472  ulation infrastr
-00009a70: 7563 7475 7265 2229 0a0a 2020 2020 7265  ucture")..    re
-00009a80: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
-00009a90: 2829 0a0a 0a64 6566 205f 6372 6561 7465  ()...def _create
-00009aa0: 5f6f 725f 6578 7465 6e64 5f73 696d 756c  _or_extend_simul
-00009ab0: 6174 696f 6e28 0a20 2020 2073 696d 756c  ation(.    simul
-00009ac0: 6174 696f 6e5f 6469 6374 3a20 6469 6374  ation_dict: dict
-00009ad0: 2c0a 2020 2020 6964 5f73 696d 756c 6174  ,.    id_simulat
-00009ae0: 696f 6e3a 2069 6e74 203d 204e 6f6e 652c  ion: int = None,
-00009af0: 0a20 2020 2061 6c6c 6f63 6174 696f 6e5f  .    allocation_
-00009b00: 7374 7261 7465 6779 3a20 4f70 7469 6f6e  strategy: Option
-00009b10: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-00009b20: 2920 2d3e 2069 6e74 3a0a 2020 2020 2222  ) -> int:.    ""
-00009b30: 2243 7265 6174 6520 6120 7369 6d75 6c61  "Create a simula
-00009b40: 7469 6f6e 2c20 6f72 2065 7874 656e 6420  tion, or extend 
-00009b50: 616e 2065 7869 7374 696e 6720 7369 6d75  an existing simu
-00009b60: 6c61 7469 6f6e 2077 6974 6820 6e65 770a  lation with new.
-00009b70: 2020 2020 6e6f 6465 7320 616e 6420 6c69      nodes and li
-00009b80: 6e6b 732c 2061 6e64 2072 6574 7572 6e20  nks, and return 
-00009b90: 6120 7369 6d75 6c61 7469 6f6e 2049 442e  a simulation ID.
-00009ba0: 2222 220a 0a20 2020 2023 2047 6574 2074  """..    # Get t
-00009bb0: 6865 2070 6174 6873 2069 6620 736f 6d65  he paths if some
-00009bc0: 2068 6176 6520 6265 656e 2070 726f 7669   have been provi
-00009bd0: 6465 640a 2020 2020 7265 736f 7572 6365  ded.    resource
-00009be0: 735f 7061 7468 7320 3d20 7369 6d75 6c61  s_paths = simula
-00009bf0: 7469 6f6e 5f64 6963 742e 706f 7028 2272  tion_dict.pop("r
-00009c00: 6573 6f75 7263 6573 5f70 6174 6873 222c  esources_paths",
-00009c10: 205b 5d29 0a0a 2020 2020 6461 7461 203d   [])..    data =
-00009c20: 206a 736f 6e2e 6475 6d70 7328 7369 6d75   json.dumps(simu
-00009c30: 6c61 7469 6f6e 5f64 6963 7429 0a0a 2020  lation_dict)..  
-00009c40: 2020 2320 4372 6561 7469 6f6e 206f 6620    # Creation of 
-00009c50: 6120 666f 6c64 6572 2063 6f6e 7461 696e  a folder contain
-00009c60: 696e 6720 616c 6c20 7468 6520 7265 736f  ing all the reso
-00009c70: 7572 6365 732c 2074 6869 7320 666f 6c64  urces, this fold
-00009c80: 6572 2077 696c 6c20 7468 656e 2062 6520  er will then be 
-00009c90: 7a69 7070 6564 0a20 2020 2077 6974 6820  zipped.    with 
-00009ca0: 5465 6d70 6f72 6172 7944 6972 6563 746f  TemporaryDirecto
-00009cb0: 7279 2870 7265 6669 783d 2263 7962 6572  ry(prefix="cyber
-00009cc0: 5f72 616e 6765 5f63 725f 636f 7265 5f72  _range_cr_core_r
-00009cd0: 6573 6f75 7263 6573 2229 2061 7320 6d61  esources") as ma
-00009ce0: 696e 5f72 6573 6f75 7263 6573 3a0a 0a20  in_resources:.. 
-00009cf0: 2020 2020 2020 2023 2063 6f70 7920 616c         # copy al
-00009d00: 6c20 7265 736f 7572 6365 7320 696e 2074  l resources in t
-00009d10: 6865 206d 6169 6e20 7465 6d70 6f72 6172  he main temporar
-00009d20: 7920 666f 6c64 6572 0a20 2020 2020 2020  y folder.       
-00009d30: 2066 6f72 2072 6573 6f75 7263 6520 696e   for resource in
-00009d40: 2072 6573 6f75 7263 6573 5f70 6174 6873   resources_paths
-00009d50: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00009d60: 206f 732e 7061 7468 2e69 7364 6972 2872   os.path.isdir(r
-00009d70: 6573 6f75 7263 6529 3a0a 2020 2020 2020  esource):.      
-00009d80: 2020 2020 2020 2020 2020 7368 7574 696c            shutil
-00009d90: 2e63 6f70 7974 7265 6528 0a20 2020 2020  .copytree(.     
-00009da0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009db0: 6573 6f75 7263 652c 0a20 2020 2020 2020  esource,.       
-00009dc0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00009dd0: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
-00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009df0: 2020 206d 6169 6e5f 7265 736f 7572 6365     main_resource
-00009e00: 732c 206f 732e 7061 7468 2e62 6173 656e  s, os.path.basen
-00009e10: 616d 6528 6f73 2e70 6174 682e 6e6f 726d  ame(os.path.norm
-00009e20: 7061 7468 2872 6573 6f75 7263 6529 290a  path(resource)).
-00009e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e40: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00009e50: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00009e60: 2020 2020 2065 6c69 6620 6f73 2e70 6174       elif os.pat
-00009e70: 682e 6973 6669 6c65 2872 6573 6f75 7263  h.isfile(resourc
-00009e80: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00009e90: 2020 2020 7368 7574 696c 2e63 6f70 7966      shutil.copyf
-00009ea0: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
-00009eb0: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
-00009ec0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00009ed0: 2020 2020 2020 206f 732e 7061 7468 2e6a         os.path.j
-00009ee0: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-00009ef0: 2020 2020 2020 2020 2020 2020 206d 6169               mai
-00009f00: 6e5f 7265 736f 7572 6365 732c 206f 732e  n_resources, os.
-00009f10: 7061 7468 2e62 6173 656e 616d 6528 6f73  path.basename(os
-00009f20: 2e70 6174 682e 6e6f 726d 7061 7468 2872  .path.normpath(r
-00009f30: 6573 6f75 7263 6529 290a 2020 2020 2020  esource)).      
-00009f40: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-00009f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009f60: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
-00009f70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009f80: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00009f90: 7469 6f6e 2866 2243 616e 206e 6f74 2063  tion(f"Can not c
-00009fa0: 6f70 7920 7b72 6573 6f75 7263 657d 2229  opy {resource}")
-00009fb0: 0a0a 2020 2020 2020 2020 2320 5765 2068  ..        # We h
-00009fc0: 6176 6520 746f 2063 7265 6174 6520 6120  ave to create a 
-00009fd0: 6e65 7720 7465 6d70 6f72 6172 7920 666f  new temporary fo
-00009fe0: 6c64 6572 2074 6f20 686f 7374 2074 6865  lder to host the
-00009ff0: 2061 7263 6869 7665 0a20 2020 2020 2020   archive.       
-0000a000: 2077 6974 6820 5465 6d70 6f72 6172 7944   with TemporaryD
-0000a010: 6972 6563 746f 7279 2870 7265 6669 783d  irectory(prefix=
-0000a020: 2263 7962 6572 5f72 616e 6765 5f63 725f  "cyber_range_cr_
-0000a030: 636f 7265 5f61 7263 6869 7665 2229 2061  core_archive") a
-0000a040: 7320 7465 6d70 5f64 6972 3a0a 2020 2020  s temp_dir:.    
-0000a050: 2020 2020 2020 2020 7a69 705f 6669 6c65          zip_file
-0000a060: 5f6e 616d 6520 3d20 5f7a 6970 5f72 6573  _name = _zip_res
-0000a070: 6f75 7263 6573 286d 6169 6e5f 7265 736f  ources(main_reso
-0000a080: 7572 6365 732c 2074 656d 705f 6469 7229  urces, temp_dir)
-0000a090: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000a0a0: 6f75 7263 6573 5f66 696c 6520 3d20 6f70  ources_file = op
-0000a0b0: 656e 287a 6970 5f66 696c 655f 6e61 6d65  en(zip_file_name
-0000a0c0: 2c20 2272 6222 290a 2020 2020 2020 2020  , "rb").        
-0000a0d0: 2020 2020 6669 6c65 7320 3d20 7b22 7265      files = {"re
-0000a0e0: 736f 7572 6365 735f 6669 6c65 223a 2072  sources_file": r
-0000a0f0: 6573 6f75 7263 6573 5f66 696c 652c 2022  esources_file, "
-0000a100: 6461 7461 223a 2064 6174 617d 0a20 2020  data": data}.   
-0000a110: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-0000a120: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000a130: 2069 645f 7369 6d75 6c61 7469 6f6e 2069   id_simulation i
-0000a140: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000a150: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
-0000a160: 6561 7465 206e 6577 2073 696d 756c 6174  eate new simulat
-0000a170: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000a180: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000a190: 205f 706f 7374 280a 2020 2020 2020 2020   _post(.        
-0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1b0: 222f 7369 6d75 6c61 7469 6f6e 2f22 2c0a  "/simulation/",.
-0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1d0: 2020 2020 2020 2020 6669 6c65 733d 6669          files=fi
-0000a1e0: 6c65 732c 0a20 2020 2020 2020 2020 2020  les,.           
-0000a1f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000a200: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000a210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a220: 2020 2020 2023 2045 7874 656e 6420 616e       # Extend an
-0000a230: 2065 7869 7374 696e 6720 7369 6d75 6c61   existing simula
-0000a240: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0000a250: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-0000a260: 3d20 5f70 6f73 7428 0a20 2020 2020 2020  = _post(.       
-0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a280: 2066 222f 7369 6d75 6c61 7469 6f6e 2f7b   f"/simulation/{
-0000a290: 6964 5f73 696d 756c 6174 696f 6e7d 2f65  id_simulation}/e
-0000a2a0: 7874 656e 6422 2c0a 2020 2020 2020 2020  xtend",.        
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 6669 6c65 733d 6669 6c65 732c 0a20 2020  files=files,.   
-0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2e0: 2029 0a20 2020 2020 2020 2020 2020 2066   ).            f
-0000a2f0: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
-0000a300: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-0000a310: 735f 6669 6c65 2e63 6c6f 7365 2829 0a0a  s_file.close()..
-0000a320: 2020 2020 6966 206e 6f74 206d 6169 6e5f      if not main_
-0000a330: 7265 736f 7572 6365 733a 0a20 2020 2020  resources:.     
-0000a340: 2020 2069 6620 6964 5f73 696d 756c 6174     if id_simulat
-0000a350: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-0000a360: 2020 2020 2020 2020 2023 2043 7265 6174           # Creat
-0000a370: 6520 6e65 7720 7369 6d75 6c61 7469 6f6e  e new simulation
-0000a380: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000a390: 756c 7420 3d20 5f70 6f73 7428 0a20 2020  ult = _post(.   
-0000a3a0: 2020 2020 2020 2020 2020 2020 2022 2f73               "/s
-0000a3b0: 696d 756c 6174 696f 6e2f 222c 0a20 2020  imulation/",.   
-0000a3c0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-0000a3d0: 613d 6461 7461 2c0a 2020 2020 2020 2020  a=data,.        
-0000a3e0: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
-0000a3f0: 7b22 436f 6e74 656e 742d 5479 7065 223a  {"Content-Type":
-0000a400: 2022 6170 706c 6963 6174 696f 6e2f 6a73   "application/js
-0000a410: 6f6e 227d 2c0a 2020 2020 2020 2020 2020  on"},.          
-0000a420: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
-0000a430: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000a440: 4578 7465 6e64 2061 6e20 6578 6973 7469  Extend an existi
-0000a450: 6e67 2073 696d 756c 6174 696f 6e0a 2020  ng simulation.  
-0000a460: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000a470: 203d 205f 706f 7374 280a 2020 2020 2020   = _post(.      
-0000a480: 2020 2020 2020 2020 2020 6622 2f73 696d            f"/sim
-0000a490: 756c 6174 696f 6e2f 7b69 645f 7369 6d75  ulation/{id_simu
-0000a4a0: 6c61 7469 6f6e 7d2f 6578 7465 6e64 222c  lation}/extend",
-0000a4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a4c0: 2064 6174 613d 6461 7461 2c0a 2020 2020   data=data,.    
-0000a4d0: 2020 2020 2020 2020 2020 2020 6865 6164              head
-0000a4e0: 6572 733d 7b22 436f 6e74 656e 742d 5479  ers={"Content-Ty
-0000a4f0: 7065 223a 2022 6170 706c 6963 6174 696f  pe": "applicatio
-0000a500: 6e2f 6a73 6f6e 227d 2c0a 2020 2020 2020  n/json"},.      
-0000a510: 2020 2020 2020 290a 0a20 2020 2069 6620        )..    if 
-0000a520: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-0000a530: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-0000a540: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-0000a550: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-0000a560: 2070 6f73 7420 7369 6d75 6c61 7469 6f6e   post simulation
-0000a570: 2069 6e66 6f72 6d61 7469 6f6e 2074 6f20   information to 
-0000a580: 636f 7265 2041 5049 2229 0a0a 2020 2020  core API")..    
-0000a590: 6964 5f73 696d 756c 6174 696f 6e20 3d20  id_simulation = 
-0000a5a0: 7265 7375 6c74 2e6a 736f 6e28 295b 2269  result.json()["i
-0000a5b0: 6422 5d0a 2020 2020 6e65 775f 6e6f 6465  d"].    new_node
-0000a5c0: 7320 3d20 7265 7375 6c74 2e6a 736f 6e28  s = result.json(
-0000a5d0: 295b 226e 6577 5f6e 6f64 6573 225d 0a20  )["new_nodes"]. 
-0000a5e0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
-0000a5f0: 225b 2b5d 204e 6577 206e 6f64 6573 2066  "[+] New nodes f
-0000a600: 6f72 2073 696d 756c 6174 696f 6e20 6964  or simulation id
-0000a610: 2027 7b69 645f 7369 6d75 6c61 7469 6f6e   '{id_simulation
-0000a620: 7d27 3a20 277b 6e65 775f 6e6f 6465 737d  }': '{new_nodes}
-0000a630: 2722 290a 0a20 2020 2023 2050 7265 7061  '")..    # Prepa
-0000a640: 7265 2064 6973 6b20 7265 736f 7572 6365  re disk resource
-0000a650: 730a 2020 2020 706f 7374 5f64 6174 6120  s.    post_data 
-0000a660: 3d20 7b22 6e6f 6465 7322 3a20 6e65 775f  = {"nodes": new_
-0000a670: 6e6f 6465 737d 0a20 2020 205f 7369 6d75  nodes}.    _simu
-0000a680: 6c61 7469 6f6e 5f65 7865 6375 7465 5f6f  lation_execute_o
-0000a690: 7065 7261 7469 6f6e 280a 2020 2020 2020  peration(.      
-0000a6a0: 2020 2270 6f73 7422 2c0a 2020 2020 2020    "post",.      
-0000a6b0: 2020 2270 7265 7061 7265 222c 0a20 2020    "prepare",.   
-0000a6c0: 2020 2020 2069 645f 7369 6d75 6c61 7469       id_simulati
-0000a6d0: 6f6e 2c0a 2020 2020 2020 2020 2250 5245  on,.        "PRE
-0000a6e0: 5041 5249 4e47 222c 0a20 2020 2020 2020  PARING",.       
-0000a6f0: 206f 7074 696f 6e61 6c5f 7061 7261 6d31   optional_param1
-0000a700: 3d61 6c6c 6f63 6174 696f 6e5f 7374 7261  =allocation_stra
-0000a710: 7465 6779 2c0a 2020 2020 2020 2020 706f  tegy,.        po
-0000a720: 7374 5f64 6174 613d 706f 7374 5f64 6174  st_data=post_dat
-0000a730: 612c 0a20 2020 2029 0a0a 2020 2020 2320  a,.    )..    # 
-0000a740: 544f 444f 3a20 4368 6563 6b20 7468 6174  TODO: Check that
-0000a750: 2074 6865 2064 6f63 6b65 7220 766f 6c75   the docker volu
-0000a760: 6d65 7320 7468 6174 2077 696c 6c20 6265  mes that will be
-0000a770: 206d 6f75 6e74 6564 2062 7920 7369 6d75   mounted by simu
-0000a780: 5f72 756e 2061 7265 2070 7265 7365 6e74  _run are present
-0000a790: 206f 6e20 7468 6520 6669 6c65 7379 7374   on the filesyst
-0000a7a0: 656d 0a20 2020 2023 2066 6f72 202e 2e2e  em.    # for ...
-0000a7b0: 3a20 5f73 696d 755f 6372 6561 7465 5f76  : _simu_create_v
-0000a7c0: 616c 6964 6174 655f 7265 736f 7572 6365  alidate_resource
-0000a7d0: 735f 6578 6973 7473 2829 0a0a 2020 2020  s_exists()..    
-0000a7e0: 7265 7475 726e 2028 6964 5f73 696d 756c  return (id_simul
-0000a7f0: 6174 696f 6e2c 206e 6577 5f6e 6f64 6573  ation, new_nodes
-0000a800: 290a 0a0a 6465 6620 7369 6d75 6c61 7469  )...def simulati
-0000a810: 6f6e 5f73 7461 7475 7328 6964 5f73 696d  on_status(id_sim
-0000a820: 756c 6174 696f 6e3a 2069 6e74 2920 2d3e  ulation: int) ->
-0000a830: 2073 7472 3a0a 2020 2020 2222 2252 6574   str:.    """Ret
-0000a840: 7572 6e20 6f6e 6c79 2074 6865 2073 7461  urn only the sta
-0000a850: 7475 7320 6f66 2074 6865 2073 696d 756c  tus of the simul
-0000a860: 6174 696f 6e22 2222 0a20 2020 2072 6573  ation""".    res
-0000a870: 756c 7420 3d20 5f67 6574 2866 222f 7369  ult = _get(f"/si
-0000a880: 6d75 6c61 7469 6f6e 2f7b 6964 5f73 696d  mulation/{id_sim
-0000a890: 756c 6174 696f 6e7d 2f73 7461 7475 7322  ulation}/status"
-0000a8a0: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
-0000a8b0: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-0000a8c0: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
-0000a8d0: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
-0000a8e0: 742c 2022 4361 6e6e 6f74 2072 6574 7269  t, "Cannot retri
-0000a8f0: 6576 6520 7369 6d75 6c61 7469 6f6e 2069  eve simulation i
-0000a900: 6e66 6f20 6672 6f6d 2049 5420 5369 6d75  nfo from IT Simu
-0000a910: 6c61 7469 6f6e 2041 5049 2229 0a0a 2020  lation API")..  
-0000a920: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
-0000a930: 6a73 6f6e 2829 0a0a 0a64 6566 2066 6574  json()...def fet
-0000a940: 6368 5f73 696d 756c 6174 696f 6e28 6964  ch_simulation(id
-0000a950: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
-0000a960: 2920 2d3e 2064 6963 743a 0a20 2020 2022  ) -> dict:.    "
-0000a970: 2222 5265 7475 726e 2061 2073 696d 756c  ""Return a simul
-0000a980: 6174 696f 6e20 6469 6374 2067 6976 656e  ation dict given
-0000a990: 2061 2073 696d 756c 6174 696f 6e20 6964   a simulation id
-0000a9a0: 2e22 2222 0a20 2020 2072 6573 756c 7420  .""".    result 
-0000a9b0: 3d20 5f67 6574 2866 222f 7369 6d75 6c61  = _get(f"/simula
-0000a9c0: 7469 6f6e 2f7b 6964 5f73 696d 756c 6174  tion/{id_simulat
-0000a9d0: 696f 6e7d 2229 0a0a 2020 2020 6966 2072  ion}")..    if r
-0000a9e0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-0000a9f0: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-0000aa00: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-0000aa10: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-0000aa20: 7265 7472 6965 7665 2073 696d 756c 6174  retrieve simulat
-0000aa30: 696f 6e20 696e 666f 2066 726f 6d20 4954  ion info from IT
-0000aa40: 2053 696d 756c 6174 696f 6e20 4150 4922   Simulation API"
-0000aa50: 290a 0a20 2020 2073 696d 756c 6174 696f  )..    simulatio
-0000aa60: 6e5f 6469 6374 203d 2072 6573 756c 742e  n_dict = result.
-0000aa70: 6a73 6f6e 2829 0a0a 2020 2020 7265 7475  json()..    retu
-0000aa80: 726e 2073 696d 756c 6174 696f 6e5f 6469  rn simulation_di
-0000aa90: 6374 0a0a 0a64 6566 2066 6574 6368 5f73  ct...def fetch_s
-0000aaa0: 696d 756c 6174 696f 6e73 2829 202d 3e20  imulations() -> 
-0000aab0: 4c69 7374 5b41 6e79 5d3a 0a20 2020 2022  List[Any]:.    "
-0000aac0: 2222 4765 7420 7468 6520 6c69 7374 206f  ""Get the list o
-0000aad0: 6620 7369 6d75 6c61 7469 6f6e 732c 2069  f simulations, i
-0000aae0: 6e63 6c75 6469 6e67 2074 6865 2063 7572  ncluding the cur
-0000aaf0: 7265 6e74 6c79 2072 756e 6e69 6e67 2073  rently running s
-0000ab00: 696d 7561 6c74 696f 6e2c 2061 6c6f 6e67  imualtion, along
-0000ab10: 2077 6974 680a 2020 2020 696e 666f 726d   with.    inform
-0000ab20: 6174 696f 6e20 6f6e 206e 6f64 6573 0a0a  ation on nodes..
-0000ab30: 2020 2020 2222 220a 2020 2020 7265 7375      """.    resu
-0000ab40: 6c74 203d 205f 6765 7428 222f 7369 6d75  lt = _get("/simu
-0000ab50: 6c61 7469 6f6e 2f22 290a 0a20 2020 2069  lation/")..    i
-0000ab60: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
-0000ab70: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
-0000ab80: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
-0000ab90: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
-0000aba0: 6f74 2072 6574 7269 6576 6520 7369 6d75  ot retrieve simu
-0000abb0: 6c61 7469 6f6e 2069 6e66 6f20 6672 6f6d  lation info from
-0000abc0: 2049 5420 5369 6d75 6c61 7469 6f6e 2041   IT Simulation A
-0000abd0: 5049 2229 0a0a 2020 2020 7369 6d75 6c61  PI")..    simula
-0000abe0: 7469 6f6e 5f6c 6973 7420 3d20 7265 7375  tion_list = resu
-0000abf0: 6c74 2e6a 736f 6e28 290a 2020 2020 7265  lt.json().    re
-0000ac00: 7475 726e 2073 696d 756c 6174 696f 6e5f  turn simulation_
-0000ac10: 6c69 7374 0a0a 0a64 6566 2064 656c 6574  list...def delet
-0000ac20: 655f 7369 6d75 6c61 7469 6f6e 2869 645f  e_simulation(id_
-0000ac30: 7369 6d75 6c61 7469 6f6e 3a20 696e 7429  simulation: int)
-0000ac40: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
-0000ac50: 4465 6c65 7465 2061 2073 696d 756c 6174  Delete a simulat
-0000ac60: 696f 6e20 696e 2064 6174 6162 6173 652e  ion in database.
-0000ac70: 2222 220a 0a20 2020 2023 2044 6573 7472  """..    # Destr
-0000ac80: 6f79 2073 696d 756c 6174 696f 6e20 6966  oy simulation if
-0000ac90: 2069 7420 6973 2072 756e 6e69 6e67 0a20   it is running. 
-0000aca0: 2020 2069 6620 7369 6d75 6c61 7469 6f6e     if simulation
-0000acb0: 5f73 7461 7475 7328 6964 5f73 696d 756c  _status(id_simul
-0000acc0: 6174 696f 6e29 203d 3d20 2252 554e 4e49  ation) == "RUNNI
-0000acd0: 4e47 223a 0a0a 2020 2020 2020 2020 6e6f  NG":..        no
-0000ace0: 6465 733a 204c 6973 745b 7374 725d 203d  des: List[str] =
-0000acf0: 205b 5d0a 2020 2020 2020 2020 706f 7374   [].        post
-0000ad00: 5f64 6174 6120 3d20 7b22 6e6f 6465 7322  _data = {"nodes"
-0000ad10: 3a20 6e6f 6465 737d 0a0a 2020 2020 2020  : nodes}..      
-0000ad20: 2020 5f73 696d 756c 6174 696f 6e5f 6578    _simulation_ex
-0000ad30: 6563 7574 655f 6f70 6572 6174 696f 6e28  ecute_operation(
-0000ad40: 0a20 2020 2020 2020 2020 2020 2022 706f  .            "po
-0000ad50: 7374 222c 2022 6465 7374 726f 7922 2c20  st", "destroy", 
-0000ad60: 6964 5f73 696d 756c 6174 696f 6e2c 2022  id_simulation, "
-0000ad70: 5354 4f50 5049 4e47 222c 2070 6f73 745f  STOPPING", post_
-0000ad80: 6461 7461 3d70 6f73 745f 6461 7461 0a20  data=post_data. 
-0000ad90: 2020 2020 2020 2029 0a0a 2020 2020 5f73         )..    _s
-0000ada0: 696d 756c 6174 696f 6e5f 6578 6563 7574  imulation_execut
-0000adb0: 655f 6f70 6572 6174 696f 6e28 2267 6574  e_operation("get
-0000adc0: 222c 2022 6465 6c65 7465 5f73 6e61 7073  ", "delete_snaps
-0000add0: 686f 7473 222c 2069 645f 7369 6d75 6c61  hots", id_simula
-0000ade0: 7469 6f6e 2c20 2253 544f 5050 494e 4722  tion, "STOPPING"
-0000adf0: 290a 0a20 2020 2023 2044 656c 6574 6520  )..    # Delete 
-0000ae00: 7369 6d75 6c61 7469 6f6e 206e 6f64 6573  simulation nodes
-0000ae10: 0a20 2020 2064 656c 6574 655f 6e6f 6465  .    delete_node
-0000ae20: 7328 6964 5f73 696d 756c 6174 696f 6e29  s(id_simulation)
-0000ae30: 0a0a 2020 2020 2320 4465 6c65 7465 2073  ..    # Delete s
-0000ae40: 696d 756c 6174 696f 6e0a 2020 2020 7265  imulation.    re
-0000ae50: 7375 6c74 203d 205f 6465 6c65 7465 2866  sult = _delete(f
-0000ae60: 222f 7369 6d75 6c61 7469 6f6e 2f7b 6964  "/simulation/{id
-0000ae70: 5f73 696d 756c 6174 696f 6e7d 2229 0a0a  _simulation}")..
-0000ae80: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
-0000ae90: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
-0000aea0: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
-0000aeb0: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
-0000aec0: 2243 616e 6e6f 7420 6465 6c65 7465 2073  "Cannot delete s
-0000aed0: 696d 756c 6174 696f 6e20 6672 6f6d 2049  imulation from I
-0000aee0: 5420 5369 6d75 6c61 7469 6f6e 2041 5049  T Simulation API
-0000aef0: 2229 0a0a 2020 2020 7265 7475 726e 2072  ")..    return r
-0000af00: 6573 756c 742e 6a73 6f6e 2829 0a0a 0a64  esult.json()...d
-0000af10: 6566 206e 6f64 655f 7374 6174 7573 2869  ef node_status(i
-0000af20: 645f 6e6f 6465 3a20 696e 7429 202d 3e20  d_node: int) -> 
-0000af30: 7374 723a 0a20 2020 2022 2222 5265 7472  str:.    """Retr
-0000af40: 6965 7665 206e 6f64 6520 7374 6174 7573  ieve node status
-0000af50: 2e22 2222 0a0a 2020 2020 7265 7375 6c74  ."""..    result
-0000af60: 203d 205f 6765 7428 6622 2f6e 6f64 652f   = _get(f"/node/
-0000af70: 7b69 645f 6e6f 6465 7d2f 7374 6174 7573  {id_node}/status
-0000af80: 2229 0a0a 2020 2020 6966 2072 6573 756c  ")..    if resul
-0000af90: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
-0000afa0: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
-0000afb0: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
-0000afc0: 6c74 2c20 2243 616e 6e6f 7420 7265 7472  lt, "Cannot retr
-0000afd0: 6965 7665 206e 6f64 6520 696e 666f 2066  ieve node info f
-0000afe0: 726f 6d20 4954 2053 696d 756c 6174 696f  rom IT Simulatio
-0000aff0: 6e20 4150 4922 290a 0a20 2020 2072 6574  n API")..    ret
-0000b000: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
-0000b010: 290a 0a0a 6465 6620 7374 6f70 5f6e 6f64  )...def stop_nod
-0000b020: 655f 6279 5f6e 616d 6528 6964 5f73 696d  e_by_name(id_sim
-0000b030: 756c 6174 696f 6e3a 2069 6e74 2c20 6e6f  ulation: int, no
-0000b040: 6465 5f6e 616d 653a 2073 7472 2920 2d3e  de_name: str) ->
-0000b050: 204e 6f6e 653a 0a20 2020 2022 2222 5374   None:.    """St
-0000b060: 6f70 2061 206e 6f64 6520 6966 2069 7420  op a node if it 
-0000b070: 6973 2072 756e 6e69 6e67 2e22 2222 0a0a  is running."""..
-0000b080: 2020 2020 2320 5265 7472 6965 7665 2069      # Retrieve i
-0000b090: 645f 6e6f 6465 0a20 2020 206e 6f64 6520  d_node.    node 
-0000b0a0: 3d20 6665 7463 685f 6e6f 6465 5f62 795f  = fetch_node_by_
-0000b0b0: 6e61 6d65 2869 645f 7369 6d75 6c61 7469  name(id_simulati
-0000b0c0: 6f6e 2c20 6e6f 6465 5f6e 616d 6529 0a20  on, node_name). 
-0000b0d0: 2020 2069 645f 6e6f 6465 203d 206e 6f64     id_node = nod
-0000b0e0: 655b 2269 6422 5d0a 0a20 2020 2023 2044  e["id"]..    # D
-0000b0f0: 656c 6574 6520 6e6f 6465 0a20 2020 2073  elete node.    s
-0000b100: 746f 705f 6e6f 6465 2869 645f 7369 6d75  top_node(id_simu
-0000b110: 6c61 7469 6f6e 2c20 6964 5f6e 6f64 6529  lation, id_node)
-0000b120: 0a0a 0a64 6566 2073 746f 705f 6e6f 6465  ...def stop_node
-0000b130: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
-0000b140: 696e 742c 2069 645f 6e6f 6465 3a20 7374  int, id_node: st
-0000b150: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
-0000b160: 2222 2253 746f 7020 6120 6e6f 6465 2069  """Stop a node i
-0000b170: 6620 6974 2069 7320 7275 6e6e 696e 672e  f it is running.
-0000b180: 2222 220a 0a20 2020 2023 2052 6574 7269  """..    # Retri
-0000b190: 6576 6520 6e6f 6465 2061 6363 6f72 6469  eve node accordi
-0000b1a0: 6e67 2074 6f20 6974 7320 6e61 6d65 0a20  ng to its name. 
-0000b1b0: 2020 206e 6f64 6520 3d20 6665 7463 685f     node = fetch_
-0000b1c0: 6e6f 6465 2869 645f 6e6f 6465 290a 0a20  node(id_node).. 
-0000b1d0: 2020 2023 2053 6574 206e 6f64 6520 6e61     # Set node na
-0000b1e0: 6d65 7320 746f 2064 656c 6574 650a 2020  mes to delete.  
-0000b1f0: 2020 6e6f 6465 735f 746f 5f64 656c 6574    nodes_to_delet
-0000b200: 6520 3d20 5b6e 6f64 655b 226e 616d 6522  e = [node["name"
-0000b210: 5d5d 0a20 2020 2070 6f73 745f 6461 7461  ]].    post_data
-0000b220: 203d 207b 226e 6f64 6573 223a 206e 6f64   = {"nodes": nod
-0000b230: 6573 5f74 6f5f 6465 6c65 7465 7d0a 0a20  es_to_delete}.. 
-0000b240: 2020 2023 2053 746f 7020 6e6f 6465 2069     # Stop node i
-0000b250: 6620 6974 2069 7320 7275 6e6e 696e 670a  f it is running.
-0000b260: 2020 2020 6966 206e 6f64 655f 7374 6174      if node_stat
-0000b270: 7573 2869 645f 6e6f 6465 2920 3d3d 2022  us(id_node) == "
-0000b280: 5255 4e4e 494e 4722 3a0a 2020 2020 2020  RUNNING":.      
-0000b290: 2020 5f73 696d 756c 6174 696f 6e5f 6578    _simulation_ex
-0000b2a0: 6563 7574 655f 6f70 6572 6174 696f 6e28  ecute_operation(
-0000b2b0: 0a20 2020 2020 2020 2020 2020 2022 706f  .            "po
-0000b2c0: 7374 222c 0a20 2020 2020 2020 2020 2020  st",.           
-0000b2d0: 2022 6861 6c74 222c 0a20 2020 2020 2020   "halt",.       
-0000b2e0: 2020 2020 2069 645f 7369 6d75 6c61 7469       id_simulati
-0000b2f0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-0000b300: 2253 544f 5050 494e 4722 2c0a 2020 2020  "STOPPING",.    
-0000b310: 2020 2020 2020 2020 706f 7374 5f64 6174          post_dat
-0000b320: 613d 706f 7374 5f64 6174 612c 0a20 2020  a=post_data,.   
-0000b330: 2020 2020 2029 0a0a 0a64 6566 2075 7064       )...def upd
-0000b340: 6174 655f 7369 6d75 6c61 7469 6f6e 2869  ate_simulation(i
-0000b350: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
-0000b360: 742c 2073 696d 756c 6174 696f 6e5f 6469  t, simulation_di
-0000b370: 6374 3a20 6469 6374 2920 2d3e 2041 6e79  ct: dict) -> Any
-0000b380: 3a0a 2020 2020 2222 2255 7064 6174 6520  :.    """Update 
-0000b390: 7369 6d75 6c61 7469 6f6e 2069 6e66 6f72  simulation infor
-0000b3a0: 6d61 7469 6f6e 2069 6e66 6f72 6d61 7469  mation informati
-0000b3b0: 6f6e 2067 6976 656e 2061 2073 696d 756c  on given a simul
-0000b3c0: 6174 696f 6e20 6964 0a20 2020 2061 6e64  ation id.    and
-0000b3d0: 2061 2064 6963 7420 636f 6e74 6169 6e69   a dict containi
-0000b3e0: 6e67 2073 696d 756c 6174 696f 6e20 696e  ng simulation in
-0000b3f0: 666f 2e0a 2020 2020 2222 220a 2020 2020  fo..    """.    
-0000b400: 6461 7461 203d 206a 736f 6e2e 6475 6d70  data = json.dump
-0000b410: 7328 7369 6d75 6c61 7469 6f6e 5f64 6963  s(simulation_dic
-0000b420: 7429 0a20 2020 2072 6573 756c 7420 3d20  t).    result = 
-0000b430: 5f70 7574 280a 2020 2020 2020 2020 6622  _put(.        f"
-0000b440: 2f73 696d 756c 6174 696f 6e2f 7b69 645f  /simulation/{id_
-0000b450: 7369 6d75 6c61 7469 6f6e 7d22 2c0a 2020  simulation}",.  
-0000b460: 2020 2020 2020 6461 7461 3d64 6174 612c        data=data,
-0000b470: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-0000b480: 3d7b 2243 6f6e 7465 6e74 2d54 7970 6522  ={"Content-Type"
-0000b490: 3a20 2261 7070 6c69 6361 7469 6f6e 2f6a  : "application/j
-0000b4a0: 736f 6e22 7d2c 0a20 2020 2029 0a0a 2020  son"},.    )..  
-0000b4b0: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
-0000b4c0: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
-0000b4d0: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
-0000b4e0: 6572 726f 7228 7265 7375 6c74 2c20 2243  error(result, "C
-0000b4f0: 616e 6e6f 7420 7570 6461 7465 2073 696d  annot update sim
-0000b500: 756c 6174 696f 6e20 696e 666f 726d 6174  ulation informat
-0000b510: 696f 6e22 290a 0a20 2020 2072 6574 7572  ion")..    retur
-0000b520: 6e20 7265 7375 6c74 2e6a 736f 6e28 290a  n result.json().
-0000b530: 0a0a 6465 6620 6665 7463 685f 7369 6d75  ..def fetch_simu
-0000b540: 6c61 7469 6f6e 5f74 6f70 6f6c 6f67 7928  lation_topology(
-0000b550: 6964 5f73 696d 756c 6174 696f 6e3a 2069  id_simulation: i
-0000b560: 6e74 2920 2d3e 2041 6e79 3a0a 2020 2020  nt) -> Any:.    
-0000b570: 2222 2252 6574 7572 6e20 7468 6520 746f  """Return the to
-0000b580: 706f 6c6f 6779 206f 6620 6120 7369 6d75  pology of a simu
-0000b590: 6c61 7469 6f6e 2e22 2222 0a20 2020 2072  lation.""".    r
-0000b5a0: 6573 756c 7420 3d20 5f67 6574 2866 222f  esult = _get(f"/
-0000b5b0: 7369 6d75 6c61 7469 6f6e 2f7b 6964 5f73  simulation/{id_s
-0000b5c0: 696d 756c 6174 696f 6e7d 2f74 6f70 6f6c  imulation}/topol
-0000b5d0: 6f67 7922 290a 0a20 2020 2069 6620 7265  ogy")..    if re
-0000b5e0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-0000b5f0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
-0000b600: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
-0000b610: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
-0000b620: 6574 7269 6576 6520 7369 6d75 6c61 7469  etrieve simulati
-0000b630: 6f6e 2074 6f70 6f6c 6f67 7920 696e 666f  on topology info
-0000b640: 2229 0a0a 2020 2020 7265 7475 726e 2072  ")..    return r
-0000b650: 6573 756c 742e 6a73 6f6e 2829 0a0a 0a64  esult.json()...d
-0000b660: 6566 2066 6574 6368 5f73 696d 756c 6174  ef fetch_simulat
-0000b670: 696f 6e5f 746f 706f 6c6f 6779 5f79 616d  ion_topology_yam
-0000b680: 6c28 6964 5f73 696d 756c 6174 696f 6e3a  l(id_simulation:
-0000b690: 2069 6e74 2920 2d3e 2041 6e79 3a0a 2020   int) -> Any:.  
-0000b6a0: 2020 2222 2252 6574 7572 6e20 7468 6520    """Return the 
-0000b6b0: 5941 4d4c 2074 6f70 6f6c 6f67 7920 636f  YAML topology co
-0000b6c0: 6e74 656e 7420 6f66 2061 2073 696d 756c  ntent of a simul
-0000b6d0: 6174 696f 6e2e 2222 220a 2020 2020 7265  ation.""".    re
-0000b6e0: 7375 6c74 203d 205f 6765 7428 6622 2f73  sult = _get(f"/s
-0000b6f0: 696d 756c 6174 696f 6e2f 7b69 645f 7369  imulation/{id_si
-0000b700: 6d75 6c61 7469 6f6e 7d2f 746f 706f 6c6f  mulation}/topolo
-0000b710: 6779 5f79 616d 6c22 290a 0a20 2020 2069  gy_yaml")..    i
-0000b720: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
-0000b730: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
-0000b740: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
-0000b750: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
-0000b760: 6f74 2072 6574 7269 6576 6520 7369 6d75  ot retrieve simu
-0000b770: 6c61 7469 6f6e 2074 6f70 6f6c 6f67 7920  lation topology 
-0000b780: 696e 666f 2229 0a0a 2020 2020 7265 7475  info")..    retu
-0000b790: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
-0000b7a0: 0a0a 0a64 6566 2066 6574 6368 5f61 7373  ...def fetch_ass
-0000b7b0: 6574 7328 6964 5f73 696d 756c 6174 696f  ets(id_simulatio
-0000b7c0: 6e3a 2069 6e74 2920 2d3e 2041 6e79 3a0a  n: int) -> Any:.
-0000b7d0: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
-0000b7e0: 6520 6c69 7374 206f 6620 7468 6520 6173  e list of the as
-0000b7f0: 7365 7473 0a20 2020 206f 6620 6120 6769  sets.    of a gi
-0000b800: 7665 6e20 7369 6d75 6c61 7469 6f6e 2e20  ven simulation. 
-0000b810: 4974 2063 6f72 7265 7370 6f6e 6473 2074  It corresponds t
-0000b820: 6f0a 2020 2020 7468 6520 6c69 7374 206f  o.    the list o
-0000b830: 6620 7468 6520 6e6f 6465 7320 7769 7468  f the nodes with
-0000b840: 2073 6f6d 6520 6164 6469 7469 6f6e 616c   some additional
-0000b850: 0a20 2020 2069 6e66 6f72 6d61 7469 6f6e  .    information
-0000b860: 2e0a 2020 2020 2222 220a 2020 2020 7265  ..    """.    re
-0000b870: 7375 6c74 203d 205f 6765 7428 6622 2f73  sult = _get(f"/s
-0000b880: 696d 756c 6174 696f 6e2f 7b69 645f 7369  imulation/{id_si
-0000b890: 6d75 6c61 7469 6f6e 7d2f 6173 7365 7473  mulation}/assets
-0000b8a0: 2229 0a0a 2020 2020 6966 2072 6573 756c  ")..    if resul
-0000b8b0: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
-0000b8c0: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
-0000b8d0: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
-0000b8e0: 6c74 2c20 2243 616e 6e6f 7420 7265 7472  lt, "Cannot retr
-0000b8f0: 6965 7665 2061 7373 6574 7320 6672 6f6d  ieve assets from
-0000b900: 2063 6f72 6520 4150 4922 290a 0a20 2020   core API")..   
-0000b910: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
-0000b920: 736f 6e28 290a 0a0a 6465 6620 6665 7463  son()...def fetc
-0000b930: 685f 7377 6974 6368 5f62 795f 6e65 7477  h_switch_by_netw
-0000b940: 6f72 6b5f 6964 2869 645f 7369 6d75 6c61  ork_id(id_simula
-0000b950: 7469 6f6e 3a20 696e 742c 206e 6574 776f  tion: int, netwo
-0000b960: 726b 5f69 643a 2073 7472 2920 2d3e 2041  rk_id: str) -> A
-0000b970: 6e79 3a0a 2020 2020 2222 2252 6574 7572  ny:.    """Retur
-0000b980: 6e20 6120 7377 6974 6368 2067 6976 656e  n a switch given
-0000b990: 2069 7473 206e 6574 776f 726b 5f69 6422   its network_id"
-0000b9a0: 2222 0a0a 2020 2020 7265 7375 6c74 203d  ""..    result =
-0000b9b0: 205f 6765 7428 6622 2f73 696d 756c 6174   _get(f"/simulat
-0000b9c0: 696f 6e2f 7b69 645f 7369 6d75 6c61 7469  ion/{id_simulati
-0000b9d0: 6f6e 7d2f 7377 6974 6368 2f7b 6e65 7477  on}/switch/{netw
-0000b9e0: 6f72 6b5f 6964 7d22 290a 0a20 2020 2069  ork_id}")..    i
-0000b9f0: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
-0000ba00: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
-0000ba10: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
-0000ba20: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
-0000ba30: 6f74 2072 6574 7269 6576 6520 7369 6d75  ot retrieve simu
-0000ba40: 6c61 7469 6f6e 2073 7769 7463 6820 6672  lation switch fr
-0000ba50: 6f6d 2063 6f72 6520 4150 4922 290a 0a20  om core API").. 
-0000ba60: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-0000ba70: 2e6a 736f 6e28 290a 0a0a 6465 6620 6665  .json()...def fe
-0000ba80: 7463 685f 6e6f 6465 286e 6f64 655f 6964  tch_node(node_id
-0000ba90: 3a20 696e 7429 202d 3e20 416e 793a 0a20  : int) -> Any:. 
-0000baa0: 2020 2022 2222 5265 7475 726e 2061 206e     """Return a n
-0000bab0: 6f64 6520 6769 7665 6e20 6974 7320 4944  ode given its ID
-0000bac0: 2222 220a 2020 2020 7265 7375 6c74 203d  """.    result =
-0000bad0: 205f 6765 7428 6622 2f6e 6f64 652f 7b6e   _get(f"/node/{n
-0000bae0: 6f64 655f 6964 7d22 290a 0a20 2020 2069  ode_id}")..    i
-0000baf0: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
-0000bb00: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
-0000bb10: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
-0000bb20: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
-0000bb30: 6f74 2072 6574 7269 6576 6520 6e6f 6465  ot retrieve node
-0000bb40: 2066 726f 6d20 4954 2053 696d 756c 6174   from IT Simulat
-0000bb50: 696f 6e20 4150 4922 290a 0a20 2020 2072  ion API")..    r
-0000bb60: 6574 7572 6e20 7265 7375 6c74 2e6a 736f  eturn result.jso
-0000bb70: 6e28 290a 0a0a 6465 6620 6665 7463 685f  n()...def fetch_
-0000bb80: 6e6f 6465 5f62 795f 6e61 6d65 2869 645f  node_by_name(id_
-0000bb90: 7369 6d75 6c61 7469 6f6e 3a20 696e 742c  simulation: int,
-0000bba0: 206e 6f64 655f 6e61 6d65 3a20 7374 7229   node_name: str)
-0000bbb0: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
-0000bbc0: 5265 7475 726e 2061 206e 6f64 6520 6769  Return a node gi
-0000bbd0: 7665 6e20 6974 7320 6e61 6d65 2222 220a  ven its name""".
-0000bbe0: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
-0000bbf0: 6574 2866 222f 7369 6d75 6c61 7469 6f6e  et(f"/simulation
-0000bc00: 2f7b 6964 5f73 696d 756c 6174 696f 6e7d  /{id_simulation}
-0000bc10: 2f6e 6f64 652f 7b6e 6f64 655f 6e61 6d65  /node/{node_name
-0000bc20: 7d22 290a 0a20 2020 2069 6620 7265 7375  }")..    if resu
-0000bc30: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000bc40: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-0000bc50: 6861 6e64 6c65 5f65 7272 6f72 280a 2020  handle_error(.  
-0000bc60: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000bc70: 2c20 2243 616e 6e6f 7420 7265 7472 6965  , "Cannot retrie
-0000bc80: 7665 206e 6f64 6520 6261 7365 6420 6f6e  ve node based on
-0000bc90: 2069 7473 206e 616d 6520 6672 6f6d 2049   its name from I
-0000bca0: 5420 5369 6d75 6c61 7469 6f6e 2041 5049  T Simulation API
-0000bcb0: 220a 2020 2020 2020 2020 290a 0a20 2020  ".        )..   
-0000bcc0: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
-0000bcd0: 736f 6e28 290a 0a0a 6465 6620 6665 7463  son()...def fetc
-0000bce0: 685f 6e6f 6465 735f 6279 5f72 6f6c 6573  h_nodes_by_roles
-0000bcf0: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
-0000bd00: 696e 7429 202d 3e20 416e 793a 0a20 2020  int) -> Any:.   
-0000bd10: 2022 2222 5265 7475 726e 2061 2064 6963   """Return a dic
-0000bd20: 7420 776b 6572 6520 6b65 7973 2061 7265  t wkere keys are
-0000bd30: 2072 6f6c 6573 2028 7375 6368 2061 7320   roles (such as 
-0000bd40: 2761 6427 2c20 2766 696c 655f 7365 7276  'ad', 'file_serv
-0000bd50: 6572 272c 2027 636c 6965 6e74 272c 202e  er', 'client', .
-0000bd60: 2e2e 2920 616e 640a 2020 2020 7661 6c75  ..) and.    valu
-0000bd70: 6573 2061 7265 206e 6f64 6573 2e0a 0a20  es are nodes... 
-0000bd80: 2020 2022 2222 0a20 2020 2072 6573 756c     """.    resul
-0000bd90: 7420 3d20 5f67 6574 2866 222f 7369 6d75  t = _get(f"/simu
-0000bda0: 6c61 7469 6f6e 2f7b 6964 5f73 696d 756c  lation/{id_simul
-0000bdb0: 6174 696f 6e7d 2f6e 6f64 6573 5f62 795f  ation}/nodes_by_
-0000bdc0: 726f 6c65 7322 290a 0a20 2020 2069 6620  roles")..    if 
-0000bdd0: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-0000bde0: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-0000bdf0: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-0000be00: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-0000be10: 2072 6574 7269 6576 6520 6e6f 6465 7322   retrieve nodes"
-0000be20: 290a 0a20 2020 2072 6f6c 6573 5f64 6963  )..    roles_dic
-0000be30: 7420 3d20 7265 7375 6c74 2e6a 736f 6e28  t = result.json(
-0000be40: 290a 2020 2020 7265 7475 726e 2072 6f6c  ).    return rol
-0000be50: 6573 5f64 6963 740a 0a0a 6465 6620 6465  es_dict...def de
-0000be60: 6c65 7465 5f6e 6f64 655f 6279 5f6e 616d  lete_node_by_nam
-0000be70: 6528 6964 5f73 696d 756c 6174 696f 6e3a  e(id_simulation:
-0000be80: 2069 6e74 2c20 6e6f 6465 5f6e 616d 653a   int, node_name:
-0000be90: 2073 7472 2920 2d3e 2041 6e79 3a0a 2020   str) -> Any:.  
-0000bea0: 2020 2320 5265 7472 6965 7665 2069 645f    # Retrieve id_
-0000beb0: 6e6f 6465 0a20 2020 206e 6f64 6520 3d20  node.    node = 
-0000bec0: 6665 7463 685f 6e6f 6465 5f62 795f 6e61  fetch_node_by_na
-0000bed0: 6d65 2869 645f 7369 6d75 6c61 7469 6f6e  me(id_simulation
-0000bee0: 2c20 6e6f 6465 5f6e 616d 6529 0a20 2020  , node_name).   
-0000bef0: 2069 645f 6e6f 6465 203d 206e 6f64 655b   id_node = node[
-0000bf00: 2269 6422 5d0a 0a20 2020 2023 2044 656c  "id"]..    # Del
-0000bf10: 6574 6520 6e6f 6465 0a20 2020 2064 656c  ete node.    del
-0000bf20: 6574 655f 6e6f 6465 2869 645f 6e6f 6465  ete_node(id_node
-0000bf30: 290a 0a0a 6465 6620 6465 6c65 7465 5f6e  )...def delete_n
-0000bf40: 6f64 6528 6964 5f6e 6f64 653a 2069 6e74  ode(id_node: int
-0000bf50: 2920 2d3e 2041 6e79 3a0a 2020 2020 2222  ) -> Any:.    ""
-0000bf60: 2244 656c 6574 6520 6e6f 6465 2066 726f  "Delete node fro
-0000bf70: 6d20 6461 7461 6261 7365 2067 6976 656e  m database given
-0000bf80: 2069 7473 2049 442e 2222 220a 0a20 2020   its ID."""..   
-0000bf90: 2023 2046 6574 6368 2076 6972 7475 616c   # Fetch virtual
-0000bfa0: 206e 6f64 6520 6e65 7477 6f72 6b20 696e   node network in
-0000bfb0: 7465 7266 6163 6573 0a20 2020 206e 6574  terfaces.    net
-0000bfc0: 776f 726b 5f69 6e74 6572 6661 6365 7320  work_interfaces 
-0000bfd0: 3d20 6665 7463 685f 6e6f 6465 5f6e 6574  = fetch_node_net
-0000bfe0: 776f 726b 5f69 6e74 6572 6661 6365 7328  work_interfaces(
-0000bff0: 6964 5f6e 6f64 6529 0a0a 2020 2020 2320  id_node)..    # 
-0000c000: 4465 6c65 7465 2065 6163 6820 6e65 7477  Delete each netw
-0000c010: 6f72 6b20 696e 7465 7266 6163 6573 0a20  ork interfaces. 
-0000c020: 2020 2066 6f72 206e 6574 776f 726b 5f69     for network_i
-0000c030: 6e74 6572 6661 6365 2069 6e20 6e65 7477  nterface in netw
-0000c040: 6f72 6b5f 696e 7465 7266 6163 6573 3a0a  ork_interfaces:.
-0000c050: 2020 2020 2020 2020 6465 6c65 7465 5f6e          delete_n
-0000c060: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-0000c070: 286e 6574 776f 726b 5f69 6e74 6572 6661  (network_interfa
-0000c080: 6365 5b22 6964 225d 290a 0a20 2020 2023  ce["id"])..    #
-0000c090: 2044 656c 6574 6520 6e6f 6465 0a20 2020   Delete node.   
-0000c0a0: 2072 6573 756c 7420 3d20 5f64 656c 6574   result = _delet
-0000c0b0: 6528 6622 2f6e 6f64 652f 7b69 645f 6e6f  e(f"/node/{id_no
-0000c0c0: 6465 7d22 290a 0a20 2020 2069 6620 7265  de}")..    if re
-0000c0d0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-0000c0e0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
-0000c0f0: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
-0000c100: 6573 756c 742c 2022 4361 6e6e 6f74 2064  esult, "Cannot d
-0000c110: 656c 6574 6520 6e6f 6465 2229 0a0a 2020  elete node")..  
-0000c120: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
-0000c130: 6a73 6f6e 2829 0a0a 0a64 6566 2066 6574  json()...def fet
-0000c140: 6368 5f6e 6f64 6573 2869 645f 7369 6d75  ch_nodes(id_simu
-0000c150: 6c61 7469 6f6e 3a20 696e 7429 202d 3e20  lation: int) -> 
-0000c160: 416e 793a 0a20 2020 2022 2222 5265 7475  Any:.    """Retu
-0000c170: 726e 2073 696d 756c 6174 696f 6e20 6e6f  rn simulation no
-0000c180: 6465 7320 6469 6374 2067 6976 656e 0a20  des dict given. 
-0000c190: 2020 2061 2073 696d 756c 6174 696f 6e20     a simulation 
-0000c1a0: 4944 2c20 7768 6572 6520 6b65 7973 2061  ID, where keys a
-0000c1b0: 7265 206e 6f64 6520 6e61 6d65 732e 0a20  re node names.. 
-0000c1c0: 2020 2022 2222 0a20 2020 2072 6573 756c     """.    resul
-0000c1d0: 7420 3d20 5f67 6574 2866 222f 7369 6d75  t = _get(f"/simu
-0000c1e0: 6c61 7469 6f6e 2f7b 6964 5f73 696d 756c  lation/{id_simul
-0000c1f0: 6174 696f 6e7d 2f6e 6f64 6522 290a 0a20  ation}/node").. 
-0000c200: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-0000c210: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-0000c220: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-0000c230: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-0000c240: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
-0000c250: 6e6f 6465 7320 6672 6f6d 2049 5420 5369  nodes from IT Si
-0000c260: 6d75 6c61 7469 6f6e 2041 5049 2229 0a0a  mulation API")..
-0000c270: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0000c280: 742e 6a73 6f6e 2829 0a0a 0a64 6566 2066  t.json()...def f
-0000c290: 6574 6368 5f76 6972 7475 616c 5f6d 6163  etch_virtual_mac
-0000c2a0: 6869 6e65 7328 6964 5f73 696d 756c 6174  hines(id_simulat
-0000c2b0: 696f 6e3a 2069 6e74 2920 2d3e 204c 6973  ion: int) -> Lis
-0000c2c0: 745b 6469 6374 5d3a 0a20 2020 2022 2222  t[dict]:.    """
-0000c2d0: 5265 7475 726e 2073 696d 756c 6174 696f  Return simulatio
-0000c2e0: 6e20 7669 7274 7561 6c20 6d61 6368 696e  n virtual machin
-0000c2f0: 6573 2064 6963 7420 6769 7665 6e20 6120  es dict given a 
-0000c300: 7369 6d75 6c61 7469 6f6e 2049 442c 0a20  simulation ID,. 
-0000c310: 2020 2077 6865 7265 206b 6579 7320 6172     where keys ar
-0000c320: 6520 7669 7274 7561 6c20 6d61 6368 696e  e virtual machin
-0000c330: 6520 6e61 6d65 732e 0a20 2020 2022 2222  e names..    """
-0000c340: 0a20 2020 2072 6573 756c 7473 203d 2066  .    results = f
-0000c350: 6574 6368 5f6e 6f64 6573 2869 645f 7369  etch_nodes(id_si
-0000c360: 6d75 6c61 7469 6f6e 290a 0a20 2020 2076  mulation)..    v
-0000c370: 6d5f 6f6e 6c79 203d 2066 696c 7465 7228  m_only = filter(
-0000c380: 6c61 6d62 6461 206d 3a20 6d5b 2274 7970  lambda m: m["typ
-0000c390: 6522 5d20 3d3d 2022 7669 7274 7561 6c5f  e"] == "virtual_
-0000c3a0: 6d61 6368 696e 6522 2c20 7265 7375 6c74  machine", result
-0000c3b0: 7329 0a20 2020 2072 6574 7572 6e20 6c69  s).    return li
-0000c3c0: 7374 2876 6d5f 6f6e 6c79 290a 0a0a 6465  st(vm_only)...de
-0000c3d0: 6620 6465 6c65 7465 5f6e 6f64 6573 2869  f delete_nodes(i
-0000c3e0: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
-0000c3f0: 7429 202d 3e20 7374 723a 0a20 2020 2022  t) -> str:.    "
-0000c400: 2222 4465 6c65 7465 2073 696d 756c 6174  ""Delete simulat
-0000c410: 696f 6e20 6e6f 6465 7320 6769 7665 6e20  ion nodes given 
-0000c420: 6120 7369 6d75 6c61 7469 6f6e 2049 442e  a simulation ID.
-0000c430: 2222 220a 0a20 2020 2023 2046 6574 6368  """..    # Fetch
-0000c440: 2073 696d 756c 6174 696f 6e20 6e6f 6465   simulation node
-0000c450: 730a 2020 2020 7265 7375 6c74 203d 205f  s.    result = _
-0000c460: 6765 7428 6622 2f73 696d 756c 6174 696f  get(f"/simulatio
-0000c470: 6e2f 7b69 645f 7369 6d75 6c61 7469 6f6e  n/{id_simulation
-0000c480: 7d2f 6e6f 6465 2229 0a0a 2020 2020 6966  }/node")..    if
-0000c490: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-0000c4a0: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-0000c4b0: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-0000c4c0: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
-0000c4d0: 7420 6465 6c65 7465 2073 696d 756c 6174  t delete simulat
-0000c4e0: 696f 6e20 6e6f 6465 7322 290a 0a20 2020  ion nodes")..   
-0000c4f0: 206e 6f64 6573 5f6c 6973 7420 3d20 7265   nodes_list = re
-0000c500: 7375 6c74 2e6a 736f 6e28 290a 0a20 2020  sult.json()..   
-0000c510: 2023 2044 656c 6574 6520 6561 6368 206e   # Delete each n
-0000c520: 6f64 650a 2020 2020 666f 7220 6e6f 6465  ode.    for node
-0000c530: 2069 6e20 6e6f 6465 735f 6c69 7374 3a0a   in nodes_list:.
-0000c540: 2020 2020 2020 2020 6465 6c65 7465 5f6e          delete_n
-0000c550: 6f64 6528 6e6f 6465 5b22 6964 225d 290a  ode(node["id"]).
-0000c560: 0a20 2020 2072 6573 756c 745f 6a73 6f6e  .    result_json
-0000c570: 203d 2022 7b7d 220a 2020 2020 7265 7475   = "{}".    retu
-0000c580: 726e 2072 6573 756c 745f 6a73 6f6e 0a0a  rn result_json..
-0000c590: 0a64 6566 2075 7064 6174 655f 6e6f 6465  .def update_node
-0000c5a0: 286e 6f64 655f 6964 3a20 696e 742c 206e  (node_id: int, n
-0000c5b0: 6f64 655f 6469 6374 3a20 6469 6374 2920  ode_dict: dict) 
-0000c5c0: 2d3e 2041 6e79 3a0a 2020 2020 2222 2255  -> Any:.    """U
-0000c5d0: 7064 6174 6520 6e6f 6465 2069 6e66 6f72  pdate node infor
-0000c5e0: 6d61 7469 6f6e 2067 6976 656e 2061 206e  mation given a n
-0000c5f0: 6f64 6520 6964 2061 6e64 2061 2064 6963  ode id and a dic
-0000c600: 7420 636f 6e74 6169 6e69 6e67 0a20 2020  t containing.   
-0000c610: 206e 6f64 6520 6461 7461 2e0a 2020 2020   node data..    
-0000c620: 2222 220a 2020 2020 6461 7461 203d 206a  """.    data = j
-0000c630: 736f 6e2e 6475 6d70 7328 6e6f 6465 5f64  son.dumps(node_d
-0000c640: 6963 7429 0a20 2020 2072 6573 756c 7420  ict).    result 
-0000c650: 3d20 5f70 7574 280a 2020 2020 2020 2020  = _put(.        
-0000c660: 6622 2f6e 6f64 652f 7b6e 6f64 655f 6964  f"/node/{node_id
-0000c670: 7d22 2c0a 2020 2020 2020 2020 6461 7461  }",.        data
-0000c680: 3d64 6174 612c 0a20 2020 2020 2020 2068  =data,.        h
-0000c690: 6561 6465 7273 3d7b 2243 6f6e 7465 6e74  eaders={"Content
-0000c6a0: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
-0000c6b0: 7469 6f6e 2f6a 736f 6e22 7d2c 0a20 2020  tion/json"},.   
-0000c6c0: 2029 0a0a 2020 2020 6966 2072 6573 756c   )..    if resul
-0000c6d0: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
-0000c6e0: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
-0000c6f0: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
-0000c700: 6c74 2c20 2243 616e 6e6f 7420 7570 6461  lt, "Cannot upda
-0000c710: 7465 206e 6f64 6520 696e 666f 726d 6174  te node informat
-0000c720: 696f 6e20 7769 7468 2063 6f72 6520 4150  ion with core AP
-0000c730: 4922 290a 0a20 2020 2072 6574 7572 6e20  I")..    return 
-0000c740: 7265 7375 6c74 2e6a 736f 6e28 290a 0a0a  result.json()...
-0000c750: 6465 6620 6765 745f 6e6f 6465 5f64 6566  def get_node_def
-0000c760: 6175 6c74 5f67 6174 6577 6179 2869 645f  ault_gateway(id_
-0000c770: 6e6f 6465 3a20 696e 7429 202d 3e20 4f70  node: int) -> Op
-0000c780: 7469 6f6e 616c 5b73 7472 5d3a 0a20 2020  tional[str]:.   
-0000c790: 2022 2222 5265 7472 6965 7665 206e 6f64   """Retrieve nod
-0000c7a0: 6520 6465 6661 756c 7420 6761 7465 7761  e default gatewa
-0000c7b0: 792c 2077 6869 6368 2063 616e 2065 6974  y, which can eit
-0000c7c0: 6865 7220 6265 2061 6e20 4950 2061 6464  her be an IP add
-0000c7d0: 7265 7373 0a20 2020 206f 6620 7468 6520  ress.    of the 
-0000c7e0: 666f 726d 2078 782e 7878 2e78 782e 7878  form xx.xx.xx.xx
-0000c7f0: 206f 7220 4e6f 6e65 2069 6620 6e6f 2067   or None if no g
-0000c800: 6174 6577 6179 2069 7320 7365 742e 0a0a  ateway is set...
-0000c810: 2020 2020 2222 220a 0a20 2020 2072 6573      """..    res
-0000c820: 756c 7420 3d20 5f67 6574 2866 222f 6e6f  ult = _get(f"/no
-0000c830: 6465 2f7b 6964 5f6e 6f64 657d 2f64 6566  de/{id_node}/def
-0000c840: 6175 6c74 5f67 6174 6577 6179 2229 0a0a  ault_gateway")..
-0000c850: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
-0000c860: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
-0000c870: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
-0000c880: 655f 6572 726f 7228 0a20 2020 2020 2020  e_error(.       
-0000c890: 2020 2020 2072 6573 756c 742c 2022 4361       result, "Ca
-0000c8a0: 6e6e 6f74 2072 6574 7269 6576 6520 6e6f  nnot retrieve no
-0000c8b0: 6465 2064 6566 6175 6c74 2067 6174 6577  de default gatew
-0000c8c0: 6179 2066 726f 6d20 4954 2053 696d 756c  ay from IT Simul
-0000c8d0: 6174 696f 6e20 4150 4922 0a20 2020 2020  ation API".     
-0000c8e0: 2020 2029 0a0a 2020 2020 6465 6661 756c     )..    defaul
-0000c8f0: 745f 6761 7465 7761 7920 3d20 7265 7375  t_gateway = resu
-0000c900: 6c74 2e6a 736f 6e28 290a 0a20 2020 2072  lt.json()..    r
-0000c910: 6574 7572 6e20 6465 6661 756c 745f 6761  eturn default_ga
-0000c920: 7465 7761 790a 0a0a 6465 6620 6765 745f  teway...def get_
-0000c930: 6e6f 6465 5f73 7461 7469 7374 6963 735f  node_statistics_
-0000c940: 6279 5f69 6428 6964 5f6e 6f64 653a 2069  by_id(id_node: i
-0000c950: 6e74 2920 2d3e 2041 6e79 3a0a 2020 2020  nt) -> Any:.    
-0000c960: 2222 220a 2020 2020 5265 7475 726e 2061  """.    Return a
-0000c970: 6767 7265 6761 7465 6420 7374 6174 6973  ggregated statis
-0000c980: 7469 6373 2066 726f 6d20 4350 552c 206d  tics from CPU, m
-0000c990: 656d 6f72 792c 2062 6c6f 636b 2064 6576  emory, block dev
-0000c9a0: 6963 6573 2061 6e64 206e 6574 776f 726b  ices and network
-0000c9b0: 2069 6e74 6572 6661 6365 732e 0a20 2020   interfaces..   
-0000c9c0: 204e 6f74 653a 2079 6f75 2063 616e 2067   Note: you can g
-0000c9d0: 6574 2074 6865 206e 6f64 6520 4944 7320  et the node IDs 
-0000c9e0: 7573 696e 6720 7468 6520 7369 6d75 5f73  using the simu_s
-0000c9f0: 7461 7475 7320 636f 6d6d 616e 6420 286f  tatus command (o
-0000ca00: 7220 7468 6520 6665 7463 685f 7369 6d75  r the fetch_simu
-0000ca10: 6c61 7469 6f6e 7328 2920 6675 6e63 7469  lations() functi
-0000ca20: 6f6e 292e 0a20 2020 2022 2222 0a20 2020  on)..    """.   
-0000ca30: 2072 6573 756c 7420 3d20 5f67 6574 2866   result = _get(f
-0000ca40: 222f 6e6f 6465 2f7b 6964 5f6e 6f64 657d  "/node/{id_node}
-0000ca50: 2f73 7461 7473 2229 0a0a 2020 2020 6966  /stats")..    if
-0000ca60: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-0000ca70: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-0000ca80: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-0000ca90: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
-0000caa0: 7420 7265 7472 6965 7665 206e 6f64 6520  t retrieve node 
-0000cab0: 7374 6174 6973 7469 6373 2229 0a0a 2020  statistics")..  
-0000cac0: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
-0000cad0: 6a73 6f6e 2829 0a0a 0a64 6566 206e 6f64  json()...def nod
-0000cae0: 655f 6c6f 6773 2869 645f 6e6f 6465 3a20  e_logs(id_node: 
-0000caf0: 696e 7429 202d 3e20 416e 793a 0a20 2020  int) -> Any:.   
-0000cb00: 2022 2222 0a20 2020 2052 6574 7269 6576   """.    Retriev
-0000cb10: 6520 6c6f 6773 2066 726f 6d20 7370 6563  e logs from spec
-0000cb20: 6966 6965 6420 6e6f 6465 2028 6f6e 6c79  ified node (only
-0000cb30: 2077 6f72 6b20 666f 7220 446f 636b 6572   work for Docker
-0000cb40: 206e 6f64 6529 2e0a 0a20 2020 2052 6574   node)...    Ret
-0000cb50: 7572 6e20 7468 6520 6c6f 6773 2073 7472  urn the logs str
-0000cb60: 696e 672e 0a20 2020 2022 2222 0a0a 2020  ing..    """..  
-0000cb70: 2020 2320 4368 6563 6b20 7468 6174 2074    # Check that t
-0000cb80: 6865 2074 6172 6765 7420 6e6f 6465 2069  he target node i
-0000cb90: 7320 6120 646f 636b 6572 206e 6f64 6520  s a docker node 
-0000cba0: 286e 6f64 655f 6578 6563 206f 6e6c 790a  (node_exec only.
-0000cbb0: 2020 2020 2320 776f 726b 7320 666f 7220      # works for 
-0000cbc0: 446f 636b 6572 206e 6f64 6520 666f 7220  Docker node for 
-0000cbd0: 6e6f 7729 0a20 2020 206e 6f64 6520 3d20  now).    node = 
-0000cbe0: 6665 7463 685f 6e6f 6465 2869 645f 6e6f  fetch_node(id_no
-0000cbf0: 6465 290a 2020 2020 6966 206e 6f64 655b  de).    if node[
-0000cc00: 2274 7970 6522 5d20 213d 2022 646f 636b  "type"] != "dock
-0000cc10: 6572 223a 0a20 2020 2020 2020 2072 6169  er":.        rai
-0000cc20: 7365 2045 7863 6570 7469 6f6e 2822 4361  se Exception("Ca
-0000cc30: 6e6e 6f74 2065 7865 6375 7465 2063 6f6d  nnot execute com
-0000cc40: 6d61 6e64 2066 6f72 206e 6f64 6573 2064  mand for nodes d
-0000cc50: 6966 6665 7265 6e74 2066 726f 6d20 646f  ifferent from do
-0000cc60: 636b 6572 206e 6f64 6573 2229 0a0a 2020  cker nodes")..  
-0000cc70: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
-0000cc80: 6622 2f6e 6f64 652f 7b69 645f 6e6f 6465  f"/node/{id_node
-0000cc90: 7d2f 6c6f 6773 2229 0a0a 2020 2020 6966  }/logs")..    if
-0000cca0: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-0000ccb0: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-0000ccc0: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-0000ccd0: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
-0000cce0: 7420 7265 7472 6965 7665 206c 6f67 7320  t retrieve logs 
-0000ccf0: 6672 6f6d 2049 5420 5369 6d75 6c61 7469  from IT Simulati
-0000cd00: 6f6e 2041 5049 2229 0a0a 2020 2020 6c6f  on API")..    lo
-0000cd10: 6773 203d 2072 6573 756c 742e 6a73 6f6e  gs = result.json
-0000cd20: 2829 0a0a 2020 2020 7265 7475 726e 206c  ()..    return l
-0000cd30: 6f67 730a 0a0a 6465 6620 6e6f 6465 5f65  ogs...def node_e
-0000cd40: 7865 6328 6964 5f6e 6f64 653a 2069 6e74  xec(id_node: int
-0000cd50: 2c20 636f 6d6d 616e 643a 2073 7472 2920  , command: str) 
-0000cd60: 2d3e 2041 6e79 3a0a 2020 2020 2222 220a  -> Any:.    """.
-0000cd70: 2020 2020 4578 6563 7574 6520 6120 636f      Execute a co
-0000cd80: 6d6d 616e 6420 6f6e 2073 7065 6369 6669  mmand on specifi
-0000cd90: 6564 206e 6f64 6520 286f 6e6c 7920 776f  ed node (only wo
-0000cda0: 726b 2066 6f72 2044 6f63 6b65 7220 6e6f  rk for Docker no
-0000cdb0: 6465 292e 0a0a 2020 2020 5265 7475 726e  de)...    Return
-0000cdc0: 2061 2074 7570 6c65 2028 6578 6974 5f63   a tuple (exit_c
-0000cdd0: 6f64 653a 2069 6e74 2c20 7374 646f 7574  ode: int, stdout
-0000cde0: 3a20 7374 722c 2073 7464 6572 723a 2073  : str, stderr: s
-0000cdf0: 7472 2920 6f66 2074 6865 2065 7865 6375  tr) of the execu
-0000ce00: 7465 6420 636f 6d6d 616e 642e 0a20 2020  ted command..   
-0000ce10: 2022 2222 0a0a 2020 2020 2320 4368 6563   """..    # Chec
-0000ce20: 6b20 7468 6174 2074 6865 2074 6172 6765  k that the targe
-0000ce30: 7420 6e6f 6465 2069 7320 6120 646f 636b  t node is a dock
-0000ce40: 6572 206e 6f64 6520 286e 6f64 655f 6578  er node (node_ex
-0000ce50: 6563 206f 6e6c 790a 2020 2020 2320 776f  ec only.    # wo
-0000ce60: 726b 7320 666f 7220 446f 636b 6572 206e  rks for Docker n
-0000ce70: 6f64 6520 666f 7220 6e6f 7729 0a20 2020  ode for now).   
-0000ce80: 206e 6f64 6520 3d20 6665 7463 685f 6e6f   node = fetch_no
-0000ce90: 6465 2869 645f 6e6f 6465 290a 2020 2020  de(id_node).    
-0000cea0: 6966 206e 6f64 655b 2274 7970 6522 5d20  if node["type"] 
-0000ceb0: 213d 2022 646f 636b 6572 223a 0a20 2020  != "docker":.   
-0000cec0: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-0000ced0: 7469 6f6e 2822 4361 6e6e 6f74 2065 7865  tion("Cannot exe
-0000cee0: 6375 7465 2063 6f6d 6d61 6e64 2066 6f72  cute command for
-0000cef0: 206e 6f64 6573 2064 6966 6665 7265 6e74   nodes different
-0000cf00: 2066 726f 6d20 646f 636b 6572 206e 6f64   from docker nod
-0000cf10: 6573 2229 0a0a 2020 2020 7374 6174 7573  es")..    status
-0000cf20: 5f6b 6579 203d 2022 7374 6174 7573 220a  _key = "status".
-0000cf30: 2020 2020 6578 6974 5f63 6f64 6520 3d20      exit_code = 
-0000cf40: 2265 7869 745f 636f 6465 220a 2020 2020  "exit_code".    
-0000cf50: 7374 646f 7574 203d 2022 7374 646f 7574  stdout = "stdout
-0000cf60: 220a 2020 2020 7374 6465 7272 203d 2022  ".    stderr = "
-0000cf70: 7374 6465 7272 220a 0a20 2020 2070 6f73  stderr"..    pos
-0000cf80: 745f 6461 7461 203d 207b 2263 6f6d 6d61  t_data = {"comma
-0000cf90: 6e64 223a 2063 6f6d 6d61 6e64 7d0a 2020  nd": command}.  
-0000cfa0: 2020 6461 7461 203d 206a 736f 6e2e 6475    data = json.du
-0000cfb0: 6d70 7328 706f 7374 5f64 6174 6129 0a20  mps(post_data). 
-0000cfc0: 2020 2072 6573 756c 7420 3d20 5f70 6f73     result = _pos
-0000cfd0: 7428 0a20 2020 2020 2020 2066 222f 6e6f  t(.        f"/no
-0000cfe0: 6465 2f7b 6964 5f6e 6f64 657d 2f65 7865  de/{id_node}/exe
-0000cff0: 6322 2c20 6461 7461 3d64 6174 612c 2068  c", data=data, h
-0000d000: 6561 6465 7273 3d7b 2243 6f6e 7465 6e74  eaders={"Content
-0000d010: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
-0000d020: 7469 6f6e 2f6a 736f 6e22 7d0a 2020 2020  tion/json"}.    
-0000d030: 290a 0a20 2020 2069 6620 280a 2020 2020  )..    if (.    
-0000d040: 2020 2020 7265 7375 6c74 2e73 7461 7475      result.statu
-0000d050: 735f 636f 6465 2021 3d20 3230 300a 2020  s_code != 200.  
-0000d060: 2020 2020 2020 6f72 2073 7461 7475 735f        or status_
-0000d070: 6b65 7920 6e6f 7420 696e 2072 6573 756c  key not in resul
-0000d080: 742e 6a73 6f6e 2829 0a20 2020 2020 2020  t.json().       
-0000d090: 206f 7220 7265 7375 6c74 2e6a 736f 6e28   or result.json(
-0000d0a0: 295b 7374 6174 7573 5f6b 6579 5d20 213d  )[status_key] !=
-0000d0b0: 2022 5354 4152 5445 4422 0a20 2020 2029   "STARTED".    )
-0000d0c0: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
-0000d0d0: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
-0000d0e0: 2243 616e 6e6f 7420 696e 6974 6961 7465  "Cannot initiate
-0000d0f0: 2065 7865 6320 636f 6d6d 616e 6420 6672   exec command fr
-0000d100: 6f6d 2049 5420 5369 6d75 6c61 7469 6f6e  om IT Simulation
-0000d110: 2041 5049 2229 0a0a 2020 2020 6c6f 6767   API")..    logg
-0000d120: 6572 2e69 6e66 6f28 6622 5b2b 5d20 4578  er.info(f"[+] Ex
-0000d130: 6563 7574 696e 6720 636f 6d6d 616e 6420  ecuting command 
-0000d140: 277b 636f 6d6d 616e 647d 2720 666f 7220  '{command}' for 
-0000d150: 6e6f 6465 2027 7b69 645f 6e6f 6465 7d27  node '{id_node}'
-0000d160: 2e2e 2e22 290a 0a20 2020 2023 2057 6169  ...")..    # Wai
-0000d170: 7420 666f 7220 7468 6520 6f70 6572 6174  t for the operat
-0000d180: 696f 6e20 746f 2062 6520 636f 6d70 6c65  ion to be comple
-0000d190: 7465 6420 696e 2062 6163 6b65 6e64 0a20  ted in backend. 
-0000d1a0: 2020 2023 204e 6f74 6520 3a20 6c6f 6f70     # Note : loop
-0000d1b0: 2069 6e73 7069 7265 6420 6672 6f6d 205f   inspired from _
-0000d1c0: 7369 6d75 6c61 7469 6f6e 5f65 7865 6375  simulation_execu
-0000d1d0: 7465 5f6f 7065 7261 7469 6f6e 0a20 2020  te_operation.   
-0000d1e0: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
-0000d1f0: 2020 2020 2023 2053 6c65 6570 2062 6566       # Sleep bef
-0000d200: 6f72 6520 6e65 7874 2069 7465 7261 7469  ore next iterati
-0000d210: 6f6e 0a20 2020 2020 2020 2074 696d 652e  on.        time.
-0000d220: 736c 6565 7028 3229 0a0a 2020 2020 2020  sleep(2)..      
-0000d230: 2020 2320 4665 7463 6820 7468 6520 6375    # Fetch the cu
-0000d240: 7272 656e 7420 7374 6174 7573 206f 6620  rrent status of 
-0000d250: 7468 6520 6d65 6d64 756d 700a 2020 2020  the memdump.    
-0000d260: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
-0000d270: 7428 6622 2f6e 6f64 652f 7b69 645f 6e6f  t(f"/node/{id_no
-0000d280: 6465 7d2f 6578 6563 5f73 7461 7475 7322  de}/exec_status"
-0000d290: 290a 0a20 2020 2020 2020 2069 6620 7265  )..        if re
-0000d2a0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-0000d2b0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
-0000d2c0: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
-0000d2d0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000d2e0: 2020 2020 7265 7375 6c74 2c20 2243 616e      result, "Can
-0000d2f0: 6e6f 7420 6765 7420 7374 6174 7573 206f  not get status o
-0000d300: 6620 6578 6563 2063 6f6d 6d61 6e64 2066  f exec command f
-0000d310: 726f 6d20 4954 2053 696d 756c 6174 696f  rom IT Simulatio
-0000d320: 6e20 4150 4922 0a20 2020 2020 2020 2020  n API".         
-0000d330: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
-0000d340: 7375 6c74 5f6a 736f 6e20 3d20 7265 7375  sult_json = resu
-0000d350: 6c74 2e6a 736f 6e28 290a 2020 2020 2020  lt.json().      
-0000d360: 2020 6966 206e 6f74 2028 616c 6c28 6b20    if not (all(k 
-0000d370: 696e 2072 6573 756c 745f 6a73 6f6e 2066  in result_json f
-0000d380: 6f72 206b 2069 6e20 2865 7869 745f 636f  or k in (exit_co
-0000d390: 6465 2c20 7374 646f 7574 2c20 7374 6465  de, stdout, stde
-0000d3a0: 7272 2c20 7374 6174 7573 5f6b 6579 2929  rr, status_key))
-0000d3b0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000d3c0: 6169 7365 2045 7863 6570 7469 6f6e 280a  aise Exception(.
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 6622 436f 6e74 656e 7473 206f 6620 6578  f"Contents of ex
-0000d3f0: 6563 2063 6f6d 6d61 6e64 2073 7461 7475  ec command statu
-0000d400: 7320 7570 6461 7465 2069 7320 6e6f 7420  s update is not 
-0000d410: 696e 2074 6865 2065 7870 6563 7465 6420  in the expected 
-0000d420: 666f 726d 6174 2028 6174 7472 6962 7574  format (attribut
-0000d430: 6573 2027 7b65 7869 745f 636f 6465 7d27  es '{exit_code}'
-0000d440: 2c20 277b 7374 646f 7574 7d27 2c20 277b  , '{stdout}', '{
-0000d450: 7374 6465 7272 7d27 2061 6e64 2027 7b73  stderr}' and '{s
-0000d460: 7461 7475 735f 6b65 797d 2720 6578 7065  tatus_key}' expe
-0000d470: 6374 6564 2922 0a20 2020 2020 2020 2020  cted)".         
-0000d480: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-0000d490: 4c6f 6720 696e 666f 206f 6e20 7072 6f67  Log info on prog
-0000d4a0: 7265 7373 696f 6e0a 2020 2020 2020 2020  ression.        
-0000d4b0: 6966 2072 6573 756c 745f 6a73 6f6e 5b73  if result_json[s
-0000d4c0: 7461 7475 735f 6b65 795d 203d 3d20 2253  tatus_key] == "S
-0000d4d0: 5441 5254 4544 223a 0a20 2020 2020 2020  TARTED":.       
-0000d4e0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-0000d4f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000d500: 2020 6622 2020 5b2b 5d20 4375 7272 656e    f"  [+] Curren
-0000d510: 746c 7920 7761 6974 696e 6720 666f 7220  tly waiting for 
-0000d520: 6578 6563 2063 6f6d 6d61 6e64 2066 6f72  exec command for
-0000d530: 206e 6f64 6520 277b 6964 5f6e 6f64 657d   node '{id_node}
-0000d540: 2729 2074 6f20 7374 6172 742e 2e2e 220a  ') to start...".
-0000d550: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000d560: 2020 2020 2020 656c 6966 2072 6573 756c        elif resul
-0000d570: 745f 6a73 6f6e 5b73 7461 7475 735f 6b65  t_json[status_ke
-0000d580: 795d 203d 3d20 2250 524f 4752 4553 5322  y] == "PROGRESS"
-0000d590: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-0000d5a0: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
-0000d5b0: 2020 2020 2020 2020 2020 2066 2220 205b             f"  [
-0000d5c0: 2b5d 2043 7572 7265 6e74 6c79 2070 6572  +] Currently per
-0000d5d0: 666f 726d 696e 6720 6578 6563 2063 6f6d  forming exec com
-0000d5e0: 6d61 6e64 2066 6f72 206e 6f64 6520 277b  mand for node '{
-0000d5f0: 6964 5f6e 6f64 657d 2729 2e2e 2e22 0a20  id_node}')...". 
-0000d600: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000d610: 2020 2020 2065 6c69 6620 7265 7375 6c74       elif result
-0000d620: 5f6a 736f 6e5b 7374 6174 7573 5f6b 6579  _json[status_key
-0000d630: 5d20 3d3d 2022 5355 4343 4553 5322 3a0a  ] == "SUCCESS":.
-0000d640: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0000d650: 6b0a 2020 2020 2020 2020 656c 7365 3a0a  k.        else:.
-0000d660: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000d670: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
-0000d680: 2020 2020 2020 2020 2020 2020 2022 4572               "Er
-0000d690: 726f 7220 6475 7269 6e67 2065 7865 6320  ror during exec 
-0000d6a0: 636f 6d6d 616e 6420 666f 7220 6e6f 6465  command for node
-0000d6b0: 207b 7d20 6f70 6572 6174 696f 6e3a 2027   {} operation: '
-0000d6c0: 7b7d 2722 2e66 6f72 6d61 7428 0a20 2020  {}'".format(.   
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6e0: 2069 645f 6e6f 6465 2c20 7265 7375 6c74   id_node, result
-0000d6f0: 5f6a 736f 6e5b 7374 6174 7573 5f6b 6579  _json[status_key
-0000d700: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000d710: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000d720: 290a 0a20 2020 206c 6f67 6765 722e 696e  )..    logger.in
-0000d730: 666f 2822 5b2b 5d20 4e6f 6465 2065 7865  fo("[+] Node exe
-0000d740: 6320 636f 6d6d 616e 6420 6669 6e69 7368  c command finish
-0000d750: 6564 2229 0a0a 2020 2020 7265 7475 726e  ed")..    return
-0000d760: 2028 7265 7375 6c74 5f6a 736f 6e5b 6578   (result_json[ex
-0000d770: 6974 5f63 6f64 655d 2c20 7265 7375 6c74  it_code], result
-0000d780: 5f6a 736f 6e5b 7374 646f 7574 5d2c 2072  _json[stdout], r
-0000d790: 6573 756c 745f 6a73 6f6e 5b73 7464 6572  esult_json[stder
-0000d7a0: 725d 290a 0a0a 6465 6620 6e6f 6465 5f6d  r])...def node_m
-0000d7b0: 656d 6f72 7964 756d 7028 6964 5f6e 6f64  emorydump(id_nod
-0000d7c0: 653a 2069 6e74 2920 2d3e 2041 6e79 3a0a  e: int) -> Any:.
-0000d7d0: 2020 2020 2222 220a 2020 2020 5265 7475      """.    Retu
-0000d7e0: 726e 2052 414d 2064 756d 7020 6f66 2061  rn RAM dump of a
-0000d7f0: 206e 6f64 6520 696e 2061 2072 756e 6e69   node in a runni
-0000d800: 6e67 2073 696d 756c 6174 696f 6e0a 2020  ng simulation.  
-0000d810: 2020 4e6f 7465 3a20 796f 7520 6361 6e20    Note: you can 
-0000d820: 6765 7420 7468 6520 6e6f 6465 2049 4473  get the node IDs
-0000d830: 2075 7369 6e67 2074 6865 2073 696d 755f   using the simu_
-0000d840: 7374 6174 7573 2063 6f6d 6d61 6e64 2028  status command (
-0000d850: 6f72 2074 6865 2066 6574 6368 5f73 696d  or the fetch_sim
-0000d860: 756c 6174 696f 6e73 2829 2066 756e 6374  ulations() funct
-0000d870: 696f 6e29 2e0a 2020 2020 2222 220a 2020  ion)..    """.  
-0000d880: 2020 6669 6c65 5f70 6174 685f 6b65 7920    file_path_key 
-0000d890: 3d20 2266 696c 655f 7061 7468 220a 2020  = "file_path".  
-0000d8a0: 2020 6669 6c65 5f73 697a 655f 6b65 7920    file_size_key 
-0000d8b0: 3d20 2266 696c 655f 7369 7a65 220a 2020  = "file_size".  
-0000d8c0: 2020 7374 6174 7573 5f6b 6579 203d 2022    status_key = "
-0000d8d0: 7374 6174 7573 220a 0a20 2020 2072 6573  status"..    res
-0000d8e0: 756c 7420 3d20 5f67 6574 2866 222f 6e6f  ult = _get(f"/no
-0000d8f0: 6465 2f7b 6964 5f6e 6f64 657d 2f6d 656d  de/{id_node}/mem
-0000d900: 6f72 7964 756d 7022 290a 0a20 2020 2069  orydump")..    i
-0000d910: 6620 280a 2020 2020 2020 2020 7265 7375  f (.        resu
-0000d920: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000d930: 3d20 3230 300a 2020 2020 2020 2020 6f72  = 200.        or
-0000d940: 2073 7461 7475 735f 6b65 7920 6e6f 7420   status_key not 
-0000d950: 696e 2072 6573 756c 742e 6a73 6f6e 2829  in result.json()
-0000d960: 0a20 2020 2020 2020 206f 7220 7265 7375  .        or resu
-0000d970: 6c74 2e6a 736f 6e28 295b 7374 6174 7573  lt.json()[status
-0000d980: 5f6b 6579 5d20 213d 2022 5354 4152 5445  _key] != "STARTE
-0000d990: 4422 0a20 2020 2029 3a0a 2020 2020 2020  D".    ):.      
-0000d9a0: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-0000d9b0: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-0000d9c0: 696e 6974 6961 7465 206e 6f64 6520 6d65  initiate node me
-0000d9d0: 6d6f 7279 2064 756d 7020 6672 6f6d 2063  mory dump from c
-0000d9e0: 6f72 6520 4150 4922 290a 0a20 2020 206c  ore API")..    l
-0000d9f0: 6f67 6765 722e 696e 666f 2822 5b2b 5d20  ogger.info("[+] 
-0000da00: 496e 6974 6961 6c69 7a65 6420 6d65 6d6f  Initialized memo
-0000da10: 7279 2064 756d 7020 6f66 206e 6f64 6520  ry dump of node 
-0000da20: 277b 7d27 2e2e 2e22 2e66 6f72 6d61 7428  '{}'...".format(
-0000da30: 6964 5f6e 6f64 6529 290a 0a20 2020 2023  id_node))..    #
-0000da40: 2057 6169 7420 666f 7220 7468 6520 6f70   Wait for the op
-0000da50: 6572 6174 696f 6e20 746f 2062 6520 636f  eration to be co
-0000da60: 6d70 6c65 7465 6420 696e 2062 6163 6b65  mpleted in backe
-0000da70: 6e64 0a20 2020 2023 204e 6f74 6520 3a20  nd.    # Note : 
-0000da80: 6c6f 6f70 2069 6e73 7069 7265 6420 6672  loop inspired fr
-0000da90: 6f6d 205f 7369 6d75 6c61 7469 6f6e 5f65  om _simulation_e
-0000daa0: 7865 6375 7465 5f6f 7065 7261 7469 6f6e  xecute_operation
-0000dab0: 0a20 2020 2077 6869 6c65 2054 7275 653a  .    while True:
-0000dac0: 0a20 2020 2020 2020 2023 2053 6c65 6570  .        # Sleep
-0000dad0: 2062 6566 6f72 6520 6e65 7874 2069 7465   before next ite
-0000dae0: 7261 7469 6f6e 0a20 2020 2020 2020 2074  ration.        t
-0000daf0: 696d 652e 736c 6565 7028 3229 0a0a 2020  ime.sleep(2)..  
-0000db00: 2020 2020 2020 2320 4665 7463 6820 7468        # Fetch th
-0000db10: 6520 6375 7272 656e 7420 7374 6174 7573  e current status
-0000db20: 206f 6620 7468 6520 6d65 6d64 756d 700a   of the memdump.
-0000db30: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000db40: 205f 6765 7428 6622 2f6e 6f64 652f 7b69   _get(f"/node/{i
-0000db50: 645f 6e6f 6465 7d2f 6d65 6d6f 7279 6475  d_node}/memorydu
-0000db60: 6d70 5f73 7461 7475 7322 290a 0a20 2020  mp_status")..   
-0000db70: 2020 2020 2069 6620 7265 7375 6c74 2e73       if result.s
-0000db80: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-0000db90: 303a 0a20 2020 2020 2020 2020 2020 205f  0:.            _
-0000dba0: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-0000dbb0: 756c 742c 2022 4361 6e6e 6f74 2067 6574  ult, "Cannot get
-0000dbc0: 2073 7461 7475 7320 6f66 206e 6f64 6520   status of node 
-0000dbd0: 6d65 6d6f 7279 2064 756d 7020 6672 6f6d  memory dump from
-0000dbe0: 2063 6f72 6520 4150 4922 290a 0a20 2020   core API")..   
-0000dbf0: 2020 2020 2072 6573 756c 745f 6a73 6f6e       result_json
-0000dc00: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
-0000dc10: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000dc20: 280a 2020 2020 2020 2020 2020 2020 616c  (.            al
-0000dc30: 6c28 6b20 696e 2072 6573 756c 745f 6a73  l(k in result_js
-0000dc40: 6f6e 2066 6f72 206b 2069 6e20 2866 696c  on for k in (fil
-0000dc50: 655f 7061 7468 5f6b 6579 2c20 6669 6c65  e_path_key, file
-0000dc60: 5f73 697a 655f 6b65 792c 2073 7461 7475  _size_key, statu
-0000dc70: 735f 6b65 7929 290a 2020 2020 2020 2020  s_key)).        
-0000dc80: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000dc90: 6169 7365 2045 7863 6570 7469 6f6e 280a  aise Exception(.
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcb0: 6622 436f 6e74 656e 7473 206f 6620 6d65  f"Contents of me
-0000dcc0: 6d6f 7279 2064 756d 7020 7374 6174 7573  mory dump status
-0000dcd0: 2075 7064 6174 6520 6973 206e 6f74 2069   update is not i
-0000dce0: 6e20 7468 6520 6578 7065 6374 6564 2066  n the expected f
-0000dcf0: 6f72 6d61 7420 2861 7474 7269 6275 7465  ormat (attribute
-0000dd00: 7320 277b 6669 6c65 5f70 6174 685f 6b65  s '{file_path_ke
-0000dd10: 797d 272c 2027 7b66 696c 655f 7369 7a65  y}', '{file_size
-0000dd20: 5f6b 6579 7d27 2061 6e64 2027 7b73 7461  _key}' and '{sta
-0000dd30: 7475 735f 6b65 797d 2720 6578 7065 6374  tus_key}' expect
-0000dd40: 6564 2922 0a20 2020 2020 2020 2020 2020  ed)".           
-0000dd50: 2029 0a0a 2020 2020 2020 2020 2320 4c6f   )..        # Lo
-0000dd60: 6720 696e 666f 206f 6e20 7072 6f67 7265  g info on progre
-0000dd70: 7373 696f 6e0a 2020 2020 2020 2020 6966  ssion.        if
-0000dd80: 2072 6573 756c 745f 6a73 6f6e 5b73 7461   result_json[sta
-0000dd90: 7475 735f 6b65 795d 203d 3d20 2250 524f  tus_key] == "PRO
-0000dda0: 4752 4553 5322 3a0a 2020 2020 2020 2020  GRESS":.        
-0000ddb0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-0000ddc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ddd0: 2022 2020 5b2b 5d20 4375 7272 656e 746c   "  [+] Currentl
-0000dde0: 7920 7065 7266 6f72 6d69 6e67 206d 656d  y performing mem
-0000ddf0: 6f72 7920 6475 6d70 206f 6620 6e6f 6465  ory dump of node
-0000de00: 2027 7b7d 2720 2863 7572 7265 6e74 2064   '{}' (current d
-0000de10: 756d 7020 6669 6c65 2073 697a 6520 6973  ump file size is
-0000de20: 207b 7d29 2e2e 2e22 2e66 6f72 6d61 7428   {})...".format(
-0000de30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de40: 2020 2020 2069 645f 6e6f 6465 2c20 6e61       id_node, na
-0000de50: 7475 7261 6c73 697a 6528 7265 7375 6c74  turalsize(result
-0000de60: 5f6a 736f 6e5b 6669 6c65 5f73 697a 655f  _json[file_size_
-0000de70: 6b65 795d 2c20 6269 6e61 7279 3d54 7275  key], binary=Tru
-0000de80: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000de90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000dea0: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
-0000deb0: 7265 7375 6c74 5f6a 736f 6e5b 7374 6174  result_json[stat
-0000dec0: 7573 5f6b 6579 5d20 3d3d 2022 5355 4343  us_key] == "SUCC
-0000ded0: 4553 5322 3a0a 2020 2020 2020 2020 2020  ESS":.          
-0000dee0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-0000def0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000df00: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-0000df10: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-0000df20: 2020 2022 4572 726f 7220 6475 7269 6e67     "Error during
-0000df30: 206d 656d 6f72 7920 6475 6d70 206f 6620   memory dump of 
-0000df40: 6e6f 6465 207b 7d20 6f70 6572 6174 696f  node {} operatio
-0000df50: 6e3a 2027 7b7d 2722 2e66 6f72 6d61 7428  n: '{}'".format(
-0000df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df70: 2020 2020 2069 645f 6e6f 6465 2c20 7265       id_node, re
-0000df80: 7375 6c74 5f6a 736f 6e5b 7374 6174 7573  sult_json[status
-0000df90: 5f6b 6579 5d0a 2020 2020 2020 2020 2020  _key].          
-0000dfa0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000dfb0: 2020 2020 290a 0a20 2020 206c 6f67 6765      )..    logge
-0000dfc0: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
-0000dfd0: 225b 2b5d 204e 6f64 6520 6d65 6d6f 7279  "[+] Node memory
-0000dfe0: 2064 756d 7020 2872 6177 2064 756d 7020   dump (raw dump 
-0000dff0: 7769 7468 206c 6962 7669 7274 2920 6f62  with libvirt) ob
-0000e000: 7461 696e 6564 2c20 616e 6420 706c 6163  tained, and plac
-0000e010: 6564 2069 6e20 6669 6c65 207b 7d20 287b  ed in file {} ({
-0000e020: 7d29 206f 6e20 7468 6520 7365 7276 6572  }) on the server
-0000e030: 2e22 2e66 6f72 6d61 7428 0a20 2020 2020  .".format(.     
-0000e040: 2020 2020 2020 2072 6573 756c 745f 6a73         result_js
-0000e050: 6f6e 5b66 696c 655f 7061 7468 5f6b 6579  on[file_path_key
-0000e060: 5d2c 0a20 2020 2020 2020 2020 2020 206e  ],.            n
-0000e070: 6174 7572 616c 7369 7a65 2872 6573 756c  aturalsize(resul
-0000e080: 745f 6a73 6f6e 5b66 696c 655f 7369 7a65  t_json[file_size
-0000e090: 5f6b 6579 5d2c 2062 696e 6172 793d 5472  _key], binary=Tr
-0000e0a0: 7565 292c 0a20 2020 2020 2020 2029 0a20  ue),.        ). 
-0000e0b0: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
-0000e0c0: 2072 6573 756c 745f 6a73 6f6e 5b66 696c   result_json[fil
-0000e0d0: 655f 7061 7468 5f6b 6579 5d2c 2072 6573  e_path_key], res
-0000e0e0: 756c 745f 6a73 6f6e 5b66 696c 655f 7369  ult_json[file_si
-0000e0f0: 7a65 5f6b 6579 5d0a 0a0a 6465 6620 6665  ze_key]...def fe
-0000e100: 7463 685f 6e6f 6465 5f6e 6574 776f 726b  tch_node_network
-0000e110: 5f69 6e74 6572 6661 6365 7328 6964 5f6e  _interfaces(id_n
-0000e120: 6f64 653a 2069 6e74 2920 2d3e 2041 6e79  ode: int) -> Any
-0000e130: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
-0000e140: 6e65 7477 6f72 6b20 696e 7465 7266 6163  network interfac
-0000e150: 6573 206c 6973 7420 6769 7665 6e20 6120  es list given a 
-0000e160: 6e6f 6465 2049 442e 2222 220a 2020 2020  node ID.""".    
-0000e170: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
-0000e180: 2f6e 6f64 652f 7b69 645f 6e6f 6465 7d2f  /node/{id_node}/
-0000e190: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-0000e1a0: 6522 290a 0a20 2020 2069 6620 7265 7375  e")..    if resu
-0000e1b0: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000e1c0: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-0000e1d0: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-0000e1e0: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
-0000e1f0: 7269 6576 6520 6e6f 6465 206e 6574 776f  rieve node netwo
-0000e200: 726b 2069 6e74 6572 6661 6365 7322 290a  rk interfaces").
-0000e210: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
-0000e220: 6c74 2e6a 736f 6e28 290a 0a0a 6465 6620  lt.json()...def 
-0000e230: 6665 7463 685f 7369 6d75 6c61 7469 6f6e  fetch_simulation
-0000e240: 5f6e 6574 776f 726b 5f69 6e74 6572 6661  _network_interfa
-0000e250: 6365 7328 6964 5f73 696d 756c 6174 696f  ces(id_simulatio
-0000e260: 6e3a 2069 6e74 2920 2d3e 2041 6e79 3a0a  n: int) -> Any:.
-0000e270: 2020 2020 2222 2252 6574 7572 6e20 6e65      """Return ne
-0000e280: 7477 6f72 6b20 696e 7465 7266 6163 6573  twork interfaces
-0000e290: 206c 6973 7420 6769 7665 6e20 6120 7369   list given a si
-0000e2a0: 6d75 6c61 7469 6f6e 2049 442e 2222 220a  mulation ID.""".
-0000e2b0: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
-0000e2c0: 7428 6622 2f73 696d 756c 6174 696f 6e2f  t(f"/simulation/
-0000e2d0: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d2f  {id_simulation}/
-0000e2e0: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-0000e2f0: 6522 290a 0a20 2020 2069 6620 7265 7375  e")..    if resu
-0000e300: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000e310: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-0000e320: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-0000e330: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
-0000e340: 7269 6576 6520 7369 6d75 6c61 7469 6f6e  rieve simulation
-0000e350: 206e 6574 776f 726b 2069 6e74 6572 6661   network interfa
-0000e360: 6365 7322 290a 0a20 2020 2072 6574 7572  ces")..    retur
-0000e370: 6e20 7265 7375 6c74 2e6a 736f 6e28 290a  n result.json().
-0000e380: 0a0a 6465 6620 6665 7463 685f 6e65 7477  ..def fetch_netw
-0000e390: 6f72 6b5f 696e 7465 7266 6163 655f 6279  ork_interface_by
-0000e3a0: 5f6d 6163 2869 645f 7369 6d75 6c61 7469  _mac(id_simulati
-0000e3b0: 6f6e 3a20 696e 742c 206d 6163 5f61 6464  on: int, mac_add
-0000e3c0: 7265 7373 3a20 7374 7229 202d 3e20 416e  ress: str) -> An
-0000e3d0: 793a 0a20 2020 2022 2222 5265 7475 726e  y:.    """Return
-0000e3e0: 206e 6574 776f 726b 2069 6e74 6572 6661   network interfa
-0000e3f0: 6365 206c 6973 7420 6769 7665 6e20 6120  ce list given a 
-0000e400: 6d61 6320 6164 6472 6573 732e 2222 220a  mac address.""".
-0000e410: 2020 2020 2320 4665 7463 6820 6e6f 6465      # Fetch node
-0000e420: 206e 6574 776f 726b 2069 6e74 6572 6661   network interfa
-0000e430: 6365 730a 2020 2020 7265 7375 6c74 203d  ces.    result =
-0000e440: 205f 6765 7428 6622 2f73 696d 756c 6174   _get(f"/simulat
-0000e450: 696f 6e2f 7b69 645f 7369 6d75 6c61 7469  ion/{id_simulati
-0000e460: 6f6e 7d2f 6e65 7477 6f72 6b5f 696e 7465  on}/network_inte
-0000e470: 7266 6163 6522 290a 0a20 2020 2069 6620  rface")..    if 
-0000e480: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-0000e490: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-0000e4a0: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-0000e4b0: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-0000e4c0: 2072 6574 7269 6576 6520 6e65 7477 6f72   retrieve networ
-0000e4d0: 6b20 696e 7465 7266 6163 6573 2229 0a0a  k interfaces")..
-0000e4e0: 2020 2020 6e65 7477 6f72 6b5f 696e 7465      network_inte
-0000e4f0: 7266 6163 6573 203d 2072 6573 756c 742e  rfaces = result.
-0000e500: 6a73 6f6e 2829 0a0a 2020 2020 666f 7220  json()..    for 
-0000e510: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-0000e520: 6520 696e 206e 6574 776f 726b 5f69 6e74  e in network_int
-0000e530: 6572 6661 6365 733a 0a20 2020 2020 2020  erfaces:.       
-0000e540: 2069 6620 6e65 7477 6f72 6b5f 696e 7465   if network_inte
-0000e550: 7266 6163 655b 226d 6163 5f61 6464 7265  rface["mac_addre
-0000e560: 7373 225d 203d 3d20 6d61 635f 6164 6472  ss"] == mac_addr
-0000e570: 6573 733a 0a20 2020 2020 2020 2020 2020  ess:.           
-0000e580: 2072 6574 7572 6e20 6e65 7477 6f72 6b5f   return network_
-0000e590: 696e 7465 7266 6163 650a 2020 2020 656c  interface.    el
-0000e5a0: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-0000e5b0: 726e 204e 6f6e 650a 0a0a 6465 6620 6465  rn None...def de
-0000e5c0: 6c65 7465 5f6e 6574 776f 726b 5f69 6e74  lete_network_int
-0000e5d0: 6572 6661 6365 2869 645f 6e65 7477 6f72  erface(id_networ
-0000e5e0: 6b5f 696e 7465 7266 6163 653a 2069 6e74  k_interface: int
-0000e5f0: 2920 2d3e 2041 6e79 3a0a 2020 2020 2222  ) -> Any:.    ""
-0000e600: 2244 656c 6574 6520 6e65 7477 6f72 6b20  "Delete network 
-0000e610: 696e 7465 7266 6163 6520 6769 7665 6e20  interface given 
-0000e620: 616e 2069 642e 2222 220a 2020 2020 7265  an id.""".    re
-0000e630: 7375 6c74 203d 205f 6465 6c65 7465 2866  sult = _delete(f
-0000e640: 222f 6e65 7477 6f72 6b5f 696e 7465 7266  "/network_interf
-0000e650: 6163 652f 7b69 645f 6e65 7477 6f72 6b5f  ace/{id_network_
-0000e660: 696e 7465 7266 6163 657d 2229 0a0a 2020  interface}")..  
-0000e670: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
-0000e680: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
-0000e690: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
-0000e6a0: 6572 726f 7228 0a20 2020 2020 2020 2020  error(.         
-0000e6b0: 2020 2072 6573 756c 742c 2022 4361 6e6e     result, "Cann
-0000e6c0: 6f74 2072 6574 7269 6576 6520 6e6f 6465  ot retrieve node
-0000e6d0: 206e 6574 776f 726b 2069 6e74 6572 6661   network interfa
-0000e6e0: 6365 7320 6672 6f6d 2049 5420 5369 6d75  ces from IT Simu
-0000e6f0: 6c61 7469 6f6e 2041 5049 220a 2020 2020  lation API".    
-0000e700: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
-0000e710: 6e20 7265 7375 6c74 2e6a 736f 6e28 290a  n result.json().
-0000e720: 0a0a 6465 6620 7570 6461 7465 5f6e 6574  ..def update_net
-0000e730: 776f 726b 5f69 6e74 6572 6661 6365 280a  work_interface(.
-0000e740: 2020 2020 6964 5f6e 6574 776f 726b 5f69      id_network_i
-0000e750: 6e74 6572 6661 6365 3a20 696e 742c 206e  nterface: int, n
-0000e760: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-0000e770: 5f64 6963 743a 2064 6963 740a 2920 2d3e  _dict: dict.) ->
-0000e780: 2041 6e79 3a0a 2020 2020 2222 2255 7064   Any:.    """Upd
-0000e790: 6174 6520 6e65 7477 6f72 6b20 696e 7465  ate network inte
-0000e7a0: 7266 6163 6520 696e 666f 726d 6174 696f  rface informatio
-0000e7b0: 6e20 696e 666f 726d 6174 696f 6e20 6769  n information gi
-0000e7c0: 7665 6e20 6120 6e65 7477 6f72 6b20 696e  ven a network in
-0000e7d0: 7465 7266 6163 6520 6964 2061 6e64 2061  terface id and a
-0000e7e0: 0a20 2020 2064 6963 7420 636f 6e74 6169  .    dict contai
-0000e7f0: 6e69 6e67 206e 6574 776f 726b 2069 6e66  ning network inf
-0000e800: 6f2e 0a0a 2020 2020 2222 220a 2020 2020  o...    """.    
-0000e810: 6461 7461 203d 206a 736f 6e2e 6475 6d70  data = json.dump
-0000e820: 7328 6e65 7477 6f72 6b5f 696e 7465 7266  s(network_interf
-0000e830: 6163 655f 6469 6374 290a 2020 2020 7265  ace_dict).    re
-0000e840: 7375 6c74 203d 205f 7075 7428 0a20 2020  sult = _put(.   
-0000e850: 2020 2020 2066 222f 6e65 7477 6f72 6b5f       f"/network_
-0000e860: 696e 7465 7266 6163 652f 7b69 645f 6e65  interface/{id_ne
-0000e870: 7477 6f72 6b5f 696e 7465 7266 6163 657d  twork_interface}
-0000e880: 222c 0a20 2020 2020 2020 2064 6174 613d  ",.        data=
-0000e890: 6461 7461 2c0a 2020 2020 2020 2020 6865  data,.        he
-0000e8a0: 6164 6572 733d 7b22 436f 6e74 656e 742d  aders={"Content-
-0000e8b0: 5479 7065 223a 2022 6170 706c 6963 6174  Type": "applicat
-0000e8c0: 696f 6e2f 6a73 6f6e 227d 2c0a 2020 2020  ion/json"},.    
-0000e8d0: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
-0000e8e0: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-0000e8f0: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
-0000e900: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
-0000e910: 742c 2022 4361 6e6e 6f74 2075 7064 6174  t, "Cannot updat
-0000e920: 6520 6e65 7477 6f72 6b20 696e 7465 7266  e network interf
-0000e930: 6163 6520 696e 666f 726d 6174 696f 6e22  ace information"
-0000e940: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
-0000e950: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
-0000e960: 6620 6665 7463 685f 7072 6f62 6528 7072  f fetch_probe(pr
-0000e970: 6f62 655f 6964 3a20 696e 7429 202d 3e20  obe_id: int) -> 
-0000e980: 416e 793a 0a20 2020 2022 2222 5265 7475  Any:.    """Retu
-0000e990: 726e 2061 2070 726f 6265 2067 6976 656e  rn a probe given
-0000e9a0: 2069 7473 2049 4422 2222 0a0a 2020 2020   its ID"""..    
-0000e9b0: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
-0000e9c0: 2f70 726f 6265 2f7b 7072 6f62 655f 6964  /probe/{probe_id
-0000e9d0: 7d22 290a 0a20 2020 2069 6620 7265 7375  }")..    if resu
-0000e9e0: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000e9f0: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-0000ea00: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-0000ea10: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
-0000ea20: 7269 6576 6520 7072 6f62 6520 6672 6f6d  rieve probe from
-0000ea30: 2063 6f72 6520 4150 4922 290a 0a20 2020   core API")..   
-0000ea40: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
-0000ea50: 736f 6e28 290a 0a0a 6465 6620 6665 7463  son()...def fetc
-0000ea60: 685f 7072 6f62 6573 2869 645f 7369 6d75  h_probes(id_simu
-0000ea70: 6c61 7469 6f6e 3a20 696e 7429 202d 3e20  lation: int) -> 
-0000ea80: 416e 793a 0a20 2020 2022 2222 5265 7475  Any:.    """Retu
-0000ea90: 726e 2073 696d 756c 6174 696f 6e20 7072  rn simulation pr
-0000eaa0: 6f62 6573 2064 6963 7420 6769 7665 6e0a  obes dict given.
-0000eab0: 2020 2020 6120 7369 6d75 6c61 7469 6f6e      a simulation
-0000eac0: 2049 442c 2077 6865 7265 206b 6579 7320   ID, where keys 
-0000ead0: 6172 6520 7072 6f62 6573 2069 6473 2e0a  are probes ids..
-0000eae0: 2020 2020 2222 220a 0a20 2020 2072 6573      """..    res
-0000eaf0: 756c 7420 3d20 5f67 6574 2866 222f 7369  ult = _get(f"/si
-0000eb00: 6d75 6c61 7469 6f6e 2f7b 6964 5f73 696d  mulation/{id_sim
-0000eb10: 756c 6174 696f 6e7d 2f70 726f 6265 2229  ulation}/probe")
-0000eb20: 0a0a 2020 2020 6966 2072 6573 756c 742e  ..    if result.
-0000eb30: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
-0000eb40: 3030 3a0a 2020 2020 2020 2020 5f68 616e  00:.        _han
-0000eb50: 646c 655f 6572 726f 7228 7265 7375 6c74  dle_error(result
-0000eb60: 2c20 2243 616e 6e6f 7420 7265 7472 6965  , "Cannot retrie
-0000eb70: 7665 2073 696d 756c 6174 696f 6e20 7072  ve simulation pr
-0000eb80: 6f62 6573 2066 726f 6d20 636f 7265 2041  obes from core A
-0000eb90: 5049 2229 0a0a 2020 2020 7265 7475 726e  PI")..    return
-0000eba0: 2072 6573 756c 742e 6a73 6f6e 2829 0a0a   result.json()..
-0000ebb0: 0a64 6566 2063 7265 6174 655f 7072 6f62  .def create_prob
-0000ebc0: 6528 0a20 2020 2069 645f 7369 6d75 6c61  e(.    id_simula
-0000ebd0: 7469 6f6e 3a20 696e 742c 0a20 2020 206e  tion: int,.    n
-0000ebe0: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-0000ebf0: 733a 204c 6973 745b 696e 745d 2c0a 2020  s: List[int],.  
-0000ec00: 2020 6966 6163 653a 2073 7472 2c0a 2020    iface: str,.  
-0000ec10: 2020 7063 6170 3a20 626f 6f6c 2c0a 2020    pcap: bool,.  
-0000ec20: 2020 6669 6c74 6572 3a20 7374 722c 0a20    filter: str,. 
-0000ec30: 2020 2064 6972 6563 7469 6f6e 3a20 7374     direction: st
-0000ec40: 722c 0a29 202d 3e20 696e 743a 0a20 2020  r,.) -> int:.   
-0000ec50: 2022 2222 4372 6561 7465 2061 206e 6577   """Create a new
-0000ec60: 2070 726f 6265 2066 6f72 2074 6865 2073   probe for the s
-0000ec70: 696d 756c 6174 696f 6e20 6769 7665 6e20  imulation given 
-0000ec80: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
-0000ec90: 6720 7072 6f62 6520 6461 7461 2222 220a  g probe data""".
-0000eca0: 0a20 2020 2064 6174 615f 6469 6374 203d  .    data_dict =
-0000ecb0: 207b 0a20 2020 2020 2020 2022 6966 6163   {.        "ifac
-0000ecc0: 6522 3a20 6966 6163 652c 0a20 2020 2020  e": iface,.     
-0000ecd0: 2020 2022 7063 6170 223a 2070 6361 702c     "pcap": pcap,
-0000ece0: 0a20 2020 2020 2020 2022 6669 6c74 6572  .        "filter
-0000ecf0: 223a 2066 696c 7465 722c 0a20 2020 2020  ": filter,.     
-0000ed00: 2020 2022 6e65 7477 6f72 6b5f 696e 7465     "network_inte
-0000ed10: 7266 6163 6573 223a 206e 6574 776f 726b  rfaces": network
-0000ed20: 5f69 6e74 6572 6661 6365 732c 0a20 2020  _interfaces,.   
-0000ed30: 2020 2020 2022 6469 7265 6374 696f 6e22       "direction"
-0000ed40: 3a20 6469 7265 6374 696f 6e2c 0a20 2020  : direction,.   
-0000ed50: 207d 0a0a 2020 2020 6461 7461 203d 206a   }..    data = j
-0000ed60: 736f 6e2e 6475 6d70 7328 6461 7461 5f64  son.dumps(data_d
-0000ed70: 6963 7429 0a20 2020 2072 6573 756c 7420  ict).    result 
-0000ed80: 3d20 5f70 6f73 7428 0a20 2020 2020 2020  = _post(.       
-0000ed90: 2066 222f 7369 6d75 6c61 7469 6f6e 2f7b   f"/simulation/{
-0000eda0: 6964 5f73 696d 756c 6174 696f 6e7d 2f70  id_simulation}/p
-0000edb0: 726f 6265 222c 0a20 2020 2020 2020 2064  robe",.        d
-0000edc0: 6174 613d 6461 7461 2c0a 2020 2020 2020  ata=data,.      
-0000edd0: 2020 6865 6164 6572 733d 7b22 436f 6e74    headers={"Cont
-0000ede0: 656e 742d 5479 7065 223a 2022 6170 706c  ent-Type": "appl
-0000edf0: 6963 6174 696f 6e2f 6a73 6f6e 227d 2c0a  ication/json"},.
-0000ee00: 2020 2020 290a 0a20 2020 2069 6620 7265      )..    if re
-0000ee10: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-0000ee20: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
-0000ee30: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
-0000ee40: 6573 756c 742c 2022 4361 6e6e 6f74 2063  esult, "Cannot c
-0000ee50: 7265 6174 6520 7072 6f62 6520 7769 7468  reate probe with
-0000ee60: 2063 6f72 6520 4150 4922 290a 0a20 2020   core API")..   
-0000ee70: 2070 726f 6265 5f69 6420 3d20 7265 7375   probe_id = resu
-0000ee80: 6c74 2e6a 736f 6e28 295b 2269 6422 5d0a  lt.json()["id"].
-0000ee90: 0a20 2020 2072 6574 7572 6e20 7072 6f62  .    return prob
-0000eea0: 655f 6964 0a0a 0a64 6566 2075 7064 6174  e_id...def updat
-0000eeb0: 655f 7072 6f62 6528 7072 6f62 655f 6964  e_probe(probe_id
-0000eec0: 3a20 696e 742c 2070 726f 6265 5f64 6963  : int, probe_dic
-0000eed0: 743a 2064 6963 7429 202d 3e20 416e 793a  t: dict) -> Any:
-0000eee0: 0a20 2020 2022 2222 5570 6461 7465 2070  .    """Update p
-0000eef0: 726f 6265 2069 6e66 6f72 6d61 7469 6f6e  robe information
-0000ef00: 2067 6976 656e 2061 2070 726f 6265 2069   given a probe i
-0000ef10: 6420 616e 6420 6120 6469 6374 2063 6f6e  d and a dict con
-0000ef20: 7461 696e 696e 670a 2020 2020 7072 6f62  taining.    prob
-0000ef30: 6520 6461 7461 2e0a 2020 2020 2222 220a  e data..    """.
-0000ef40: 0a20 2020 2064 6174 6120 3d20 6a73 6f6e  .    data = json
-0000ef50: 2e64 756d 7073 2870 726f 6265 5f64 6963  .dumps(probe_dic
-0000ef60: 7429 0a20 2020 2072 6573 756c 7420 3d20  t).    result = 
-0000ef70: 5f70 7574 280a 2020 2020 2020 2020 6622  _put(.        f"
-0000ef80: 2f70 726f 6265 2f7b 7072 6f62 655f 6964  /probe/{probe_id
-0000ef90: 7d22 2c0a 2020 2020 2020 2020 6461 7461  }",.        data
-0000efa0: 3d64 6174 612c 0a20 2020 2020 2020 2068  =data,.        h
-0000efb0: 6561 6465 7273 3d7b 2243 6f6e 7465 6e74  eaders={"Content
-0000efc0: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
-0000efd0: 7469 6f6e 2f6a 736f 6e22 7d2c 0a20 2020  tion/json"},.   
-0000efe0: 2029 0a0a 2020 2020 6966 2072 6573 756c   )..    if resul
-0000eff0: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
-0000f000: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
-0000f010: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
-0000f020: 6c74 2c20 2243 616e 6e6f 7420 7570 6461  lt, "Cannot upda
-0000f030: 7465 2070 726f 6265 2069 6e66 6f72 6d61  te probe informa
-0000f040: 7469 6f6e 2077 6974 6820 636f 7265 2041  tion with core A
-0000f050: 5049 2229 0a0a 2020 2020 7265 7475 726e  PI")..    return
-0000f060: 2072 6573 756c 742e 6a73 6f6e 2829 0a0a   result.json()..
-0000f070: 0a64 6566 2064 656c 6574 655f 7072 6f62  .def delete_prob
-0000f080: 6528 7072 6f62 655f 6964 3a20 696e 7429  e(probe_id: int)
-0000f090: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
-0000f0a0: 4465 6c65 7465 2073 696d 756c 6174 696f  Delete simulatio
-0000f0b0: 6e20 7072 6f62 6520 6769 7665 6e20 6974  n probe given it
-0000f0c0: 7320 4944 2e22 2222 0a0a 2020 2020 2320  s ID."""..    # 
-0000f0d0: 4465 6c65 7465 2070 726f 6265 0a20 2020  Delete probe.   
-0000f0e0: 2072 6573 756c 7420 3d20 5f64 656c 6574   result = _delet
-0000f0f0: 6528 6622 2f70 726f 6265 2f7b 7072 6f62  e(f"/probe/{prob
-0000f100: 655f 6964 7d22 290a 0a20 2020 2069 6620  e_id}")..    if 
-0000f110: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-0000f120: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-0000f130: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-0000f140: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-0000f150: 2064 656c 6574 6520 7072 6f62 6522 290a   delete probe").
-0000f160: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
-0000f170: 6c74 2e6a 736f 6e28 290a 0a0a 6465 6620  lt.json()...def 
-0000f180: 6665 7463 685f 6261 7365 626f 7865 7328  fetch_baseboxes(
-0000f190: 2920 2d3e 2041 6e79 3a0a 2020 2020 2222  ) -> Any:.    ""
-0000f1a0: 2252 6574 7572 6e20 6261 7365 626f 7865  "Return baseboxe
-0000f1b0: 7320 6c69 7374 2e22 2222 0a20 2020 2072  s list.""".    r
-0000f1c0: 6573 756c 7420 3d20 5f67 6574 2822 2f62  esult = _get("/b
-0000f1d0: 6173 6562 6f78 2229 0a0a 2020 2020 6966  asebox")..    if
-0000f1e0: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-0000f1f0: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-0000f200: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-0000f210: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
-0000f220: 7420 7265 7472 6965 7665 2062 6173 6562  t retrieve baseb
-0000f230: 6f78 6573 206c 6973 7420 6672 6f6d 2049  oxes list from I
-0000f240: 5420 5369 6d75 6c61 7469 6f6e 2041 5049  T Simulation API
-0000f250: 2229 0a0a 2020 2020 6261 7365 626f 7865  ")..    baseboxe
-0000f260: 7320 3d20 7265 7375 6c74 2e6a 736f 6e28  s = result.json(
-0000f270: 290a 2020 2020 7265 7475 726e 2062 6173  ).    return bas
-0000f280: 6562 6f78 6573 0a0a 0a64 6566 2066 6574  eboxes...def fet
-0000f290: 6368 5f62 6173 6562 6f78 2869 645f 6261  ch_basebox(id_ba
-0000f2a0: 7365 626f 783a 2073 7472 2920 2d3e 2041  sebox: str) -> A
-0000f2b0: 6e79 3a0a 2020 2020 2222 2252 6574 7572  ny:.    """Retur
-0000f2c0: 6e20 6261 7365 626f 7820 6769 7665 6e20  n basebox given 
-0000f2d0: 6120 6261 7365 626f 7820 6964 2e22 2222  a basebox id."""
-0000f2e0: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
-0000f2f0: 6574 2866 222f 6261 7365 626f 782f 6964  et(f"/basebox/id
-0000f300: 2f7b 6964 5f62 6173 6562 6f78 7d22 290a  /{id_basebox}").
-0000f310: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
-0000f320: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-0000f330: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
-0000f340: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
-0000f350: 2022 4361 6e6e 6f74 2072 6574 7269 6576   "Cannot retriev
-0000f360: 6520 6261 7365 626f 7820 696e 666f 2066  e basebox info f
-0000f370: 726f 6d20 4954 2053 696d 756c 6174 696f  rom IT Simulatio
-0000f380: 6e20 4150 4922 290a 0a20 2020 2062 6173  n API")..    bas
-0000f390: 6562 6f78 203d 2072 6573 756c 742e 6a73  ebox = result.js
-0000f3a0: 6f6e 2829 0a20 2020 2072 6574 7572 6e20  on().    return 
-0000f3b0: 6261 7365 626f 780a 0a0a 6465 6620 7265  basebox...def re
-0000f3c0: 6c6f 6164 5f62 6173 6562 6f78 6573 2829  load_baseboxes()
-0000f3d0: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
-0000f3e0: 0a20 2020 2043 616c 6c20 7468 6520 6379  .    Call the cy
-0000f3f0: 6265 7220 7261 6e67 6520 4150 4920 746f  ber range API to
-0000f400: 2072 656c 6f61 6420 7468 6520 6c69 7374   reload the list
-0000f410: 206f 6620 6176 6169 6c61 626c 6520 6261   of available ba
-0000f420: 7365 626f 7865 732e 0a0a 2020 2020 3a72  seboxes...    :r
-0000f430: 6574 7572 6e3a 0a20 2020 2022 2222 0a20  eturn:.    """. 
-0000f440: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
-0000f450: 2822 2f62 6173 6562 6f78 2f72 656c 6f61  ("/basebox/reloa
-0000f460: 6422 290a 0a20 2020 2069 6620 7265 7375  d")..    if resu
-0000f470: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000f480: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-0000f490: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-0000f4a0: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
-0000f4b0: 7269 6576 6520 6261 7365 626f 7820 696e  rieve basebox in
-0000f4c0: 666f 2066 726f 6d20 4954 2053 696d 756c  fo from IT Simul
-0000f4d0: 6174 696f 6e20 4150 4922 290a 0a20 2020  ation API")..   
-0000f4e0: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
-0000f4f0: 736f 6e28 290a 0a0a 6465 6620 7665 7269  son()...def veri
-0000f500: 6679 5f62 6173 6562 6f78 5f72 6573 756c  fy_basebox_resul
-0000f510: 7428 7461 736b 5f69 643a 2073 7472 2920  t(task_id: str) 
-0000f520: 2d3e 2041 6e79 3a0a 2020 2020 2222 220a  -> Any:.    """.
-0000f530: 2020 2020 2043 616c 6c20 7468 6520 4150       Call the AP
-0000f540: 4920 746f 2067 6574 2074 6865 2072 6573  I to get the res
-0000f550: 756c 7420 7468 6520 6375 7272 656e 7420  ult the current 
-0000f560: 7665 7269 6669 6361 7469 6f6e 2e0a 0a20  verification... 
-0000f570: 2020 203a 7061 7261 6d20 7461 736b 5f69     :param task_i
-0000f580: 643a 2074 6865 2074 6173 6b20 6964 0a20  d: the task id. 
-0000f590: 2020 203a 7265 7475 726e 3a20 7468 6520     :return: the 
-0000f5a0: 7265 7375 6c74 206f 6620 7468 6520 7665  result of the ve
-0000f5b0: 7269 6669 6361 7469 6f6e 0a0a 2020 2020  rification..    
-0000f5c0: 2222 220a 0a20 2020 2064 6174 6120 3d20  """..    data = 
-0000f5d0: 7b22 7461 736b 5f69 6422 3a20 7461 736b  {"task_id": task
-0000f5e0: 5f69 647d 0a0a 2020 2020 7472 793a 0a20  _id}..    try:. 
-0000f5f0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0000f600: 5f70 6f73 7428 0a20 2020 2020 2020 2020  _post(.         
-0000f610: 2020 2022 2f62 6173 6562 6f78 2f72 6573     "/basebox/res
-0000f620: 756c 745f 7665 7269 6679 222c 0a20 2020  ult_verify",.   
-0000f630: 2020 2020 2020 2020 2064 6174 613d 6461           data=da
-0000f640: 7461 2c0a 2020 2020 2020 2020 290a 0a20  ta,.        ).. 
-0000f650: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
-0000f660: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-0000f670: 3230 303a 0a20 2020 2020 2020 2020 2020  200:.           
-0000f680: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
-0000f690: 6573 756c 742c 2022 4361 6e6e 6f74 2067  esult, "Cannot g
-0000f6a0: 6574 2076 6572 6966 6963 6174 696f 6e20  et verification 
-0000f6b0: 7265 7375 6c74 2229 0a0a 2020 2020 2020  result")..      
-0000f6c0: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
-0000f6d0: 6a73 6f6e 2829 0a0a 2020 2020 6578 6365  json()..    exce
-0000f6e0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000f6f0: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
-0000f700: 2045 7863 6570 7469 6f6e 2822 4973 7375   Exception("Issu
-0000f710: 6520 7768 656e 2067 6574 7469 6e67 2076  e when getting v
-0000f720: 6572 6966 6963 6174 696f 6e20 7265 7375  erification resu
-0000f730: 6c74 3a20 277b 7d27 222e 666f 726d 6174  lt: '{}'".format
-0000f740: 2865 2929 0a0a 0a64 6566 2076 6572 6966  (e))...def verif
-0000f750: 795f 6261 7365 626f 785f 7374 6f70 2874  y_basebox_stop(t
-0000f760: 6173 6b5f 6964 3a20 7374 7229 202d 3e20  ask_id: str) -> 
-0000f770: 416e 793a 0a20 2020 2022 2222 0a20 2020  Any:.    """.   
-0000f780: 2043 616c 6c20 7468 6520 4150 4920 746f   Call the API to
-0000f790: 2073 746f 7020 7468 6520 6375 7272 656e   stop the curren
-0000f7a0: 7420 7665 7269 6669 6361 7469 6f6e 0a20  t verification. 
-0000f7b0: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
-0000f7c0: 2222 220a 2020 2020 6461 7461 203d 207b  """.    data = {
-0000f7d0: 2274 6173 6b5f 6964 223a 2074 6173 6b5f  "task_id": task_
-0000f7e0: 6964 7d0a 0a20 2020 2072 6573 756c 7420  id}..    result 
-0000f7f0: 3d20 5f70 6f73 7428 222f 6261 7365 626f  = _post("/basebo
-0000f800: 782f 7374 6f70 5f76 6572 6966 7922 2c20  x/stop_verify", 
-0000f810: 6461 7461 3d64 6174 6129 0a0a 2020 2020  data=data)..    
-0000f820: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
-0000f830: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
-0000f840: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
-0000f850: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
-0000f860: 6e6f 7420 7374 6f70 2076 6572 6966 6963  not stop verific
-0000f870: 6174 696f 6e20 7461 736b 2229 0a0a 2020  ation task")..  
-0000f880: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
-0000f890: 6a73 6f6e 2829 0a0a 0a64 6566 2076 6572  json()...def ver
-0000f8a0: 6966 795f 6261 7365 626f 785f 7374 6174  ify_basebox_stat
-0000f8b0: 7573 2874 6173 6b5f 6964 3a20 7374 7229  us(task_id: str)
-0000f8c0: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
-0000f8d0: 0a20 2020 2043 616c 6c20 7468 6520 4150  .    Call the AP
-0000f8e0: 4920 746f 2067 6574 2074 6865 2073 7461  I to get the sta
-0000f8f0: 7475 7320 6f66 2063 7572 7265 6e74 2076  tus of current v
-0000f900: 6572 6966 6963 6174 696f 6e0a 2020 2020  erification.    
-0000f910: 3a72 6574 7572 6e3a 0a20 2020 2022 2222  :return:.    """
-0000f920: 0a20 2020 2064 6174 6120 3d20 7b22 7461  .    data = {"ta
-0000f930: 736b 5f69 6422 3a20 7461 736b 5f69 647d  sk_id": task_id}
-0000f940: 0a0a 2020 2020 7472 793a 0a20 2020 2020  ..    try:.     
-0000f950: 2020 2072 6573 756c 7420 3d20 5f70 6f73     result = _pos
-0000f960: 7428 222f 6261 7365 626f 782f 7374 6174  t("/basebox/stat
-0000f970: 7573 5f76 6572 6966 7922 2c20 6461 7461  us_verify", data
-0000f980: 3d64 6174 6129 0a0a 2020 2020 2020 2020  =data)..        
-0000f990: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
-0000f9a0: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
-0000f9b0: 2020 2020 2020 2020 2020 5f68 616e 646c            _handl
-0000f9c0: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
-0000f9d0: 2243 616e 6e6f 7420 6765 7420 7665 7269  "Cannot get veri
-0000f9e0: 6679 2073 7461 7475 7322 290a 0a20 2020  fy status")..   
-0000f9f0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0000fa00: 6c74 2e6a 736f 6e28 290a 0a20 2020 2065  lt.json()..    e
-0000fa10: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0000fa20: 6173 2065 3a0a 2020 2020 2020 2020 7261  as e:.        ra
-0000fa30: 6973 6520 4578 6365 7074 696f 6e28 2249  ise Exception("I
-0000fa40: 7373 7565 2077 6865 6e20 6765 7474 696e  ssue when gettin
-0000fa50: 6720 7665 7269 6679 2073 7461 7475 733a  g verify status:
-0000fa60: 2027 7b7d 2722 2e66 6f72 6d61 7428 6529   '{}'".format(e)
-0000fa70: 290a 0a0a 6465 6620 7665 7269 6679 5f62  )...def verify_b
-0000fa80: 6173 6562 6f78 2869 645f 6261 7365 626f  asebox(id_basebo
-0000fa90: 783a 2069 6e74 2920 2d3e 2041 6e79 3a0a  x: int) -> Any:.
-0000faa0: 2020 2020 2222 220a 2020 2020 4361 6c6c      """.    Call
-0000fab0: 2074 6865 2041 5049 2074 6f20 7665 7269   the API to veri
-0000fac0: 6679 2074 6865 2063 6865 636b 7375 6d20  fy the checksum 
-0000fad0: 6f66 2074 6865 2067 6976 656e 2062 6173  of the given bas
-0000fae0: 6562 6f78 0a20 2020 203a 7061 7261 6d20  ebox.    :param 
-0000faf0: 6964 5f62 6173 6562 6f78 3a20 7468 6520  id_basebox: the 
-0000fb00: 6964 206f 6620 7468 6520 6261 7365 626f  id of the basebo
-0000fb10: 7820 746f 2076 6572 6966 790a 2020 2020  x to verify.    
-0000fb20: 3a72 6574 7572 6e3a 0a20 2020 2022 2222  :return:.    """
-0000fb30: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
-0000fb40: 6574 2866 222f 6261 7365 626f 782f 7665  et(f"/basebox/ve
-0000fb50: 7269 6679 2f7b 6964 5f62 6173 6562 6f78  rify/{id_basebox
-0000fb60: 7d22 290a 0a20 2020 2069 6620 7265 7375  }")..    if resu
-0000fb70: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000fb80: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-0000fb90: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-0000fba0: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
-0000fbb0: 7269 6576 6520 6261 7365 626f 7820 696e  rieve basebox in
-0000fbc0: 666f 2066 726f 6d20 4954 2053 696d 756c  fo from IT Simul
-0000fbd0: 6174 696f 6e20 4150 4922 290a 0a20 2020  ation API")..   
-0000fbe0: 2072 6573 756c 7420 3d20 7265 7375 6c74   result = result
-0000fbf0: 2e6a 736f 6e28 290a 2020 2020 7461 736b  .json().    task
-0000fc00: 5f69 6420 3d20 7265 7375 6c74 5b22 7461  _id = result["ta
-0000fc10: 736b 5f69 6422 5d0a 2020 2020 7375 6363  sk_id"].    succ
-0000fc20: 6573 7320 3d20 7265 7375 6c74 5b22 7265  ess = result["re
-0000fc30: 7375 6c74 225d 203d 3d20 2253 5441 5254  sult"] == "START
-0000fc40: 4544 220a 0a20 2020 2069 6620 6e6f 7420  ED"..    if not 
-0000fc50: 7375 6363 6573 733a 0a20 2020 2020 2020  success:.       
-0000fc60: 205f 7261 6973 655f 6572 726f 725f 6d73   _raise_error_ms
-0000fc70: 6728 7265 7375 6c74 290a 0a20 2020 206c  g(result)..    l
-0000fc80: 6f67 6765 722e 696e 666f 2866 225b 2b5d  ogger.info(f"[+]
-0000fc90: 2056 6572 6966 6963 6174 696f 6e20 7461   Verification ta
-0000fca0: 736b 2049 443a 207b 7461 736b 5f69 647d  sk ID: {task_id}
-0000fcb0: 2229 0a0a 2020 2020 7265 7375 6c74 203d  ")..    result =
-0000fcc0: 205f 5f68 616e 646c 655f 7761 6974 280a   __handle_wait(.
-0000fcd0: 2020 2020 2020 2020 7761 6974 3d54 7275          wait=Tru
-0000fce0: 652c 2074 6173 6b5f 6964 3d74 6173 6b5f  e, task_id=task_
-0000fcf0: 6964 2c20 6c6f 675f 7375 6666 6978 3d69  id, log_suffix=i
-0000fd00: 645f 6261 7365 626f 782c 2074 696d 656f  d_basebox, timeo
-0000fd10: 7574 3d33 3630 300a 2020 2020 290a 0a20  ut=3600.    ).. 
-0000fd20: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
-0000fd30: 2020 2020 2273 7563 6365 7373 223a 2072      "success": r
-0000fd40: 6573 756c 745b 2272 6573 756c 7422 5d5b  esult["result"][
-0000fd50: 2273 7563 6365 7373 225d 2c0a 2020 2020  "success"],.    
-0000fd60: 2020 2020 2274 6173 6b5f 6964 223a 2074      "task_id": t
-0000fd70: 6173 6b5f 6964 2c0a 2020 2020 2020 2020  ask_id,.        
-0000fd80: 2276 616c 6964 5f63 6865 636b 7375 6d22  "valid_checksum"
-0000fd90: 3a20 7265 7375 6c74 5b22 7265 7375 6c74  : result["result
-0000fda0: 225d 5b22 7661 6c69 645f 6368 6563 6b73  "]["valid_checks
-0000fdb0: 756d 225d 2c0a 2020 2020 7d0a 0a0a 6465  um"],.    }...de
-0000fdc0: 6620 7665 7269 6679 5f62 6173 6562 6f78  f verify_basebox
-0000fdd0: 6573 2829 202d 3e20 416e 793a 0a20 2020  es() -> Any:.   
-0000fde0: 2022 2222 0a20 2020 2043 616c 6c20 7468   """.    Call th
-0000fdf0: 6520 4150 4920 746f 2076 6572 6966 7920  e API to verify 
-0000fe00: 7468 6520 6368 6563 6b73 756d 206f 6620  the checksum of 
-0000fe10: 616c 6c20 6261 7365 626f 7865 730a 2020  all baseboxes.  
-0000fe20: 2020 3a72 6574 7572 6e3a 0a20 2020 2022    :return:.    "
-0000fe30: 2222 0a20 2020 2072 6573 756c 7420 3d20  "".    result = 
-0000fe40: 5f67 6574 2822 2f62 6173 6562 6f78 2f76  _get("/basebox/v
-0000fe50: 6572 6966 792f 2229 0a0a 2020 2020 6966  erify/")..    if
-0000fe60: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-0000fe70: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-0000fe80: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-0000fe90: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
-0000fea0: 7420 7265 7472 6965 7665 2062 6173 6562  t retrieve baseb
-0000feb0: 6f78 2069 6e66 6f20 6672 6f6d 2049 5420  ox info from IT 
-0000fec0: 5369 6d75 6c61 7469 6f6e 2041 5049 2229  Simulation API")
-0000fed0: 0a0a 2020 2020 7265 7375 6c74 203d 2072  ..    result = r
-0000fee0: 6573 756c 742e 6a73 6f6e 2829 0a20 2020  esult.json().   
-0000fef0: 2074 6173 6b5f 6964 203d 2072 6573 756c   task_id = resul
-0000ff00: 745b 2274 6173 6b5f 6964 225d 0a20 2020  t["task_id"].   
-0000ff10: 2073 7563 6365 7373 203d 2072 6573 756c   success = resul
-0000ff20: 745b 2272 6573 756c 7422 5d20 3d3d 2022  t["result"] == "
-0000ff30: 5354 4152 5445 4422 0a0a 2020 2020 6966  STARTED"..    if
-0000ff40: 206e 6f74 2073 7563 6365 7373 3a0a 2020   not success:.  
-0000ff50: 2020 2020 2020 5f72 6169 7365 5f65 7272        _raise_err
-0000ff60: 6f72 5f6d 7367 2872 6573 756c 7429 0a0a  or_msg(result)..
-0000ff70: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-0000ff80: 6622 5b2b 5d20 5665 7269 6669 6361 7469  f"[+] Verificati
-0000ff90: 6f6e 2074 6173 6b20 4944 3a20 7b74 6173  on task ID: {tas
-0000ffa0: 6b5f 6964 7d22 290a 0a20 2020 2072 6573  k_id}")..    res
-0000ffb0: 756c 7420 3d20 5f5f 6861 6e64 6c65 5f77  ult = __handle_w
-0000ffc0: 6169 7428 0a20 2020 2020 2020 2077 6169  ait(.        wai
-0000ffd0: 743d 5472 7565 2c20 7461 736b 5f69 643d  t=True, task_id=
-0000ffe0: 7461 736b 5f69 642c 206c 6f67 5f73 7566  task_id, log_suf
-0000fff0: 6669 783d 2261 6c6c 2062 6173 6562 6f78  fix="all basebox
-00010000: 6573 222c 2074 696d 656f 7574 3d33 3630  es", timeout=360
-00010010: 300a 2020 2020 290a 0a20 2020 2072 6574  0.    )..    ret
-00010020: 7572 6e20 7b0a 2020 2020 2020 2020 2273  urn {.        "s
-00010030: 7563 6365 7373 223a 2072 6573 756c 745b  uccess": result[
-00010040: 2272 6573 756c 7422 5d5b 2273 7563 6365  "result"]["succe
-00010050: 7373 225d 2c0a 2020 2020 2020 2020 2274  ss"],.        "t
-00010060: 6173 6b5f 6964 223a 2074 6173 6b5f 6964  ask_id": task_id
-00010070: 2c0a 2020 2020 2020 2020 2272 6573 756c  ,.        "resul
-00010080: 7422 3a20 7265 7375 6c74 5b22 7265 7375  t": result["resu
-00010090: 6c74 225d 5b22 7661 6c69 645f 6368 6563  lt"]["valid_chec
-000100a0: 6b73 756d 225d 2c0a 2020 2020 7d0a 0a0a  ksum"],.    }...
-000100b0: 6465 6620 6665 7463 685f 646f 6d61 696e  def fetch_domain
-000100c0: 7328 2920 2d3e 2044 6963 745b 7374 722c  s() -> Dict[str,
-000100d0: 2073 7472 5d3a 0a20 2020 2022 2222 5265   str]:.    """Re
-000100e0: 7475 726e 7320 7468 6520 6d61 7070 696e  turns the mappin
-000100f0: 6720 646f 6d61 696e 2d3e 4950 2222 220a  g domain->IP""".
-00010100: 0a20 2020 2023 2046 4958 4d45 286d 756c  .    # FIXME(mul
-00010110: 7469 2d74 656e 616e 7429 3a20 7765 2073  ti-tenant): we s
-00010120: 686f 756c 6420 7265 7472 6965 7665 2064  hould retrieve d
-00010130: 6f6d 6169 6e73 2061 6363 6f72 6469 6e67  omains according
-00010140: 2074 6f20 6120 7369 6d75 6c61 7469 6f6e   to a simulation
-00010150: 2069 640a 2020 2020 7265 7375 6c74 203d   id.    result =
-00010160: 205f 6765 7428 222f 6e65 7477 6f72 6b5f   _get("/network_
-00010170: 696e 7465 7266 6163 652f 646f 6d61 696e  interface/domain
-00010180: 7322 290a 0a20 2020 2069 6620 7265 7375  s")..    if resu
-00010190: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-000101a0: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-000101b0: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-000101c0: 756c 742c 2022 4572 726f 7220 7768 696c  ult, "Error whil
-000101d0: 6520 6665 7463 6869 6e67 2064 6f6d 6169  e fetching domai
-000101e0: 6e73 2229 0a0a 2020 2020 7265 7475 726e  ns")..    return
-000101f0: 2072 6573 756c 742e 6a73 6f6e 2829 0a0a   result.json()..
-00010200: 0a64 6566 2066 6574 6368 5f77 6562 7369  .def fetch_websi
-00010210: 7465 7328 2920 2d3e 2041 6e79 3a0a 2020  tes() -> Any:.  
-00010220: 2020 2222 2252 6574 7572 6e20 7765 6273    """Return webs
-00010230: 6974 6573 206c 6973 742e 2222 220a 2020  ites list.""".  
-00010240: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
-00010250: 222f 7765 6273 6974 6522 290a 0a20 2020  "/website")..   
-00010260: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
-00010270: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
-00010280: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
-00010290: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
-000102a0: 6e6e 6f74 2072 6574 7269 6576 6520 7765  nnot retrieve we
-000102b0: 6273 6974 6573 206c 6973 7420 6672 6f6d  bsites list from
-000102c0: 2049 5420 5369 6d75 6c61 7469 6f6e 2041   IT Simulation A
-000102d0: 5049 2229 0a0a 2020 2020 7765 6273 6974  PI")..    websit
-000102e0: 6573 203d 2072 6573 756c 742e 6a73 6f6e  es = result.json
-000102f0: 2829 0a20 2020 2072 6574 7572 6e20 7765  ().    return we
-00010300: 6273 6974 6573 0a0a 0a64 6566 2074 6f70  bsites...def top
-00010310: 6f6c 6f67 795f 6164 645f 7765 6273 6974  ology_add_websit
-00010320: 6573 280a 2020 2020 746f 706f 6c6f 6779  es(.    topology
-00010330: 5f79 616d 6c3a 2073 7472 2c20 7765 6273  _yaml: str, webs
-00010340: 6974 6573 3a20 4c69 7374 5b73 7472 5d2c  ites: List[str],
-00010350: 2073 7769 7463 685f 6e61 6d65 3a20 7374   switch_name: st
-00010360: 720a 2920 2d3e 2073 7472 3a0a 2020 2020  r.) -> str:.    
-00010370: 2222 2241 6464 2064 6f63 6b65 7220 7765  """Add docker we
-00010380: 6273 6974 6573 206e 6f64 6520 746f 2061  bsites node to a
-00010390: 2067 6976 656e 2074 6f70 6f6c 6f67 792c   given topology,
-000103a0: 2061 6e64 2072 6574 7572 6e20 7468 6520   and return the 
-000103b0: 7570 6461 7465 6420 746f 706f 6c6f 6779  updated topology
-000103c0: 2e22 2222 0a0a 2020 2020 6461 7461 5f64  ."""..    data_d
-000103d0: 6963 7420 3d20 7b0a 2020 2020 2020 2020  ict = {.        
-000103e0: 2274 6f70 6f6c 6f67 795f 7961 6d6c 223a  "topology_yaml":
-000103f0: 2074 6f70 6f6c 6f67 795f 7961 6d6c 2c0a   topology_yaml,.
-00010400: 2020 2020 2020 2020 2277 6562 7369 7465          "website
-00010410: 7322 3a20 7765 6273 6974 6573 2c0a 2020  s": websites,.  
-00010420: 2020 2020 2020 2273 7769 7463 685f 6e61        "switch_na
-00010430: 6d65 223a 2073 7769 7463 685f 6e61 6d65  me": switch_name
-00010440: 2c0a 2020 2020 7d0a 2020 2020 6461 7461  ,.    }.    data
-00010450: 203d 206a 736f 6e2e 6475 6d70 7328 6461   = json.dumps(da
-00010460: 7461 5f64 6963 7429 0a20 2020 2072 6573  ta_dict).    res
-00010470: 756c 7420 3d20 5f70 6f73 7428 0a20 2020  ult = _post(.   
-00010480: 2020 2020 2022 2f74 6f70 6f6c 6f67 792f       "/topology/
-00010490: 6164 645f 7765 6273 6974 6573 222c 0a20  add_websites",. 
-000104a0: 2020 2020 2020 2064 6174 613d 6461 7461         data=data
-000104b0: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-000104c0: 733d 7b22 436f 6e74 656e 742d 5479 7065  s={"Content-Type
-000104d0: 223a 2022 6170 706c 6963 6174 696f 6e2f  ": "application/
-000104e0: 6a73 6f6e 227d 2c0a 2020 2020 290a 0a20  json"},.    ).. 
-000104f0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-00010500: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-00010510: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-00010520: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-00010530: 4572 726f 7220 7768 696c 6520 6164 6469  Error while addi
-00010540: 6e67 2077 6562 7369 7465 7320 746f 2061  ng websites to a
-00010550: 2074 6f70 6f6c 6f67 7922 290a 0a20 2020   topology")..   
-00010560: 2074 6f70 6f6c 6f67 795f 7961 6d6c 203d   topology_yaml =
-00010570: 2072 6573 756c 742e 6a73 6f6e 2829 5b22   result.json()["
-00010580: 746f 706f 6c6f 6779 5f79 616d 6c22 5d0a  topology_yaml"].
-00010590: 0a20 2020 2072 6574 7572 6e20 746f 706f  .    return topo
-000105a0: 6c6f 6779 5f79 616d 6c0a 0a0a 6465 6620  logy_yaml...def 
-000105b0: 746f 706f 6c6f 6779 5f61 6464 5f64 6761  topology_add_dga
-000105c0: 280a 2020 2020 746f 706f 6c6f 6779 5f79  (.    topology_y
-000105d0: 616d 6c3a 2073 7472 2c0a 2020 2020 616c  aml: str,.    al
-000105e0: 676f 7269 7468 6d3a 2073 7472 2c0a 2020  gorithm: str,.  
-000105f0: 2020 7377 6974 6368 5f6e 616d 653a 2073    switch_name: s
-00010600: 7472 2c0a 2020 2020 6e75 6d62 6572 3a20  tr,.    number: 
-00010610: 696e 742c 0a20 2020 2072 6573 6f75 7263  int,.    resourc
-00010620: 6573 5f64 6972 3a20 7374 722c 0a29 202d  es_dir: str,.) -
-00010630: 3e20 5475 706c 655b 7374 722c 204c 6973  > Tuple[str, Lis
-00010640: 745b 7374 725d 5d3a 0a20 2020 2022 2222  t[str]]:.    """
-00010650: 4164 6420 646f 636b 6572 2065 6d70 7479  Add docker empty
-00010660: 2077 6562 7369 7465 7320 7769 7468 2044   websites with D
-00010670: 4741 206e 6f64 6520 746f 2061 2067 6976  GA node to a giv
-00010680: 656e 2074 6f70 6f6c 6f67 792c 2061 6e64  en topology, and
-00010690: 2072 6574 7572 6e20 7468 6520 7570 6461   return the upda
-000106a0: 7465 6420 746f 706f 6c6f 6779 0a20 2020  ted topology.   
-000106b0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-000106c0: 2074 6865 2064 6f6d 6169 6e73 2e22 2222   the domains."""
-000106d0: 0a0a 2020 2020 6461 7461 5f64 6963 7420  ..    data_dict 
-000106e0: 3d20 7b0a 2020 2020 2020 2020 2274 6f70  = {.        "top
-000106f0: 6f6c 6f67 795f 7961 6d6c 223a 2074 6f70  ology_yaml": top
-00010700: 6f6c 6f67 795f 7961 6d6c 2c0a 2020 2020  ology_yaml,.    
-00010710: 2020 2020 2261 6c67 6f72 6974 686d 223a      "algorithm":
-00010720: 2061 6c67 6f72 6974 686d 2c0a 2020 2020   algorithm,.    
-00010730: 2020 2020 2273 7769 7463 685f 6e61 6d65      "switch_name
-00010740: 223a 2073 7769 7463 685f 6e61 6d65 2c0a  ": switch_name,.
-00010750: 2020 2020 2020 2020 226e 756d 6265 7222          "number"
-00010760: 3a20 6e75 6d62 6572 2c0a 2020 2020 2020  : number,.      
-00010770: 2020 2272 6573 6f75 7263 6573 5f64 6972    "resources_dir
-00010780: 223a 2072 6573 6f75 7263 6573 5f64 6972  ": resources_dir
-00010790: 2c0a 2020 2020 7d0a 2020 2020 6461 7461  ,.    }.    data
-000107a0: 203d 206a 736f 6e2e 6475 6d70 7328 6461   = json.dumps(da
-000107b0: 7461 5f64 6963 7429 0a20 2020 2072 6573  ta_dict).    res
-000107c0: 756c 7420 3d20 5f70 6f73 7428 0a20 2020  ult = _post(.   
-000107d0: 2020 2020 2022 2f74 6f70 6f6c 6f67 792f       "/topology/
-000107e0: 6164 645f 6467 6122 2c0a 2020 2020 2020  add_dga",.      
-000107f0: 2020 6461 7461 3d64 6174 612c 0a20 2020    data=data,.   
-00010800: 2020 2020 2068 6561 6465 7273 3d7b 2243       headers={"C
-00010810: 6f6e 7465 6e74 2d54 7970 6522 3a20 2261  ontent-Type": "a
-00010820: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e22  pplication/json"
-00010830: 7d2c 0a20 2020 2029 0a0a 2020 2020 6966  },.    )..    if
-00010840: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-00010850: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-00010860: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-00010870: 7228 7265 7375 6c74 2c20 2245 7272 6f72  r(result, "Error
-00010880: 2077 6869 6c65 2061 6464 696e 6720 7765   while adding we
-00010890: 6273 6974 6573 2074 6f20 6120 746f 706f  bsites to a topo
-000108a0: 6c6f 6779 2229 0a0a 2020 2020 746f 706f  logy")..    topo
-000108b0: 6c6f 6779 5f79 616d 6c20 3d20 7265 7375  logy_yaml = resu
-000108c0: 6c74 2e6a 736f 6e28 295b 2274 6f70 6f6c  lt.json()["topol
-000108d0: 6f67 795f 7961 6d6c 225d 0a20 2020 2064  ogy_yaml"].    d
-000108e0: 6f6d 6169 6e73 203d 2072 6573 756c 742e  omains = result.
-000108f0: 6a73 6f6e 2829 5b22 646f 6d61 696e 7322  json()["domains"
-00010900: 5d0a 0a20 2020 2072 6574 7572 6e20 746f  ]..    return to
-00010910: 706f 6c6f 6779 5f79 616d 6c2c 2064 6f6d  pology_yaml, dom
-00010920: 6169 6e73 0a0a 0a64 6566 2074 6f70 6f6c  ains...def topol
-00010930: 6f67 795f 6164 645f 646e 735f 7365 7276  ogy_add_dns_serv
-00010940: 6572 280a 2020 2020 746f 706f 6c6f 6779  er(.    topology
-00010950: 5f79 616d 6c3a 2073 7472 2c0a 2020 2020  _yaml: str,.    
-00010960: 7377 6974 6368 5f6e 616d 653a 2073 7472  switch_name: str
-00010970: 2c0a 2020 2020 7265 736f 7572 6365 735f  ,.    resources_
-00010980: 6469 723a 2073 7472 2c0a 2920 2d3e 2054  dir: str,.) -> T
-00010990: 7570 6c65 5b73 7472 2c20 7374 725d 3a0a  uple[str, str]:.
-000109a0: 2020 2020 6461 7461 5f64 6963 7420 3d20      data_dict = 
-000109b0: 7b0a 2020 2020 2020 2020 2274 6f70 6f6c  {.        "topol
-000109c0: 6f67 795f 7961 6d6c 223a 2074 6f70 6f6c  ogy_yaml": topol
-000109d0: 6f67 795f 7961 6d6c 2c0a 2020 2020 2020  ogy_yaml,.      
-000109e0: 2020 2273 7769 7463 685f 6e61 6d65 223a    "switch_name":
-000109f0: 2073 7769 7463 685f 6e61 6d65 2c0a 2020   switch_name,.  
-00010a00: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
-00010a10: 5f64 6972 223a 2072 6573 6f75 7263 6573  _dir": resources
-00010a20: 5f64 6972 2c0a 2020 2020 7d0a 2020 2020  _dir,.    }.    
-00010a30: 6461 7461 203d 206a 736f 6e2e 6475 6d70  data = json.dump
-00010a40: 7328 6461 7461 5f64 6963 7429 0a20 2020  s(data_dict).   
-00010a50: 2072 6573 756c 7420 3d20 5f70 6f73 7428   result = _post(
-00010a60: 0a20 2020 2020 2020 2022 2f74 6f70 6f6c  .        "/topol
-00010a70: 6f67 792f 6164 645f 646e 735f 7365 7276  ogy/add_dns_serv
-00010a80: 6572 222c 0a20 2020 2020 2020 2064 6174  er",.        dat
-00010a90: 613d 6461 7461 2c0a 2020 2020 2020 2020  a=data,.        
-00010aa0: 6865 6164 6572 733d 7b22 436f 6e74 656e  headers={"Conten
-00010ab0: 742d 5479 7065 223a 2022 6170 706c 6963  t-Type": "applic
-00010ac0: 6174 696f 6e2f 6a73 6f6e 227d 2c0a 2020  ation/json"},.  
-00010ad0: 2020 290a 0a20 2020 2069 6620 7265 7375    )..    if resu
-00010ae0: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-00010af0: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-00010b00: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-00010b10: 756c 742c 2022 4572 726f 7220 7768 696c  ult, "Error whil
-00010b20: 6520 6164 6469 6e67 2061 2044 4e53 2073  e adding a DNS s
-00010b30: 6572 7665 7220 746f 2061 2074 6f70 6f6c  erver to a topol
-00010b40: 6f67 7922 290a 0a20 2020 2074 6f70 6f6c  ogy")..    topol
-00010b50: 6f67 795f 7961 6d6c 203d 2072 6573 756c  ogy_yaml = resul
-00010b60: 742e 6a73 6f6e 2829 5b22 746f 706f 6c6f  t.json()["topolo
-00010b70: 6779 5f79 616d 6c22 5d0a 2020 2020 646e  gy_yaml"].    dn
-00010b80: 735f 636f 6e66 203d 2072 6573 756c 742e  s_conf = result.
-00010b90: 6a73 6f6e 2829 5b22 646e 735f 636f 6e66  json()["dns_conf
-00010ba0: 225d 0a0a 2020 2020 7265 7475 726e 2074  "]..    return t
-00010bb0: 6f70 6f6c 6f67 795f 7961 6d6c 2c20 646e  opology_yaml, dn
-00010bc0: 735f 636f 6e66 0a0a 0a64 6566 2074 6f6f  s_conf...def too
-00010bd0: 6c73 5f67 656e 6572 6174 655f 646f 6d61  ls_generate_doma
-00010be0: 696e 7328 0a20 2020 2061 6c67 6f72 6974  ins(.    algorit
-00010bf0: 686d 3a20 7374 722c 0a20 2020 206e 756d  hm: str,.    num
-00010c00: 6265 723a 2069 6e74 2c0a 2920 2d3e 204c  ber: int,.) -> L
-00010c10: 6973 745b 7374 725d 3a0a 2020 2020 2222  ist[str]:.    ""
-00010c20: 220a 2020 2020 4765 6e65 7261 7465 2064  ".    Generate d
-00010c30: 6f6d 6169 6e20 6e61 6d65 7320 6163 636f  omain names acco
-00010c40: 7264 696e 6720 746f 2074 6865 2067 6976  rding to the giv
-00010c50: 656e 2061 6c67 6f72 6974 686d 0a20 2020  en algorithm.   
-00010c60: 203a 7061 7261 6d20 616c 676f 7269 7468   :param algorith
-00010c70: 6d3a 2061 6c67 6f72 6974 686d 2074 6f20  m: algorithm to 
-00010c80: 7573 650a 2020 2020 3a70 6172 616d 206e  use.    :param n
-00010c90: 756d 6265 723a 206e 756d 6265 7220 6f66  umber: number of
-00010ca0: 2064 6f6d 6169 6e73 2074 6f20 6765 6e65   domains to gene
-00010cb0: 7261 7465 0a20 2020 203a 7265 7475 726e  rate.    :return
-00010cc0: 3a20 4120 6c69 7374 206f 6620 646f 6d61  : A list of doma
-00010cd0: 696e 730a 2020 2020 2222 220a 2020 2020  ins.    """.    
-00010ce0: 6461 7461 5f64 6963 7420 3d20 7b0a 2020  data_dict = {.  
-00010cf0: 2020 2020 2020 2261 6c67 6f72 6974 686d        "algorithm
-00010d00: 223a 2061 6c67 6f72 6974 686d 2c0a 2020  ": algorithm,.  
-00010d10: 2020 2020 2020 226e 756d 6265 7222 3a20        "number": 
-00010d20: 6e75 6d62 6572 2c0a 2020 2020 7d0a 2020  number,.    }.  
-00010d30: 2020 6461 7461 203d 206a 736f 6e2e 6475    data = json.du
-00010d40: 6d70 7328 6461 7461 5f64 6963 7429 0a20  mps(data_dict). 
-00010d50: 2020 2072 6573 756c 7420 3d20 5f70 6f73     result = _pos
-00010d60: 7428 0a20 2020 2020 2020 2022 2f64 6f6d  t(.        "/dom
-00010d70: 6169 6e2f 6765 6e65 7261 7465 5f64 6f6d  ain/generate_dom
-00010d80: 6169 6e73 222c 0a20 2020 2020 2020 2064  ains",.        d
-00010d90: 6174 613d 6461 7461 2c0a 2020 2020 2020  ata=data,.      
-00010da0: 2020 6865 6164 6572 733d 7b22 436f 6e74    headers={"Cont
-00010db0: 656e 742d 5479 7065 223a 2022 6170 706c  ent-Type": "appl
-00010dc0: 6963 6174 696f 6e2f 6a73 6f6e 227d 2c0a  ication/json"},.
-00010dd0: 2020 2020 290a 0a20 2020 2069 6620 7265      )..    if re
-00010de0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-00010df0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
-00010e00: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
-00010e10: 6573 756c 742c 2022 4572 726f 7220 7768  esult, "Error wh
-00010e20: 696c 6520 6765 6e65 7261 7469 6e67 2064  ile generating d
-00010e30: 6f6d 6169 6e73 2229 0a0a 2020 2020 646f  omains")..    do
-00010e40: 6d61 696e 7320 3d20 7265 7375 6c74 2e6a  mains = result.j
-00010e50: 736f 6e28 295b 2264 6f6d 6169 6e73 225d  son()["domains"]
-00010e60: 0a0a 2020 2020 7265 7475 726e 2064 6f6d  ..    return dom
-00010e70: 6169 6e73 0a0a 0a64 6566 2066 6574 6368  ains...def fetch
-00010e80: 5f74 6f70 6f6c 6f67 6965 7328 2920 2d3e  _topologies() ->
-00010e90: 2041 6e79 3a0a 2020 2020 2222 2252 6574   Any:.    """Ret
-00010ea0: 7572 6e20 746f 706f 6c6f 6769 6573 206c  urn topologies l
-00010eb0: 6973 742e 2222 220a 2020 2020 7265 7375  ist.""".    resu
-00010ec0: 6c74 203d 205f 6765 7428 222f 746f 706f  lt = _get("/topo
-00010ed0: 6c6f 6779 2229 0a0a 2020 2020 6966 2072  logy")..    if r
-00010ee0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-00010ef0: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-00010f00: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-00010f10: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-00010f20: 7265 7472 6965 7665 2074 6f70 6f6c 6f67  retrieve topolog
-00010f30: 6965 7320 6c69 7374 2066 726f 6d20 4954  ies list from IT
-00010f40: 2053 696d 756c 6174 696f 6e20 4150 4922   Simulation API"
-00010f50: 290a 0a20 2020 2074 6f70 6f6c 6f67 6965  )..    topologie
-00010f60: 7320 3d20 7265 7375 6c74 2e6a 736f 6e28  s = result.json(
-00010f70: 290a 2020 2020 7265 7475 726e 2074 6f70  ).    return top
-00010f80: 6f6c 6f67 6965 730a 0a0a 2323 230a 2320  ologies...###.# 
-00010f90: 5369 6d75 6c61 7469 6f6e 2063 6f6d 6d61  Simulation comma
-00010fa0: 6e64 730a 2323 230a 0a0a 6465 6620 7374  nds.###...def st
-00010fb0: 6172 745f 7369 6d75 6c61 7469 6f6e 280a  art_simulation(.
-00010fc0: 2020 2020 6964 5f73 696d 756c 6174 696f      id_simulatio
-00010fd0: 6e3a 2069 6e74 2c0a 2020 2020 7573 655f  n: int,.    use_
-00010fe0: 696e 7374 616c 6c5f 7469 6d65 3a20 626f  install_time: bo
-00010ff0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-00011000: 7469 6d65 6f75 743a 2069 6e74 203d 2033  timeout: int = 3
-00011010: 3030 2c0a 2020 2020 6e6f 6465 733a 204f  00,.    nodes: O
-00011020: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
-00011030: 5d5d 203d 204e 6f6e 652c 0a29 202d 3e20  ]] = None,.) -> 
-00011040: 4e6f 6e65 3a0a 2020 2020 2222 2253 7461  None:.    """Sta
-00011050: 7274 2074 6865 2073 696d 756c 6174 696f  rt the simulatio
-00011060: 6e2c 2077 6974 6820 6375 7272 656e 7420  n, with current 
-00011070: 7469 6d65 2028 6279 2064 6566 6175 6c74  time (by default
-00011080: 2920 6f72 2074 696d 6520 7768 6572 650a  ) or time where.
-00011090: 2020 2020 7468 6520 564d 2077 6173 2063      the VM was c
-000110a0: 7265 6174 6564 2028 7573 655f 696e 7374  reated (use_inst
-000110b0: 616c 6c5f 7469 6d65 3d54 7275 6529 2e20  all_time=True). 
-000110c0: 4974 2069 7320 706f 7373 6962 6c65 2074  It is possible t
-000110d0: 6f0a 2020 2020 7370 6563 6966 7920 7468  o.    specify th
-000110e0: 6520 6e6f 6465 7320 746f 2073 7461 7274  e nodes to start
-000110f0: 2e20 4279 2064 6566 6175 6c74 2c20 616c  . By default, al
-00011100: 6c20 6e6f 6465 7320 6172 6520 7374 6172  l nodes are star
-00011110: 7465 642e 0a0a 2020 2020 2222 220a 2020  ted...    """.  
-00011120: 2020 2320 4368 6563 6b20 7468 6174 206e    # Check that n
-00011130: 6f20 6f74 6865 7220 7369 6d75 6c61 7469  o other simulati
-00011140: 6f6e 2069 7320 7275 6e6e 696e 670a 2020  on is running.  
-00011150: 2020 7369 6d75 6c61 7469 6f6e 5f6c 6973    simulation_lis
-00011160: 7420 3d20 6665 7463 685f 7369 6d75 6c61  t = fetch_simula
-00011170: 7469 6f6e 7328 290a 2020 2020 666f 7220  tions().    for 
-00011180: 7369 6d75 6c61 7469 6f6e 2069 6e20 7369  simulation in si
-00011190: 6d75 6c61 7469 6f6e 5f6c 6973 743a 0a20  mulation_list:. 
-000111a0: 2020 2020 2020 2069 6620 7369 6d75 6c61         if simula
-000111b0: 7469 6f6e 5b22 6964 225d 2021 3d20 6964  tion["id"] != id
-000111c0: 5f73 696d 756c 6174 696f 6e20 616e 6420  _simulation and 
-000111d0: 7369 6d75 6c61 7469 6f6e 5b22 7374 6174  simulation["stat
-000111e0: 7573 225d 203d 3d20 2252 554e 4e49 4e47  us"] == "RUNNING
-000111f0: 223a 0a20 2020 2020 2020 2020 2020 2072  ":.            r
-00011200: 6169 7365 2045 7863 6570 7469 6f6e 280a  aise Exception(.
-00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011220: 2243 616e 6e6f 7420 7374 6172 7420 6120  "Cannot start a 
-00011230: 6e65 7720 7369 6d75 6c61 7469 6f6e 2c20  new simulation, 
-00011240: 6173 2074 6865 2073 696d 756c 6174 696f  as the simulatio
-00011250: 6e20 277b 7d27 2069 7320 220a 2020 2020  n '{}' is ".    
-00011260: 2020 2020 2020 2020 2020 2020 2261 6c72              "alr
-00011270: 6561 6479 2072 756e 6e69 6e67 222e 666f  eady running".fo
-00011280: 726d 6174 2873 696d 756c 6174 696f 6e5b  rmat(simulation[
-00011290: 2269 6422 5d29 0a20 2020 2020 2020 2020  "id"]).         
-000112a0: 2020 2029 0a0a 2020 2020 2320 496e 6974     )..    # Init
-000112b0: 6961 7465 2074 6865 2073 696d 756c 6174  iate the simulat
-000112c0: 696f 6e0a 2020 2020 6966 206e 6f64 6573  ion.    if nodes
-000112d0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000112e0: 2020 6e6f 6465 7320 3d20 5b5d 0a20 2020    nodes = [].   
-000112f0: 2070 6f73 745f 6461 7461 203d 207b 226e   post_data = {"n
-00011300: 6f64 6573 223a 206e 6f64 6573 7d0a 0a20  odes": nodes}.. 
-00011310: 2020 205f 7369 6d75 6c61 7469 6f6e 5f65     _simulation_e
-00011320: 7865 6375 7465 5f6f 7065 7261 7469 6f6e  xecute_operation
-00011330: 280a 2020 2020 2020 2020 2270 6f73 7422  (.        "post"
-00011340: 2c0a 2020 2020 2020 2020 2273 7461 7274  ,.        "start
-00011350: 222c 0a20 2020 2020 2020 2069 645f 7369  ",.        id_si
-00011360: 6d75 6c61 7469 6f6e 2c0a 2020 2020 2020  mulation,.      
-00011370: 2020 2253 5441 5254 494e 4722 2c0a 2020    "STARTING",.  
-00011380: 2020 2020 2020 6f70 7469 6f6e 616c 5f70        optional_p
-00011390: 6172 616d 313d 7573 655f 696e 7374 616c  aram1=use_instal
-000113a0: 6c5f 7469 6d65 2c0a 2020 2020 2020 2020  l_time,.        
-000113b0: 6f70 7469 6f6e 616c 5f70 6172 616d 323d  optional_param2=
-000113c0: 7469 6d65 6f75 742c 0a20 2020 2020 2020  timeout,.       
-000113d0: 2070 6f73 745f 6461 7461 3d70 6f73 745f   post_data=post_
-000113e0: 6461 7461 2c0a 2020 2020 290a 0a0a 6465  data,.    )...de
-000113f0: 6620 7061 7573 655f 7369 6d75 6c61 7469  f pause_simulati
-00011400: 6f6e 2869 645f 7369 6d75 6c61 7469 6f6e  on(id_simulation
-00011410: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-00011420: 2020 2020 2222 2250 6175 7365 2061 2073      """Pause a s
-00011430: 696d 756c 6174 696f 6e20 2863 616c 6c73  imulation (calls
-00011440: 206c 6962 7669 7274 2073 7573 7065 6e64   libvirt suspend
-00011450: 2041 5049 292e 2222 220a 2020 2020 5f73   API).""".    _s
-00011460: 696d 756c 6174 696f 6e5f 6578 6563 7574  imulation_execut
-00011470: 655f 6f70 6572 6174 696f 6e28 2267 6574  e_operation("get
-00011480: 222c 2022 7061 7573 6522 2c20 6964 5f73  ", "pause", id_s
-00011490: 696d 756c 6174 696f 6e2c 2022 5041 5553  imulation, "PAUS
-000114a0: 494e 4722 290a 0a0a 6465 6620 756e 7061  ING")...def unpa
-000114b0: 7573 655f 7369 6d75 6c61 7469 6f6e 2869  use_simulation(i
-000114c0: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
-000114d0: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-000114e0: 2222 2255 6e70 6175 7365 2061 2073 696d  """Unpause a sim
-000114f0: 756c 6174 696f 6e20 2863 616c 6c73 206c  ulation (calls l
-00011500: 6962 7669 7274 2072 6573 756d 6520 4150  ibvirt resume AP
-00011510: 4929 2e22 2222 0a20 2020 205f 7369 6d75  I).""".    _simu
-00011520: 6c61 7469 6f6e 5f65 7865 6375 7465 5f6f  lation_execute_o
-00011530: 7065 7261 7469 6f6e 2822 6765 7422 2c20  peration("get", 
-00011540: 2275 6e70 6175 7365 222c 2069 645f 7369  "unpause", id_si
-00011550: 6d75 6c61 7469 6f6e 2c20 2255 4e50 4155  mulation, "UNPAU
-00011560: 5349 4e47 2229 0a0a 0a64 6566 2063 7265  SING")...def cre
-00011570: 6174 655f 6261 636b 7570 5f73 696d 756c  ate_backup_simul
-00011580: 6174 696f 6e28 0a20 2020 2069 645f 7369  ation(.    id_si
-00011590: 6d75 6c61 7469 6f6e 3a20 696e 742c 0a20  mulation: int,. 
-000115a0: 2020 206e 6f64 6573 3a20 4f70 7469 6f6e     nodes: Option
-000115b0: 616c 5b4c 6973 745b 7374 725d 5d20 3d20  al[List[str]] = 
-000115c0: 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e 653a  None,.) -> None:
-000115d0: 0a20 2020 2022 2222 4372 6561 7465 2062  .    """Create b
-000115e0: 6163 6b75 7020 6f66 2061 2073 696d 756c  ackup of a simul
-000115f0: 6174 696f 6e2e 2049 7420 6973 2070 6f73  ation. It is pos
-00011600: 7369 626c 6520 746f 2073 7065 6369 6679  sible to specify
-00011610: 2074 6865 206e 6f64 6573 0a20 2020 2074   the nodes.    t
-00011620: 6f20 6261 636b 7570 2e20 4279 2064 6566  o backup. By def
-00011630: 6175 6c74 2c20 616c 6c20 6e6f 6465 7320  ault, all nodes 
-00011640: 6172 6520 6261 636b 6564 2075 702e 0a0a  are backed up...
-00011650: 2020 2020 2222 220a 0a20 2020 2069 6620      """..    if 
-00011660: 6e6f 6465 7320 6973 204e 6f6e 653a 0a20  nodes is None:. 
-00011670: 2020 2020 2020 206e 6f64 6573 203d 205b         nodes = [
-00011680: 5d0a 2020 2020 706f 7374 5f64 6174 6120  ].    post_data 
-00011690: 3d20 7b22 6e6f 6465 7322 3a20 6e6f 6465  = {"nodes": node
-000116a0: 737d 0a0a 2020 2020 5f73 696d 756c 6174  s}..    _simulat
-000116b0: 696f 6e5f 6578 6563 7574 655f 6f70 6572  ion_execute_oper
-000116c0: 6174 696f 6e28 0a20 2020 2020 2020 2022  ation(.        "
-000116d0: 706f 7374 222c 2022 6372 6561 7465 5f62  post", "create_b
-000116e0: 6163 6b75 7022 2c20 6964 5f73 696d 756c  ackup", id_simul
-000116f0: 6174 696f 6e2c 2022 5052 4550 4152 494e  ation, "PREPARIN
-00011700: 4722 2c20 706f 7374 5f64 6174 613d 706f  G", post_data=po
-00011710: 7374 5f64 6174 610a 2020 2020 290a 0a0a  st_data.    )...
-00011720: 6465 6620 7265 7374 6f72 655f 6261 636b  def restore_back
-00011730: 7570 5f73 696d 756c 6174 696f 6e28 0a20  up_simulation(. 
-00011740: 2020 2069 645f 7369 6d75 6c61 7469 6f6e     id_simulation
-00011750: 3a20 696e 742c 0a20 2020 206e 6f64 6573  : int,.    nodes
-00011760: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00011770: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2920  str]] = None,.) 
-00011780: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-00011790: 5265 7374 6f72 6520 6261 636b 7570 206f  Restore backup o
-000117a0: 6620 6120 7369 6d75 6c61 7469 6f6e 2e20  f a simulation. 
-000117b0: 4974 2069 7320 706f 7373 6962 6c65 2074  It is possible t
-000117c0: 6f20 7370 6563 6966 7920 7468 6520 6e6f  o specify the no
-000117d0: 6465 730a 2020 2020 746f 2072 6573 746f  des.    to resto
-000117e0: 7265 2e20 4279 2064 6566 6175 6c74 2c20  re. By default, 
-000117f0: 616c 6c20 6e6f 6465 7320 6172 6520 7265  all nodes are re
-00011800: 7374 6f72 6564 2e0a 0a20 2020 2022 2222  stored...    """
-00011810: 0a0a 2020 2020 6966 206e 6f64 6573 2069  ..    if nodes i
-00011820: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00011830: 6e6f 6465 7320 3d20 5b5d 0a20 2020 2070  nodes = [].    p
-00011840: 6f73 745f 6461 7461 203d 207b 226e 6f64  ost_data = {"nod
-00011850: 6573 223a 206e 6f64 6573 7d0a 0a20 2020  es": nodes}..   
-00011860: 205f 7369 6d75 6c61 7469 6f6e 5f65 7865   _simulation_exe
-00011870: 6375 7465 5f6f 7065 7261 7469 6f6e 280a  cute_operation(.
-00011880: 2020 2020 2020 2020 2270 6f73 7422 2c20          "post", 
-00011890: 2272 6573 746f 7265 5f62 6163 6b75 7022  "restore_backup"
-000118a0: 2c20 6964 5f73 696d 756c 6174 696f 6e2c  , id_simulation,
-000118b0: 2022 5052 4550 4152 494e 4722 2c20 706f   "PREPARING", po
-000118c0: 7374 5f64 6174 613d 706f 7374 5f64 6174  st_data=post_dat
-000118d0: 610a 2020 2020 290a 0a0a 6465 6620 6861  a.    )...def ha
-000118e0: 6c74 5f73 696d 756c 6174 696f 6e28 0a20  lt_simulation(. 
-000118f0: 2020 2069 645f 7369 6d75 6c61 7469 6f6e     id_simulation
-00011900: 3a20 696e 742c 206e 6f64 6573 3a20 4f70  : int, nodes: Op
-00011910: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
-00011920: 5d20 3d20 4e6f 6e65 0a29 202d 3e20 4f70  ] = None.) -> Op
-00011930: 7469 6f6e 616c 5b75 7569 642e 5555 4944  tional[uuid.UUID
-00011940: 5d3a 0a20 2020 2022 2222 5072 6f70 6572  ]:.    """Proper
-00011950: 6c79 2073 746f 7020 6120 7369 6d75 6c61  ly stop a simula
-00011960: 7469 6f6e 2c20 6279 2073 656e 6469 6e67  tion, by sending
-00011970: 2061 2073 6875 7464 6f77 6e20 7369 676e   a shutdown sign
-00011980: 616c 2074 6f20 7468 650a 2020 2020 6f70  al to the.    op
-00011990: 6572 6174 696e 6720 7379 7374 656d 732e  erating systems.
-000119a0: 2049 7420 6973 2070 6f73 7369 626c 6520   It is possible 
-000119b0: 746f 2073 7065 6369 6679 2074 6865 206e  to specify the n
-000119c0: 6f64 6573 2074 6f0a 2020 2020 7374 6172  odes to.    star
-000119d0: 742e 2042 7920 6465 6661 756c 742c 2061  t. By default, a
-000119e0: 6c6c 206e 6f64 6573 2061 7265 2073 7461  ll nodes are sta
-000119f0: 7274 6564 2e0a 0a20 2020 2022 2222 0a20  rted...    """. 
-00011a00: 2020 2069 6620 6e6f 6465 7320 6973 204e     if nodes is N
-00011a10: 6f6e 653a 0a20 2020 2020 2020 206e 6f64  one:.        nod
-00011a20: 6573 203d 205b 5d0a 2020 2020 706f 7374  es = [].    post
-00011a30: 5f64 6174 6120 3d20 7b22 6e6f 6465 7322  _data = {"nodes"
-00011a40: 3a20 6e6f 6465 737d 0a0a 2020 2020 5f73  : nodes}..    _s
-00011a50: 696d 756c 6174 696f 6e5f 6578 6563 7574  imulation_execut
-00011a60: 655f 6f70 6572 6174 696f 6e28 0a20 2020  e_operation(.   
-00011a70: 2020 2020 2022 706f 7374 222c 0a20 2020       "post",.   
-00011a80: 2020 2020 2022 7374 6f70 222c 0a20 2020       "stop",.   
-00011a90: 2020 2020 2069 645f 7369 6d75 6c61 7469       id_simulati
-00011aa0: 6f6e 2c0a 2020 2020 2020 2020 2253 544f  on,.        "STO
-00011ab0: 5050 494e 4722 2c0a 2020 2020 2020 2020  PPING",.        
-00011ac0: 706f 7374 5f64 6174 613d 706f 7374 5f64  post_data=post_d
-00011ad0: 6174 612c 0a20 2020 2029 0a0a 0a64 6566  ata,.    )...def
-00011ae0: 2064 6573 7472 6f79 5f73 696d 756c 6174   destroy_simulat
-00011af0: 696f 6e28 6964 5f73 696d 756c 6174 696f  ion(id_simulatio
-00011b00: 6e3a 2069 6e74 2c20 6e6f 6465 733a 204f  n: int, nodes: O
-00011b10: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
-00011b20: 5d5d 203d 204e 6f6e 6529 202d 3e20 4e6f  ]] = None) -> No
-00011b30: 6e65 3a0a 2020 2020 2222 2253 746f 7020  ne:.    """Stop 
-00011b40: 6120 7369 6d75 6c61 7469 6f6e 2074 6872  a simulation thr
-00011b50: 6f75 6768 2061 2068 6172 6420 7265 7365  ough a hard rese
-00011b60: 742e 2222 220a 0a20 2020 2069 6620 6e6f  t."""..    if no
-00011b70: 6465 7320 6973 204e 6f6e 653a 0a20 2020  des is None:.   
-00011b80: 2020 2020 206e 6f64 6573 203d 205b 5d0a       nodes = [].
-00011b90: 2020 2020 706f 7374 5f64 6174 6120 3d20      post_data = 
-00011ba0: 7b22 6e6f 6465 7322 3a20 6e6f 6465 737d  {"nodes": nodes}
-00011bb0: 0a0a 2020 2020 5f73 696d 756c 6174 696f  ..    _simulatio
-00011bc0: 6e5f 6578 6563 7574 655f 6f70 6572 6174  n_execute_operat
-00011bd0: 696f 6e28 0a20 2020 2020 2020 2022 706f  ion(.        "po
-00011be0: 7374 222c 2022 6465 7374 726f 7922 2c20  st", "destroy", 
-00011bf0: 6964 5f73 696d 756c 6174 696f 6e2c 2022  id_simulation, "
-00011c00: 5354 4f50 5049 4e47 222c 2070 6f73 745f  STOPPING", post_
-00011c10: 6461 7461 3d70 6f73 745f 6461 7461 0a20  data=post_data. 
-00011c20: 2020 2029 0a0a 0a64 6566 2063 6c6f 6e65     )...def clone
-00011c30: 5f73 696d 756c 6174 696f 6e28 6964 5f73  _simulation(id_s
-00011c40: 696d 756c 6174 696f 6e3a 2069 6e74 2920  imulation: int) 
-00011c50: 2d3e 2069 6e74 3a0a 2020 2020 2222 2243  -> int:.    """C
-00011c60: 6c6f 6e65 2061 2073 696d 756c 6174 696f  lone a simulatio
-00011c70: 6e20 616e 6420 6372 6561 7465 2061 206e  n and create a n
-00011c80: 6577 2073 696d 756c 6174 696f 6e2c 2061  ew simulation, a
-00011c90: 6e64 2072 6574 7572 6e20 7468 6520 6e65  nd return the ne
-00011ca0: 7720 4944 2e22 2222 0a20 2020 2069 645f  w ID.""".    id_
-00011cb0: 6e65 775f 7369 6d75 6c61 7469 6f6e 203d  new_simulation =
-00011cc0: 205f 7369 6d75 6c61 7469 6f6e 5f65 7865   _simulation_exe
-00011cd0: 6375 7465 5f6f 7065 7261 7469 6f6e 280a  cute_operation(.
-00011ce0: 2020 2020 2020 2020 2267 6574 222c 2022          "get", "
-00011cf0: 636c 6f6e 6522 2c20 6964 5f73 696d 756c  clone", id_simul
-00011d00: 6174 696f 6e2c 2022 434c 4f4e 494e 4722  ation, "CLONING"
-00011d10: 0a20 2020 2029 0a20 2020 2072 6574 7572  .    ).    retur
-00011d20: 6e20 6964 5f6e 6577 5f73 696d 756c 6174  n id_new_simulat
-00011d30: 696f 6e0a 0a0a 6465 6620 6e65 745f 6372  ion...def net_cr
-00011d40: 6561 7465 5f70 726f 6265 2820 2023 206e  eate_probe(  # n
-00011d50: 6f71 613a 2043 3930 310a 2020 2020 6964  oqa: C901.    id
-00011d60: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
-00011d70: 2c0a 2020 2020 7369 6d75 5f6e 6f64 6573  ,.    simu_nodes
-00011d80: 3a20 4469 6374 2c0a 2020 2020 6966 6163  : Dict,.    ifac
-00011d90: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-00011da0: 203d 204e 6f6e 652c 0a20 2020 2070 6361   = None,.    pca
-00011db0: 703a 204f 7074 696f 6e61 6c5b 626f 6f6c  p: Optional[bool
-00011dc0: 5d20 3d20 4661 6c73 652c 0a20 2020 2066  ] = False,.    f
-00011dd0: 696c 7465 723a 204f 7074 696f 6e61 6c5b  ilter: Optional[
-00011de0: 7374 725d 203d 2022 222c 0a20 2020 2064  str] = "",.    d
-00011df0: 6972 6563 7469 6f6e 3a20 4f70 7469 6f6e  irection: Option
-00011e00: 616c 5b73 7472 5d20 3d20 2262 6f74 6822  al[str] = "both"
-00011e10: 2c0a 2920 2d3e 2069 6e74 3a0a 2020 2020  ,.) -> int:.    
-00011e20: 2222 2243 7265 6174 6520 6120 6e65 7720  """Create a new 
-00011e30: 7072 6f62 6520 616e 6420 636f 6e66 6967  probe and config
-00011e40: 7572 6520 6869 7320 6e65 7477 6f72 6b20  ure his network 
-00011e50: 636f 6c6c 6563 7469 6f6e 7320 706f 696e  collections poin
-00011e60: 7473 2e0a 0a20 2020 203a 7061 7261 6d20  ts...    :param 
-00011e70: 6964 5f73 696d 756c 6174 696f 6e3a 2054  id_simulation: T
-00011e80: 6865 2069 6420 6f66 2074 6865 2073 696d  he id of the sim
-00011e90: 756c 6174 696f 6e2e 0a20 2020 203a 7061  ulation..    :pa
-00011ea0: 7261 6d20 7369 6d75 5f6e 6f64 6573 3a20  ram simu_nodes: 
-00011eb0: 4120 6469 6374 696f 6e61 7279 2073 746f  A dictionary sto
-00011ec0: 7269 6e67 2074 6865 2063 6f6c 6c65 6374  ring the collect
-00011ed0: 696f 6e20 706f 696e 7473 2074 6f20 6361  ion points to ca
-00011ee0: 7074 7572 652e 0a20 2020 203a 7061 7261  pture..    :para
-00011ef0: 6d20 6966 6163 653a 2049 6e74 6572 6661  m iface: Interfa
-00011f00: 6365 2077 6865 7265 2074 6865 2074 7261  ce where the tra
-00011f10: 6666 6963 2069 7320 6d69 7272 6f72 6564  ffic is mirrored
-00011f20: 2074 6f2e 0a20 2020 203a 7061 7261 6d20   to..    :param 
-00011f30: 7063 6170 3a20 4120 626f 6f6c 6561 6e20  pcap: A boolean 
-00011f40: 696e 6469 6361 7469 6e67 2069 6620 7468  indicating if th
-00011f50: 6520 6361 7074 7572 6520 7368 6f75 6c64  e capture should
-00011f60: 2062 6520 7361 7665 6420 6f6e 2064 6973   be saved on dis
-00011f70: 6b20 696e 2061 2070 6361 7020 6669 6c65  k in a pcap file
-00011f80: 2028 746f 2062 6520 696e 636c 7564 6564   (to be included
-00011f90: 2069 6e20 6461 7461 7365 7429 0a20 2020   in dataset).   
-00011fa0: 203a 7061 7261 6d20 6669 6c74 6572 3a20   :param filter: 
-00011fb0: 5374 7269 6e67 2066 696c 7465 7269 6e67  String filtering
-00011fc0: 2074 6370 6475 6d70 2063 6170 7475 7265   tcpdump capture
-00011fd0: 0a20 2020 203a 7061 7261 6d20 6469 7265  .    :param dire
-00011fe0: 6374 696f 6e3a 2053 656c 6563 7420 7768  ction: Select wh
-00011ff0: 6963 6820 7472 6166 6669 6320 746f 206d  ich traffic to m
-00012000: 6f6e 6974 6f72 206f 6e20 7468 6520 6d69  onitor on the mi
-00012010: 7272 6f72 6564 2069 6e74 6572 6661 6365  rrored interface
-00012020: 2873 293a 2065 6974 6865 7220 2769 6e67  (s): either 'ing
-00012030: 7265 7373 272c 2027 6567 7265 7373 2720  ress', 'egress' 
-00012040: 6f72 2027 626f 7468 272e 0a0a 2020 2020  or 'both'...    
-00012050: 3a74 7970 6520 6964 5f73 696d 756c 6174  :type id_simulat
-00012060: 696f 6e3a 203a 636c 6173 733a 6069 6e74  ion: :class:`int
-00012070: 602c 2065 7820 3a20 310a 2020 2020 3a74  `, ex : 1.    :t
-00012080: 7970 6520 7369 6d75 5f6e 6f64 6573 3a20  ype simu_nodes: 
-00012090: 3a63 6c61 7373 3a60 4469 6374 602c 2065  :class:`Dict`, e
-000120a0: 7820 3a20 7b27 7377 6974 6368 7327 3a20  x : {'switchs': 
-000120b0: 5b5b 2773 7769 7463 6831 272c 2027 636c  [['switch1', 'cl
-000120c0: 6965 6e74 3127 5d5d 2c20 276e 6f64 6573  ient1']], 'nodes
-000120d0: 273a 205b 2763 6c69 656e 7432 275d 7d0a  ': ['client2']}.
-000120e0: 2020 2020 3a74 7970 6520 6966 6163 653a      :type iface:
-000120f0: 203a 636c 6173 733a 6073 7472 602c 2065   :class:`str`, e
-00012100: 7820 3a20 6475 6d6d 7930 0a20 2020 203a  x : dummy0.    :
-00012110: 7479 7065 2070 6361 703a 203a 636c 6173  type pcap: :clas
-00012120: 733a 6062 6f6f 6c60 2c20 6578 203a 2074  s:`bool`, ex : t
-00012130: 7275 650a 2020 2020 3a74 7970 6520 6669  rue.    :type fi
-00012140: 6c74 6572 3a20 3a63 6c61 7373 3a60 7374  lter: :class:`st
-00012150: 7260 2c20 6578 203a 2074 6370 2070 6f72  r`, ex : tcp por
-00012160: 7420 3830 0a20 2020 203a 7479 7065 2064  t 80.    :type d
-00012170: 6972 6563 7469 6f6e 3a20 3a63 6c61 7373  irection: :class
-00012180: 3a60 7374 7260 2c20 6578 203a 2069 6e67  :`str`, ex : ing
-00012190: 7265 7373 0a20 2020 2022 2222 0a0a 2020  ress.    """..  
-000121a0: 2020 6e65 7477 6f72 6b5f 696e 7465 7266    network_interf
-000121b0: 6163 6573 203d 205b 5d0a 0a20 2020 2069  aces = []..    i
-000121c0: 6620 7369 6d75 5f6e 6f64 6573 5b22 7377  f simu_nodes["sw
-000121d0: 6974 6368 7322 5d20 6973 204e 6f6e 6520  itchs"] is None 
-000121e0: 616e 6420 7369 6d75 5f6e 6f64 6573 5b22  and simu_nodes["
-000121f0: 6e6f 6465 7322 5d20 6973 204e 6f6e 653a  nodes"] is None:
-00012200: 0a20 2020 2020 2020 2023 2043 6f6e 7369  .        # Consi
-00012210: 6465 7220 616c 6c20 6e6f 6465 206f 6620  der all node of 
-00012220: 7468 6520 7369 6d75 6c61 7469 6f6e 2028  the simulation (
-00012230: 6578 6365 7074 2072 6f75 7465 7273 2074  except routers t
-00012240: 6861 7420 6172 650a 2020 2020 2020 2020  hat are.        
-00012250: 2320 4f56 4e20 6162 7374 7261 6374 206f  # OVN abstract o
-00012260: 626a 6563 7473 206f 6e20 7768 6963 6820  bjects on which 
-00012270: 6974 2069 7320 6e6f 7420 706f 7373 6962  it is not possib
-00012280: 6c65 2074 6f20 6361 7074 7572 650a 2020  le to capture.  
-00012290: 2020 2020 2020 2320 7472 6166 6669 6329        # traffic)
-000122a0: 0a20 2020 2020 2020 2066 6f72 206e 6f64  .        for nod
-000122b0: 6520 696e 2066 6574 6368 5f6e 6f64 6573  e in fetch_nodes
-000122c0: 2869 645f 7369 6d75 6c61 7469 6f6e 293a  (id_simulation):
-000122d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000122e0: 6e6f 6465 5b22 7479 7065 225d 2021 3d20  node["type"] != 
-000122f0: 2272 6f75 7465 7222 3a0a 2020 2020 2020  "router":.      
-00012300: 2020 2020 2020 2020 2020 666f 7220 6e65            for ne
-00012310: 7477 6f72 6b5f 696e 7465 7266 6163 6520  twork_interface 
-00012320: 696e 206e 6f64 655b 226e 6574 776f 726b  in node["network
-00012330: 5f69 6e74 6572 6661 6365 7322 5d3a 0a20  _interfaces"]:. 
-00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012350: 2020 206e 6574 776f 726b 5f69 6e74 6572     network_inter
-00012360: 6661 6365 732e 6170 7065 6e64 286e 6574  faces.append(net
-00012370: 776f 726b 5f69 6e74 6572 6661 6365 5b22  work_interface["
-00012380: 6d61 635f 6164 6472 6573 7322 5d29 0a20  mac_address"]). 
-00012390: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000123a0: 2069 6620 7369 6d75 5f6e 6f64 6573 5b22   if simu_nodes["
-000123b0: 7377 6974 6368 7322 5d20 6973 206e 6f74  switchs"] is not
-000123c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000123d0: 2020 2023 204d 6972 726f 7220 7472 6166     # Mirror traf
-000123e0: 6669 6320 6672 6f6d 206e 6f64 6520 696e  fic from node in
-000123f0: 7465 7266 6163 6573 2063 6f6e 6e65 6374  terfaces connect
-00012400: 6564 2074 6f20 7468 6520 7370 6563 6966  ed to the specif
-00012410: 6965 6420 7377 6974 6368 730a 2020 2020  ied switchs.    
-00012420: 2020 2020 2020 2020 666f 7220 7377 6974          for swit
-00012430: 6368 5f6e 6f64 6573 2069 6e20 7369 6d75  ch_nodes in simu
-00012440: 5f6e 6f64 6573 5b22 7377 6974 6368 7322  _nodes["switchs"
-00012450: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00012460: 2020 2073 7769 7463 6820 3d20 6665 7463     switch = fetc
-00012470: 685f 6e6f 6465 5f62 795f 6e61 6d65 2869  h_node_by_name(i
-00012480: 645f 7369 6d75 6c61 7469 6f6e 2c20 7377  d_simulation, sw
-00012490: 6974 6368 5f6e 6f64 6573 5b30 5d29 0a0a  itch_nodes[0])..
-000124a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124b0: 2320 4368 6563 6b20 6966 2073 7065 6369  # Check if speci
-000124c0: 6669 6320 6e6f 6465 7320 6172 6520 6465  fic nodes are de
-000124d0: 6669 6e65 642c 2066 6f72 2074 6869 7320  fined, for this 
-000124e0: 7377 6974 6368 0a20 2020 2020 2020 2020  switch.         
-000124f0: 2020 2020 2020 2069 6620 7377 6974 6368         if switch
-00012500: 5f6e 6f64 6573 5b31 3a5d 3a0a 2020 2020  _nodes[1:]:.    
-00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012520: 666f 7220 6e6f 6465 5f6e 616d 6520 696e  for node_name in
-00012530: 2073 7769 7463 685f 6e6f 6465 735b 313a   switch_nodes[1:
-00012540: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00012550: 2020 2020 2020 2020 2020 206e 6f64 6520             node 
-00012560: 3d20 6665 7463 685f 6e6f 6465 5f62 795f  = fetch_node_by_
-00012570: 6e61 6d65 2869 645f 7369 6d75 6c61 7469  name(id_simulati
-00012580: 6f6e 2c20 6e6f 6465 5f6e 616d 6529 0a0a  on, node_name)..
-00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125a0: 2020 2020 2020 2020 666f 7220 6e65 7477          for netw
-000125b0: 6f72 6b5f 696e 7465 7266 6163 6520 696e  ork_interface in
-000125c0: 206e 6f64 655b 226e 6574 776f 726b 5f69   node["network_i
-000125d0: 6e74 6572 6661 6365 7322 5d3a 0a20 2020  nterfaces"]:.   
-000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125f0: 2020 2020 2020 2020 2069 6620 6e65 7477           if netw
-00012600: 6f72 6b5f 696e 7465 7266 6163 655b 2273  ork_interface["s
-00012610: 7769 7463 685f 6e61 6d65 225d 203d 3d20  witch_name"] == 
-00012620: 7377 6974 6368 5b22 6e61 6d65 225d 3a0a  switch["name"]:.
-00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012650: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-00012660: 6573 2e61 7070 656e 6428 0a20 2020 2020  es.append(.     
-00012670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012680: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00012690: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-000126a0: 5b22 6d61 635f 6164 6472 6573 7322 5d0a  ["mac_address"].
-000126b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126f0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012710: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012730: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00012740: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 2020 2022 5468 6520 6e6f 6465 2027 7b7d     "The node '{}
-00012770: 2720 6973 6e27 7420 6c69 6e6b 6564 2077  ' isn't linked w
-00012780: 6974 6820 7468 6520 7377 6974 6368 2027  ith the switch '
-00012790: 7b7d 2722 2e66 6f72 6d61 7428 0a20 2020  {}'".format(.   
-000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127c0: 206e 6f64 655f 6e61 6d65 2c20 7377 6974   node_name, swit
-000127d0: 6368 5b22 6e61 6d65 225d 0a20 2020 2020  ch["name"].     
-000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00012800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012810: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00012820: 2020 2020 2020 2020 2020 2023 2045 6c73             # Els
-00012830: 652c 2063 6f6e 7369 6465 7220 616c 6c20  e, consider all 
-00012840: 6e6f 6465 7320 636f 6e6e 6563 7465 6420  nodes connected 
-00012850: 746f 2074 6865 2073 7769 7463 680a 2020  to the switch.  
-00012860: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00012870: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00012880: 2020 2020 2020 2020 666f 7220 6e6f 6465          for node
-00012890: 2069 6e20 6665 7463 685f 6e6f 6465 7328   in fetch_nodes(
-000128a0: 6964 5f73 696d 756c 6174 696f 6e29 3a0a  id_simulation):.
-000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128c0: 2020 2020 2020 2020 6966 206e 6f64 655b          if node[
-000128d0: 2274 7970 6522 5d20 213d 2022 726f 7574  "type"] != "rout
-000128e0: 6572 223a 0a20 2020 2020 2020 2020 2020  er":.           
-000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012900: 2066 6f72 206e 6574 776f 726b 5f69 6e74   for network_int
-00012910: 6572 6661 6365 2069 6e20 6e6f 6465 5b22  erface in node["
-00012920: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-00012930: 6573 225d 3a0a 2020 2020 2020 2020 2020  es"]:.          
-00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012950: 2020 2020 2020 6966 206e 6574 776f 726b        if network
-00012960: 5f69 6e74 6572 6661 6365 5b22 7377 6974  _interface["swit
-00012970: 6368 5f6e 616d 6522 5d20 3d3d 2073 7769  ch_name"] == swi
-00012980: 7463 685b 226e 616d 6522 5d3a 0a20 2020  tch["name"]:.   
-00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129b0: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
-000129c0: 6365 732e 6170 7065 6e64 280a 2020 2020  ces.append(.    
-000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129f0: 2020 2020 6e65 7477 6f72 6b5f 696e 7465      network_inte
-00012a00: 7266 6163 655b 226d 6163 5f61 6464 7265  rface["mac_addre
-00012a10: 7373 225d 0a20 2020 2020 2020 2020 2020  ss"].           
-00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a30: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00012a40: 2020 2020 6966 2073 696d 755f 6e6f 6465      if simu_node
-00012a50: 735b 226e 6f64 6573 225d 2069 7320 6e6f  s["nodes"] is no
-00012a60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00012a70: 2020 2020 2320 4d69 7272 6f72 2074 7261      # Mirror tra
-00012a80: 6666 6963 206f 6e20 616c 6c20 696e 7465  ffic on all inte
-00012a90: 7266 6163 6573 2066 726f 6d20 7468 6520  rfaces from the 
-00012aa0: 7370 6563 6966 6965 6420 6e6f 6465 730a  specified nodes.
-00012ab0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00012ac0: 6e6f 6465 5f6e 616d 6520 696e 2073 696d  node_name in sim
-00012ad0: 755f 6e6f 6465 735b 226e 6f64 6573 225d  u_nodes["nodes"]
-00012ae0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012af0: 2020 666f 7220 6e65 7477 6f72 6b5f 696e    for network_in
-00012b00: 7465 7266 6163 6520 696e 2066 6574 6368  terface in fetch
-00012b10: 5f6e 6f64 655f 6279 5f6e 616d 6528 6964  _node_by_name(id
-00012b20: 5f73 696d 756c 6174 696f 6e2c 206e 6f64  _simulation, nod
-00012b30: 655f 6e61 6d65 295b 0a20 2020 2020 2020  e_name)[.       
-00012b40: 2020 2020 2020 2020 2020 2020 2022 6e65               "ne
-00012b50: 7477 6f72 6b5f 696e 7465 7266 6163 6573  twork_interfaces
-00012b60: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00012b70: 2020 5d3a 0a20 2020 2020 2020 2020 2020    ]:.           
-00012b80: 2020 2020 2020 2020 206e 6574 776f 726b           network
-00012b90: 5f69 6e74 6572 6661 6365 732e 6170 7065  _interfaces.appe
-00012ba0: 6e64 286e 6574 776f 726b 5f69 6e74 6572  nd(network_inter
-00012bb0: 6661 6365 5b22 6d61 635f 6164 6472 6573  face["mac_addres
-00012bc0: 7322 5d29 0a0a 2020 2020 7072 6f62 655f  s"])..    probe_
-00012bd0: 6964 203d 2063 7265 6174 655f 7072 6f62  id = create_prob
-00012be0: 6528 0a20 2020 2020 2020 2069 645f 7369  e(.        id_si
-00012bf0: 6d75 6c61 7469 6f6e 2c20 6e65 7477 6f72  mulation, networ
-00012c00: 6b5f 696e 7465 7266 6163 6573 2c20 6966  k_interfaces, if
-00012c10: 6163 652c 2070 6361 702c 2066 696c 7465  ace, pcap, filte
-00012c20: 722c 2064 6972 6563 7469 6f6e 0a20 2020  r, direction.   
-00012c30: 2029 0a0a 2020 2020 7265 7475 726e 2070   )..    return p
-00012c40: 726f 6265 5f69 640a 0a0a 6465 6620 6e65  robe_id...def ne
-00012c50: 745f 7374 6172 745f 7072 6f62 6528 6964  t_start_probe(id
-00012c60: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
-00012c70: 2c20 7072 6f62 655f 6964 3a20 696e 7429  , probe_id: int)
-00012c80: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
-00012c90: 2252 6564 6972 6563 7420 6e65 7477 6f72  "Redirect networ
-00012ca0: 6b20 7472 6166 6669 6320 746f 2074 6865  k traffic to the
-00012cb0: 2070 726f 6265 2069 6e74 6572 6661 6365   probe interface
-00012cc0: 2e0a 0a20 2020 203a 7061 7261 6d20 6964  ...    :param id
-00012cd0: 5f73 696d 756c 6174 696f 6e3a 2054 6865  _simulation: The
-00012ce0: 2069 6420 6f66 2074 6865 2073 696d 756c   id of the simul
-00012cf0: 6174 696f 6e2e 0a20 2020 203a 7061 7261  ation..    :para
-00012d00: 6d20 7072 6f62 655f 6964 3a20 5468 6520  m probe_id: The 
-00012d10: 6964 206f 6620 7468 6520 7072 6f62 650a  id of the probe.
-00012d20: 0a20 2020 203a 7479 7065 2069 645f 7369  .    :type id_si
-00012d30: 6d75 6c61 7469 6f6e 3a20 3a63 6c61 7373  mulation: :class
-00012d40: 3a60 696e 7460 2c20 6578 203a 2031 0a20  :`int`, ex : 1. 
-00012d50: 2020 203a 7479 7065 2070 726f 6265 5f69     :type probe_i
-00012d60: 643a 203a 636c 6173 733a 6069 6e74 602c  d: :class:`int`,
-00012d70: 2065 7820 3a20 310a 0a20 2020 2022 2222   ex : 1..    """
-00012d80: 0a0a 2020 2020 7265 7375 6c74 203d 205f  ..    result = _
-00012d90: 6765 7428 6622 2f73 696d 756c 6174 696f  get(f"/simulatio
-00012da0: 6e2f 7b69 645f 7369 6d75 6c61 7469 6f6e  n/{id_simulation
-00012db0: 7d2f 7072 6f62 652f 7b70 726f 6265 5f69  }/probe/{probe_i
-00012dc0: 647d 2229 0a0a 2020 2020 6966 2072 6573  d}")..    if res
-00012dd0: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
-00012de0: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
-00012df0: 5f68 616e 646c 655f 6572 726f 7228 0a20  _handle_error(. 
-00012e00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00012e10: 742c 2022 4361 6e6e 6f74 2061 6374 6976  t, "Cannot activ
-00012e20: 6174 6520 6e65 7477 6f72 6b20 7472 6166  ate network traf
-00012e30: 6669 6320 7265 6469 7265 6374 696f 6e20  fic redirection 
-00012e40: 6672 6f6d 2049 5420 5369 6d75 6c61 7469  from IT Simulati
-00012e50: 6f6e 2041 5049 220a 2020 2020 2020 2020  on API".        
-00012e60: 290a 0a0a 6465 6620 6e65 745f 7374 6f70  )...def net_stop
-00012e70: 5f70 726f 6265 2869 645f 7369 6d75 6c61  _probe(id_simula
-00012e80: 7469 6f6e 3a20 696e 742c 2070 726f 6265  tion: int, probe
-00012e90: 5f69 643a 2069 6e74 2920 2d3e 204e 6f6e  _id: int) -> Non
-00012ea0: 653a 0a20 2020 2022 2222 5374 6f70 2072  e:.    """Stop r
-00012eb0: 6564 6972 6563 7469 6f6e 206f 6620 6e65  edirection of ne
-00012ec0: 7477 6f72 6b20 7472 6166 6669 6320 746f  twork traffic to
-00012ed0: 2074 6865 2070 726f 6265 2069 6e74 6572   the probe inter
-00012ee0: 6661 6365 2e0a 0a20 2020 203a 7061 7261  face...    :para
-00012ef0: 6d20 6964 5f73 696d 756c 6174 696f 6e3a  m id_simulation:
-00012f00: 2054 6865 2069 6420 6f66 2074 6865 2073   The id of the s
-00012f10: 696d 756c 6174 696f 6e2e 0a20 2020 203a  imulation..    :
-00012f20: 7061 7261 6d20 7072 6f62 655f 6964 3a20  param probe_id: 
-00012f30: 5468 6520 6964 206f 6620 7468 6520 7072  The id of the pr
-00012f40: 6f62 650a 0a20 2020 203a 7479 7065 2069  obe..    :type i
-00012f50: 645f 7369 6d75 6c61 7469 6f6e 3a20 3a63  d_simulation: :c
-00012f60: 6c61 7373 3a60 696e 7460 2c20 6578 203a  lass:`int`, ex :
-00012f70: 2031 0a20 2020 203a 7479 7065 2070 726f   1.    :type pro
-00012f80: 6265 5f69 643a 203a 636c 6173 733a 6069  be_id: :class:`i
-00012f90: 6e74 602c 2065 7820 3a20 310a 0a20 2020  nt`, ex : 1..   
-00012fa0: 2022 2222 0a0a 2020 2020 7265 7375 6c74   """..    result
-00012fb0: 203d 205f 6765 7428 6622 2f73 696d 756c   = _get(f"/simul
-00012fc0: 6174 696f 6e2f 7b69 645f 7369 6d75 6c61  ation/{id_simula
-00012fd0: 7469 6f6e 7d2f 7374 6f70 5f70 726f 6265  tion}/stop_probe
-00012fe0: 2f7b 7072 6f62 655f 6964 7d22 290a 0a20  /{probe_id}").. 
-00012ff0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-00013000: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-00013010: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-00013020: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
-00013030: 2020 2020 7265 7375 6c74 2c20 2243 616e      result, "Can
-00013040: 6e6f 7420 7374 6f70 206e 6574 776f 726b  not stop network
-00013050: 2074 7261 6666 6963 2072 6564 6972 6563   traffic redirec
-00013060: 7469 6f6e 2066 726f 6d20 4954 2053 696d  tion from IT Sim
-00013070: 756c 6174 696f 6e20 4150 4922 0a20 2020  ulation API".   
-00013080: 2020 2020 2029 0a0a 0a64 6566 2066 6574       )...def fet
-00013090: 6368 5f6c 6973 745f 7072 6f62 6573 2869  ch_list_probes(i
-000130a0: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
-000130b0: 7429 202d 3e20 4469 6374 3a0a 2020 2020  t) -> Dict:.    
-000130c0: 2222 2252 6574 7572 6e20 7468 6520 6c69  """Return the li
-000130d0: 7374 206f 6620 7072 6f62 6573 2077 6974  st of probes wit
-000130e0: 6820 7468 6569 7220 6461 7461 0a0a 2020  h their data..  
-000130f0: 2020 3a70 6172 616d 2069 645f 7369 6d75    :param id_simu
-00013100: 6c61 7469 6f6e 3a20 5468 6520 6964 206f  lation: The id o
-00013110: 6620 7468 6520 7369 6d75 6c61 7469 6f6e  f the simulation
-00013120: 0a0a 2020 2020 3a74 7970 6520 6964 5f73  ..    :type id_s
-00013130: 696d 756c 6174 696f 6e3a 203a 636c 6173  imulation: :clas
-00013140: 733a 6069 6e74 602c 2065 7820 3a20 310a  s:`int`, ex : 1.
-00013150: 0a20 2020 203a 7265 7475 726e 3a20 4120  .    :return: A 
-00013160: 6c69 7374 206f 6620 7072 6f62 6573 2077  list of probes w
-00013170: 6974 6820 7468 6569 7220 6461 7461 0a20  ith their data. 
-00013180: 2020 2022 2222 0a0a 2020 2020 7265 7375     """..    resu
-00013190: 6c74 203d 207b 7d0a 0a20 2020 2070 726f  lt = {}..    pro
-000131a0: 6265 7320 3d20 6665 7463 685f 7072 6f62  bes = fetch_prob
-000131b0: 6573 2869 645f 7369 6d75 6c61 7469 6f6e  es(id_simulation
-000131c0: 290a 2020 2020 666f 7220 7072 6f62 6520  ).    for probe 
-000131d0: 696e 2070 726f 6265 733a 0a20 2020 2020  in probes:.     
-000131e0: 2020 2072 6573 756c 745b 7072 6f62 655b     result[probe[
-000131f0: 2269 6422 5d5d 203d 207b 0a20 2020 2020  "id"]] = {.     
-00013200: 2020 2020 2020 2022 636f 6c6c 6563 7469         "collecti
-00013210: 6e67 5f70 6f69 6e74 7322 3a20 6665 7463  ng_points": fetc
-00013220: 685f 7072 6f62 655f 636f 6c6c 6563 7469  h_probe_collecti
-00013230: 6e67 5f70 6f69 6e74 7328 6964 5f73 696d  ng_points(id_sim
-00013240: 756c 6174 696f 6e2c 2070 726f 6265 292c  ulation, probe),
-00013250: 0a20 2020 2020 2020 2020 2020 2022 6966  .            "if
-00013260: 6163 6522 3a20 7072 6f62 655b 2269 6661  ace": probe["ifa
-00013270: 6365 225d 2c0a 2020 2020 2020 2020 2020  ce"],.          
-00013280: 2020 2270 6361 7022 3a20 7072 6f62 655b    "pcap": probe[
-00013290: 2270 6361 7022 5d2c 0a20 2020 2020 2020  "pcap"],.       
-000132a0: 2020 2020 2022 6669 6c74 6572 223a 2070       "filter": p
-000132b0: 726f 6265 5b22 6669 6c74 6572 225d 2c0a  robe["filter"],.
-000132c0: 2020 2020 2020 2020 2020 2020 2263 6170              "cap
-000132d0: 7475 7265 5f69 6e5f 7072 6f67 7265 7373  ture_in_progress
-000132e0: 223a 2070 726f 6265 5b22 6361 7074 7572  ": probe["captur
-000132f0: 655f 696e 5f70 726f 6772 6573 7322 5d2c  e_in_progress"],
-00013300: 0a20 2020 2020 2020 2020 2020 2022 6469  .            "di
-00013310: 7265 6374 696f 6e22 3a20 7072 6f62 655b  rection": probe[
-00013320: 2264 6972 6563 7469 6f6e 225d 2c0a 2020  "direction"],.  
-00013330: 2020 2020 2020 7d0a 0a20 2020 2072 6574        }..    ret
-00013340: 7572 6e20 7265 7375 6c74 0a0a 0a64 6566  urn result...def
-00013350: 2066 6574 6368 5f70 726f 6265 5f63 6f6c   fetch_probe_col
-00013360: 6c65 6374 696e 675f 706f 696e 7473 2869  lecting_points(i
-00013370: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
-00013380: 742c 2070 726f 6265 3a20 4469 6374 2920  t, probe: Dict) 
-00013390: 2d3e 2041 6e79 3a0a 2020 2020 2222 2252  -> Any:.    """R
-000133a0: 6574 7572 6e20 7468 6520 6c69 7374 206f  eturn the list o
-000133b0: 6620 636f 6c6c 6563 7469 6e67 2070 6f69  f collecting poi
-000133c0: 6e74 7320 7573 6564 2074 6f20 6361 7074  nts used to capt
-000133d0: 7572 6520 7468 6520 6e65 7477 6f72 6b20  ure the network 
-000133e0: 7472 6166 6669 6320 746f 2061 2067 6976  traffic to a giv
-000133f0: 656e 2070 726f 6265 206f 6620 6120 7369  en probe of a si
-00013400: 6d75 6c61 7469 6f6e 2e0a 0a20 2020 203a  mulation...    :
-00013410: 7061 7261 6d20 6964 5f73 696d 756c 6174  param id_simulat
-00013420: 696f 6e3a 2054 6865 2069 6420 6f66 2074  ion: The id of t
-00013430: 6865 2073 696d 756c 6174 696f 6e2e 0a20  he simulation.. 
-00013440: 2020 203a 7061 7261 6d20 7072 6f62 653a     :param probe:
-00013450: 2054 6865 2067 6976 656e 2070 726f 6265   The given probe
-00013460: 206f 6620 7468 6520 7369 6d75 6c61 7469   of the simulati
-00013470: 6f6e 0a0a 2020 2020 3a74 7970 6520 6964  on..    :type id
-00013480: 5f73 696d 756c 6174 696f 6e3a 203a 636c  _simulation: :cl
-00013490: 6173 733a 6069 6e74 602c 2065 7820 3a20  ass:`int`, ex : 
-000134a0: 310a 2020 2020 3a74 7970 6520 7072 6f62  1.    :type prob
-000134b0: 653a 203a 636c 6173 733a 6063 6c61 7373  e: :class:`class
-000134c0: 603a 6044 6963 7460 2c20 6578 203a 207b  `:`Dict`, ex : {
-000134d0: 2769 6661 6365 273a 2027 6475 6d6d 7930  'iface': 'dummy0
-000134e0: 272c 2027 6964 273a 2031 2c20 2770 6361  ', 'id': 1, 'pca
-000134f0: 7027 3a20 5472 7565 2c20 2763 6170 7475  p': True, 'captu
-00013500: 7265 5f69 6e5f 7072 6f67 7265 7373 273a  re_in_progress':
-00013510: 2046 616c 7365 2c20 2766 696c 7465 7227   False, 'filter'
-00013520: 3a20 2774 6370 2070 6f72 7420 3830 272c  : 'tcp port 80',
-00013530: 2027 7369 6d75 6c61 7469 6f6e 5f69 6427   'simulation_id'
-00013540: 3a20 312c 2027 6e65 7477 6f72 6b5f 696e  : 1, 'network_in
-00013550: 7465 7266 6163 6573 273a 205b 2730 303a  terfaces': ['00:
-00013560: 3231 3a61 313a 3037 3a37 643a 6265 275d  21:a1:07:7d:be']
-00013570: 2c20 2764 6972 6563 7469 6f6e 273a 2027  , 'direction': '
-00013580: 696e 6772 6573 7327 7d0a 0a20 2020 2022  ingress'}..    "
-00013590: 2222 0a0a 2020 2020 636f 6c6c 6563 7469  ""..    collecti
-000135a0: 6e67 5f70 6f69 6e74 7320 3d20 7b22 7377  ng_points = {"sw
-000135b0: 6974 6368 7322 3a20 7b7d 2c20 226e 6f64  itchs": {}, "nod
-000135c0: 6573 223a 205b 5d7d 0a0a 2020 2020 6e65  es": []}..    ne
-000135d0: 7477 6f72 6b5f 696e 7465 7266 6163 6573  twork_interfaces
-000135e0: 203d 205b 0a20 2020 2020 2020 2066 6574   = [.        fet
-000135f0: 6368 5f6e 6574 776f 726b 5f69 6e74 6572  ch_network_inter
-00013600: 6661 6365 5f62 795f 6d61 6328 6964 5f73  face_by_mac(id_s
-00013610: 696d 756c 6174 696f 6e2c 206e 290a 2020  imulation, n).  
-00013620: 2020 2020 2020 666f 7220 6e20 696e 2070        for n in p
-00013630: 726f 6265 5b22 6e65 7477 6f72 6b5f 696e  robe["network_in
-00013640: 7465 7266 6163 6573 225d 0a20 2020 205d  terfaces"].    ]
-00013650: 0a0a 2020 2020 6e6f 6465 735f 746f 5f63  ..    nodes_to_c
-00013660: 6170 7475 7265 203d 205b 5d0a 2020 2020  apture = [].    
-00013670: 666f 7220 6e65 7477 6f72 6b5f 696e 7465  for network_inte
-00013680: 7266 6163 6520 696e 206e 6574 776f 726b  rface in network
-00013690: 5f69 6e74 6572 6661 6365 733a 0a20 2020  _interfaces:.   
-000136a0: 2020 2020 206e 6f64 6520 3d20 6665 7463       node = fetc
-000136b0: 685f 6e6f 6465 286e 6574 776f 726b 5f69  h_node(network_i
-000136c0: 6e74 6572 6661 6365 5b22 6e6f 6465 5f69  nterface["node_i
-000136d0: 6422 5d29 0a20 2020 2020 2020 2069 6620  d"]).        if 
-000136e0: 6e6f 6465 206e 6f74 2069 6e20 6e6f 6465  node not in node
-000136f0: 735f 746f 5f63 6170 7475 7265 3a0a 2020  s_to_capture:.  
-00013700: 2020 2020 2020 2020 2020 6e6f 6465 735f            nodes_
-00013710: 746f 5f63 6170 7475 7265 2e61 7070 656e  to_capture.appen
-00013720: 6428 6e6f 6465 290a 0a20 2020 2023 2052  d(node)..    # R
-00013730: 6574 7572 6e20 4e6f 6e65 2069 6620 7468  eturn None if th
-00013740: 6572 6520 6973 206e 6f74 6869 6e67 2074  ere is nothing t
-00013750: 6f20 6361 7074 7572 650a 2020 2020 6966  o capture.    if
-00013760: 206e 6f64 6573 5f74 6f5f 6361 7074 7572   nodes_to_captur
-00013770: 6520 3d3d 205b 5d3a 0a20 2020 2020 2020  e == []:.       
-00013780: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-00013790: 2020 2320 5265 7475 726e 207b 7d20 6966    # Return {} if
-000137a0: 2065 7665 7279 206e 6f64 6520 6d75 7374   every node must
-000137b0: 2062 6520 6361 7074 7572 6564 0a20 2020   be captured.   
-000137c0: 2069 6620 6c65 6e28 6e65 7477 6f72 6b5f   if len(network_
-000137d0: 696e 7465 7266 6163 6573 2920 3d3d 206c  interfaces) == l
-000137e0: 656e 280a 2020 2020 2020 2020 6665 7463  en(.        fetc
-000137f0: 685f 7369 6d75 6c61 7469 6f6e 5f6e 6574  h_simulation_net
-00013800: 776f 726b 5f69 6e74 6572 6661 6365 7328  work_interfaces(
-00013810: 6964 5f73 696d 756c 6174 696f 6e29 0a20  id_simulation). 
-00013820: 2020 2029 3a0a 2020 2020 2020 2020 7265     ):.        re
-00013830: 7475 726e 207b 7d0a 0a20 2020 2066 6f72  turn {}..    for
-00013840: 206e 6f64 6520 696e 206e 6f64 6573 5f74   node in nodes_t
-00013850: 6f5f 6361 7074 7572 653a 0a0a 2020 2020  o_capture:..    
-00013860: 2020 2020 2320 4966 2065 7665 7279 206e      # If every n
-00013870: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-00013880: 2066 726f 6d20 6120 6e6f 6465 2069 7320   from a node is 
-00013890: 6361 7074 7572 6564 2c20 6974 2067 6f65  captured, it goe
-000138a0: 7320 746f 2074 6865 2022 6e6f 6465 7322  s to the "nodes"
-000138b0: 2064 6963 740a 2020 2020 2020 2020 6361   dict.        ca
-000138c0: 7074 7572 655f 616c 6c5f 6e65 7477 6f72  pture_all_networ
-000138d0: 6b5f 696e 7465 7266 6163 6573 203d 2054  k_interfaces = T
-000138e0: 7275 650a 2020 2020 2020 2020 666f 7220  rue.        for 
-000138f0: 6e6f 6465 5f6e 6574 776f 726b 5f69 6e74  node_network_int
-00013900: 6572 6661 6365 2069 6e20 6e6f 6465 5b22  erface in node["
-00013910: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-00013920: 6573 225d 3a0a 2020 2020 2020 2020 2020  es"]:.          
-00013930: 2020 6361 7074 7572 655f 616c 6c5f 6e65    capture_all_ne
-00013940: 7477 6f72 6b5f 696e 7465 7266 6163 6573  twork_interfaces
-00013950: 203d 2063 6170 7475 7265 5f61 6c6c 5f6e   = capture_all_n
-00013960: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-00013970: 7320 616e 6420 280a 2020 2020 2020 2020  s and (.        
-00013980: 2020 2020 2020 2020 6e6f 6465 5f6e 6574          node_net
-00013990: 776f 726b 5f69 6e74 6572 6661 6365 2069  work_interface i
-000139a0: 6e20 6e65 7477 6f72 6b5f 696e 7465 7266  n network_interf
-000139b0: 6163 6573 0a20 2020 2020 2020 2020 2020  aces.           
-000139c0: 2029 0a0a 2020 2020 2020 2020 6966 2063   )..        if c
-000139d0: 6170 7475 7265 5f61 6c6c 5f6e 6574 776f  apture_all_netwo
-000139e0: 726b 5f69 6e74 6572 6661 6365 733a 0a20  rk_interfaces:. 
-000139f0: 2020 2020 2020 2020 2020 2063 6f6c 6c65             colle
-00013a00: 6374 696e 675f 706f 696e 7473 5b22 6e6f  cting_points["no
-00013a10: 6465 7322 5d2e 6170 7065 6e64 286e 6f64  des"].append(nod
-00013a20: 655b 226e 616d 6522 5d29 0a20 2020 2020  e["name"]).     
-00013a30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00013a40: 2020 2020 2023 2045 6c73 652c 2069 7420       # Else, it 
-00013a50: 676f 6573 2074 6f20 7468 6520 2273 7769  goes to the "swi
-00013a60: 7463 6873 2220 6469 6374 0a20 2020 2020  tchs" dict.     
-00013a70: 2020 2020 2020 2066 6f72 206e 6f64 655f         for node_
-00013a80: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-00013a90: 6520 696e 206e 6f64 655b 226e 6574 776f  e in node["netwo
-00013aa0: 726b 5f69 6e74 6572 6661 6365 7322 5d3a  rk_interfaces"]:
-00013ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ac0: 2069 6620 6e6f 6465 5f6e 6574 776f 726b   if node_network
-00013ad0: 5f69 6e74 6572 6661 6365 2069 6e20 6e65  _interface in ne
-00013ae0: 7477 6f72 6b5f 696e 7465 7266 6163 6573  twork_interfaces
-00013af0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013b00: 2020 2020 2020 7377 6974 6368 203d 207b        switch = {
-00013b10: 226e 616d 6522 3a20 6e6f 6465 5f6e 6574  "name": node_net
-00013b20: 776f 726b 5f69 6e74 6572 6661 6365 5b22  work_interface["
-00013b30: 7377 6974 6368 5f6e 616d 6522 5d7d 0a0a  switch_name"]}..
-00013b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b50: 2020 2020 6966 2073 7769 7463 685b 226e      if switch["n
-00013b60: 616d 6522 5d20 6e6f 7420 696e 2063 6f6c  ame"] not in col
-00013b70: 6c65 6374 696e 675f 706f 696e 7473 5b22  lecting_points["
-00013b80: 7377 6974 6368 7322 5d2e 6b65 7973 2829  switchs"].keys()
-00013b90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013ba0: 2020 2020 2020 2020 2020 636f 6c6c 6563            collec
-00013bb0: 7469 6e67 5f70 6f69 6e74 735b 2273 7769  ting_points["swi
-00013bc0: 7463 6873 225d 5b73 7769 7463 685b 226e  tchs"][switch["n
-00013bd0: 616d 6522 5d5d 203d 205b 5d0a 2020 2020  ame"]] = [].    
-00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bf0: 636f 6c6c 6563 7469 6e67 5f70 6f69 6e74  collecting_point
-00013c00: 735b 2273 7769 7463 6873 225d 5b73 7769  s["switchs"][swi
-00013c10: 7463 685b 226e 616d 6522 5d5d 2e61 7070  tch["name"]].app
-00013c20: 656e 6428 6e6f 6465 5b22 6e61 6d65 225d  end(node["name"]
-00013c30: 290a 0a20 2020 2072 6574 7572 6e20 636f  )..    return co
-00013c40: 6c6c 6563 7469 6e67 5f70 6f69 6e74 730a  llecting_points.
-00013c50: 0a0a 6465 6620 736e 6170 7368 6f74 5f73  ..def snapshot_s
-00013c60: 696d 756c 6174 696f 6e28 6964 5f73 696d  imulation(id_sim
-00013c70: 756c 6174 696f 6e3a 2069 6e74 2920 2d3e  ulation: int) ->
-00013c80: 2073 7472 3a0a 2020 2020 2222 2243 7265   str:.    """Cre
-00013c90: 6174 6520 6120 736e 6170 7368 6f74 206f  ate a snapshot o
-00013ca0: 6620 6120 7369 6d75 6c61 7469 6f6e 2e0a  f a simulation..
-00013cb0: 0a20 2020 2041 6c6c 2074 6865 2066 696c  .    All the fil
-00013cc0: 6573 2077 696c 6c20 6265 2073 746f 7265  es will be store
-00013cd0: 6420 746f 0a20 2020 202f 6379 6265 722d  d to.    /cyber-
-00013ce0: 7261 6e67 652d 6361 7461 6c6f 672f 7369  range-catalog/si
-00013cf0: 6d75 6c61 7469 6f6e 732f 3c68 6173 6820  mulations/<hash 
-00013d00: 6361 6d70 6169 676e 3e2f 3c74 696d 6573  campaign>/<times
-00013d10: 7461 6d70 3e2f 0a0a 2020 2020 5468 6973  tamp>/..    This
-00013d20: 2041 5049 2063 616c 6c20 7265 7475 726e   API call return
-00013d30: 7320 7468 6520 7061 7468 2077 6865 7265  s the path where
-00013d40: 2074 6865 2074 6f70 6f6c 6f67 7920 6669   the topology fi
-00013d50: 6c65 2077 696c 6c20 6265 2073 746f 7265  le will be store
-00013d60: 642e 0a0a 2020 2020 5061 7261 6d65 7465  d...    Paramete
-00013d70: 7273 3a0a 0a20 2020 2069 645f 7369 6d75  rs:..    id_simu
-00013d80: 6c61 7469 6f6e 3a20 696e 740a 2020 2020  lation: int.    
-00013d90: 2020 2020 5369 6d75 6c61 7469 6f6e 2074      Simulation t
-00013da0: 6f20 736e 6170 7368 6f74 0a0a 2020 2020  o snapshot..    
-00013db0: 2222 220a 0a20 2020 2023 2073 696d 755f  """..    # simu_
-00013dc0: 736e 6170 2063 616e 206f 6e6c 7920 6265  snap can only be
-00013dd0: 2064 6f6e 6520 6f6e 2061 2052 554e 4e49   done on a RUNNI
-00013de0: 4e47 2073 696d 756c 6174 696f 6e0a 2020  NG simulation.  
-00013df0: 2020 6966 2073 696d 756c 6174 696f 6e5f    if simulation_
-00013e00: 7374 6174 7573 2869 645f 7369 6d75 6c61  status(id_simula
-00013e10: 7469 6f6e 2920 213d 2022 5255 4e4e 494e  tion) != "RUNNIN
-00013e20: 4722 3a0a 2020 2020 2020 2020 7261 6973  G":.        rais
-00013e30: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
-00013e40: 2020 2020 2020 2020 2022 4361 6e6e 6f74           "Cannot
-00013e50: 2063 7265 6174 6520 6120 736e 6170 7368   create a snapsh
-00013e60: 6f74 206f 6620 7468 6520 7369 6d75 6c61  ot of the simula
-00013e70: 7469 6f6e 2c20 6173 2074 6865 2073 696d  tion, as the sim
-00013e80: 756c 6174 696f 6e20 277b 7d27 2069 7320  ulation '{}' is 
-00013e90: 220a 2020 2020 2020 2020 2020 2020 226e  ".            "n
-00013ea0: 6f74 2072 756e 6e69 6e67 222e 666f 726d  ot running".form
-00013eb0: 6174 2869 645f 7369 6d75 6c61 7469 6f6e  at(id_simulation
-00013ec0: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-00013ed0: 2023 2043 616c 6c20 736e 6170 7368 6f74   # Call snapshot
-00013ee0: 2041 5049 0a20 2020 2072 6573 756c 7420   API.    result 
-00013ef0: 3d20 5f70 6f73 7428 6622 2f73 696d 756c  = _post(f"/simul
-00013f00: 6174 696f 6e2f 7b69 645f 7369 6d75 6c61  ation/{id_simula
-00013f10: 7469 6f6e 7d2f 736e 6170 7368 6f74 2229  tion}/snapshot")
-00013f20: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
-00013f30: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-00013f40: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
-00013f50: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
-00013f60: 2022 4572 726f 7220 7768 696c 6520 6372   "Error while cr
-00013f70: 6561 7469 6e67 2073 6e61 7073 686f 7422  eating snapshot"
-00013f80: 290a 0a20 2020 2079 616d 6c3a 2073 7472  )..    yaml: str
-00013f90: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
-00013fa0: 0a0a 2020 2020 6c6f 6767 6572 2e69 6e66  ..    logger.inf
-00013fb0: 6f28 6622 5b2b 5d20 5374 6172 7469 6e67  o(f"[+] Starting
-00013fc0: 2074 6865 2073 6e61 7073 686f 7420 6f66   the snapshot of
-00013fd0: 2073 696d 756c 6174 696f 6e20 7b69 645f   simulation {id_
-00013fe0: 7369 6d75 6c61 7469 6f6e 7d2e 2e2e 2229  simulation}...")
-00013ff0: 0a20 2020 2077 6869 6c65 2073 696d 756c  .    while simul
-00014000: 6174 696f 6e5f 7374 6174 7573 2869 645f  ation_status(id_
-00014010: 7369 6d75 6c61 7469 6f6e 2920 213d 2022  simulation) != "
-00014020: 534e 4150 5348 4f54 223a 0a20 2020 2020  SNAPSHOT":.     
-00014030: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
-00014040: 0a0a 2020 2020 2020 2020 7369 6d75 6c61  ..        simula
-00014050: 7469 6f6e 5f64 6963 7420 3d20 6665 7463  tion_dict = fetc
-00014060: 685f 7369 6d75 6c61 7469 6f6e 2869 645f  h_simulation(id_
-00014070: 7369 6d75 6c61 7469 6f6e 290a 2020 2020  simulation).    
-00014080: 2020 2020 6375 7272 656e 745f 7374 6174      current_stat
-00014090: 7573 203d 2073 696d 756c 6174 696f 6e5f  us = simulation_
-000140a0: 6469 6374 5b22 7374 6174 7573 225d 0a20  dict["status"]. 
-000140b0: 2020 2020 2020 2069 6620 6375 7272 656e         if curren
-000140c0: 745f 7374 6174 7573 203d 3d20 2245 5252  t_status == "ERR
-000140d0: 4f52 223a 0a20 2020 2020 2020 2020 2020  OR":.           
-000140e0: 2065 7272 6f72 5f6d 6573 7361 6765 203d   error_message =
-000140f0: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
-00014100: 5b22 6572 726f 725f 6d73 6722 5d0a 2020  ["error_msg"].  
-00014110: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00014120: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
-00014130: 2020 2020 2020 2020 2020 2022 4572 726f             "Erro
-00014140: 7220 6475 7269 6e67 2073 696d 756c 6174  r during simulat
-00014150: 696f 6e20 736e 6170 7368 6f74 3a20 277b  ion snapshot: '{
-00014160: 7d27 222e 666f 726d 6174 2865 7272 6f72  }'".format(error
-00014170: 5f6d 6573 7361 6765 290a 2020 2020 2020  _message).      
-00014180: 2020 2020 2020 290a 0a20 2020 206c 6f67        )..    log
-00014190: 6765 722e 696e 666f 2822 5b2b 5d20 536e  ger.info("[+] Sn
-000141a0: 6170 7368 6f74 2070 726f 6365 7373 2068  apshot process h
-000141b0: 6173 2073 7461 7274 6564 2229 0a0a 2020  as started")..  
-000141c0: 2020 7768 696c 6520 7369 6d75 6c61 7469    while simulati
-000141d0: 6f6e 5f73 7461 7475 7328 6964 5f73 696d  on_status(id_sim
-000141e0: 756c 6174 696f 6e29 2021 3d20 2252 4541  ulation) != "REA
-000141f0: 4459 223a 0a20 2020 2020 2020 206c 6f67  DY":.        log
-00014200: 6765 722e 696e 666f 2822 2020 5b2b 5d20  ger.info("  [+] 
-00014210: 536e 6170 7368 6f74 2069 6e20 7072 6f67  Snapshot in prog
-00014220: 7265 7373 2e2e 2e22 290a 2020 2020 2020  ress...").      
-00014230: 2020 7469 6d65 2e73 6c65 6570 2831 290a    time.sleep(1).
-00014240: 0a20 2020 2020 2020 2073 696d 756c 6174  .        simulat
-00014250: 696f 6e5f 6469 6374 203d 2066 6574 6368  ion_dict = fetch
-00014260: 5f73 696d 756c 6174 696f 6e28 6964 5f73  _simulation(id_s
-00014270: 696d 756c 6174 696f 6e29 0a20 2020 2020  imulation).     
-00014280: 2020 2063 7572 7265 6e74 5f73 7461 7475     current_statu
-00014290: 7320 3d20 7369 6d75 6c61 7469 6f6e 5f64  s = simulation_d
-000142a0: 6963 745b 2273 7461 7475 7322 5d0a 2020  ict["status"].  
-000142b0: 2020 2020 2020 6966 2063 7572 7265 6e74        if current
-000142c0: 5f73 7461 7475 7320 3d3d 2022 4552 524f  _status == "ERRO
-000142d0: 5222 3a0a 2020 2020 2020 2020 2020 2020  R":.            
-000142e0: 6572 726f 725f 6d65 7373 6167 6520 3d20  error_message = 
-000142f0: 7369 6d75 6c61 7469 6f6e 5f64 6963 745b  simulation_dict[
-00014300: 2265 7272 6f72 5f6d 7367 225d 0a20 2020  "error_msg"].   
-00014310: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
-00014320: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
-00014330: 2020 2020 2020 2020 2020 2245 7272 6f72            "Error
-00014340: 2064 7572 696e 6720 7369 6d75 6c61 7469   during simulati
-00014350: 6f6e 2073 6e61 7073 686f 743a 2027 7b7d  on snapshot: '{}
-00014360: 2722 2e66 6f72 6d61 7428 6572 726f 725f  '".format(error_
-00014370: 6d65 7373 6167 6529 0a20 2020 2020 2020  message).       
-00014380: 2020 2020 2029 0a0a 2020 2020 7265 7475       )..    retu
-00014390: 726e 2079 616d 6c0a 0a0a 6465 6620 636f  rn yaml...def co
-000143a0: 6d70 7574 655f 696e 6672 6173 7472 7563  mpute_infrastruc
-000143b0: 7475 7265 5f73 7461 7475 7328 2920 2d3e  ture_status() ->
-000143c0: 2041 6e79 3a0a 2020 2020 2222 2247 6574   Any:.    """Get
-000143d0: 2076 6972 7463 6c69 656e 7420 7365 7276   virtclient serv
-000143e0: 6963 6520 7374 6174 7573 2e22 2222 0a20  ice status.""". 
-000143f0: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
-00014400: 2822 2f73 696d 756c 6174 696f 6e2f 636f  ("/simulation/co
-00014410: 6d70 7574 655f 696e 6672 6173 7472 7563  mpute_infrastruc
-00014420: 7475 7265 5f73 7461 7475 7322 290a 0a20  ture_status").. 
-00014430: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-00014440: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-00014450: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-00014460: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-00014470: 4361 6e6e 6f74 2067 6574 2063 6f6d 7075  Cannot get compu
-00014480: 7465 2069 6e66 7261 7374 7275 6374 7572  te infrastructur
-00014490: 6520 7374 6174 7573 2229 0a0a 2020 2020  e status")..    
-000144a0: 7369 6d75 6c61 7469 6f6e 5f64 6963 7420  simulation_dict 
-000144b0: 3d20 7265 7375 6c74 2e6a 736f 6e28 290a  = result.json().
-000144c0: 2020 2020 7265 7475 726e 2073 696d 756c      return simul
-000144d0: 6174 696f 6e5f 6469 6374 0a0a 0a64 6566  ation_dict...def
-000144e0: 2061 6464 5f64 6e73 5f65 6e74 7269 6573   add_dns_entries
-000144f0: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
-00014500: 696e 742c 2064 6e73 5f65 6e74 7269 6573  int, dns_entries
-00014510: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-00014520: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
-00014530: 2241 6464 2076 6f6c 6174 696c 6520 444e  "Add volatile DN
-00014540: 5320 656e 7472 6965 7320 746f 2074 6865  S entries to the
-00014550: 2063 7572 7265 6e74 2073 696d 756c 6174   current simulat
-00014560: 696f 6e2e 2056 6f6c 6174 696c 6520 6d65  ion. Volatile me
-00014570: 616e 7320 7468 6174 2069 7420 6973 206e  ans that it is n
-00014580: 6f74 0a20 2020 2073 746f 7265 6420 696e  ot.    stored in
-00014590: 2064 6174 6162 6173 652e 0a0a 2020 2020   database...    
-000145a0: 2222 220a 0a20 2020 2064 6174 6120 3d20  """..    data = 
-000145b0: 6a73 6f6e 2e64 756d 7073 2864 6e73 5f65  json.dumps(dns_e
-000145c0: 6e74 7269 6573 290a 2020 2020 7265 7375  ntries).    resu
-000145d0: 6c74 203d 205f 706f 7374 280a 2020 2020  lt = _post(.    
-000145e0: 2020 2020 6622 2f73 696d 756c 6174 696f      f"/simulatio
-000145f0: 6e2f 7b69 645f 7369 6d75 6c61 7469 6f6e  n/{id_simulation
-00014600: 7d2f 6164 645f 646e 735f 656e 7472 6965  }/add_dns_entrie
-00014610: 7322 2c0a 2020 2020 2020 2020 6461 7461  s",.        data
-00014620: 3d64 6174 612c 0a20 2020 2020 2020 2068  =data,.        h
-00014630: 6561 6465 7273 3d7b 2243 6f6e 7465 6e74  eaders={"Content
-00014640: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
-00014650: 7469 6f6e 2f6a 736f 6e22 7d2c 0a20 2020  tion/json"},.   
-00014660: 2029 0a0a 2020 2020 6966 2072 6573 756c   )..    if resul
-00014670: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
-00014680: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
-00014690: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
-000146a0: 6c74 2c20 2245 7272 6f72 2077 6869 6c65  lt, "Error while
-000146b0: 2061 6464 696e 6720 444e 5320 656e 7472   adding DNS entr
-000146c0: 6965 7322 290a 0a0a 6465 6620 636f 6e6e  ies")...def conn
-000146d0: 6563 745f 686f 7374 2869 645f 7369 6d75  ect_host(id_simu
-000146e0: 6c61 7469 6f6e 3a20 696e 7429 202d 3e20  lation: int) -> 
-000146f0: 4e6f 6e65 3a0a 2020 2020 2222 2243 6f6e  None:.    """Con
-00014700: 6e65 6374 2074 6865 2068 6f73 7420 696e  nect the host in
-00014710: 7465 7266 6163 6520 746f 2074 6865 2063  terface to the c
-00014720: 7572 7265 6e74 2073 696d 756c 6174 696f  urrent simulatio
-00014730: 6e2e 2222 220a 0a20 2020 2072 6573 756c  n."""..    resul
-00014740: 7420 3d20 5f67 6574 2866 222f 7369 6d75  t = _get(f"/simu
-00014750: 6c61 7469 6f6e 2f7b 6964 5f73 696d 756c  lation/{id_simul
-00014760: 6174 696f 6e7d 2f63 6f6e 6e65 6374 5f68  ation}/connect_h
-00014770: 6f73 7422 290a 0a20 2020 2069 6620 7265  ost")..    if re
-00014780: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-00014790: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
-000147a0: 205f 6861 6e64 6c65 5f65 7272 6f72 280a   _handle_error(.
-000147b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000147c0: 6c74 2c0a 2020 2020 2020 2020 2020 2020  lt,.            
-000147d0: 6622 4361 6e6e 6f74 2065 7865 6375 7465  f"Cannot execute
-000147e0: 206f 7065 7261 7469 6f6e 2027 636f 6e6e   operation 'conn
-000147f0: 6563 745f 686f 7374 2720 6f6e 2073 696d  ect_host' on sim
-00014800: 756c 6174 696f 6e20 277b 6964 5f73 696d  ulation '{id_sim
-00014810: 756c 6174 696f 6e7d 272e 222c 0a20 2020  ulation}'.",.   
-00014820: 2020 2020 2029 0a0a 0a64 6566 2064 6973       )...def dis
-00014830: 636f 6e6e 6563 745f 686f 7374 2869 645f  connect_host(id_
-00014840: 7369 6d75 6c61 7469 6f6e 3a20 696e 7429  simulation: int)
-00014850: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
-00014860: 2244 6973 636f 6e6e 6563 7420 7468 6520  "Disconnect the 
-00014870: 686f 7374 2069 6e74 6572 6661 6365 2074  host interface t
-00014880: 6f20 7468 6520 6375 7272 656e 7420 7369  o the current si
-00014890: 6d75 6c61 7469 6f6e 2e22 2222 0a0a 2020  mulation."""..  
-000148a0: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
-000148b0: 6622 2f73 696d 756c 6174 696f 6e2f 7b69  f"/simulation/{i
-000148c0: 645f 7369 6d75 6c61 7469 6f6e 7d2f 6469  d_simulation}/di
-000148d0: 7363 6f6e 6e65 6374 5f68 6f73 7422 290a  sconnect_host").
-000148e0: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
-000148f0: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-00014900: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
-00014910: 6c65 5f65 7272 6f72 280a 2020 2020 2020  le_error(.      
-00014920: 2020 2020 2020 7265 7375 6c74 2c0a 2020        result,.  
-00014930: 2020 2020 2020 2020 2020 6622 4361 6e6e            f"Cann
-00014940: 6f74 2065 7865 6375 7465 206f 7065 7261  ot execute opera
-00014950: 7469 6f6e 2027 6469 7363 6f6e 6e65 6374  tion 'disconnect
-00014960: 5f68 6f73 7427 206f 6e20 7369 6d75 6c61  _host' on simula
-00014970: 7469 6f6e 2027 7b69 645f 7369 6d75 6c61  tion '{id_simula
-00014980: 7469 6f6e 7d27 2e22 2c0a 2020 2020 2020  tion}'.",.      
-00014990: 2020 290a 0a0a 6465 6620 6765 6e65 7261    )...def genera
-000149a0: 7465 5f6d 616c 6963 696f 7573 5f64 6f6d  te_malicious_dom
-000149b0: 6169 6e73 2861 6c67 6f72 6974 686d 3a20  ains(algorithm: 
-000149c0: 7374 7220 3d20 4e6f 6e65 2c20 6e75 6d62  str = None, numb
-000149d0: 6572 3a20 696e 7420 3d20 3129 202d 3e20  er: int = 1) -> 
-000149e0: 4c69 7374 5b73 7472 5d3a 0a20 2020 2022  List[str]:.    "
-000149f0: 2222 4765 6e65 7261 7465 2061 6e64 2072  ""Generate and r
-00014a00: 6574 7572 6e20 6120 6c69 7374 206f 6620  eturn a list of 
-00014a10: 6d61 6c69 6369 6f75 7320 646f 6d61 696e  malicious domain
-00014a20: 732e 2222 220a 0a20 2020 2064 6174 615f  s."""..    data_
-00014a30: 6469 6374 203d 207b 0a20 2020 2020 2020  dict = {.       
-00014a40: 2022 616c 676f 7269 7468 6d22 3a20 616c   "algorithm": al
-00014a50: 676f 7269 7468 6d2c 0a20 2020 2020 2020  gorithm,.       
-00014a60: 2022 6e75 6d62 6572 223a 206e 756d 6265   "number": numbe
-00014a70: 722c 0a20 2020 207d 0a20 2020 2064 6174  r,.    }.    dat
-00014a80: 6120 3d20 6a73 6f6e 2e64 756d 7073 2864  a = json.dumps(d
-00014a90: 6174 615f 6469 6374 290a 0a20 2020 2072  ata_dict)..    r
-00014aa0: 6573 756c 7420 3d20 5f70 6f73 7428 0a20  esult = _post(. 
-00014ab0: 2020 2020 2020 2022 2f74 6f70 6f6c 6f67         "/topolog
-00014ac0: 792f 6765 6e65 7261 7465 5f6d 616c 6963  y/generate_malic
-00014ad0: 696f 7573 5f64 6f6d 6169 6e73 222c 0a20  ious_domains",. 
-00014ae0: 2020 2020 2020 2064 6174 613d 6461 7461         data=data
-00014af0: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-00014b00: 733d 7b22 436f 6e74 656e 742d 5479 7065  s={"Content-Type
-00014b10: 223a 2022 6170 706c 6963 6174 696f 6e2f  ": "application/
-00014b20: 6a73 6f6e 227d 2c0a 2020 2020 290a 0a20  json"},.    ).. 
-00014b30: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-00014b40: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-00014b50: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-00014b60: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-00014b70: 4572 726f 7220 7768 696c 6520 6164 6469  Error while addi
-00014b80: 6e67 2044 4e53 2065 6e74 7269 6573 2229  ng DNS entries")
-00014b90: 0a0a 2020 2020 646f 6d61 696e 7320 3d20  ..    domains = 
-00014ba0: 7265 7375 6c74 2e6a 736f 6e28 290a 2020  result.json().  
-00014bb0: 2020 7265 7475 726e 2064 6f6d 6169 6e73    return domains
-00014bc0: 5b22 646f 6d61 696e 7322 5d0a 0a0a 6465  ["domains"]...de
-00014bd0: 6620 6372 6561 7465 5f64 6174 6173 6574  f create_dataset
-00014be0: 280a 2020 2020 6964 5f73 696d 756c 6174  (.    id_simulat
-00014bf0: 696f 6e3a 2069 6e74 2c20 646f 6e74 5f63  ion: int, dont_c
-00014c00: 6865 636b 5f6c 6f67 735f 7061 7468 3a20  heck_logs_path: 
-00014c10: 626f 6f6c 203d 2046 616c 7365 0a29 202d  bool = False.) -
-00014c20: 3e20 4f70 7469 6f6e 616c 5b75 7569 642e  > Optional[uuid.
-00014c30: 5555 4944 5d3a 0a20 2020 2022 2222 0a20  UUID]:.    """. 
-00014c40: 2020 2048 616e 646c 6573 2074 6865 2063     Handles the c
-00014c50: 7265 6174 696f 6e20 6f66 2074 6865 2064  reation of the d
-00014c60: 6174 6173 6574 2061 6674 6572 2074 6865  ataset after the
-00014c70: 2065 6e64 206f 6620 6120 7369 6d75 6c61   end of a simula
-00014c80: 7469 6f6e 0a0a 2020 2020 4d75 7374 2062  tion..    Must b
-00014c90: 6520 6361 6c6c 6564 2061 6674 6572 2061  e called after a
-00014ca0: 2053 544f 5020 6f70 6572 6174 696f 6e2c   STOP operation,
-00014cb0: 2061 6e64 206f 6e63 6520 616c 6c20 636f   and once all co
-00014cc0: 6d70 7574 6520 7365 7276 6572 730a 2020  mpute servers.  
-00014cd0: 2020 2876 6972 7463 6c69 656e 7429 2068    (virtclient) h
-00014ce0: 6176 6520 6675 6c6c 7920 7374 6f70 7065  ave fully stoppe
-00014cf0: 642e 0a0a 2020 2020 4261 7369 6361 6c6c  d...    Basicall
-00014d00: 792c 2074 6869 7320 6675 6e63 7469 6f6e  y, this function
-00014d10: 2063 6f6d 6d75 6e69 6361 7465 7320 7769   communicates wi
-00014d20: 7468 2074 6865 2074 6865 2063 6f72 6520  th the the core 
-00014d30: 4150 492c 2077 6869 6368 2069 7473 656c  API, which itsel
-00014d40: 660a 2020 2020 636f 6d6d 756e 6963 6174  f.    communicat
-00014d50: 6573 2077 6974 6820 7468 6520 7075 626c  es with the publ
-00014d60: 6973 6820 7365 7276 6572 2773 2022 6261  ish server's "ba
-00014d70: 636b 656e 6422 2041 5049 2e0a 0a20 2020  ckend" API...   
-00014d80: 203a 7061 7261 6d20 6964 5f73 696d 756c   :param id_simul
-00014d90: 6174 696f 6e3a 2074 6865 2073 696d 756c  ation: the simul
-00014da0: 6174 696f 6e20 7768 6963 6820 7761 7320  ation which was 
-00014db0: 6a75 7374 2073 746f 7070 6564 2061 6e64  just stopped and
-00014dc0: 2066 726f 6d20 7768 6963 6820 6f75 7470   from which outp
-00014dd0: 7574 2074 6865 2064 6174 6173 6574 2073  ut the dataset s
-00014de0: 686f 756c 6420 6265 2063 7265 6174 6564  hould be created
-00014df0: 0a20 2020 203a 7265 7475 726e 3a20 7468  .    :return: th
-00014e00: 6520 6e65 7720 6461 7461 7365 7420 6964  e new dataset id
-00014e10: 0a20 2020 2022 2222 0a0a 2020 2020 6c6f  .    """..    lo
-00014e20: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
-00014e30: 2020 2022 5b2b 5d20 476f 696e 6720 746f     "[+] Going to
-00014e40: 2063 7265 6174 6520 6461 7461 7365 7420   create dataset 
-00014e50: 6261 7365 6420 6f6e 2064 6174 6120 7072  based on data pr
-00014e60: 6f64 7563 6564 2062 7920 7369 6d75 6c61  oduced by simula
-00014e70: 7469 6f6e 2049 4420 277b 7d27 222e 666f  tion ID '{}'".fo
-00014e80: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00014e90: 2020 6964 5f73 696d 756c 6174 696f 6e0a    id_simulation.
-00014ea0: 2020 2020 2020 2020 290a 2020 2020 290a          ).    ).
-00014eb0: 0a20 2020 2069 6620 646f 6e74 5f63 6865  .    if dont_che
-00014ec0: 636b 5f6c 6f67 735f 7061 7468 2069 7320  ck_logs_path is 
-00014ed0: 4661 6c73 653a 0a20 2020 2020 2020 2069  False:.        i
-00014ee0: 6620 5f63 6865 636b 5f6c 6f67 735f 7061  f _check_logs_pa
-00014ef0: 7468 2869 645f 7369 6d75 6c61 7469 6f6e  th(id_simulation
-00014f00: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00014f10: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00014f20: 2320 4173 6b20 7468 6520 636f 7265 2041  # Ask the core A
-00014f30: 5049 2074 6f20 636f 6e74 6163 7420 7468  PI to contact th
-00014f40: 6520 2f62 6163 6b65 6e64 2f20 7075 626c  e /backend/ publ
-00014f50: 6973 6820 7365 7276 6572 2041 5049 0a20  ish server API. 
-00014f60: 2020 2023 2069 6e20 6f72 6465 7220 746f     # in order to
-00014f70: 2073 7461 7274 2074 6865 2064 6174 6173   start the datas
-00014f80: 6574 2063 7265 6174 696f 6e20 7072 6f63  et creation proc
-00014f90: 6573 730a 2020 2020 7265 7375 6c74 203d  ess.    result =
-00014fa0: 205f 706f 7374 2866 222f 6372 6561 7465   _post(f"/create
-00014fb0: 5f64 6174 6173 6574 2f7b 6964 5f73 696d  _dataset/{id_sim
-00014fc0: 756c 6174 696f 6e7d 2229 0a20 2020 2069  ulation}").    i
-00014fd0: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
-00014fe0: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
-00014ff0: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
-00015000: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
-00015010: 6f74 2069 6e69 7469 6174 6520 7468 6520  ot initiate the 
-00015020: 6372 6561 7469 6f6e 206f 6620 7468 6520  creation of the 
-00015030: 6461 7461 7365 7422 290a 0a20 2020 2064  dataset")..    d
-00015040: 6174 6173 6574 5f69 6420 3d20 7265 7375  ataset_id = resu
-00015050: 6c74 2e6a 736f 6e28 295b 2264 6174 6173  lt.json()["datas
-00015060: 6574 5f69 6422 5d0a 0a20 2020 206c 6f67  et_id"]..    log
-00015070: 6765 722e 696e 666f 2866 2220 205b 2b5d  ger.info(f"  [+]
-00015080: 2044 6174 6173 6574 2070 7265 2d63 7265   Dataset pre-cre
-00015090: 6174 6564 2077 6974 6820 6461 7461 7365  ated with datase
-000150a0: 7420 6964 207b 6461 7461 7365 745f 6964  t id {dataset_id
-000150b0: 7d22 290a 0a20 2020 2023 2053 7461 7274  }")..    # Start
-000150c0: 2061 6e20 6163 7469 7665 2077 6169 7469   an active waiti
-000150d0: 6e67 206c 6f6f 7020 756e 7469 6c20 7468  ng loop until th
-000150e0: 6520 6461 7461 7365 7420 6372 6561 7469  e dataset creati
-000150f0: 6f6e 2069 6620 6675 6c6c 7920 636f 6d70  on if fully comp
-00015100: 6c65 7465 0a20 2020 2023 2049 6e64 6565  lete.    # Indee
-00015110: 642c 2064 6174 6173 6574 2063 7265 6174  d, dataset creat
-00015120: 696f 6e20 696e 766f 6c76 6573 2074 6865  ion involves the
-00015130: 2064 6f77 6e6c 6f61 6420 6f66 2070 6f74   download of pot
-00015140: 656e 7469 616c 6c79 206c 6172 6765 0a20  entially large. 
-00015150: 2020 2023 2066 696c 6573 206f 7665 7273     # files overs
-00015160: 2074 6865 206e 6574 776f 726b 2c20 7768   the network, wh
-00015170: 6963 6820 6361 6e20 7461 6b65 2073 6f6d  ich can take som
-00015180: 6520 7469 6d65 210a 2020 2020 6d61 785f  e time!.    max_
-00015190: 7265 7472 6965 7320 3d20 350a 2020 2020  retries = 5.    
-000151a0: 7265 7472 6965 7320 3d20 6d61 785f 7265  retries = max_re
-000151b0: 7472 6965 730a 2020 2020 7768 696c 6520  tries.    while 
-000151c0: 5472 7565 3a0a 2020 2020 2020 2020 7469  True:.        ti
-000151d0: 6d65 2e73 6c65 6570 2832 290a 0a20 2020  me.sleep(2)..   
-000151e0: 2020 2020 2072 6573 756c 7420 3d20 5f67       result = _g
-000151f0: 6574 2866 222f 6372 6561 7465 5f64 6174  et(f"/create_dat
-00015200: 6173 6574 2f73 7461 7475 732f 7b64 6174  aset/status/{dat
-00015210: 6173 6574 5f69 647d 2229 0a20 2020 2020  aset_id}").     
-00015220: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-00015230: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-00015240: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015250: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00015260: 2020 7265 7375 6c74 2e68 6561 6465 7273    result.headers
-00015270: 2e67 6574 2822 636f 6e74 656e 742d 7479  .get("content-ty
-00015280: 7065 2229 203d 3d20 2261 7070 6c69 6361  pe") == "applica
-00015290: 7469 6f6e 2f6a 736f 6e22 0a20 2020 2020  tion/json".     
-000152a0: 2020 2020 2020 2020 2020 2061 6e64 2022             and "
-000152b0: 6d65 7373 6167 6522 2069 6e20 7265 7375  message" in resu
-000152c0: 6c74 2e6a 736f 6e28 290a 2020 2020 2020  lt.json().      
-000152d0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-000152e0: 2020 2020 2020 2020 2065 7272 6f72 5f6d           error_m
-000152f0: 7367 203d 2072 6573 756c 742e 6a73 6f6e  sg = result.json
-00015300: 2829 5b22 6d65 7373 6167 6522 5d0a 2020  ()["message"].  
-00015310: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00015320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015330: 6572 726f 725f 6d73 6720 3d20 7265 7375  error_msg = resu
-00015340: 6c74 2e74 6578 740a 0a20 2020 2020 2020  lt.text..       
-00015350: 2020 2020 2023 2052 6574 7279 2074 6f20       # Retry to 
-00015360: 6765 7420 7468 6520 7374 6174 7573 2061  get the status a
-00015370: 2063 6f75 706c 6520 6f66 2074 696d 6573   couple of times
-00015380: 2062 6566 6f72 6520 7173 656e 6469 6e67   before qsending
-00015390: 2062 6163 6b20 616e 2065 7272 6f72 0a20   back an error. 
-000153a0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-000153b0: 7472 6965 7320 3d3d 2030 3a0a 2020 2020  tries == 0:.    
-000153c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000153d0: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
-000153e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153f0: 2022 4572 726f 7220 6475 7269 6e67 2063   "Error during c
-00015400: 7265 6174 696f 6e20 6f66 2064 6174 6173  reation of datas
-00015410: 6574 207b 7d3a 2063 6f75 6c64 206e 6f74  et {}: could not
-00015420: 2067 6574 2073 7461 7475 7320 6f66 2074   get status of t
-00015430: 6865 2064 6174 6173 6574 2063 7265 6174  he dataset creat
-00015440: 696f 6e20 6166 7465 7220 7b7d 2074 7269  ion after {} tri
-00015450: 6573 2e20 436f 7265 2041 5049 2048 5454  es. Core API HTT
-00015460: 5020 7374 6174 7573 3a20 7b7d 2e20 5265  P status: {}. Re
-00015470: 7370 6f6e 7365 3a20 7b7d 2022 2e66 6f72  sponse: {} ".for
-00015480: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00015490: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-000154a0: 6173 6574 5f69 642c 206d 6178 5f72 6574  aset_id, max_ret
-000154b0: 7269 6573 2c20 7265 7375 6c74 2e73 7461  ries, result.sta
-000154c0: 7475 735f 636f 6465 2c20 6572 726f 725f  tus_code, error_
-000154d0: 6d73 670a 2020 2020 2020 2020 2020 2020  msg.            
-000154e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000154f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00015500: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00015510: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00015520: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
-00015530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015540: 2020 2220 205b 2b5d 2043 6f75 6c64 206e    "  [+] Could n
-00015550: 6f74 2067 6574 2073 7461 7475 7320 6f66  ot get status of
-00015560: 2064 6174 6173 6574 2063 7265 6174 696f   dataset creatio
-00015570: 6e20 2852 6574 7269 6573 206c 6566 743a  n (Retries left:
-00015580: 207b 7d2e 2043 6f72 6520 4150 4920 4854   {}. Core API HT
-00015590: 5450 2073 7461 7475 733a 207b 7d2e 2052  TP status: {}. R
-000155a0: 6573 706f 6e73 653a 207b 7d29 222e 666f  esponse: {})".fo
-000155b0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-000155c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000155d0: 7472 6965 732c 2072 6573 756c 742e 7374  tries, result.st
-000155e0: 6174 7573 5f63 6f64 652c 2065 7272 6f72  atus_code, error
-000155f0: 5f6d 7367 0a20 2020 2020 2020 2020 2020  _msg.           
-00015600: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00015610: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00015620: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00015630: 7269 6573 202d 3d20 310a 2020 2020 2020  ries -= 1.      
-00015640: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00015650: 2020 2020 2320 5265 7365 7420 7468 6520      # Reset the 
-00015660: 6e75 6d62 6572 206f 6620 7265 7472 6965  number of retrie
-00015670: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
-00015680: 7472 6965 7320 3d20 6d61 785f 7265 7472  tries = max_retr
-00015690: 6965 730a 0a20 2020 2020 2020 2020 2020  ies..           
-000156a0: 2023 2047 6574 2074 6865 2073 7461 7475   # Get the statu
-000156b0: 7320 616e 6420 6d65 7373 6167 650a 2020  s and message.  
-000156c0: 2020 2020 2020 2020 2020 6461 7461 7365            datase
-000156d0: 745f 6372 6561 7469 6f6e 5f73 7461 7475  t_creation_statu
-000156e0: 7320 3d20 7265 7375 6c74 2e6a 736f 6e28  s = result.json(
-000156f0: 295b 2273 7461 7475 7322 5d0a 2020 2020  )["status"].    
-00015700: 2020 2020 2020 2020 6461 7461 7365 745f          dataset_
-00015710: 6372 6561 7469 6f6e 5f6d 6573 7361 6765  creation_message
-00015720: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
-00015730: 5b22 6d65 7373 6167 6522 5d0a 0a20 2020  ["message"]..   
-00015740: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00015750: 696e 666f 280a 2020 2020 2020 2020 2020  info(.          
-00015760: 2020 2020 2020 2220 205b 2b5d 2044 6174        "  [+] Dat
-00015770: 6173 6574 2063 7265 6174 696f 6e20 696e  aset creation in
-00015780: 2070 726f 6772 6573 7320 2853 7461 7475   progress (Statu
-00015790: 733a 207b 7d29 222e 666f 726d 6174 280a  s: {})".format(.
-000157a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157b0: 2020 2020 6461 7461 7365 745f 6372 6561      dataset_crea
-000157c0: 7469 6f6e 5f73 7461 7475 730a 2020 2020  tion_status.    
-000157d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000157e0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000157f0: 2020 2020 2020 2020 2069 6620 6461 7461           if data
-00015800: 7365 745f 6372 6561 7469 6f6e 5f73 7461  set_creation_sta
-00015810: 7475 7320 3d3d 2022 4649 4e49 5348 4544  tus == "FINISHED
-00015820: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00015830: 2020 2023 2041 6c6c 2077 656e 7420 7765     # All went we
-00015840: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
-00015850: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00015860: 2020 2020 2065 6c69 6620 6461 7461 7365       elif datase
-00015870: 745f 6372 6561 7469 6f6e 5f73 7461 7475  t_creation_statu
-00015880: 7320 3d3d 2022 4649 4e49 5348 4544 5f45  s == "FINISHED_E
-00015890: 5252 4f52 223a 0a20 2020 2020 2020 2020  RROR":.         
-000158a0: 2020 2020 2020 2023 2054 6865 2064 6174         # The dat
-000158b0: 6173 6574 2063 7265 6174 696f 6e20 656e  aset creation en
-000158c0: 636f 756e 7465 7265 6420 6572 726f 7273  countered errors
-000158d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000158e0: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-000158f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00015900: 2020 2020 2020 2245 7272 6f72 2064 7572        "Error dur
-00015910: 696e 6720 6372 6561 7469 6f6e 206f 6620  ing creation of 
-00015920: 6461 7461 7365 7420 7b7d 3a20 6461 7461  dataset {}: data
-00015930: 7365 7420 6372 6561 7469 6f6e 2065 6e64  set creation end
-00015940: 6564 2077 6974 6820 6572 726f 7273 2028  ed with errors (
-00015950: 277b 7d27 292e 222e 666f 726d 6174 280a  '{}').".format(.
-00015960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015970: 2020 2020 2020 2020 6461 7461 7365 745f          dataset_
-00015980: 6964 2c20 6461 7461 7365 745f 6372 6561  id, dataset_crea
-00015990: 7469 6f6e 5f6d 6573 7361 6765 0a20 2020  tion_message.   
-000159a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159b0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000159c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000159d0: 2023 204f 7468 6572 7769 7365 2c20 6461   # Otherwise, da
-000159e0: 7461 7365 7420 6372 6561 7469 6f6e 2069  taset creation i
-000159f0: 7320 6e6f 7420 6669 6e69 7368 6564 2c20  s not finished, 
-00015a00: 6a75 7374 206c 6f6f 700a 0a20 2020 206c  just loop..    l
-00015a10: 6f67 6765 722e 696e 666f 2822 5b2b 5d20  ogger.info("[+] 
-00015a20: 4461 7461 7365 7420 6372 6561 7469 6f6e  Dataset creation
-00015a30: 2077 6173 2063 6f72 7265 6374 6c79 2065   was correctly e
-00015a40: 7865 6375 7465 6422 290a 0a20 2020 2023  xecuted")..    #
-00015a50: 2053 6574 2074 6865 2073 696d 756c 6174   Set the simulat
-00015a60: 696f 6e20 7374 6174 7573 2074 6f20 5245  ion status to RE
-00015a70: 4144 590a 2020 2020 7570 6461 7465 5f73  ADY.    update_s
-00015a80: 696d 756c 6174 696f 6e28 6964 5f73 696d  imulation(id_sim
-00015a90: 756c 6174 696f 6e2c 207b 2273 7461 7475  ulation, {"statu
-00015aa0: 7322 3a20 2252 4541 4459 227d 290a 0a20  s": "READY"}).. 
-00015ab0: 2020 2073 696d 756c 6174 696f 6e20 3d20     simulation = 
-00015ac0: 6665 7463 685f 7369 6d75 6c61 7469 6f6e  fetch_simulation
-00015ad0: 2869 645f 7369 6d75 6c61 7469 6f6e 290a  (id_simulation).
-00015ae0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00015af0: 225b 2b5d 2043 7572 7265 6e74 2073 696d  "[+] Current sim
-00015b00: 756c 6174 696f 6e20 7374 6174 7573 3a20  ulation status: 
-00015b10: 277b 7d27 222e 666f 726d 6174 2873 696d  '{}'".format(sim
-00015b20: 756c 6174 696f 6e5b 2273 7461 7475 7322  ulation["status"
-00015b30: 5d29 290a 0a20 2020 2072 6574 7572 6e20  ]))..    return 
-00015b40: 7575 6964 2e55 5549 4428 6461 7461 7365  uuid.UUID(datase
-00015b50: 745f 6964 290a 0a0a 6465 6620 5f63 6865  t_id)...def _che
-00015b60: 636b 5f6c 6f67 735f 7061 7468 2869 645f  ck_logs_path(id_
-00015b70: 7369 6d75 6c61 7469 6f6e 3a20 696e 7429  simulation: int)
-00015b80: 202d 3e20 626f 6f6c 3a0a 2020 2020 2222   -> bool:.    ""
-00015b90: 220a 2020 2020 5265 7475 726e 2074 7275  ".    Return tru
-00015ba0: 6520 6966 2061 2062 6164 2070 6174 6820  e if a bad path 
-00015bb0: 7761 7320 7365 7420 666f 7220 7468 6520  was set for the 
-00015bc0: 7273 7973 6c6f 6727 7320 6c6f 6720 766f  rsyslog's log vo
-00015bd0: 6c75 6d65 0a0a 2020 2020 446f 2061 2073  lume..    Do a s
-00015be0: 6d61 6c6c 2063 6865 636b 2066 6f72 2074  mall check for t
-00015bf0: 6865 2073 616b 6520 6f66 2068 656c 7069  he sake of helpi
-00015c00: 6e67 2074 6865 2075 7365 7220 616e 6420  ng the user and 
-00015c10: 6769 7669 6e67 2062 6574 7465 720a 2020  giving better.  
-00015c20: 2020 7573 6572 2065 7870 6572 6965 6e63    user experienc
-00015c30: 653a 2063 6865 636b 2069 6620 7468 6520  e: check if the 
-00015c40: 7273 7973 6c6f 6720 646f 636b 6572 2028  rsyslog docker (
-00015c50: 7768 6963 6820 636f 6c6c 6563 7473 206c  which collects l
-00015c60: 6f67 7329 0a20 2020 2069 7320 696e 7369  ogs).    is insi
-00015c70: 6465 2074 6865 2074 6f70 6f6c 6f67 792c  de the topology,
-00015c80: 2061 6e64 2069 6620 736f 2c20 6368 6563   and if so, chec
-00015c90: 6b20 7468 6520 2268 6f73 745f 7061 7468  k the "host_path
-00015ca0: 2220 666f 7220 6c6f 6773 0a20 2020 2028  " for logs.    (
-00015cb0: 6120 7370 6563 6966 6963 2070 6174 6820  a specific path 
-00015cc0: 6973 2065 7870 6563 7465 642c 2061 6e64  is expected, and
-00015cd0: 2069 7320 6861 7264 636f 6465 6420 696e   is hardcoded in
-00015ce0: 2069 745f 7369 6d75 6c61 7469 6f6e 290a   it_simulation).
-00015cf0: 2020 2020 2222 220a 2020 2020 2320 544f      """.    # TO
-00015d00: 444f 2843 5244 293a 2074 6869 7320 6368  DO(CRD): this ch
-00015d10: 6563 6b20 7769 6c6c 2061 6c77 6179 7320  eck will always 
-00015d20: 6661 696c 2077 6865 6e20 6372 5f61 7069  fail when cr_api
-00015d30: 5f63 6c69 656e 742c 2074 6865 0a20 2020  _client, the.   
-00015d40: 2023 2069 745f 7369 6d75 6c61 7469 6f6e   # it_simulation
-00015d50: 2064 6f63 6b65 722c 2061 6e64 2074 6865   docker, and the
-00015d60: 2072 7379 736c 6f67 2064 6f63 6b65 7220   rsyslog docker 
-00015d70: 6172 6520 6e6f 7420 6f6e 2074 6865 2073  are not on the s
-00015d80: 616d 6520 6d61 6368 696e 650a 0a20 2020  ame machine..   
-00015d90: 2074 6f70 6f6c 6f67 7920 3d20 5941 4d4c   topology = YAML
-00015da0: 2829 2e6c 6f61 6428 6665 7463 685f 7369  ().load(fetch_si
-00015db0: 6d75 6c61 7469 6f6e 5f74 6f70 6f6c 6f67  mulation_topolog
-00015dc0: 795f 7961 6d6c 2869 645f 7369 6d75 6c61  y_yaml(id_simula
-00015dd0: 7469 6f6e 2929 0a0a 2020 2020 2320 5468  tion))..    # Th
-00015de0: 6520 7061 7468 206f 6620 7468 6520 6c6f  e path of the lo
-00015df0: 6773 2c20 6f6e 2074 6865 2063 6f6d 7075  gs, on the compu
-00015e00: 7465 2073 6572 7665 7220 6669 6c65 2073  te server file s
-00015e10: 7973 7465 6d20 7368 6f75 6c64 2041 4c57  ystem should ALW
-00015e20: 4159 5320 6265 2061 7320 666f 6c6c 6f77  AYS be as follow
-00015e30: 730a 2020 2020 7273 7973 6c6f 675f 646f  s.    rsyslog_do
-00015e40: 636b 6572 5f70 7265 7365 6e74 3a20 626f  cker_present: bo
-00015e50: 6f6c 203d 2046 616c 7365 0a20 2020 2070  ol = False.    p
-00015e60: 6f74 656e 7469 616c 5f6c 6f67 735f 6162  otential_logs_ab
-00015e70: 736f 6c75 7465 5f70 6174 683a 204c 6973  solute_path: Lis
-00015e80: 745b 5061 7468 5d20 3d20 5b5d 0a20 2020  t[Path] = [].   
-00015e90: 2066 6f72 206e 6f64 6520 696e 2074 6f70   for node in top
-00015ea0: 6f6c 6f67 795b 226e 6f64 6573 225d 3a0a  ology["nodes"]:.
-00015eb0: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-00015ec0: 2020 2020 2020 2020 206e 6f64 655b 2274           node["t
-00015ed0: 7970 6522 5d20 3d3d 2022 646f 636b 6572  ype"] == "docker
-00015ee0: 220a 2020 2020 2020 2020 2020 2020 616e  ".            an
-00015ef0: 6420 2272 7379 736c 6f67 2220 696e 206e  d "rsyslog" in n
-00015f00: 6f64 655b 2262 6173 655f 696d 6167 6522  ode["base_image"
-00015f10: 5d0a 2020 2020 2020 2020 2020 2020 616e  ].            an
-00015f20: 6420 2276 6f6c 756d 6573 2220 696e 206e  d "volumes" in n
-00015f30: 6f64 650a 2020 2020 2020 2020 293a 0a20  ode.        ):. 
-00015f40: 2020 2020 2020 2020 2020 2072 7379 736c             rsysl
-00015f50: 6f67 5f64 6f63 6b65 725f 7072 6573 656e  og_docker_presen
-00015f60: 7420 3d20 5472 7565 0a20 2020 2020 2020  t = True.       
-00015f70: 2020 2020 2066 6f72 2076 6f6c 756d 6520       for volume 
-00015f80: 696e 206e 6f64 655b 2276 6f6c 756d 6573  in node["volumes
-00015f90: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-00015fa0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-00015fb0: 2020 2020 2020 2020 2020 2020 2022 686f               "ho
-00015fc0: 7374 5f70 6174 6822 2069 6e20 766f 6c75  st_path" in volu
-00015fd0: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
-00015fe0: 2020 2020 2020 2061 6e64 2022 7772 6974         and "writ
-00015ff0: 6162 6c65 2220 696e 2076 6f6c 756d 650a  able" in volume.
-00016000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016010: 2020 2020 616e 6420 766f 6c75 6d65 5b22      and volume["
-00016020: 7772 6974 6162 6c65 225d 0a20 2020 2020  writable"].     
-00016030: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00016040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016050: 2020 706f 7465 6e74 6961 6c5f 6c6f 6773    potential_logs
-00016060: 5f61 6273 6f6c 7574 655f 7061 7468 2e61  _absolute_path.a
-00016070: 7070 656e 6428 5061 7468 2876 6f6c 756d  ppend(Path(volum
-00016080: 655b 2268 6f73 745f 7061 7468 225d 2929  e["host_path"]))
-00016090: 0a0a 2020 2020 2320 4966 206e 6f20 7273  ..    # If no rs
-000160a0: 7973 6c6f 6720 646f 636b 6572 2069 7320  yslog docker is 
-000160b0: 7072 6573 656e 742c 206a 7375 7420 6973  present, jsut is
-000160c0: 7375 6520 6120 6e6f 6e2d 626c 6f63 6b69  sue a non-blocki
-000160d0: 6e67 2077 6172 6e69 6e67 0a20 2020 2069  ng warning.    i
-000160e0: 6620 6e6f 7420 7273 7973 6c6f 675f 646f  f not rsyslog_do
-000160f0: 636b 6572 5f70 7265 7365 6e74 3a0a 2020  cker_present:.  
-00016100: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
-00016110: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
-00016120: 2020 2220 205b 2b5d 2054 6865 2063 6f6c    "  [+] The col
-00016130: 6c65 6374 696f 6e20 6f66 206c 6f67 7320  lection of logs 
-00016140: 7761 7320 6e6f 7420 6163 7469 7661 7465  was not activate
-00016150: 6420 666f 7220 7468 6520 7369 6d75 6c61  d for the simula
-00016160: 7469 6f6e 2028 7468 6520 7273 7973 6c6f  tion (the rsyslo
-00016170: 6720 646f 636b 6572 2069 7320 6e6f 7420  g docker is not 
-00016180: 7072 6573 656e 7420 696e 2074 6865 2074  present in the t
-00016190: 6f70 6f6c 6f67 7929 2e20 4e6f 206c 6f67  opology). No log
-000161a0: 2077 696c 6c20 6265 2069 6e63 6c75 6465   will be include
-000161b0: 6420 696e 2074 6865 2064 6174 6173 6574  d in the dataset
-000161c0: 2e22 0a20 2020 2020 2020 2029 0a20 2020  .".        ).   
-000161d0: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
-000161e0: 726f 6e67 5f68 6f73 745f 7061 7468 203d  rong_host_path =
-000161f0: 2054 7275 650a 2020 2020 2020 2020 666f   True.        fo
-00016200: 7220 7020 696e 2070 6f74 656e 7469 616c  r p in potential
-00016210: 5f6c 6f67 735f 6162 736f 6c75 7465 5f70  _logs_absolute_p
-00016220: 6174 683a 0a20 2020 2020 2020 2020 2020  ath:.           
-00016230: 2069 6620 6e6f 7420 702e 6973 5f61 6273   if not p.is_abs
-00016240: 6f6c 7574 6528 2920 616e 6420 7020 3d3d  olute() and p ==
-00016250: 2050 6174 6828 2273 6861 7265 645f 7265   Path("shared_re
-00016260: 736f 7572 6365 732f 7273 7973 6c6f 672f  sources/rsyslog/
-00016270: 6c6f 6773 2229 3a0a 2020 2020 2020 2020  logs"):.        
-00016280: 2020 2020 2020 2020 7772 6f6e 675f 686f          wrong_ho
-00016290: 7374 5f70 6174 6820 3d20 4661 6c73 650a  st_path = False.
-000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162b0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-000162c0: 2020 656c 6966 2070 2e69 735f 6162 736f    elif p.is_abso
-000162d0: 6c75 7465 2829 2061 6e64 2050 6174 6828  lute() and Path(
-000162e0: 7374 7228 7029 5b31 3a5d 2920 3d3d 2050  str(p)[1:]) == P
-000162f0: 6174 6828 0a20 2020 2020 2020 2020 2020  ath(.           
-00016300: 2020 2020 2022 7368 6172 6564 5f72 6573       "shared_res
-00016310: 6f75 7263 6573 2f72 7379 736c 6f67 2f6c  ources/rsyslog/l
-00016320: 6f67 7322 0a20 2020 2020 2020 2020 2020  ogs".           
-00016330: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00016340: 2020 2020 7772 6f6e 675f 686f 7374 5f70      wrong_host_p
-00016350: 6174 6820 3d20 4661 6c73 650a 2020 2020  ath = False.    
-00016360: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00016370: 6b0a 2020 2020 2020 2020 2020 2020 656c  k.            el
-00016380: 6966 2070 2e69 735f 6162 736f 6c75 7465  if p.is_absolute
-00016390: 2829 2061 6e64 2070 203d 3d20 5061 7468  () and p == Path
-000163a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000163b0: 2020 222f 6379 6265 722d 7261 6e67 652d    "/cyber-range-
-000163c0: 6361 7461 6c6f 672f 7369 6d75 6c61 7469  catalog/simulati
-000163d0: 6f6e 735f 7265 736f 7572 6365 732f 312f  ons_resources/1/
-000163e0: 7368 6172 6564 5f72 6573 6f75 7263 6573  shared_resources
-000163f0: 2f72 7379 736c 6f67 2f6c 6f67 7322 0a20  /rsyslog/logs". 
-00016400: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00016410: 2020 2020 2020 2020 2020 2020 2020 7772                wr
-00016420: 6f6e 675f 686f 7374 5f70 6174 6820 3d20  ong_host_path = 
-00016430: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00016440: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
-00016450: 2020 2020 2069 6620 7772 6f6e 675f 686f       if wrong_ho
-00016460: 7374 5f70 6174 683a 0a20 2020 2020 2020  st_path:.       
-00016470: 2020 2020 206c 6f67 6765 722e 6572 726f       logger.erro
-00016480: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00016490: 2020 2022 2020 5b2b 5d20 4974 2073 6565     "  [+] It see
-000164a0: 6d73 2074 6861 7420 7468 6520 7369 6d75  ms that the simu
-000164b0: 6c61 7469 6f6e 2069 6e63 6c75 6465 7320  lation includes 
-000164c0: 7468 6520 2772 7379 736c 6f67 2720 646f  the 'rsyslog' do
-000164d0: 636b 6572 2074 6861 7420 636f 6c6c 6563  cker that collec
-000164e0: 7473 2074 6865 206c 6f67 732c 2062 7574  ts the logs, but
-000164f0: 2064 6f65 7320 6e6f 7420 7370 6563 6966   does not specif
-00016500: 7920 7468 6520 6170 7072 6f70 7269 6174  y the appropriat
-00016510: 6520 686f 7374 5f70 6174 6820 666f 7220  e host_path for 
-00016520: 7468 6520 6c6f 6773 2e20 4974 2069 7320  the logs. It is 
-00016530: 6578 7065 6374 6564 2074 6861 7420 7468  expected that th
-00016540: 6520 7273 7973 6c6f 6720 646f 636b 6572  e rsyslog docker
-00016550: 206e 6f64 6520 7370 6563 6966 6965 7320   node specifies 
-00016560: 6120 2877 7269 7461 626c 6529 2076 6f6c  a (writable) vol
-00016570: 756d 6520 7769 7468 2061 2068 6f73 745f  ume with a host_
-00016580: 7061 7468 2065 7175 616c 2074 6f20 272f  path equal to '/
-00016590: 7368 6172 6564 5f72 6573 6f75 7263 6573  shared_resources
-000165a0: 2f72 7379 736c 6f67 2f6c 6f67 7327 2e20  /rsyslog/logs'. 
-000165b0: 4361 6e64 6964 6174 6573 2061 7265 2027  Candidates are '
-000165c0: 7b7d 2720 696e 7374 6561 642e 222e 666f  {}' instead.".fo
-000165d0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-000165e0: 2020 2020 2020 2020 2020 5b73 7472 2870            [str(p
-000165f0: 2920 666f 7220 7020 696e 2070 6f74 656e  ) for p in poten
-00016600: 7469 616c 5f6c 6f67 735f 6162 736f 6c75  tial_logs_absolu
-00016610: 7465 5f70 6174 685d 2c0a 2020 2020 2020  te_path],.      
-00016620: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00016630: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00016640: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
-00016650: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00016660: 2020 2020 2220 5b2b 5d20 4461 7461 7365      " [+] Datase
-00016670: 7420 6372 6561 7469 6f6e 2061 626f 7274  t creation abort
-00016680: 6564 2e20 596f 7520 6d61 7920 7769 7368  ed. You may wish
-00016690: 2074 6f20 6d6f 7665 2074 6865 206c 6f67   to move the log
-000166a0: 2066 696c 6573 2074 6f20 7468 6520 6170   files to the ap
-000166b0: 7072 6f70 7269 6174 6520 666f 6c64 6572  propriate folder
-000166c0: 206f 6e20 7468 6520 636f 6d70 7574 6520   on the compute 
-000166d0: 7365 7276 6572 2873 292c 2061 6e64 2074  server(s), and t
-000166e0: 6865 6e20 7265 7472 792e 2041 6c74 6572  hen retry. Alter
-000166f0: 6e61 7469 7665 6c79 2c20 796f 7520 6361  natively, you ca
-00016700: 6e20 6279 7061 7373 2074 6869 7320 6368  n bypass this ch
-00016710: 6563 6b20 7769 7468 2074 6865 2064 6f6e  eck with the don
-00016720: 745f 6368 6563 6b5f 6c6f 675f 7061 7468  t_check_log_path
-00016730: 206f 7074 696f 6e2e 220a 2020 2020 2020   option.".      
-00016740: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00016750: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00016760: 0a0a 6465 6620 7374 6f70 5f64 6174 6173  ..def stop_datas
-00016770: 6574 5f63 7265 6174 696f 6e28 6461 7461  et_creation(data
-00016780: 7365 745f 6964 3a20 7575 6964 2e55 5549  set_id: uuid.UUI
-00016790: 4429 202d 3e20 416e 793a 0a20 2020 2022  D) -> Any:.    "
-000167a0: 2222 0a20 2020 2053 746f 7073 2f61 626f  "".    Stops/abo
-000167b0: 7274 7320 7468 6520 6372 6561 7469 6f6e  rts the creation
-000167c0: 206f 6620 6120 6461 7461 7365 7420 7468   of a dataset th
-000167d0: 6174 2069 7320 696e 2074 6865 2070 726f  at is in the pro
-000167e0: 6365 7373 206f 6620 6265 696e 6720 6372  cess of being cr
-000167f0: 6561 7465 642e 0a0a 2020 2020 5468 6973  eated...    This
-00016800: 2066 756e 6374 696f 6e20 7368 6f75 6c64   function should
-00016810: 2062 6520 7573 6564 2c20 666f 7220 696e   be used, for in
-00016820: 7374 616e 6365 2c20 6966 2061 2064 6174  stance, if a dat
-00016830: 6173 6574 2063 7265 6174 696f 6e20 6861  aset creation ha
-00016840: 7320 6265 656e 0a20 2020 2061 7574 6f6d  s been.    autom
-00016850: 6174 6963 616c 6c79 2073 7461 7274 6564  atically started
-00016860: 2061 6c74 686f 7567 6820 7468 6520 7573   although the us
-00016870: 6572 2064 6f65 7320 6e6f 7420 7761 6e74  er does not want
-00016880: 2061 2064 6174 6173 6574 2c20 616e 6420   a dataset, and 
-00016890: 7468 6520 6461 7461 7365 740a 2020 2020  the dataset.    
-000168a0: 6372 6561 7469 6f6e 2070 726f 6365 7373  creation process
-000168b0: 2069 7320 7461 6b69 6e67 2074 6f6f 206d   is taking too m
-000168c0: 7563 6820 7469 6d65 2e0a 0a20 2020 2057  uch time...    W
-000168d0: 4152 4e49 4e47 3a20 6166 7465 7220 7374  ARNING: after st
-000168e0: 6f70 7069 6e67 2074 6865 2064 6174 6173  opping the datas
-000168f0: 6574 2063 7265 6174 696f 6e2c 2069 7420  et creation, it 
-00016900: 6973 2061 6476 6973 6564 2074 6f20 6465  is advised to de
-00016910: 6c65 7465 206f 7220 6174 206c 6561 7374  lete or at least
-00016920: 0a20 2020 2072 6570 6169 7220 7468 6520  .    repair the 
-00016930: 6461 7461 7365 742e 0a0a 2020 2020 3a70  dataset...    :p
-00016940: 6172 616d 2064 6174 6173 6574 5f69 643a  aram dataset_id:
-00016950: 2074 6865 2064 6174 6173 6574 2077 6869   the dataset whi
-00016960: 6368 2069 7320 696e 2074 6865 2070 726f  ch is in the pro
-00016970: 6365 7373 206f 6620 6265 696e 6720 6372  cess of being cr
-00016980: 6561 7465 6420 616e 6420 7468 6174 206d  eated and that m
-00016990: 7573 7420 6265 2061 626f 7274 6564 0a20  ust be aborted. 
-000169a0: 2020 203a 7265 7475 726e 3a20 7265 7475     :return: retu
-000169b0: 726e 2074 6865 206a 736f 6e20 626f 6479  rn the json body
-000169c0: 206f 6620 7468 6520 636f 7265 2041 5049   of the core API
-000169d0: 2072 6573 706f 6e73 650a 2020 2020 2222   response.    ""
-000169e0: 220a 2020 2020 2320 5369 6d70 6c79 2063  ".    # Simply c
-000169f0: 616c 6c73 2074 6865 2063 6f72 6520 4150  alls the core AP
-00016a00: 4920 7768 6963 6820 6974 7365 6c66 2061  I which itself a
-00016a10: 736b 7320 7468 6520 7075 626c 6973 680a  sks the publish.
-00016a20: 2020 2020 2320 7365 7276 6572 2028 6261      # server (ba
-00016a30: 636b 656e 6429 2074 6f20 7374 6f70 206f  ckend) to stop o
-00016a40: 6620 7468 6520 6461 7461 7365 7420 6372  f the dataset cr
-00016a50: 6561 7469 6f6e 2070 726f 6365 7373 2e0a  eation process..
-00016a60: 0a20 2020 2072 6573 756c 7420 3d20 5f70  .    result = _p
-00016a70: 7574 2822 2f63 7265 6174 655f 6461 7461  ut("/create_data
-00016a80: 7365 742f 7374 6f70 2f7b 7d22 2e66 6f72  set/stop/{}".for
-00016a90: 6d61 7428 7374 7228 6461 7461 7365 745f  mat(str(dataset_
-00016aa0: 6964 2929 290a 0a20 2020 2069 6620 7265  id)))..    if re
-00016ab0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-00016ac0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
-00016ad0: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
-00016ae0: 6573 756c 742c 2022 4361 6e6e 6f74 2073  esult, "Cannot s
-00016af0: 746f 7020 6461 7461 7365 7420 6372 6561  top dataset crea
-00016b00: 7469 6f6e 2074 6872 6f75 6768 2063 6f72  tion through cor
-00016b10: 6520 4150 4922 290a 0a20 2020 2072 6574  e API")..    ret
-00016b20: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
-00016b30: 290a 0a0a 6465 6620 6665 7463 685f 636f  )...def fetch_co
-00016b40: 6d70 7574 655f 7365 7276 6572 2863 6f6d  mpute_server(com
-00016b50: 7075 7465 5f73 6572 7665 725f 6964 3a20  pute_server_id: 
-00016b60: 696e 7429 202d 3e20 416e 793a 0a20 2020  int) -> Any:.   
-00016b70: 2022 2222 5265 7475 726e 2061 2063 6f6d   """Return a com
-00016b80: 7075 7465 2073 6572 7665 7220 6769 7665  pute server give
-00016b90: 6e20 6974 7320 4944 2222 220a 2020 2020  n its ID""".    
-00016ba0: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
-00016bb0: 2f63 6f6d 7075 7465 5f73 6572 7665 7273  /compute_servers
-00016bc0: 2f7b 636f 6d70 7574 655f 7365 7276 6572  /{compute_server
-00016bd0: 5f69 647d 2229 0a0a 2020 2020 6966 2072  _id}")..    if r
-00016be0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-00016bf0: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-00016c00: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-00016c10: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-00016c20: 7265 7472 6965 7665 206e 6f64 6520 6672  retrieve node fr
-00016c30: 6f6d 2049 5420 5369 6d75 6c61 7469 6f6e  om IT Simulation
-00016c40: 2041 5049 2229 0a0a 2020 2020 7265 7475   API")..    retu
-00016c50: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
-00016c60: 0a0a 0a64 6566 2066 6574 6368 5f63 6f6d  ...def fetch_com
-00016c70: 7075 7465 5f73 6572 7665 725f 6279 5f6e  pute_server_by_n
-00016c80: 6f64 655f 6964 286e 6f64 655f 6964 3a20  ode_id(node_id: 
-00016c90: 696e 7429 202d 3e20 416e 793a 0a20 2020  int) -> Any:.   
-00016ca0: 2022 2222 5265 7475 726e 2061 2063 6f6d   """Return a com
-00016cb0: 7075 7465 2073 6572 7665 7220 7768 6572  pute server wher
-00016cc0: 6520 6120 6e6f 6465 2049 4420 6973 2072  e a node ID is r
-00016cd0: 756e 6e69 6e67 2222 220a 2020 2020 7265  unning""".    re
-00016ce0: 7375 6c74 203d 205f 6765 7428 6622 2f63  sult = _get(f"/c
-00016cf0: 6f6d 7075 7465 5f73 6572 7665 7273 2f6e  ompute_servers/n
-00016d00: 6f64 652f 7b6e 6f64 655f 6964 7d22 290a  ode/{node_id}").
-00016d10: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
-00016d20: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-00016d30: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
-00016d40: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
-00016d50: 2022 4361 6e6e 6f74 2072 6574 7269 6576   "Cannot retriev
-00016d60: 6520 6e6f 6465 2066 726f 6d20 4954 2053  e node from IT S
-00016d70: 696d 756c 6174 696f 6e20 4150 4922 290a  imulation API").
-00016d80: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
-00016d90: 6c74 2e6a 736f 6e28 290a 0a0a 6465 6620  lt.json()...def 
-00016da0: 6665 7463 685f 636f 6d70 7574 655f 7365  fetch_compute_se
-00016db0: 7276 6572 7328 2920 2d3e 204c 6973 745b  rvers() -> List[
-00016dc0: 4469 6374 5b73 7472 2c20 416e 795d 5d3a  Dict[str, Any]]:
-00016dd0: 0a20 2020 2022 2222 0a20 2020 2052 6574  .    """.    Ret
-00016de0: 7572 6e20 7468 6520 6c69 7374 206f 6620  urn the list of 
-00016df0: 636f 6d70 7574 6520 7365 7276 6572 7320  compute servers 
-00016e00: 6173 206b 6e6f 776e 2069 6e20 6461 7461  as known in data
-00016e10: 6261 7365 0a20 2020 2022 2222 0a20 2020  base.    """.   
-00016e20: 2072 6573 756c 7420 3d20 5f67 6574 2822   result = _get("
-00016e30: 2f63 6f6d 7075 7465 5f73 6572 7665 7273  /compute_servers
-00016e40: 2f22 290a 0a20 2020 2069 6620 7265 7375  /")..    if resu
-00016e50: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-00016e60: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-00016e70: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-00016e80: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
-00016e90: 7269 6576 6520 636f 6d70 7574 6520 7365  rieve compute se
-00016ea0: 7276 6572 7320 6672 6f6d 2049 5420 5369  rvers from IT Si
-00016eb0: 6d75 6c61 7469 6f6e 2041 5049 2229 0a0a  mulation API")..
-00016ec0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00016ed0: 742e 6a73 6f6e 2829 0a0a 0a64 6566 2064  t.json()...def d
-00016ee0: 656c 6574 655f 636f 6d70 7574 655f 7365  elete_compute_se
-00016ef0: 7276 6572 2863 6f6d 7075 7465 5f73 6572  rver(compute_ser
-00016f00: 7665 725f 6964 3a20 696e 7429 202d 3e20  ver_id: int) -> 
-00016f10: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
-00016f20: 2020 4465 6c65 7465 7320 6120 636f 6d70    Deletes a comp
-00016f30: 7574 6520 7365 7276 6572 2069 6e20 6461  ute server in da
-00016f40: 7461 6261 7365 2075 7369 6e67 2069 7473  tabase using its
-00016f50: 2069 640a 0a20 2020 2043 6f6d 7075 7465   id..    Compute
-00016f60: 2073 6572 7665 7273 2069 6473 2063 616e   servers ids can
-00016f70: 2062 6520 6f62 7461 696e 6564 2074 6872   be obtained thr
-00016f80: 6f75 6768 2060 6379 6265 725f 7261 6e67  ough `cyber_rang
-00016f90: 6520 7374 6174 7573 60c2 a06f 7220 3a66  e status`..or :f
-00016fa0: 756e 633a 6066 6574 6368 5f63 6f6d 7075  unc:`fetch_compu
-00016fb0: 7465 5f73 6572 7665 7260 2e0a 2020 2020  te_server`..    
-00016fc0: 2222 220a 2020 2020 7265 7375 6c74 203d  """.    result =
-00016fd0: 205f 6465 6c65 7465 2866 222f 636f 6d70   _delete(f"/comp
-00016fe0: 7574 655f 7365 7276 6572 732f 7b63 6f6d  ute_servers/{com
-00016ff0: 7075 7465 5f73 6572 7665 725f 6964 7d22  pute_server_id}"
-00017000: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
-00017010: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-00017020: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
-00017030: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
-00017040: 742c 2022 4361 6e6e 6f74 2064 656c 6574  t, "Cannot delet
-00017050: 6520 636f 6d70 7574 6520 7365 7276 6572  e compute server
-00017060: 2069 6e20 636f 7265 2041 5049 2229 0a0a   in core API")..
-00017070: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00017080: 742e 6a73 6f6e 2829 0a                   t.json().
+00009110: 2022 4649 4e49 5348 4544 2220 616e 6420   "FINISHED" and 
+00009120: 7265 7375 6c74 5b22 7265 7375 6c74 225d  result["result"]
+00009130: 5b22 7375 6363 6573 7322 5d20 6973 2054  ["success"] is T
+00009140: 7275 650a 0a20 2020 2069 6620 6e6f 7420  rue..    if not 
+00009150: 7375 6363 6573 733a 0a20 2020 2020 2020  success:.       
+00009160: 2065 7272 6f72 5f6d 7367 203d 2072 6573   error_msg = res
+00009170: 756c 745b 2272 6573 756c 7422 5d5b 2265  ult["result"]["e
+00009180: 7272 6f72 5f6d 7367 225d 0a20 2020 2020  rror_msg"].     
+00009190: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
+000091a0: 0a20 2020 2020 2020 2020 2020 2066 225b  .            f"[
+000091b0: 2d5d 2054 6865 2062 6173 6562 6f78 2076  -] The basebox v
+000091c0: 6572 6966 6963 6174 696f 6e20 7761 7320  erification was 
+000091d0: 6578 6563 7574 6564 2077 6974 6820 6572  executed with er
+000091e0: 726f 723a 207b 6572 726f 725f 6d73 677d  ror: {error_msg}
+000091f0: 220a 2020 2020 2020 2020 290a 0a20 2020  ".        )..   
+00009200: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00009210: 0a64 6566 205f 5f77 6169 745f 666f 725f  .def __wait_for_
+00009220: 7468 655f 6f70 6572 6174 696f 6e5f 746f  the_operation_to
+00009230: 5f73 7461 7274 2874 6173 6b5f 6964 3a20  _start(task_id: 
+00009240: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
+00009250: 2020 2222 220a 2020 2020 5761 6974 2066    """.    Wait f
+00009260: 6f72 2061 2074 6173 6b20 746f 2073 7461  or a task to sta
+00009270: 7274 0a20 2020 203a 7061 7261 6d20 7461  rt.    :param ta
+00009280: 736b 5f69 643a 2074 6865 2074 6173 6b20  sk_id: the task 
+00009290: 6964 0a20 2020 203a 7265 7475 726e 3a20  id.    :return: 
+000092a0: 4973 2074 6865 2074 6173 6b20 7275 6e6e  Is the task runn
+000092b0: 696e 670a 2020 2020 2222 220a 0a20 2020  ing.    """..   
+000092c0: 2072 756e 6e69 6e67 203d 2046 616c 7365   running = False
+000092d0: 0a20 2020 2074 696d 656f 7574 203d 2031  .    timeout = 1
+000092e0: 300a 2020 2020 7374 6172 745f 7469 6d65  0.    start_time
+000092f0: 203d 2074 696d 652e 7469 6d65 2829 0a20   = time.time(). 
+00009300: 2020 2077 6869 6c65 206e 6f74 2028 7275     while not (ru
+00009310: 6e6e 696e 6720 6f72 2028 7469 6d65 2e74  nning or (time.t
+00009320: 696d 6528 2920 2d20 7374 6172 745f 7469  ime() - start_ti
+00009330: 6d65 2920 3e20 7469 6d65 6f75 7429 3a0a  me) > timeout):.
+00009340: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00009350: 205f 706f 7374 2822 2f62 6173 6562 6f78   _post("/basebox
+00009360: 2f73 7461 7475 735f 7665 7269 6679 222c  /status_verify",
+00009370: 2064 6174 613d 7b22 7461 736b 5f69 6422   data={"task_id"
+00009380: 3a20 7461 736b 5f69 647d 290a 2020 2020  : task_id}).    
+00009390: 2020 2020 7265 7375 6c74 2e72 6169 7365      result.raise
+000093a0: 5f66 6f72 5f73 7461 7475 7328 290a 2020  _for_status().  
+000093b0: 2020 2020 2020 7265 7375 6c74 203d 2072        result = r
+000093c0: 6573 756c 742e 6a73 6f6e 2829 0a20 2020  esult.json().   
+000093d0: 2020 2020 2072 756e 6e69 6e67 203d 2072       running = r
+000093e0: 6573 756c 745b 2273 7461 7475 7322 5d20  esult["status"] 
+000093f0: 3d3d 2022 5255 4e4e 494e 4722 0a20 2020  == "RUNNING".   
+00009400: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+00009410: 3129 0a0a 2020 2020 6966 206e 6f74 2072  1)..    if not r
+00009420: 756e 6e69 6e67 3a0a 2020 2020 2020 2020  unning:.        
+00009430: 6c6f 6767 6572 2e65 7272 6f72 280a 2020  logger.error(.  
+00009440: 2020 2020 2020 2020 2020 6622 5b2d 5d20            f"[-] 
+00009450: 556e 6162 6c65 2074 6f20 7374 6172 7420  Unable to start 
+00009460: 6f70 6572 6174 696f 6e20 6265 666f 7265  operation before
+00009470: 2074 696d 656f 7574 206f 6620 7b74 696d   timeout of {tim
+00009480: 656f 7574 7d20 7365 636f 6e64 7322 0a20  eout} seconds". 
+00009490: 2020 2020 2020 2029 0a0a 2020 2020 7265         )..    re
+000094a0: 7475 726e 2072 756e 6e69 6e67 0a0a 0a64  turn running...d
+000094b0: 6566 205f 5f68 616e 646c 655f 7761 6974  ef __handle_wait
+000094c0: 280a 2020 2020 7761 6974 3a20 626f 6f6c  (.    wait: bool
+000094d0: 2c20 7461 736b 5f69 643a 2073 7472 2c20  , task_id: str, 
+000094e0: 6c6f 675f 7375 6666 6978 3a20 7374 722c  log_suffix: str,
+000094f0: 2074 696d 656f 7574 3a20 696e 7420 3d20   timeout: int = 
+00009500: 3336 3030 0a29 202d 3e20 626f 6f6c 3a0a  3600.) -> bool:.
+00009510: 2020 2020 2222 220a 0a20 2020 203a 7061      """..    :pa
+00009520: 7261 6d20 7761 6974 3a20 5761 6974 2066  ram wait: Wait f
+00009530: 6f72 2074 6865 206f 7065 7261 7469 6f6e  or the operation
+00009540: 2074 6f20 6265 2063 6f6d 706c 6574 6564   to be completed
+00009550: 2069 6e20 6261 636b 656e 640a 2020 2020   in backend.    
+00009560: 3a70 6172 616d 2074 6173 6b5f 6964 3a20  :param task_id: 
+00009570: 7468 6520 7461 736b 2069 640a 2020 2020  the task id.    
+00009580: 3a70 6172 616d 206c 6f67 5f73 7566 6669  :param log_suffi
+00009590: 783a 2074 6865 2073 7472 696e 6720 746f  x: the string to
+000095a0: 2062 6520 696e 7365 7274 6564 2069 6e20   be inserted in 
+000095b0: 7468 6520 6c6f 670a 2020 2020 3a70 6172  the log.    :par
+000095c0: 616d 2074 696d 656f 7574 3a20 7468 6520  am timeout: the 
+000095d0: 7469 6d65 206c 696d 6974 2062 6566 6f72  time limit befor
+000095e0: 6520 7374 6f70 7069 6e67 2074 6865 2074  e stopping the t
+000095f0: 6173 6b0a 2020 2020 3a72 6574 7572 6e3a  ask.    :return:
+00009600: 2074 6865 2072 6573 756c 7420 6f66 2074   the result of t
+00009610: 6865 2076 6572 6966 6963 6174 696f 6e0a  he verification.
+00009620: 2020 2020 2222 220a 2020 2020 7375 6363      """.    succ
+00009630: 6573 7320 3d20 5472 7565 0a0a 2020 2020  ess = True..    
+00009640: 6966 2077 6169 743a 0a20 2020 2020 2020  if wait:.       
+00009650: 2023 2057 6169 7420 666f 7220 7468 6520   # Wait for the 
+00009660: 6f70 6572 6174 696f 6e20 746f 2062 6520  operation to be 
+00009670: 636f 6d70 6c65 7465 6420 696e 2062 6163  completed in bac
+00009680: 6b65 6e64 0a0a 2020 2020 2020 2020 7265  kend..        re
+00009690: 7375 6c74 203d 205f 5f62 6173 6562 6f78  sult = __basebox
+000096a0: 6573 5f76 6572 6966 6963 6174 696f 6e5f  es_verification_
+000096b0: 7761 6974 5f75 6e74 696c 5f63 6f6d 706c  wait_until_compl
+000096c0: 6574 6528 0a20 2020 2020 2020 2020 2020  ete(.           
+000096d0: 2074 6173 6b5f 6964 3d74 6173 6b5f 6964   task_id=task_id
+000096e0: 2c20 6c6f 675f 7375 6666 6978 3d6c 6f67  , log_suffix=log
+000096f0: 5f73 7566 6669 782c 2074 696d 656f 7574  _suffix, timeout
+00009700: 3d74 696d 656f 7574 0a20 2020 2020 2020  =timeout.       
+00009710: 2029 0a0a 2020 2020 2020 2020 6669 6e69   )..        fini
+00009720: 7368 6564 203d 2022 7374 6174 7573 2220  shed = "status" 
+00009730: 696e 2072 6573 756c 7420 616e 6420 7265  in result and re
+00009740: 7375 6c74 5b22 7374 6174 7573 225d 203d  sult["status"] =
+00009750: 3d20 2246 494e 4953 4845 4422 0a20 2020  = "FINISHED".   
+00009760: 2020 2020 2073 7563 6365 7373 203d 2066       success = f
+00009770: 696e 6973 6865 640a 0a20 2020 2020 2020  inished..       
+00009780: 2069 6620 7375 6363 6573 733a 0a20 2020   if success:.   
+00009790: 2020 2020 2020 2020 2069 6620 2272 6573           if "res
+000097a0: 756c 7422 2069 6e20 7265 7375 6c74 3a0a  ult" in result:.
+000097b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097c0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+000097d0: 2020 2020 2020 2069 6620 6e6f 7420 7375         if not su
+000097e0: 6363 6573 733a 0a20 2020 2020 2020 2020  ccess:.         
+000097f0: 2020 205f 7261 6973 655f 6572 726f 725f     _raise_error_
+00009800: 6d73 6728 7265 7375 6c74 290a 0a20 2020  msg(result)..   
+00009810: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
+00009820: 2077 6169 7420 666f 7220 7468 6520 6f70   wait for the op
+00009830: 6572 6174 696f 6e20 746f 2073 7461 7274  eration to start
+00009840: 0a20 2020 2020 2020 2072 756e 6e69 6e67  .        running
+00009850: 203d 205f 5f77 6169 745f 666f 725f 7468   = __wait_for_th
+00009860: 655f 6f70 6572 6174 696f 6e5f 746f 5f73  e_operation_to_s
+00009870: 7461 7274 2874 6173 6b5f 6964 290a 0a20  tart(task_id).. 
+00009880: 2020 2020 2020 2069 6620 6e6f 7420 7275         if not ru
+00009890: 6e6e 696e 673a 0a20 2020 2020 2020 2020  nning:.         
+000098a0: 2020 2073 7563 6365 7373 203d 2046 616c     success = Fal
+000098b0: 7365 0a0a 2020 2020 7265 7475 726e 2073  se..    return s
+000098c0: 7563 6365 7373 0a0a 0a23 202d 2d2d 2d2d  uccess...# -----
+000098d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000098e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000098f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009910: 2d2d 2d2d 2d20 230a 2320 436f 7265 2041  ----- #.# Core A
+00009920: 5049 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  PI.# -----------
+00009930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
+00009970: 230a 0a0a 6465 6620 6765 745f 7665 7273  #...def get_vers
+00009980: 696f 6e28 2920 2d3e 2073 7472 3a0a 2020  ion() -> str:.  
+00009990: 2020 2222 2252 6574 7572 6e20 436f 7265    """Return Core
+000099a0: 2041 5049 2076 6572 7369 6f6e 2e22 2222   API version."""
+000099b0: 0a0a 2020 2020 7265 7375 6c74 203d 205f  ..    result = _
+000099c0: 6765 7428 222f 7369 6d75 6c61 7469 6f6e  get("/simulation
+000099d0: 2f76 6572 7369 6f6e 2229 0a0a 2020 2020  /version")..    
+000099e0: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
+000099f0: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
+00009a00: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
+00009a10: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
+00009a20: 6e6f 7420 7265 7472 6965 7665 2043 6f72  not retrieve Cor
+00009a30: 6520 4150 4920 7665 7273 696f 6e22 290a  e API version").
+00009a40: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+00009a50: 6c74 2e6a 736f 6e28 290a 0a0a 6465 6620  lt.json()...def 
+00009a60: 7265 7365 7428 6465 6c65 7465 5f63 6f6d  reset(delete_com
+00009a70: 7075 7465 5f73 6572 7665 7273 3a20 626f  pute_servers: bo
+00009a80: 6f6c 203d 2046 616c 7365 2920 2d3e 2041  ol = False) -> A
+00009a90: 6e79 3a0a 2020 2020 2222 220a 2020 2020  ny:.    """.    
+00009aa0: 5265 7365 7420 7468 6520 4954 2053 696d  Reset the IT Sim
+00009ab0: 756c 6174 696f 6e20 696e 6672 6173 7472  ulation infrastr
+00009ac0: 7563 7475 7265 0a0a 2020 2020 5468 6973  ucture..    This
+00009ad0: 2068 6173 2074 6865 2066 6f6c 6c6f 7769   has the followi
+00009ae0: 6e67 2065 6666 6563 743a 0a20 2020 202d  ng effect:.    -
+00009af0: 2063 6c65 616e 2074 6865 2064 6174 6162   clean the datab
+00009b00: 6173 6520 616e 6420 7265 2d70 6f70 756c  ase and re-popul
+00009b10: 6174 6520 6974 2077 6974 6820 7374 6174  ate it with stat
+00009b20: 6963 2069 6e66 6f20 2862 6173 6562 6f78  ic info (basebox
+00009b30: 6573 2c20 726f 6c65 732e 2e2e 290a 2020  es, roles...).  
+00009b40: 2020 2d20 6279 2064 6566 6175 742c 2074    - by defaut, t
+00009b50: 6865 2074 6162 6c65 206f 6620 636f 6d70  he table of comp
+00009b60: 7574 6520 7365 7276 6572 7320 6973 206b  ute servers is k
+00009b70: 6570 742c 2062 7574 2060 6465 6c65 7465  ept, but `delete
+00009b80: 5f63 6f6d 7075 7465 5f73 6572 7665 7273  _compute_servers
+00009b90: 3d54 7275 6560 2063 6861 6e67 6573 2074  =True` changes t
+00009ba0: 6861 7420 6265 6861 7669 6f72 0a20 2020  hat behavior.   
+00009bb0: 202d 2072 6573 6574 2074 6865 2073 696d   - reset the sim
+00009bc0: 756c 6174 696f 6e20 6d61 6e61 6765 720a  ulation manager.
+00009bd0: 2020 2020 2d20 7265 7365 7420 7468 6520      - reset the 
+00009be0: 636f 6d70 7574 6520 7365 7276 6572 7320  compute servers 
+00009bf0: 2873 746f 7020 564d 7320 616e 6420 646f  (stop VMs and do
+00009c00: 636b 6572 732c 2072 6573 6574 206e 6574  ckers, reset net
+00009c10: 776f 726b 732c 202e 2e2e 290a 2020 2020  works, ...).    
+00009c20: 2222 220a 2020 2020 7061 7261 6d73 203d  """.    params =
+00009c30: 207b 7d0a 2020 2020 6966 2064 656c 6574   {}.    if delet
+00009c40: 655f 636f 6d70 7574 655f 7365 7276 6572  e_compute_server
+00009c50: 733a 0a20 2020 2020 2020 2070 6172 616d  s:.        param
+00009c60: 7320 3d20 7b22 6465 6c65 7465 5f63 6f6d  s = {"delete_com
+00009c70: 7075 7465 5f73 6572 7665 7273 5f66 726f  pute_servers_fro
+00009c80: 6d5f 6462 223a 2064 656c 6574 655f 636f  m_db": delete_co
+00009c90: 6d70 7574 655f 7365 7276 6572 737d 0a0a  mpute_servers}..
+00009ca0: 2020 2020 7265 7375 6c74 203d 205f 6465      result = _de
+00009cb0: 6c65 7465 2822 2f73 696d 756c 6174 696f  lete("/simulatio
+00009cc0: 6e2f 636f 6d70 7574 655f 696e 6672 6173  n/compute_infras
+00009cd0: 7472 7563 7475 7265 5f72 6573 6574 222c  tructure_reset",
+00009ce0: 2070 6172 616d 733d 7061 7261 6d73 290a   params=params).
+00009cf0: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
+00009d00: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+00009d10: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
+00009d20: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
+00009d30: 2022 4361 6e6e 6f74 2072 6573 6574 2073   "Cannot reset s
+00009d40: 696d 756c 6174 696f 6e20 696e 6672 6173  imulation infras
+00009d50: 7472 7563 7475 7265 2229 0a0a 2020 2020  tructure")..    
+00009d60: 7265 7475 726e 2072 6573 756c 742e 6a73  return result.js
+00009d70: 6f6e 2829 0a0a 0a64 6566 205f 6372 6561  on()...def _crea
+00009d80: 7465 5f6f 725f 6578 7465 6e64 5f73 696d  te_or_extend_sim
+00009d90: 756c 6174 696f 6e28 0a20 2020 2073 696d  ulation(.    sim
+00009da0: 756c 6174 696f 6e5f 6469 6374 3a20 6469  ulation_dict: di
+00009db0: 6374 2c0a 2020 2020 6964 5f73 696d 756c  ct,.    id_simul
+00009dc0: 6174 696f 6e3a 2069 6e74 203d 204e 6f6e  ation: int = Non
+00009dd0: 652c 0a20 2020 2061 6c6c 6f63 6174 696f  e,.    allocatio
+00009de0: 6e5f 7374 7261 7465 6779 3a20 4f70 7469  n_strategy: Opti
+00009df0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00009e00: 2c0a 2920 2d3e 2054 7570 6c65 5b69 6e74  ,.) -> Tuple[int
+00009e10: 2c20 4c69 7374 5b73 7472 5d5d 3a0a 2020  , List[str]]:.  
+00009e20: 2020 2222 2243 7265 6174 6520 6120 7369    """Create a si
+00009e30: 6d75 6c61 7469 6f6e 2c20 6f72 2065 7874  mulation, or ext
+00009e40: 656e 6420 616e 2065 7869 7374 696e 6720  end an existing 
+00009e50: 7369 6d75 6c61 7469 6f6e 2077 6974 6820  simulation with 
+00009e60: 6e65 770a 2020 2020 6e6f 6465 7320 616e  new.    nodes an
+00009e70: 6420 6c69 6e6b 732c 2061 6e64 2072 6574  d links, and ret
+00009e80: 7572 6e20 6120 7369 6d75 6c61 7469 6f6e  urn a simulation
+00009e90: 2049 442e 2222 220a 0a20 2020 2023 2047   ID."""..    # G
+00009ea0: 6574 2074 6865 2070 6174 6873 2069 6620  et the paths if 
+00009eb0: 736f 6d65 2068 6176 6520 6265 656e 2070  some have been p
+00009ec0: 726f 7669 6465 640a 2020 2020 7265 736f  rovided.    reso
+00009ed0: 7572 6365 735f 7061 7468 7320 3d20 7369  urces_paths = si
+00009ee0: 6d75 6c61 7469 6f6e 5f64 6963 742e 706f  mulation_dict.po
+00009ef0: 7028 2272 6573 6f75 7263 6573 5f70 6174  p("resources_pat
+00009f00: 6873 222c 205b 5d29 0a0a 2020 2020 6461  hs", [])..    da
+00009f10: 7461 203d 206a 736f 6e2e 6475 6d70 7328  ta = json.dumps(
+00009f20: 7369 6d75 6c61 7469 6f6e 5f64 6963 7429  simulation_dict)
+00009f30: 0a0a 2020 2020 2320 4372 6561 7469 6f6e  ..    # Creation
+00009f40: 206f 6620 6120 666f 6c64 6572 2063 6f6e   of a folder con
+00009f50: 7461 696e 696e 6720 616c 6c20 7468 6520  taining all the 
+00009f60: 7265 736f 7572 6365 732c 2074 6869 7320  resources, this 
+00009f70: 666f 6c64 6572 2077 696c 6c20 7468 656e  folder will then
+00009f80: 2062 6520 7a69 7070 6564 0a20 2020 2077   be zipped.    w
+00009f90: 6974 6820 5465 6d70 6f72 6172 7944 6972  ith TemporaryDir
+00009fa0: 6563 746f 7279 2870 7265 6669 783d 2263  ectory(prefix="c
+00009fb0: 7962 6572 5f72 616e 6765 5f63 725f 636f  yber_range_cr_co
+00009fc0: 7265 5f72 6573 6f75 7263 6573 2229 2061  re_resources") a
+00009fd0: 7320 6d61 696e 5f72 6573 6f75 7263 6573  s main_resources
+00009fe0: 3a0a 0a20 2020 2020 2020 2023 2063 6f70  :..        # cop
+00009ff0: 7920 616c 6c20 7265 736f 7572 6365 7320  y all resources 
+0000a000: 696e 2074 6865 206d 6169 6e20 7465 6d70  in the main temp
+0000a010: 6f72 6172 7920 666f 6c64 6572 0a20 2020  orary folder.   
+0000a020: 2020 2020 2066 6f72 2072 6573 6f75 7263       for resourc
+0000a030: 6520 696e 2072 6573 6f75 7263 6573 5f70  e in resources_p
+0000a040: 6174 6873 3a0a 2020 2020 2020 2020 2020  aths:.          
+0000a050: 2020 6966 206f 732e 7061 7468 2e69 7364    if os.path.isd
+0000a060: 6972 2872 6573 6f75 7263 6529 3a0a 2020  ir(resource):.  
+0000a070: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+0000a080: 7574 696c 2e63 6f70 7974 7265 6528 0a20  util.copytree(. 
+0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0a0: 2020 2072 6573 6f75 7263 652c 0a20 2020     resource,.   
+0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0c0: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
+0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0e0: 2020 2020 2020 206d 6169 6e5f 7265 736f         main_reso
+0000a0f0: 7572 6365 732c 206f 732e 7061 7468 2e62  urces, os.path.b
+0000a100: 6173 656e 616d 6528 6f73 2e70 6174 682e  asename(os.path.
+0000a110: 6e6f 726d 7061 7468 2872 6573 6f75 7263  normpath(resourc
+0000a120: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+0000a130: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+0000a140: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000a150: 2020 2020 2020 2020 2065 6c69 6620 6f73           elif os
+0000a160: 2e70 6174 682e 6973 6669 6c65 2872 6573  .path.isfile(res
+0000a170: 6f75 7263 6529 3a0a 2020 2020 2020 2020  ource):.        
+0000a180: 2020 2020 2020 2020 7368 7574 696c 2e63          shutil.c
+0000a190: 6f70 7966 696c 6528 0a20 2020 2020 2020  opyfile(.       
+0000a1a0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0000a1b0: 6f75 7263 652c 0a20 2020 2020 2020 2020  ource,.         
+0000a1c0: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
+0000a1d0: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
+0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1f0: 206d 6169 6e5f 7265 736f 7572 6365 732c   main_resources,
+0000a200: 206f 732e 7061 7468 2e62 6173 656e 616d   os.path.basenam
+0000a210: 6528 6f73 2e70 6174 682e 6e6f 726d 7061  e(os.path.normpa
+0000a220: 7468 2872 6573 6f75 7263 6529 290a 2020  th(resource)).  
+0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a240: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+0000a250: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000a260: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a270: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+0000a280: 7863 6570 7469 6f6e 2866 2243 616e 206e  xception(f"Can n
+0000a290: 6f74 2063 6f70 7920 7b72 6573 6f75 7263  ot copy {resourc
+0000a2a0: 657d 2229 0a0a 2020 2020 2020 2020 2320  e}")..        # 
+0000a2b0: 5765 2068 6176 6520 746f 2063 7265 6174  We have to creat
+0000a2c0: 6520 6120 6e65 7720 7465 6d70 6f72 6172  e a new temporar
+0000a2d0: 7920 666f 6c64 6572 2074 6f20 686f 7374  y folder to host
+0000a2e0: 2074 6865 2061 7263 6869 7665 0a20 2020   the archive.   
+0000a2f0: 2020 2020 2077 6974 6820 5465 6d70 6f72       with Tempor
+0000a300: 6172 7944 6972 6563 746f 7279 2870 7265  aryDirectory(pre
+0000a310: 6669 783d 2263 7962 6572 5f72 616e 6765  fix="cyber_range
+0000a320: 5f63 725f 636f 7265 5f61 7263 6869 7665  _cr_core_archive
+0000a330: 2229 2061 7320 7465 6d70 5f64 6972 3a0a  ") as temp_dir:.
+0000a340: 2020 2020 2020 2020 2020 2020 7a69 705f              zip_
+0000a350: 6669 6c65 5f6e 616d 6520 3d20 5f7a 6970  file_name = _zip
+0000a360: 5f72 6573 6f75 7263 6573 286d 6169 6e5f  _resources(main_
+0000a370: 7265 736f 7572 6365 732c 2074 656d 705f  resources, temp_
+0000a380: 6469 7229 0a20 2020 2020 2020 2020 2020  dir).           
+0000a390: 2072 6573 6f75 7263 6573 5f66 696c 6520   resources_file 
+0000a3a0: 3d20 6f70 656e 287a 6970 5f66 696c 655f  = open(zip_file_
+0000a3b0: 6e61 6d65 2c20 2272 6222 290a 2020 2020  name, "rb").    
+0000a3c0: 2020 2020 2020 2020 6669 6c65 7320 3d20          files = 
+0000a3d0: 7b22 7265 736f 7572 6365 735f 6669 6c65  {"resources_file
+0000a3e0: 223a 2072 6573 6f75 7263 6573 5f66 696c  ": resources_fil
+0000a3f0: 652c 2022 6461 7461 223a 2064 6174 617d  e, "data": data}
+0000a400: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+0000a410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a420: 2020 6966 2069 645f 7369 6d75 6c61 7469    if id_simulati
+0000a430: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a450: 2320 4372 6561 7465 206e 6577 2073 696d  # Create new sim
+0000a460: 756c 6174 696f 6e0a 2020 2020 2020 2020  ulation.        
+0000a470: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000a480: 6c74 203d 205f 706f 7374 280a 2020 2020  lt = _post(.    
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 222f 7369 6d75 6c61 7469 6f6e      "/simulation
+0000a4b0: 2f22 2c0a 2020 2020 2020 2020 2020 2020  /",.            
+0000a4c0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+0000a4d0: 733d 6669 6c65 732c 0a20 2020 2020 2020  s=files,.       
+0000a4e0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000a500: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000a510: 2020 2020 2020 2020 2023 2045 7874 656e           # Exten
+0000a520: 6420 616e 2065 7869 7374 696e 6720 7369  d an existing si
+0000a530: 6d75 6c61 7469 6f6e 0a20 2020 2020 2020  mulation.       
+0000a540: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0000a550: 756c 7420 3d20 5f70 6f73 7428 0a20 2020  ult = _post(.   
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 2020 2020 2066 222f 7369 6d75 6c61 7469       f"/simulati
+0000a580: 6f6e 2f7b 6964 5f73 696d 756c 6174 696f  on/{id_simulatio
+0000a590: 6e7d 2f65 7874 656e 6422 2c0a 2020 2020  n}/extend",.    
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5b0: 2020 2020 6669 6c65 733d 6669 6c65 732c      files=files,
+0000a5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a5d0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000a5e0: 2020 2066 696e 616c 6c79 3a0a 2020 2020     finally:.    
+0000a5f0: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+0000a600: 7572 6365 735f 6669 6c65 2e63 6c6f 7365  urces_file.close
+0000a610: 2829 0a0a 2020 2020 6966 206e 6f74 206d  ()..    if not m
+0000a620: 6169 6e5f 7265 736f 7572 6365 733a 0a20  ain_resources:. 
+0000a630: 2020 2020 2020 2069 6620 6964 5f73 696d         if id_sim
+0000a640: 756c 6174 696f 6e20 6973 204e 6f6e 653a  ulation is None:
+0000a650: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+0000a660: 7265 6174 6520 6e65 7720 7369 6d75 6c61  reate new simula
+0000a670: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+0000a680: 2072 6573 756c 7420 3d20 5f70 6f73 7428   result = _post(
+0000a690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a6a0: 2022 2f73 696d 756c 6174 696f 6e2f 222c   "/simulation/",
+0000a6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a6c0: 2064 6174 613d 6461 7461 2c0a 2020 2020   data=data,.    
+0000a6d0: 2020 2020 2020 2020 2020 2020 6865 6164              head
+0000a6e0: 6572 733d 7b22 436f 6e74 656e 742d 5479  ers={"Content-Ty
+0000a6f0: 7065 223a 2022 6170 706c 6963 6174 696f  pe": "applicatio
+0000a700: 6e2f 6a73 6f6e 227d 2c0a 2020 2020 2020  n/json"},.      
+0000a710: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000a720: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000a730: 2020 2320 4578 7465 6e64 2061 6e20 6578    # Extend an ex
+0000a740: 6973 7469 6e67 2073 696d 756c 6174 696f  isting simulatio
+0000a750: 6e0a 2020 2020 2020 2020 2020 2020 7265  n.            re
+0000a760: 7375 6c74 203d 205f 706f 7374 280a 2020  sult = _post(.  
+0000a770: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000a780: 2f73 696d 756c 6174 696f 6e2f 7b69 645f  /simulation/{id_
+0000a790: 7369 6d75 6c61 7469 6f6e 7d2f 6578 7465  simulation}/exte
+0000a7a0: 6e64 222c 0a20 2020 2020 2020 2020 2020  nd",.           
+0000a7b0: 2020 2020 2064 6174 613d 6461 7461 2c0a       data=data,.
+0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7d0: 6865 6164 6572 733d 7b22 436f 6e74 656e  headers={"Conten
+0000a7e0: 742d 5479 7065 223a 2022 6170 706c 6963  t-Type": "applic
+0000a7f0: 6174 696f 6e2f 6a73 6f6e 227d 2c0a 2020  ation/json"},.  
+0000a800: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000a810: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+0000a820: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+0000a830: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+0000a840: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
+0000a850: 6e6e 6f74 2070 6f73 7420 7369 6d75 6c61  nnot post simula
+0000a860: 7469 6f6e 2069 6e66 6f72 6d61 7469 6f6e  tion information
+0000a870: 2074 6f20 636f 7265 2041 5049 2229 0a0a   to core API")..
+0000a880: 2020 2020 6964 5f73 696d 756c 6174 696f      id_simulatio
+0000a890: 6e20 3d20 7265 7375 6c74 2e6a 736f 6e28  n = result.json(
+0000a8a0: 295b 2269 6422 5d0a 2020 2020 6e65 775f  )["id"].    new_
+0000a8b0: 6e6f 6465 7320 3d20 7265 7375 6c74 2e6a  nodes = result.j
+0000a8c0: 736f 6e28 295b 226e 6577 5f6e 6f64 6573  son()["new_nodes
+0000a8d0: 225d 0a20 2020 206c 6f67 6765 722e 696e  "].    logger.in
+0000a8e0: 666f 2866 225b 2b5d 204e 6577 206e 6f64  fo(f"[+] New nod
+0000a8f0: 6573 2066 6f72 2073 696d 756c 6174 696f  es for simulatio
+0000a900: 6e20 6964 2027 7b69 645f 7369 6d75 6c61  n id '{id_simula
+0000a910: 7469 6f6e 7d27 3a20 277b 6e65 775f 6e6f  tion}': '{new_no
+0000a920: 6465 737d 2722 290a 0a20 2020 2023 2050  des}'")..    # P
+0000a930: 7265 7061 7265 2064 6973 6b20 7265 736f  repare disk reso
+0000a940: 7572 6365 730a 2020 2020 706f 7374 5f64  urces.    post_d
+0000a950: 6174 6120 3d20 7b22 6e6f 6465 7322 3a20  ata = {"nodes": 
+0000a960: 6e65 775f 6e6f 6465 737d 0a20 2020 205f  new_nodes}.    _
+0000a970: 7369 6d75 6c61 7469 6f6e 5f65 7865 6375  simulation_execu
+0000a980: 7465 5f6f 7065 7261 7469 6f6e 280a 2020  te_operation(.  
+0000a990: 2020 2020 2020 2270 6f73 7422 2c0a 2020        "post",.  
+0000a9a0: 2020 2020 2020 2270 7265 7061 7265 222c        "prepare",
+0000a9b0: 0a20 2020 2020 2020 2069 645f 7369 6d75  .        id_simu
+0000a9c0: 6c61 7469 6f6e 2c0a 2020 2020 2020 2020  lation,.        
+0000a9d0: 2250 5245 5041 5249 4e47 222c 0a20 2020  "PREPARING",.   
+0000a9e0: 2020 2020 206f 7074 696f 6e61 6c5f 7061       optional_pa
+0000a9f0: 7261 6d31 3d61 6c6c 6f63 6174 696f 6e5f  ram1=allocation_
+0000aa00: 7374 7261 7465 6779 2c0a 2020 2020 2020  strategy,.      
+0000aa10: 2020 706f 7374 5f64 6174 613d 706f 7374    post_data=post
+0000aa20: 5f64 6174 612c 0a20 2020 2029 0a0a 2020  _data,.    )..  
+0000aa30: 2020 2320 544f 444f 3a20 4368 6563 6b20    # TODO: Check 
+0000aa40: 7468 6174 2074 6865 2064 6f63 6b65 7220  that the docker 
+0000aa50: 766f 6c75 6d65 7320 7468 6174 2077 696c  volumes that wil
+0000aa60: 6c20 6265 206d 6f75 6e74 6564 2062 7920  l be mounted by 
+0000aa70: 7369 6d75 5f72 756e 2061 7265 2070 7265  simu_run are pre
+0000aa80: 7365 6e74 206f 6e20 7468 6520 6669 6c65  sent on the file
+0000aa90: 7379 7374 656d 0a20 2020 2023 2066 6f72  system.    # for
+0000aaa0: 202e 2e2e 3a20 5f73 696d 755f 6372 6561   ...: _simu_crea
+0000aab0: 7465 5f76 616c 6964 6174 655f 7265 736f  te_validate_reso
+0000aac0: 7572 6365 735f 6578 6973 7473 2829 0a0a  urces_exists()..
+0000aad0: 2020 2020 7265 7475 726e 2028 6964 5f73      return (id_s
+0000aae0: 696d 756c 6174 696f 6e2c 206e 6577 5f6e  imulation, new_n
+0000aaf0: 6f64 6573 290a 0a0a 6465 6620 7369 6d75  odes)...def simu
+0000ab00: 6c61 7469 6f6e 5f73 7461 7475 7328 6964  lation_status(id
+0000ab10: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
+0000ab20: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
+0000ab30: 2252 6574 7572 6e20 6f6e 6c79 2074 6865  "Return only the
+0000ab40: 2073 7461 7475 7320 6f66 2074 6865 2073   status of the s
+0000ab50: 696d 756c 6174 696f 6e22 2222 0a20 2020  imulation""".   
+0000ab60: 2072 6573 756c 7420 3d20 5f67 6574 2866   result = _get(f
+0000ab70: 222f 7369 6d75 6c61 7469 6f6e 2f7b 6964  "/simulation/{id
+0000ab80: 5f73 696d 756c 6174 696f 6e7d 2f73 7461  _simulation}/sta
+0000ab90: 7475 7322 290a 0a20 2020 2069 6620 7265  tus")..    if re
+0000aba0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+0000abb0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+0000abc0: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+0000abd0: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+0000abe0: 6574 7269 6576 6520 7369 6d75 6c61 7469  etrieve simulati
+0000abf0: 6f6e 2069 6e66 6f20 6672 6f6d 2049 5420  on info from IT 
+0000ac00: 5369 6d75 6c61 7469 6f6e 2041 5049 2229  Simulation API")
+0000ac10: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+0000ac20: 756c 742e 6a73 6f6e 2829 0a0a 0a64 6566  ult.json()...def
+0000ac30: 2066 6574 6368 5f73 696d 756c 6174 696f   fetch_simulatio
+0000ac40: 6e28 6964 5f73 696d 756c 6174 696f 6e3a  n(id_simulation:
+0000ac50: 2069 6e74 2920 2d3e 2064 6963 743a 0a20   int) -> dict:. 
+0000ac60: 2020 2022 2222 5265 7475 726e 2061 2073     """Return a s
+0000ac70: 696d 756c 6174 696f 6e20 6469 6374 2067  imulation dict g
+0000ac80: 6976 656e 2061 2073 696d 756c 6174 696f  iven a simulatio
+0000ac90: 6e20 6964 2e22 2222 0a20 2020 2072 6573  n id.""".    res
+0000aca0: 756c 7420 3d20 5f67 6574 2866 222f 7369  ult = _get(f"/si
+0000acb0: 6d75 6c61 7469 6f6e 2f7b 6964 5f73 696d  mulation/{id_sim
+0000acc0: 756c 6174 696f 6e7d 2229 0a0a 2020 2020  ulation}")..    
+0000acd0: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
+0000ace0: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
+0000acf0: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
+0000ad00: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
+0000ad10: 6e6f 7420 7265 7472 6965 7665 2073 696d  not retrieve sim
+0000ad20: 756c 6174 696f 6e20 696e 666f 2066 726f  ulation info fro
+0000ad30: 6d20 4954 2053 696d 756c 6174 696f 6e20  m IT Simulation 
+0000ad40: 4150 4922 290a 0a20 2020 2073 696d 756c  API")..    simul
+0000ad50: 6174 696f 6e5f 6469 6374 203d 2072 6573  ation_dict = res
+0000ad60: 756c 742e 6a73 6f6e 2829 0a0a 2020 2020  ult.json()..    
+0000ad70: 7265 7475 726e 2073 696d 756c 6174 696f  return simulatio
+0000ad80: 6e5f 6469 6374 0a0a 0a64 6566 2066 6574  n_dict...def fet
+0000ad90: 6368 5f73 696d 756c 6174 696f 6e73 2829  ch_simulations()
+0000ada0: 202d 3e20 4c69 7374 5b41 6e79 5d3a 0a20   -> List[Any]:. 
+0000adb0: 2020 2022 2222 4765 7420 7468 6520 6c69     """Get the li
+0000adc0: 7374 206f 6620 7369 6d75 6c61 7469 6f6e  st of simulation
+0000add0: 732c 2069 6e63 6c75 6469 6e67 2074 6865  s, including the
+0000ade0: 2063 7572 7265 6e74 6c79 2072 756e 6e69   currently runni
+0000adf0: 6e67 2073 696d 7561 6c74 696f 6e2c 2061  ng simualtion, a
+0000ae00: 6c6f 6e67 2077 6974 680a 2020 2020 696e  long with.    in
+0000ae10: 666f 726d 6174 696f 6e20 6f6e 206e 6f64  formation on nod
+0000ae20: 6573 0a0a 2020 2020 2222 220a 2020 2020  es..    """.    
+0000ae30: 7265 7375 6c74 203d 205f 6765 7428 222f  result = _get("/
+0000ae40: 7369 6d75 6c61 7469 6f6e 2f22 290a 0a20  simulation/").. 
+0000ae50: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+0000ae60: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+0000ae70: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+0000ae80: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
+0000ae90: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
+0000aea0: 7369 6d75 6c61 7469 6f6e 2069 6e66 6f20  simulation info 
+0000aeb0: 6672 6f6d 2049 5420 5369 6d75 6c61 7469  from IT Simulati
+0000aec0: 6f6e 2041 5049 2229 0a0a 2020 2020 7369  on API")..    si
+0000aed0: 6d75 6c61 7469 6f6e 5f6c 6973 7420 3d20  mulation_list = 
+0000aee0: 7265 7375 6c74 2e6a 736f 6e28 290a 2020  result.json().  
+0000aef0: 2020 7265 7475 726e 2073 696d 756c 6174    return simulat
+0000af00: 696f 6e5f 6c69 7374 0a0a 0a64 6566 2064  ion_list...def d
+0000af10: 656c 6574 655f 7369 6d75 6c61 7469 6f6e  elete_simulation
+0000af20: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
+0000af30: 696e 7429 202d 3e20 416e 793a 0a20 2020  int) -> Any:.   
+0000af40: 2022 2222 4465 6c65 7465 2061 2073 696d   """Delete a sim
+0000af50: 756c 6174 696f 6e20 696e 2064 6174 6162  ulation in datab
+0000af60: 6173 652e 2222 220a 0a20 2020 2023 2044  ase."""..    # D
+0000af70: 6573 7472 6f79 2073 696d 756c 6174 696f  estroy simulatio
+0000af80: 6e20 6966 2069 7420 6973 2072 756e 6e69  n if it is runni
+0000af90: 6e67 0a20 2020 2069 6620 7369 6d75 6c61  ng.    if simula
+0000afa0: 7469 6f6e 5f73 7461 7475 7328 6964 5f73  tion_status(id_s
+0000afb0: 696d 756c 6174 696f 6e29 203d 3d20 2252  imulation) == "R
+0000afc0: 554e 4e49 4e47 223a 0a0a 2020 2020 2020  UNNING":..      
+0000afd0: 2020 6e6f 6465 733a 204c 6973 745b 7374    nodes: List[st
+0000afe0: 725d 203d 205b 5d0a 2020 2020 2020 2020  r] = [].        
+0000aff0: 706f 7374 5f64 6174 6120 3d20 7b22 6e6f  post_data = {"no
+0000b000: 6465 7322 3a20 6e6f 6465 737d 0a0a 2020  des": nodes}..  
+0000b010: 2020 2020 2020 5f73 696d 756c 6174 696f        _simulatio
+0000b020: 6e5f 6578 6563 7574 655f 6f70 6572 6174  n_execute_operat
+0000b030: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+0000b040: 2022 706f 7374 222c 2022 6465 7374 726f   "post", "destro
+0000b050: 7922 2c20 6964 5f73 696d 756c 6174 696f  y", id_simulatio
+0000b060: 6e2c 2022 5354 4f50 5049 4e47 222c 2070  n, "STOPPING", p
+0000b070: 6f73 745f 6461 7461 3d70 6f73 745f 6461  ost_data=post_da
+0000b080: 7461 0a20 2020 2020 2020 2029 0a0a 2020  ta.        )..  
+0000b090: 2020 5f73 696d 756c 6174 696f 6e5f 6578    _simulation_ex
+0000b0a0: 6563 7574 655f 6f70 6572 6174 696f 6e28  ecute_operation(
+0000b0b0: 2267 6574 222c 2022 6465 6c65 7465 5f73  "get", "delete_s
+0000b0c0: 6e61 7073 686f 7473 222c 2069 645f 7369  napshots", id_si
+0000b0d0: 6d75 6c61 7469 6f6e 2c20 2253 544f 5050  mulation, "STOPP
+0000b0e0: 494e 4722 290a 0a20 2020 2023 2044 656c  ING")..    # Del
+0000b0f0: 6574 6520 7369 6d75 6c61 7469 6f6e 206e  ete simulation n
+0000b100: 6f64 6573 0a20 2020 2064 656c 6574 655f  odes.    delete_
+0000b110: 6e6f 6465 7328 6964 5f73 696d 756c 6174  nodes(id_simulat
+0000b120: 696f 6e29 0a0a 2020 2020 2320 4465 6c65  ion)..    # Dele
+0000b130: 7465 2073 696d 756c 6174 696f 6e0a 2020  te simulation.  
+0000b140: 2020 7265 7375 6c74 203d 205f 6465 6c65    result = _dele
+0000b150: 7465 2866 222f 7369 6d75 6c61 7469 6f6e  te(f"/simulation
+0000b160: 2f7b 6964 5f73 696d 756c 6174 696f 6e7d  /{id_simulation}
+0000b170: 2229 0a0a 2020 2020 6966 2072 6573 756c  ")..    if resul
+0000b180: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
+0000b190: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
+0000b1a0: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
+0000b1b0: 6c74 2c20 2243 616e 6e6f 7420 6465 6c65  lt, "Cannot dele
+0000b1c0: 7465 2073 696d 756c 6174 696f 6e20 6672  te simulation fr
+0000b1d0: 6f6d 2049 5420 5369 6d75 6c61 7469 6f6e  om IT Simulation
+0000b1e0: 2041 5049 2229 0a0a 2020 2020 7265 7475   API")..    retu
+0000b1f0: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
+0000b200: 0a0a 0a64 6566 206e 6f64 655f 7374 6174  ...def node_stat
+0000b210: 7573 2869 645f 6e6f 6465 3a20 696e 7429  us(id_node: int)
+0000b220: 202d 3e20 7374 723a 0a20 2020 2022 2222   -> str:.    """
+0000b230: 5265 7472 6965 7665 206e 6f64 6520 7374  Retrieve node st
+0000b240: 6174 7573 2e22 2222 0a0a 2020 2020 7265  atus."""..    re
+0000b250: 7375 6c74 203d 205f 6765 7428 6622 2f6e  sult = _get(f"/n
+0000b260: 6f64 652f 7b69 645f 6e6f 6465 7d2f 7374  ode/{id_node}/st
+0000b270: 6174 7573 2229 0a0a 2020 2020 6966 2072  atus")..    if r
+0000b280: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
+0000b290: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
+0000b2a0: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+0000b2b0: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
+0000b2c0: 7265 7472 6965 7665 206e 6f64 6520 696e  retrieve node in
+0000b2d0: 666f 2066 726f 6d20 4954 2053 696d 756c  fo from IT Simul
+0000b2e0: 6174 696f 6e20 4150 4922 290a 0a20 2020  ation API")..   
+0000b2f0: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
+0000b300: 736f 6e28 290a 0a0a 6465 6620 7374 6f70  son()...def stop
+0000b310: 5f6e 6f64 655f 6279 5f6e 616d 6528 6964  _node_by_name(id
+0000b320: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
+0000b330: 2c20 6e6f 6465 5f6e 616d 653a 2073 7472  , node_name: str
+0000b340: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+0000b350: 2222 5374 6f70 2061 206e 6f64 6520 6966  ""Stop a node if
+0000b360: 2069 7420 6973 2072 756e 6e69 6e67 2e22   it is running."
+0000b370: 2222 0a0a 2020 2020 2320 5265 7472 6965  ""..    # Retrie
+0000b380: 7665 2069 645f 6e6f 6465 0a20 2020 206e  ve id_node.    n
+0000b390: 6f64 6520 3d20 6665 7463 685f 6e6f 6465  ode = fetch_node
+0000b3a0: 5f62 795f 6e61 6d65 2869 645f 7369 6d75  _by_name(id_simu
+0000b3b0: 6c61 7469 6f6e 2c20 6e6f 6465 5f6e 616d  lation, node_nam
+0000b3c0: 6529 0a20 2020 2069 645f 6e6f 6465 203d  e).    id_node =
+0000b3d0: 206e 6f64 655b 2269 6422 5d0a 0a20 2020   node["id"]..   
+0000b3e0: 2023 2044 656c 6574 6520 6e6f 6465 0a20   # Delete node. 
+0000b3f0: 2020 2073 746f 705f 6e6f 6465 2869 645f     stop_node(id_
+0000b400: 7369 6d75 6c61 7469 6f6e 2c20 6964 5f6e  simulation, id_n
+0000b410: 6f64 6529 0a0a 0a64 6566 2073 746f 705f  ode)...def stop_
+0000b420: 6e6f 6465 2869 645f 7369 6d75 6c61 7469  node(id_simulati
+0000b430: 6f6e 3a20 696e 742c 2069 645f 6e6f 6465  on: int, id_node
+0000b440: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+0000b450: 2020 2020 2222 2253 746f 7020 6120 6e6f      """Stop a no
+0000b460: 6465 2069 6620 6974 2069 7320 7275 6e6e  de if it is runn
+0000b470: 696e 672e 2222 220a 0a20 2020 2023 2052  ing."""..    # R
+0000b480: 6574 7269 6576 6520 6e6f 6465 2061 6363  etrieve node acc
+0000b490: 6f72 6469 6e67 2074 6f20 6974 7320 6e61  ording to its na
+0000b4a0: 6d65 0a20 2020 206e 6f64 6520 3d20 6665  me.    node = fe
+0000b4b0: 7463 685f 6e6f 6465 2869 645f 6e6f 6465  tch_node(id_node
+0000b4c0: 290a 0a20 2020 2023 2053 6574 206e 6f64  )..    # Set nod
+0000b4d0: 6520 6e61 6d65 7320 746f 2064 656c 6574  e names to delet
+0000b4e0: 650a 2020 2020 6e6f 6465 735f 746f 5f64  e.    nodes_to_d
+0000b4f0: 656c 6574 6520 3d20 5b6e 6f64 655b 226e  elete = [node["n
+0000b500: 616d 6522 5d5d 0a20 2020 2070 6f73 745f  ame"]].    post_
+0000b510: 6461 7461 203d 207b 226e 6f64 6573 223a  data = {"nodes":
+0000b520: 206e 6f64 6573 5f74 6f5f 6465 6c65 7465   nodes_to_delete
+0000b530: 7d0a 0a20 2020 2023 2053 746f 7020 6e6f  }..    # Stop no
+0000b540: 6465 2069 6620 6974 2069 7320 7275 6e6e  de if it is runn
+0000b550: 696e 670a 2020 2020 6966 206e 6f64 655f  ing.    if node_
+0000b560: 7374 6174 7573 2869 645f 6e6f 6465 2920  status(id_node) 
+0000b570: 3d3d 2022 5255 4e4e 494e 4722 3a0a 2020  == "RUNNING":.  
+0000b580: 2020 2020 2020 5f73 696d 756c 6174 696f        _simulatio
+0000b590: 6e5f 6578 6563 7574 655f 6f70 6572 6174  n_execute_operat
+0000b5a0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+0000b5b0: 2022 706f 7374 222c 0a20 2020 2020 2020   "post",.       
+0000b5c0: 2020 2020 2022 6861 6c74 222c 0a20 2020       "halt",.   
+0000b5d0: 2020 2020 2020 2020 2069 645f 7369 6d75           id_simu
+0000b5e0: 6c61 7469 6f6e 2c0a 2020 2020 2020 2020  lation,.        
+0000b5f0: 2020 2020 2253 544f 5050 494e 4722 2c0a      "STOPPING",.
+0000b600: 2020 2020 2020 2020 2020 2020 706f 7374              post
+0000b610: 5f64 6174 613d 706f 7374 5f64 6174 612c  _data=post_data,
+0000b620: 0a20 2020 2020 2020 2029 0a0a 0a64 6566  .        )...def
+0000b630: 2075 7064 6174 655f 7369 6d75 6c61 7469   update_simulati
+0000b640: 6f6e 2869 645f 7369 6d75 6c61 7469 6f6e  on(id_simulation
+0000b650: 3a20 696e 742c 2073 696d 756c 6174 696f  : int, simulatio
+0000b660: 6e5f 6469 6374 3a20 6469 6374 2920 2d3e  n_dict: dict) ->
+0000b670: 2041 6e79 3a0a 2020 2020 2222 2255 7064   Any:.    """Upd
+0000b680: 6174 6520 7369 6d75 6c61 7469 6f6e 2069  ate simulation i
+0000b690: 6e66 6f72 6d61 7469 6f6e 2069 6e66 6f72  nformation infor
+0000b6a0: 6d61 7469 6f6e 2067 6976 656e 2061 2073  mation given a s
+0000b6b0: 696d 756c 6174 696f 6e20 6964 0a20 2020  imulation id.   
+0000b6c0: 2061 6e64 2061 2064 6963 7420 636f 6e74   and a dict cont
+0000b6d0: 6169 6e69 6e67 2073 696d 756c 6174 696f  aining simulatio
+0000b6e0: 6e20 696e 666f 2e0a 2020 2020 2222 220a  n info..    """.
+0000b6f0: 2020 2020 6461 7461 203d 206a 736f 6e2e      data = json.
+0000b700: 6475 6d70 7328 7369 6d75 6c61 7469 6f6e  dumps(simulation
+0000b710: 5f64 6963 7429 0a20 2020 2072 6573 756c  _dict).    resul
+0000b720: 7420 3d20 5f70 7574 280a 2020 2020 2020  t = _put(.      
+0000b730: 2020 6622 2f73 696d 756c 6174 696f 6e2f    f"/simulation/
+0000b740: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d22  {id_simulation}"
+0000b750: 2c0a 2020 2020 2020 2020 6461 7461 3d64  ,.        data=d
+0000b760: 6174 612c 0a20 2020 2020 2020 2068 6561  ata,.        hea
+0000b770: 6465 7273 3d7b 2243 6f6e 7465 6e74 2d54  ders={"Content-T
+0000b780: 7970 6522 3a20 2261 7070 6c69 6361 7469  ype": "applicati
+0000b790: 6f6e 2f6a 736f 6e22 7d2c 0a20 2020 2029  on/json"},.    )
+0000b7a0: 0a0a 2020 2020 6966 2072 6573 756c 742e  ..    if result.
+0000b7b0: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
+0000b7c0: 3030 3a0a 2020 2020 2020 2020 5f68 616e  00:.        _han
+0000b7d0: 646c 655f 6572 726f 7228 7265 7375 6c74  dle_error(result
+0000b7e0: 2c20 2243 616e 6e6f 7420 7570 6461 7465  , "Cannot update
+0000b7f0: 2073 696d 756c 6174 696f 6e20 696e 666f   simulation info
+0000b800: 726d 6174 696f 6e22 290a 0a20 2020 2072  rmation")..    r
+0000b810: 6574 7572 6e20 7265 7375 6c74 2e6a 736f  eturn result.jso
+0000b820: 6e28 290a 0a0a 6465 6620 6665 7463 685f  n()...def fetch_
+0000b830: 7369 6d75 6c61 7469 6f6e 5f74 6f70 6f6c  simulation_topol
+0000b840: 6f67 7928 6964 5f73 696d 756c 6174 696f  ogy(id_simulatio
+0000b850: 6e3a 2069 6e74 2920 2d3e 2041 6e79 3a0a  n: int) -> Any:.
+0000b860: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+0000b870: 6520 746f 706f 6c6f 6779 206f 6620 6120  e topology of a 
+0000b880: 7369 6d75 6c61 7469 6f6e 2e22 2222 0a20  simulation.""". 
+0000b890: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
+0000b8a0: 2866 222f 7369 6d75 6c61 7469 6f6e 2f7b  (f"/simulation/{
+0000b8b0: 6964 5f73 696d 756c 6174 696f 6e7d 2f74  id_simulation}/t
+0000b8c0: 6f70 6f6c 6f67 7922 290a 0a20 2020 2069  opology")..    i
+0000b8d0: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
+0000b8e0: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
+0000b8f0: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
+0000b900: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
+0000b910: 6f74 2072 6574 7269 6576 6520 7369 6d75  ot retrieve simu
+0000b920: 6c61 7469 6f6e 2074 6f70 6f6c 6f67 7920  lation topology 
+0000b930: 696e 666f 2229 0a0a 2020 2020 7265 7475  info")..    retu
+0000b940: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
+0000b950: 0a0a 0a64 6566 2066 6574 6368 5f73 696d  ...def fetch_sim
+0000b960: 756c 6174 696f 6e5f 746f 706f 6c6f 6779  ulation_topology
+0000b970: 5f79 616d 6c28 6964 5f73 696d 756c 6174  _yaml(id_simulat
+0000b980: 696f 6e3a 2069 6e74 2920 2d3e 2041 6e79  ion: int) -> Any
+0000b990: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
+0000b9a0: 7468 6520 5941 4d4c 2074 6f70 6f6c 6f67  the YAML topolog
+0000b9b0: 7920 636f 6e74 656e 7420 6f66 2061 2073  y content of a s
+0000b9c0: 696d 756c 6174 696f 6e2e 2222 220a 2020  imulation.""".  
+0000b9d0: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
+0000b9e0: 6622 2f73 696d 756c 6174 696f 6e2f 7b69  f"/simulation/{i
+0000b9f0: 645f 7369 6d75 6c61 7469 6f6e 7d2f 746f  d_simulation}/to
+0000ba00: 706f 6c6f 6779 5f79 616d 6c22 290a 0a20  pology_yaml").. 
+0000ba10: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+0000ba20: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+0000ba30: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+0000ba40: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
+0000ba50: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
+0000ba60: 7369 6d75 6c61 7469 6f6e 2074 6f70 6f6c  simulation topol
+0000ba70: 6f67 7920 696e 666f 2229 0a0a 2020 2020  ogy info")..    
+0000ba80: 7265 7475 726e 2072 6573 756c 742e 6a73  return result.js
+0000ba90: 6f6e 2829 0a0a 0a64 6566 2066 6574 6368  on()...def fetch
+0000baa0: 5f61 7373 6574 7328 6964 5f73 696d 756c  _assets(id_simul
+0000bab0: 6174 696f 6e3a 2069 6e74 2920 2d3e 2041  ation: int) -> A
+0000bac0: 6e79 3a0a 2020 2020 2222 2252 6574 7572  ny:.    """Retur
+0000bad0: 6e20 7468 6520 6c69 7374 206f 6620 7468  n the list of th
+0000bae0: 6520 6173 7365 7473 0a20 2020 206f 6620  e assets.    of 
+0000baf0: 6120 6769 7665 6e20 7369 6d75 6c61 7469  a given simulati
+0000bb00: 6f6e 2e20 4974 2063 6f72 7265 7370 6f6e  on. It correspon
+0000bb10: 6473 2074 6f0a 2020 2020 7468 6520 6c69  ds to.    the li
+0000bb20: 7374 206f 6620 7468 6520 6e6f 6465 7320  st of the nodes 
+0000bb30: 7769 7468 2073 6f6d 6520 6164 6469 7469  with some additi
+0000bb40: 6f6e 616c 0a20 2020 2069 6e66 6f72 6d61  onal.    informa
+0000bb50: 7469 6f6e 2e0a 2020 2020 2222 220a 2020  tion..    """.  
+0000bb60: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
+0000bb70: 6622 2f73 696d 756c 6174 696f 6e2f 7b69  f"/simulation/{i
+0000bb80: 645f 7369 6d75 6c61 7469 6f6e 7d2f 6173  d_simulation}/as
+0000bb90: 7365 7473 2229 0a0a 2020 2020 6966 2072  sets")..    if r
+0000bba0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
+0000bbb0: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
+0000bbc0: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+0000bbd0: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
+0000bbe0: 7265 7472 6965 7665 2061 7373 6574 7320  retrieve assets 
+0000bbf0: 6672 6f6d 2063 6f72 6520 4150 4922 290a  from core API").
+0000bc00: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+0000bc10: 6c74 2e6a 736f 6e28 290a 0a0a 6465 6620  lt.json()...def 
+0000bc20: 6665 7463 685f 7377 6974 6368 5f62 795f  fetch_switch_by_
+0000bc30: 6e65 7477 6f72 6b5f 6964 2869 645f 7369  network_id(id_si
+0000bc40: 6d75 6c61 7469 6f6e 3a20 696e 742c 206e  mulation: int, n
+0000bc50: 6574 776f 726b 5f69 643a 2073 7472 2920  etwork_id: str) 
+0000bc60: 2d3e 2041 6e79 3a0a 2020 2020 2222 2252  -> Any:.    """R
+0000bc70: 6574 7572 6e20 6120 7377 6974 6368 2067  eturn a switch g
+0000bc80: 6976 656e 2069 7473 206e 6574 776f 726b  iven its network
+0000bc90: 5f69 6422 2222 0a0a 2020 2020 7265 7375  _id"""..    resu
+0000bca0: 6c74 203d 205f 6765 7428 6622 2f73 696d  lt = _get(f"/sim
+0000bcb0: 756c 6174 696f 6e2f 7b69 645f 7369 6d75  ulation/{id_simu
+0000bcc0: 6c61 7469 6f6e 7d2f 7377 6974 6368 2f7b  lation}/switch/{
+0000bcd0: 6e65 7477 6f72 6b5f 6964 7d22 290a 0a20  network_id}").. 
+0000bce0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+0000bcf0: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+0000bd00: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+0000bd10: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
+0000bd20: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
+0000bd30: 7369 6d75 6c61 7469 6f6e 2073 7769 7463  simulation switc
+0000bd40: 6820 6672 6f6d 2063 6f72 6520 4150 4922  h from core API"
+0000bd50: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
+0000bd60: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
+0000bd70: 6620 6665 7463 685f 6e6f 6465 286e 6f64  f fetch_node(nod
+0000bd80: 655f 6964 3a20 696e 7429 202d 3e20 416e  e_id: int) -> An
+0000bd90: 793a 0a20 2020 2022 2222 5265 7475 726e  y:.    """Return
+0000bda0: 2061 206e 6f64 6520 6769 7665 6e20 6974   a node given it
+0000bdb0: 7320 4944 2222 220a 2020 2020 7265 7375  s ID""".    resu
+0000bdc0: 6c74 203d 205f 6765 7428 6622 2f6e 6f64  lt = _get(f"/nod
+0000bdd0: 652f 7b6e 6f64 655f 6964 7d22 290a 0a20  e/{node_id}").. 
+0000bde0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+0000bdf0: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+0000be00: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+0000be10: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
+0000be20: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
+0000be30: 6e6f 6465 2066 726f 6d20 4954 2053 696d  node from IT Sim
+0000be40: 756c 6174 696f 6e20 4150 4922 290a 0a20  ulation API").. 
+0000be50: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0000be60: 2e6a 736f 6e28 290a 0a0a 6465 6620 6665  .json()...def fe
+0000be70: 7463 685f 6e6f 6465 5f62 795f 6e61 6d65  tch_node_by_name
+0000be80: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
+0000be90: 696e 742c 206e 6f64 655f 6e61 6d65 3a20  int, node_name: 
+0000bea0: 7374 7229 202d 3e20 416e 793a 0a20 2020  str) -> Any:.   
+0000beb0: 2022 2222 5265 7475 726e 2061 206e 6f64   """Return a nod
+0000bec0: 6520 6769 7665 6e20 6974 7320 6e61 6d65  e given its name
+0000bed0: 2222 220a 0a20 2020 2072 6573 756c 7420  """..    result 
+0000bee0: 3d20 5f67 6574 2866 222f 7369 6d75 6c61  = _get(f"/simula
+0000bef0: 7469 6f6e 2f7b 6964 5f73 696d 756c 6174  tion/{id_simulat
+0000bf00: 696f 6e7d 2f6e 6f64 652f 7b6e 6f64 655f  ion}/node/{node_
+0000bf10: 6e61 6d65 7d22 290a 0a20 2020 2069 6620  name}")..    if 
+0000bf20: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
+0000bf30: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
+0000bf40: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+0000bf50: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+0000bf60: 7375 6c74 2c20 2243 616e 6e6f 7420 7265  sult, "Cannot re
+0000bf70: 7472 6965 7665 206e 6f64 6520 6261 7365  trieve node base
+0000bf80: 6420 6f6e 2069 7473 206e 616d 6520 6672  d on its name fr
+0000bf90: 6f6d 2049 5420 5369 6d75 6c61 7469 6f6e  om IT Simulation
+0000bfa0: 2041 5049 220a 2020 2020 2020 2020 290a   API".        ).
+0000bfb0: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+0000bfc0: 6c74 2e6a 736f 6e28 290a 0a0a 6465 6620  lt.json()...def 
+0000bfd0: 6665 7463 685f 6e6f 6465 735f 6279 5f72  fetch_nodes_by_r
+0000bfe0: 6f6c 6573 2869 645f 7369 6d75 6c61 7469  oles(id_simulati
+0000bff0: 6f6e 3a20 696e 7429 202d 3e20 416e 793a  on: int) -> Any:
+0000c000: 0a20 2020 2022 2222 5265 7475 726e 2061  .    """Return a
+0000c010: 2064 6963 7420 776b 6572 6520 6b65 7973   dict wkere keys
+0000c020: 2061 7265 2072 6f6c 6573 2028 7375 6368   are roles (such
+0000c030: 2061 7320 2761 6427 2c20 2766 696c 655f   as 'ad', 'file_
+0000c040: 7365 7276 6572 272c 2027 636c 6965 6e74  server', 'client
+0000c050: 272c 202e 2e2e 2920 616e 640a 2020 2020  ', ...) and.    
+0000c060: 7661 6c75 6573 2061 7265 206e 6f64 6573  values are nodes
+0000c070: 2e0a 0a20 2020 2022 2222 0a20 2020 2072  ...    """.    r
+0000c080: 6573 756c 7420 3d20 5f67 6574 2866 222f  esult = _get(f"/
+0000c090: 7369 6d75 6c61 7469 6f6e 2f7b 6964 5f73  simulation/{id_s
+0000c0a0: 696d 756c 6174 696f 6e7d 2f6e 6f64 6573  imulation}/nodes
+0000c0b0: 5f62 795f 726f 6c65 7322 290a 0a20 2020  _by_roles")..   
+0000c0c0: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+0000c0d0: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+0000c0e0: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+0000c0f0: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
+0000c100: 6e6e 6f74 2072 6574 7269 6576 6520 6e6f  nnot retrieve no
+0000c110: 6465 7322 290a 0a20 2020 2072 6f6c 6573  des")..    roles
+0000c120: 5f64 6963 7420 3d20 7265 7375 6c74 2e6a  _dict = result.j
+0000c130: 736f 6e28 290a 2020 2020 7265 7475 726e  son().    return
+0000c140: 2072 6f6c 6573 5f64 6963 740a 0a0a 6465   roles_dict...de
+0000c150: 6620 6465 6c65 7465 5f6e 6f64 655f 6279  f delete_node_by
+0000c160: 5f6e 616d 6528 6964 5f73 696d 756c 6174  _name(id_simulat
+0000c170: 696f 6e3a 2069 6e74 2c20 6e6f 6465 5f6e  ion: int, node_n
+0000c180: 616d 653a 2073 7472 2920 2d3e 2041 6e79  ame: str) -> Any
+0000c190: 3a0a 2020 2020 2320 5265 7472 6965 7665  :.    # Retrieve
+0000c1a0: 2069 645f 6e6f 6465 0a20 2020 206e 6f64   id_node.    nod
+0000c1b0: 6520 3d20 6665 7463 685f 6e6f 6465 5f62  e = fetch_node_b
+0000c1c0: 795f 6e61 6d65 2869 645f 7369 6d75 6c61  y_name(id_simula
+0000c1d0: 7469 6f6e 2c20 6e6f 6465 5f6e 616d 6529  tion, node_name)
+0000c1e0: 0a20 2020 2069 645f 6e6f 6465 203d 206e  .    id_node = n
+0000c1f0: 6f64 655b 2269 6422 5d0a 0a20 2020 2023  ode["id"]..    #
+0000c200: 2044 656c 6574 6520 6e6f 6465 0a20 2020   Delete node.   
+0000c210: 2064 656c 6574 655f 6e6f 6465 2869 645f   delete_node(id_
+0000c220: 6e6f 6465 290a 0a0a 6465 6620 6465 6c65  node)...def dele
+0000c230: 7465 5f6e 6f64 6528 6964 5f6e 6f64 653a  te_node(id_node:
+0000c240: 2069 6e74 2920 2d3e 2041 6e79 3a0a 2020   int) -> Any:.  
+0000c250: 2020 2222 2244 656c 6574 6520 6e6f 6465    """Delete node
+0000c260: 2066 726f 6d20 6461 7461 6261 7365 2067   from database g
+0000c270: 6976 656e 2069 7473 2049 442e 2222 220a  iven its ID.""".
+0000c280: 0a20 2020 2023 2046 6574 6368 2076 6972  .    # Fetch vir
+0000c290: 7475 616c 206e 6f64 6520 6e65 7477 6f72  tual node networ
+0000c2a0: 6b20 696e 7465 7266 6163 6573 0a20 2020  k interfaces.   
+0000c2b0: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
+0000c2c0: 6365 7320 3d20 6665 7463 685f 6e6f 6465  ces = fetch_node
+0000c2d0: 5f6e 6574 776f 726b 5f69 6e74 6572 6661  _network_interfa
+0000c2e0: 6365 7328 6964 5f6e 6f64 6529 0a0a 2020  ces(id_node)..  
+0000c2f0: 2020 2320 4465 6c65 7465 2065 6163 6820    # Delete each 
+0000c300: 6e65 7477 6f72 6b20 696e 7465 7266 6163  network interfac
+0000c310: 6573 0a20 2020 2066 6f72 206e 6574 776f  es.    for netwo
+0000c320: 726b 5f69 6e74 6572 6661 6365 2069 6e20  rk_interface in 
+0000c330: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+0000c340: 6573 3a0a 2020 2020 2020 2020 6465 6c65  es:.        dele
+0000c350: 7465 5f6e 6574 776f 726b 5f69 6e74 6572  te_network_inter
+0000c360: 6661 6365 286e 6574 776f 726b 5f69 6e74  face(network_int
+0000c370: 6572 6661 6365 5b22 6964 225d 290a 0a20  erface["id"]).. 
+0000c380: 2020 2023 2044 656c 6574 6520 6e6f 6465     # Delete node
+0000c390: 0a20 2020 2072 6573 756c 7420 3d20 5f64  .    result = _d
+0000c3a0: 656c 6574 6528 6622 2f6e 6f64 652f 7b69  elete(f"/node/{i
+0000c3b0: 645f 6e6f 6465 7d22 290a 0a20 2020 2069  d_node}")..    i
+0000c3c0: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
+0000c3d0: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
+0000c3e0: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
+0000c3f0: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
+0000c400: 6f74 2064 656c 6574 6520 6e6f 6465 2229  ot delete node")
+0000c410: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+0000c420: 756c 742e 6a73 6f6e 2829 0a0a 0a64 6566  ult.json()...def
+0000c430: 2066 6574 6368 5f6e 6f64 6573 2869 645f   fetch_nodes(id_
+0000c440: 7369 6d75 6c61 7469 6f6e 3a20 696e 7429  simulation: int)
+0000c450: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
+0000c460: 5265 7475 726e 2073 696d 756c 6174 696f  Return simulatio
+0000c470: 6e20 6e6f 6465 7320 6469 6374 2067 6976  n nodes dict giv
+0000c480: 656e 0a20 2020 2061 2073 696d 756c 6174  en.    a simulat
+0000c490: 696f 6e20 4944 2c20 7768 6572 6520 6b65  ion ID, where ke
+0000c4a0: 7973 2061 7265 206e 6f64 6520 6e61 6d65  ys are node name
+0000c4b0: 732e 0a20 2020 2022 2222 0a20 2020 2072  s..    """.    r
+0000c4c0: 6573 756c 7420 3d20 5f67 6574 2866 222f  esult = _get(f"/
+0000c4d0: 7369 6d75 6c61 7469 6f6e 2f7b 6964 5f73  simulation/{id_s
+0000c4e0: 696d 756c 6174 696f 6e7d 2f6e 6f64 6522  imulation}/node"
+0000c4f0: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
+0000c500: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
+0000c510: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
+0000c520: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
+0000c530: 742c 2022 4361 6e6e 6f74 2072 6574 7269  t, "Cannot retri
+0000c540: 6576 6520 6e6f 6465 7320 6672 6f6d 2049  eve nodes from I
+0000c550: 5420 5369 6d75 6c61 7469 6f6e 2041 5049  T Simulation API
+0000c560: 2229 0a0a 2020 2020 7265 7475 726e 2072  ")..    return r
+0000c570: 6573 756c 742e 6a73 6f6e 2829 0a0a 0a64  esult.json()...d
+0000c580: 6566 2066 6574 6368 5f76 6972 7475 616c  ef fetch_virtual
+0000c590: 5f6d 6163 6869 6e65 7328 6964 5f73 696d  _machines(id_sim
+0000c5a0: 756c 6174 696f 6e3a 2069 6e74 2920 2d3e  ulation: int) ->
+0000c5b0: 204c 6973 745b 6469 6374 5d3a 0a20 2020   List[dict]:.   
+0000c5c0: 2022 2222 5265 7475 726e 2073 696d 756c   """Return simul
+0000c5d0: 6174 696f 6e20 7669 7274 7561 6c20 6d61  ation virtual ma
+0000c5e0: 6368 696e 6573 2064 6963 7420 6769 7665  chines dict give
+0000c5f0: 6e20 6120 7369 6d75 6c61 7469 6f6e 2049  n a simulation I
+0000c600: 442c 0a20 2020 2077 6865 7265 206b 6579  D,.    where key
+0000c610: 7320 6172 6520 7669 7274 7561 6c20 6d61  s are virtual ma
+0000c620: 6368 696e 6520 6e61 6d65 732e 0a20 2020  chine names..   
+0000c630: 2022 2222 0a20 2020 2072 6573 756c 7473   """.    results
+0000c640: 203d 2066 6574 6368 5f6e 6f64 6573 2869   = fetch_nodes(i
+0000c650: 645f 7369 6d75 6c61 7469 6f6e 290a 0a20  d_simulation).. 
+0000c660: 2020 2076 6d5f 6f6e 6c79 203d 2066 696c     vm_only = fil
+0000c670: 7465 7228 6c61 6d62 6461 206d 3a20 6d5b  ter(lambda m: m[
+0000c680: 2274 7970 6522 5d20 3d3d 2022 7669 7274  "type"] == "virt
+0000c690: 7561 6c5f 6d61 6368 696e 6522 2c20 7265  ual_machine", re
+0000c6a0: 7375 6c74 7329 0a20 2020 2072 6574 7572  sults).    retur
+0000c6b0: 6e20 6c69 7374 2876 6d5f 6f6e 6c79 290a  n list(vm_only).
+0000c6c0: 0a0a 6465 6620 6465 6c65 7465 5f6e 6f64  ..def delete_nod
+0000c6d0: 6573 2869 645f 7369 6d75 6c61 7469 6f6e  es(id_simulation
+0000c6e0: 3a20 696e 7429 202d 3e20 7374 723a 0a20  : int) -> str:. 
+0000c6f0: 2020 2022 2222 4465 6c65 7465 2073 696d     """Delete sim
+0000c700: 756c 6174 696f 6e20 6e6f 6465 7320 6769  ulation nodes gi
+0000c710: 7665 6e20 6120 7369 6d75 6c61 7469 6f6e  ven a simulation
+0000c720: 2049 442e 2222 220a 0a20 2020 2023 2046   ID."""..    # F
+0000c730: 6574 6368 2073 696d 756c 6174 696f 6e20  etch simulation 
+0000c740: 6e6f 6465 730a 2020 2020 7265 7375 6c74  nodes.    result
+0000c750: 203d 205f 6765 7428 6622 2f73 696d 756c   = _get(f"/simul
+0000c760: 6174 696f 6e2f 7b69 645f 7369 6d75 6c61  ation/{id_simula
+0000c770: 7469 6f6e 7d2f 6e6f 6465 2229 0a0a 2020  tion}/node")..  
+0000c780: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
+0000c790: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
+0000c7a0: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
+0000c7b0: 6572 726f 7228 7265 7375 6c74 2c20 2243  error(result, "C
+0000c7c0: 616e 6e6f 7420 6465 6c65 7465 2073 696d  annot delete sim
+0000c7d0: 756c 6174 696f 6e20 6e6f 6465 7322 290a  ulation nodes").
+0000c7e0: 0a20 2020 206e 6f64 6573 5f6c 6973 7420  .    nodes_list 
+0000c7f0: 3d20 7265 7375 6c74 2e6a 736f 6e28 290a  = result.json().
+0000c800: 0a20 2020 2023 2044 656c 6574 6520 6561  .    # Delete ea
+0000c810: 6368 206e 6f64 650a 2020 2020 666f 7220  ch node.    for 
+0000c820: 6e6f 6465 2069 6e20 6e6f 6465 735f 6c69  node in nodes_li
+0000c830: 7374 3a0a 2020 2020 2020 2020 6465 6c65  st:.        dele
+0000c840: 7465 5f6e 6f64 6528 6e6f 6465 5b22 6964  te_node(node["id
+0000c850: 225d 290a 0a20 2020 2072 6573 756c 745f  "])..    result_
+0000c860: 6a73 6f6e 203d 2022 7b7d 220a 2020 2020  json = "{}".    
+0000c870: 7265 7475 726e 2072 6573 756c 745f 6a73  return result_js
+0000c880: 6f6e 0a0a 0a64 6566 2075 7064 6174 655f  on...def update_
+0000c890: 6e6f 6465 286e 6f64 655f 6964 3a20 696e  node(node_id: in
+0000c8a0: 742c 206e 6f64 655f 6469 6374 3a20 6469  t, node_dict: di
+0000c8b0: 6374 2920 2d3e 2041 6e79 3a0a 2020 2020  ct) -> Any:.    
+0000c8c0: 2222 2255 7064 6174 6520 6e6f 6465 2069  """Update node i
+0000c8d0: 6e66 6f72 6d61 7469 6f6e 2067 6976 656e  nformation given
+0000c8e0: 2061 206e 6f64 6520 6964 2061 6e64 2061   a node id and a
+0000c8f0: 2064 6963 7420 636f 6e74 6169 6e69 6e67   dict containing
+0000c900: 0a20 2020 206e 6f64 6520 6461 7461 2e0a  .    node data..
+0000c910: 2020 2020 2222 220a 2020 2020 6461 7461      """.    data
+0000c920: 203d 206a 736f 6e2e 6475 6d70 7328 6e6f   = json.dumps(no
+0000c930: 6465 5f64 6963 7429 0a20 2020 2072 6573  de_dict).    res
+0000c940: 756c 7420 3d20 5f70 7574 280a 2020 2020  ult = _put(.    
+0000c950: 2020 2020 6622 2f6e 6f64 652f 7b6e 6f64      f"/node/{nod
+0000c960: 655f 6964 7d22 2c0a 2020 2020 2020 2020  e_id}",.        
+0000c970: 6461 7461 3d64 6174 612c 0a20 2020 2020  data=data,.     
+0000c980: 2020 2068 6561 6465 7273 3d7b 2243 6f6e     headers={"Con
+0000c990: 7465 6e74 2d54 7970 6522 3a20 2261 7070  tent-Type": "app
+0000c9a0: 6c69 6361 7469 6f6e 2f6a 736f 6e22 7d2c  lication/json"},
+0000c9b0: 0a20 2020 2029 0a0a 2020 2020 6966 2072  .    )..    if r
+0000c9c0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
+0000c9d0: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
+0000c9e0: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+0000c9f0: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
+0000ca00: 7570 6461 7465 206e 6f64 6520 696e 666f  update node info
+0000ca10: 726d 6174 696f 6e20 7769 7468 2063 6f72  rmation with cor
+0000ca20: 6520 4150 4922 290a 0a20 2020 2072 6574  e API")..    ret
+0000ca30: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
+0000ca40: 290a 0a0a 6465 6620 6765 745f 6e6f 6465  )...def get_node
+0000ca50: 5f64 6566 6175 6c74 5f67 6174 6577 6179  _default_gateway
+0000ca60: 2869 645f 6e6f 6465 3a20 696e 7429 202d  (id_node: int) -
+0000ca70: 3e20 4f70 7469 6f6e 616c 5b73 7472 5d3a  > Optional[str]:
+0000ca80: 0a20 2020 2022 2222 5265 7472 6965 7665  .    """Retrieve
+0000ca90: 206e 6f64 6520 6465 6661 756c 7420 6761   node default ga
+0000caa0: 7465 7761 792c 2077 6869 6368 2063 616e  teway, which can
+0000cab0: 2065 6974 6865 7220 6265 2061 6e20 4950   either be an IP
+0000cac0: 2061 6464 7265 7373 0a20 2020 206f 6620   address.    of 
+0000cad0: 7468 6520 666f 726d 2078 782e 7878 2e78  the form xx.xx.x
+0000cae0: 782e 7878 206f 7220 4e6f 6e65 2069 6620  x.xx or None if 
+0000caf0: 6e6f 2067 6174 6577 6179 2069 7320 7365  no gateway is se
+0000cb00: 742e 0a0a 2020 2020 2222 220a 0a20 2020  t...    """..   
+0000cb10: 2072 6573 756c 7420 3d20 5f67 6574 2866   result = _get(f
+0000cb20: 222f 6e6f 6465 2f7b 6964 5f6e 6f64 657d  "/node/{id_node}
+0000cb30: 2f64 6566 6175 6c74 5f67 6174 6577 6179  /default_gateway
+0000cb40: 2229 0a0a 2020 2020 6966 2072 6573 756c  ")..    if resul
+0000cb50: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
+0000cb60: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
+0000cb70: 616e 646c 655f 6572 726f 7228 0a20 2020  andle_error(.   
+0000cb80: 2020 2020 2020 2020 2072 6573 756c 742c           result,
+0000cb90: 2022 4361 6e6e 6f74 2072 6574 7269 6576   "Cannot retriev
+0000cba0: 6520 6e6f 6465 2064 6566 6175 6c74 2067  e node default g
+0000cbb0: 6174 6577 6179 2066 726f 6d20 4954 2053  ateway from IT S
+0000cbc0: 696d 756c 6174 696f 6e20 4150 4922 0a20  imulation API". 
+0000cbd0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+0000cbe0: 6661 756c 745f 6761 7465 7761 7920 3d20  fault_gateway = 
+0000cbf0: 7265 7375 6c74 2e6a 736f 6e28 290a 0a20  result.json().. 
+0000cc00: 2020 2072 6574 7572 6e20 6465 6661 756c     return defaul
+0000cc10: 745f 6761 7465 7761 790a 0a0a 6465 6620  t_gateway...def 
+0000cc20: 6765 745f 6e6f 6465 5f73 7461 7469 7374  get_node_statist
+0000cc30: 6963 735f 6279 5f69 6428 6964 5f6e 6f64  ics_by_id(id_nod
+0000cc40: 653a 2069 6e74 2920 2d3e 2041 6e79 3a0a  e: int) -> Any:.
+0000cc50: 2020 2020 2222 220a 2020 2020 5265 7475      """.    Retu
+0000cc60: 726e 2061 6767 7265 6761 7465 6420 7374  rn aggregated st
+0000cc70: 6174 6973 7469 6373 2066 726f 6d20 4350  atistics from CP
+0000cc80: 552c 206d 656d 6f72 792c 2062 6c6f 636b  U, memory, block
+0000cc90: 2064 6576 6963 6573 2061 6e64 206e 6574   devices and net
+0000cca0: 776f 726b 2069 6e74 6572 6661 6365 732e  work interfaces.
+0000ccb0: 0a20 2020 204e 6f74 653a 2079 6f75 2063  .    Note: you c
+0000ccc0: 616e 2067 6574 2074 6865 206e 6f64 6520  an get the node 
+0000ccd0: 4944 7320 7573 696e 6720 7468 6520 7369  IDs using the si
+0000cce0: 6d75 5f73 7461 7475 7320 636f 6d6d 616e  mu_status comman
+0000ccf0: 6420 286f 7220 7468 6520 6665 7463 685f  d (or the fetch_
+0000cd00: 7369 6d75 6c61 7469 6f6e 7328 2920 6675  simulations() fu
+0000cd10: 6e63 7469 6f6e 292e 0a20 2020 2022 2222  nction)..    """
+0000cd20: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
+0000cd30: 6574 2866 222f 6e6f 6465 2f7b 6964 5f6e  et(f"/node/{id_n
+0000cd40: 6f64 657d 2f73 7461 7473 2229 0a0a 2020  ode}/stats")..  
+0000cd50: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
+0000cd60: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
+0000cd70: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
+0000cd80: 6572 726f 7228 7265 7375 6c74 2c20 2243  error(result, "C
+0000cd90: 616e 6e6f 7420 7265 7472 6965 7665 206e  annot retrieve n
+0000cda0: 6f64 6520 7374 6174 6973 7469 6373 2229  ode statistics")
+0000cdb0: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+0000cdc0: 756c 742e 6a73 6f6e 2829 0a0a 0a64 6566  ult.json()...def
+0000cdd0: 206e 6f64 655f 6c6f 6773 2869 645f 6e6f   node_logs(id_no
+0000cde0: 6465 3a20 696e 7429 202d 3e20 416e 793a  de: int) -> Any:
+0000cdf0: 0a20 2020 2022 2222 0a20 2020 2052 6574  .    """.    Ret
+0000ce00: 7269 6576 6520 6c6f 6773 2066 726f 6d20  rieve logs from 
+0000ce10: 7370 6563 6966 6965 6420 6e6f 6465 2028  specified node (
+0000ce20: 6f6e 6c79 2077 6f72 6b20 666f 7220 446f  only work for Do
+0000ce30: 636b 6572 206e 6f64 6529 2e0a 0a20 2020  cker node)...   
+0000ce40: 2052 6574 7572 6e20 7468 6520 6c6f 6773   Return the logs
+0000ce50: 2073 7472 696e 672e 0a20 2020 2022 2222   string..    """
+0000ce60: 0a0a 2020 2020 2320 4368 6563 6b20 7468  ..    # Check th
+0000ce70: 6174 2074 6865 2074 6172 6765 7420 6e6f  at the target no
+0000ce80: 6465 2069 7320 6120 646f 636b 6572 206e  de is a docker n
+0000ce90: 6f64 6520 286e 6f64 655f 6578 6563 206f  ode (node_exec o
+0000cea0: 6e6c 790a 2020 2020 2320 776f 726b 7320  nly.    # works 
+0000ceb0: 666f 7220 446f 636b 6572 206e 6f64 6520  for Docker node 
+0000cec0: 666f 7220 6e6f 7729 0a20 2020 206e 6f64  for now).    nod
+0000ced0: 6520 3d20 6665 7463 685f 6e6f 6465 2869  e = fetch_node(i
+0000cee0: 645f 6e6f 6465 290a 2020 2020 6966 206e  d_node).    if n
+0000cef0: 6f64 655b 2274 7970 6522 5d20 213d 2022  ode["type"] != "
+0000cf00: 646f 636b 6572 223a 0a20 2020 2020 2020  docker":.       
+0000cf10: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+0000cf20: 2822 4361 6e6e 6f74 2065 7865 6375 7465  ("Cannot execute
+0000cf30: 2063 6f6d 6d61 6e64 2066 6f72 206e 6f64   command for nod
+0000cf40: 6573 2064 6966 6665 7265 6e74 2066 726f  es different fro
+0000cf50: 6d20 646f 636b 6572 206e 6f64 6573 2229  m docker nodes")
+0000cf60: 0a0a 2020 2020 7265 7375 6c74 203d 205f  ..    result = _
+0000cf70: 6765 7428 6622 2f6e 6f64 652f 7b69 645f  get(f"/node/{id_
+0000cf80: 6e6f 6465 7d2f 6c6f 6773 2229 0a0a 2020  node}/logs")..  
+0000cf90: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
+0000cfa0: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
+0000cfb0: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
+0000cfc0: 6572 726f 7228 7265 7375 6c74 2c20 2243  error(result, "C
+0000cfd0: 616e 6e6f 7420 7265 7472 6965 7665 206c  annot retrieve l
+0000cfe0: 6f67 7320 6672 6f6d 2049 5420 5369 6d75  ogs from IT Simu
+0000cff0: 6c61 7469 6f6e 2041 5049 2229 0a0a 2020  lation API")..  
+0000d000: 2020 6c6f 6773 203d 2072 6573 756c 742e    logs = result.
+0000d010: 6a73 6f6e 2829 0a0a 2020 2020 7265 7475  json()..    retu
+0000d020: 726e 206c 6f67 730a 0a0a 6465 6620 6e6f  rn logs...def no
+0000d030: 6465 5f65 7865 6328 6964 5f6e 6f64 653a  de_exec(id_node:
+0000d040: 2069 6e74 2c20 636f 6d6d 616e 643a 2073   int, command: s
+0000d050: 7472 2920 2d3e 2041 6e79 3a0a 2020 2020  tr) -> Any:.    
+0000d060: 2222 220a 2020 2020 4578 6563 7574 6520  """.    Execute 
+0000d070: 6120 636f 6d6d 616e 6420 6f6e 2073 7065  a command on spe
+0000d080: 6369 6669 6564 206e 6f64 6520 286f 6e6c  cified node (onl
+0000d090: 7920 776f 726b 2066 6f72 2044 6f63 6b65  y work for Docke
+0000d0a0: 7220 6e6f 6465 292e 0a0a 2020 2020 5265  r node)...    Re
+0000d0b0: 7475 726e 2061 2074 7570 6c65 2028 6578  turn a tuple (ex
+0000d0c0: 6974 5f63 6f64 653a 2069 6e74 2c20 7374  it_code: int, st
+0000d0d0: 646f 7574 3a20 7374 722c 2073 7464 6572  dout: str, stder
+0000d0e0: 723a 2073 7472 2920 6f66 2074 6865 2065  r: str) of the e
+0000d0f0: 7865 6375 7465 6420 636f 6d6d 616e 642e  xecuted command.
+0000d100: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
+0000d110: 4368 6563 6b20 7468 6174 2074 6865 2074  Check that the t
+0000d120: 6172 6765 7420 6e6f 6465 2069 7320 6120  arget node is a 
+0000d130: 646f 636b 6572 206e 6f64 6520 286e 6f64  docker node (nod
+0000d140: 655f 6578 6563 206f 6e6c 790a 2020 2020  e_exec only.    
+0000d150: 2320 776f 726b 7320 666f 7220 446f 636b  # works for Dock
+0000d160: 6572 206e 6f64 6520 666f 7220 6e6f 7729  er node for now)
+0000d170: 0a20 2020 206e 6f64 6520 3d20 6665 7463  .    node = fetc
+0000d180: 685f 6e6f 6465 2869 645f 6e6f 6465 290a  h_node(id_node).
+0000d190: 2020 2020 6966 206e 6f64 655b 2274 7970      if node["typ
+0000d1a0: 6522 5d20 213d 2022 646f 636b 6572 223a  e"] != "docker":
+0000d1b0: 0a20 2020 2020 2020 2072 6169 7365 2045  .        raise E
+0000d1c0: 7863 6570 7469 6f6e 2822 4361 6e6e 6f74  xception("Cannot
+0000d1d0: 2065 7865 6375 7465 2063 6f6d 6d61 6e64   execute command
+0000d1e0: 2066 6f72 206e 6f64 6573 2064 6966 6665   for nodes diffe
+0000d1f0: 7265 6e74 2066 726f 6d20 646f 636b 6572  rent from docker
+0000d200: 206e 6f64 6573 2229 0a0a 2020 2020 7374   nodes")..    st
+0000d210: 6174 7573 5f6b 6579 203d 2022 7374 6174  atus_key = "stat
+0000d220: 7573 220a 2020 2020 6578 6974 5f63 6f64  us".    exit_cod
+0000d230: 6520 3d20 2265 7869 745f 636f 6465 220a  e = "exit_code".
+0000d240: 2020 2020 7374 646f 7574 203d 2022 7374      stdout = "st
+0000d250: 646f 7574 220a 2020 2020 7374 6465 7272  dout".    stderr
+0000d260: 203d 2022 7374 6465 7272 220a 0a20 2020   = "stderr"..   
+0000d270: 2070 6f73 745f 6461 7461 203d 207b 2263   post_data = {"c
+0000d280: 6f6d 6d61 6e64 223a 2063 6f6d 6d61 6e64  ommand": command
+0000d290: 7d0a 2020 2020 6461 7461 203d 206a 736f  }.    data = jso
+0000d2a0: 6e2e 6475 6d70 7328 706f 7374 5f64 6174  n.dumps(post_dat
+0000d2b0: 6129 0a20 2020 2072 6573 756c 7420 3d20  a).    result = 
+0000d2c0: 5f70 6f73 7428 0a20 2020 2020 2020 2066  _post(.        f
+0000d2d0: 222f 6e6f 6465 2f7b 6964 5f6e 6f64 657d  "/node/{id_node}
+0000d2e0: 2f65 7865 6322 2c20 6461 7461 3d64 6174  /exec", data=dat
+0000d2f0: 612c 2068 6561 6465 7273 3d7b 2243 6f6e  a, headers={"Con
+0000d300: 7465 6e74 2d54 7970 6522 3a20 2261 7070  tent-Type": "app
+0000d310: 6c69 6361 7469 6f6e 2f6a 736f 6e22 7d0a  lication/json"}.
+0000d320: 2020 2020 290a 0a20 2020 2069 6620 280a      )..    if (.
+0000d330: 2020 2020 2020 2020 7265 7375 6c74 2e73          result.s
+0000d340: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+0000d350: 300a 2020 2020 2020 2020 6f72 2073 7461  0.        or sta
+0000d360: 7475 735f 6b65 7920 6e6f 7420 696e 2072  tus_key not in r
+0000d370: 6573 756c 742e 6a73 6f6e 2829 0a20 2020  esult.json().   
+0000d380: 2020 2020 206f 7220 7265 7375 6c74 2e6a       or result.j
+0000d390: 736f 6e28 295b 7374 6174 7573 5f6b 6579  son()[status_key
+0000d3a0: 5d20 213d 2022 5354 4152 5445 4422 0a20  ] != "STARTED". 
+0000d3b0: 2020 2029 3a0a 2020 2020 2020 2020 5f68     ):.        _h
+0000d3c0: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
+0000d3d0: 6c74 2c20 2243 616e 6e6f 7420 696e 6974  lt, "Cannot init
+0000d3e0: 6961 7465 2065 7865 6320 636f 6d6d 616e  iate exec comman
+0000d3f0: 6420 6672 6f6d 2049 5420 5369 6d75 6c61  d from IT Simula
+0000d400: 7469 6f6e 2041 5049 2229 0a0a 2020 2020  tion API")..    
+0000d410: 6c6f 6767 6572 2e69 6e66 6f28 6622 5b2b  logger.info(f"[+
+0000d420: 5d20 4578 6563 7574 696e 6720 636f 6d6d  ] Executing comm
+0000d430: 616e 6420 277b 636f 6d6d 616e 647d 2720  and '{command}' 
+0000d440: 666f 7220 6e6f 6465 2027 7b69 645f 6e6f  for node '{id_no
+0000d450: 6465 7d27 2e2e 2e22 290a 0a20 2020 2023  de}'...")..    #
+0000d460: 2057 6169 7420 666f 7220 7468 6520 6f70   Wait for the op
+0000d470: 6572 6174 696f 6e20 746f 2062 6520 636f  eration to be co
+0000d480: 6d70 6c65 7465 6420 696e 2062 6163 6b65  mpleted in backe
+0000d490: 6e64 0a20 2020 2023 204e 6f74 6520 3a20  nd.    # Note : 
+0000d4a0: 6c6f 6f70 2069 6e73 7069 7265 6420 6672  loop inspired fr
+0000d4b0: 6f6d 205f 7369 6d75 6c61 7469 6f6e 5f65  om _simulation_e
+0000d4c0: 7865 6375 7465 5f6f 7065 7261 7469 6f6e  xecute_operation
+0000d4d0: 0a20 2020 2077 6869 6c65 2054 7275 653a  .    while True:
+0000d4e0: 0a20 2020 2020 2020 2023 2053 6c65 6570  .        # Sleep
+0000d4f0: 2062 6566 6f72 6520 6e65 7874 2069 7465   before next ite
+0000d500: 7261 7469 6f6e 0a20 2020 2020 2020 2074  ration.        t
+0000d510: 696d 652e 736c 6565 7028 3229 0a0a 2020  ime.sleep(2)..  
+0000d520: 2020 2020 2020 2320 4665 7463 6820 7468        # Fetch th
+0000d530: 6520 6375 7272 656e 7420 7374 6174 7573  e current status
+0000d540: 206f 6620 7468 6520 6d65 6d64 756d 700a   of the memdump.
+0000d550: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0000d560: 205f 6765 7428 6622 2f6e 6f64 652f 7b69   _get(f"/node/{i
+0000d570: 645f 6e6f 6465 7d2f 6578 6563 5f73 7461  d_node}/exec_sta
+0000d580: 7475 7322 290a 0a20 2020 2020 2020 2069  tus")..        i
+0000d590: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
+0000d5a0: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
+0000d5b0: 2020 2020 2020 2020 205f 6861 6e64 6c65           _handle
+0000d5c0: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
+0000d5d0: 2020 2020 2020 2020 7265 7375 6c74 2c20          result, 
+0000d5e0: 2243 616e 6e6f 7420 6765 7420 7374 6174  "Cannot get stat
+0000d5f0: 7573 206f 6620 6578 6563 2063 6f6d 6d61  us of exec comma
+0000d600: 6e64 2066 726f 6d20 4954 2053 696d 756c  nd from IT Simul
+0000d610: 6174 696f 6e20 4150 4922 0a20 2020 2020  ation API".     
+0000d620: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000d630: 2020 7265 7375 6c74 5f6a 736f 6e20 3d20    result_json = 
+0000d640: 7265 7375 6c74 2e6a 736f 6e28 290a 2020  result.json().  
+0000d650: 2020 2020 2020 6966 206e 6f74 2028 616c        if not (al
+0000d660: 6c28 6b20 696e 2072 6573 756c 745f 6a73  l(k in result_js
+0000d670: 6f6e 2066 6f72 206b 2069 6e20 2865 7869  on for k in (exi
+0000d680: 745f 636f 6465 2c20 7374 646f 7574 2c20  t_code, stdout, 
+0000d690: 7374 6465 7272 2c20 7374 6174 7573 5f6b  stderr, status_k
+0000d6a0: 6579 2929 293a 0a20 2020 2020 2020 2020  ey))):.         
+0000d6b0: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+0000d6c0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+0000d6d0: 2020 2020 6622 436f 6e74 656e 7473 206f      f"Contents o
+0000d6e0: 6620 6578 6563 2063 6f6d 6d61 6e64 2073  f exec command s
+0000d6f0: 7461 7475 7320 7570 6461 7465 2069 7320  tatus update is 
+0000d700: 6e6f 7420 696e 2074 6865 2065 7870 6563  not in the expec
+0000d710: 7465 6420 666f 726d 6174 2028 6174 7472  ted format (attr
+0000d720: 6962 7574 6573 2027 7b65 7869 745f 636f  ibutes '{exit_co
+0000d730: 6465 7d27 2c20 277b 7374 646f 7574 7d27  de}', '{stdout}'
+0000d740: 2c20 277b 7374 6465 7272 7d27 2061 6e64  , '{stderr}' and
+0000d750: 2027 7b73 7461 7475 735f 6b65 797d 2720   '{status_key}' 
+0000d760: 6578 7065 6374 6564 2922 0a20 2020 2020  expected)".     
+0000d770: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000d780: 2020 2320 4c6f 6720 696e 666f 206f 6e20    # Log info on 
+0000d790: 7072 6f67 7265 7373 696f 6e0a 2020 2020  progression.    
+0000d7a0: 2020 2020 6966 2072 6573 756c 745f 6a73      if result_js
+0000d7b0: 6f6e 5b73 7461 7475 735f 6b65 795d 203d  on[status_key] =
+0000d7c0: 3d20 2253 5441 5254 4544 223a 0a20 2020  = "STARTED":.   
+0000d7d0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000d7e0: 696e 666f 280a 2020 2020 2020 2020 2020  info(.          
+0000d7f0: 2020 2020 2020 6622 2020 5b2b 5d20 4375        f"  [+] Cu
+0000d800: 7272 656e 746c 7920 7761 6974 696e 6720  rrently waiting 
+0000d810: 666f 7220 6578 6563 2063 6f6d 6d61 6e64  for exec command
+0000d820: 2066 6f72 206e 6f64 6520 277b 6964 5f6e   for node '{id_n
+0000d830: 6f64 657d 2729 2074 6f20 7374 6172 742e  ode}') to start.
+0000d840: 2e2e 220a 2020 2020 2020 2020 2020 2020  ..".            
+0000d850: 290a 2020 2020 2020 2020 656c 6966 2072  ).        elif r
+0000d860: 6573 756c 745f 6a73 6f6e 5b73 7461 7475  esult_json[statu
+0000d870: 735f 6b65 795d 203d 3d20 2250 524f 4752  s_key] == "PROGR
+0000d880: 4553 5322 3a0a 2020 2020 2020 2020 2020  ESS":.          
+0000d890: 2020 6c6f 6767 6572 2e69 6e66 6f28 0a20    logger.info(. 
+0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000d8b0: 2220 205b 2b5d 2043 7572 7265 6e74 6c79  "  [+] Currently
+0000d8c0: 2070 6572 666f 726d 696e 6720 6578 6563   performing exec
+0000d8d0: 2063 6f6d 6d61 6e64 2066 6f72 206e 6f64   command for nod
+0000d8e0: 6520 277b 6964 5f6e 6f64 657d 2729 2e2e  e '{id_node}')..
+0000d8f0: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
+0000d900: 0a20 2020 2020 2020 2065 6c69 6620 7265  .        elif re
+0000d910: 7375 6c74 5f6a 736f 6e5b 7374 6174 7573  sult_json[status
+0000d920: 5f6b 6579 5d20 3d3d 2022 5355 4343 4553  _key] == "SUCCES
+0000d930: 5322 3a0a 2020 2020 2020 2020 2020 2020  S":.            
+0000d940: 6272 6561 6b0a 2020 2020 2020 2020 656c  break.        el
+0000d950: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000d960: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+0000d970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d980: 2022 4572 726f 7220 6475 7269 6e67 2065   "Error during e
+0000d990: 7865 6320 636f 6d6d 616e 6420 666f 7220  xec command for 
+0000d9a0: 6e6f 6465 207b 7d20 6f70 6572 6174 696f  node {} operatio
+0000d9b0: 6e3a 2027 7b7d 2722 2e66 6f72 6d61 7428  n: '{}'".format(
+0000d9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d9d0: 2020 2020 2069 645f 6e6f 6465 2c20 7265       id_node, re
+0000d9e0: 7375 6c74 5f6a 736f 6e5b 7374 6174 7573  sult_json[status
+0000d9f0: 5f6b 6579 5d0a 2020 2020 2020 2020 2020  _key].          
+0000da00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000da10: 2020 2020 290a 0a20 2020 206c 6f67 6765      )..    logge
+0000da20: 722e 696e 666f 2822 5b2b 5d20 4e6f 6465  r.info("[+] Node
+0000da30: 2065 7865 6320 636f 6d6d 616e 6420 6669   exec command fi
+0000da40: 6e69 7368 6564 2229 0a0a 2020 2020 7265  nished")..    re
+0000da50: 7475 726e 2028 7265 7375 6c74 5f6a 736f  turn (result_jso
+0000da60: 6e5b 6578 6974 5f63 6f64 655d 2c20 7265  n[exit_code], re
+0000da70: 7375 6c74 5f6a 736f 6e5b 7374 646f 7574  sult_json[stdout
+0000da80: 5d2c 2072 6573 756c 745f 6a73 6f6e 5b73  ], result_json[s
+0000da90: 7464 6572 725d 290a 0a0a 6465 6620 6e6f  tderr])...def no
+0000daa0: 6465 5f6d 656d 6f72 7964 756d 7028 6964  de_memorydump(id
+0000dab0: 5f6e 6f64 653a 2069 6e74 2920 2d3e 2041  _node: int) -> A
+0000dac0: 6e79 3a0a 2020 2020 2222 220a 2020 2020  ny:.    """.    
+0000dad0: 5265 7475 726e 2052 414d 2064 756d 7020  Return RAM dump 
+0000dae0: 6f66 2061 206e 6f64 6520 696e 2061 2072  of a node in a r
+0000daf0: 756e 6e69 6e67 2073 696d 756c 6174 696f  unning simulatio
+0000db00: 6e0a 2020 2020 4e6f 7465 3a20 796f 7520  n.    Note: you 
+0000db10: 6361 6e20 6765 7420 7468 6520 6e6f 6465  can get the node
+0000db20: 2049 4473 2075 7369 6e67 2074 6865 2073   IDs using the s
+0000db30: 696d 755f 7374 6174 7573 2063 6f6d 6d61  imu_status comma
+0000db40: 6e64 2028 6f72 2074 6865 2066 6574 6368  nd (or the fetch
+0000db50: 5f73 696d 756c 6174 696f 6e73 2829 2066  _simulations() f
+0000db60: 756e 6374 696f 6e29 2e0a 2020 2020 2222  unction)..    ""
+0000db70: 220a 0a20 2020 2023 2320 544f 444f 3a20  "..    ## TODO: 
+0000db80: 696d 706c 656d 656e 7420 7468 6973 206f  implement this o
+0000db90: 7065 7261 7469 6f6e 2069 6e20 4150 4920  peration in API 
+0000dba0: 6261 636b 656e 640a 2020 2020 7261 6973  backend.    rais
+0000dbb0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+0000dbc0: 4572 726f 7228 290a 0a20 2020 2023 2066  Error()..    # f
+0000dbd0: 696c 655f 7061 7468 5f6b 6579 203d 2022  ile_path_key = "
+0000dbe0: 6669 6c65 5f70 6174 6822 0a20 2020 2023  file_path".    #
+0000dbf0: 2066 696c 655f 7369 7a65 5f6b 6579 203d   file_size_key =
+0000dc00: 2022 6669 6c65 5f73 697a 6522 0a20 2020   "file_size".   
+0000dc10: 2023 2073 7461 7475 735f 6b65 7920 3d20   # status_key = 
+0000dc20: 2273 7461 7475 7322 0a0a 2020 2020 2320  "status"..    # 
+0000dc30: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
+0000dc40: 2f6e 6f64 652f 7b69 645f 6e6f 6465 7d2f  /node/{id_node}/
+0000dc50: 6d65 6d6f 7279 6475 6d70 2229 0a0a 2020  memorydump")..  
+0000dc60: 2020 2320 6966 2028 0a20 2020 2023 2020    # if (.    #  
+0000dc70: 2020 2072 6573 756c 742e 7374 6174 7573     result.status
+0000dc80: 5f63 6f64 6520 213d 2032 3030 0a20 2020  _code != 200.   
+0000dc90: 2023 2020 2020 206f 7220 7374 6174 7573   #     or status
+0000dca0: 5f6b 6579 206e 6f74 2069 6e20 7265 7375  _key not in resu
+0000dcb0: 6c74 2e6a 736f 6e28 290a 2020 2020 2320  lt.json().    # 
+0000dcc0: 2020 2020 6f72 2072 6573 756c 742e 6a73      or result.js
+0000dcd0: 6f6e 2829 5b73 7461 7475 735f 6b65 795d  on()[status_key]
+0000dce0: 2021 3d20 2253 5441 5254 4544 220a 2020   != "STARTED".  
+0000dcf0: 2020 2320 293a 0a20 2020 2023 2020 2020    # ):.    #    
+0000dd00: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+0000dd10: 6573 756c 742c 2022 4361 6e6e 6f74 2069  esult, "Cannot i
+0000dd20: 6e69 7469 6174 6520 6e6f 6465 206d 656d  nitiate node mem
+0000dd30: 6f72 7920 6475 6d70 2066 726f 6d20 636f  ory dump from co
+0000dd40: 7265 2041 5049 2229 0a0a 2020 2020 2320  re API")..    # 
+0000dd50: 6c6f 6767 6572 2e69 6e66 6f28 225b 2b5d  logger.info("[+]
+0000dd60: 2049 6e69 7469 616c 697a 6564 206d 656d   Initialized mem
+0000dd70: 6f72 7920 6475 6d70 206f 6620 6e6f 6465  ory dump of node
+0000dd80: 2027 7b7d 272e 2e2e 222e 666f 726d 6174   '{}'...".format
+0000dd90: 2869 645f 6e6f 6465 2929 0a0a 2020 2020  (id_node))..    
+0000dda0: 2320 2320 5761 6974 2066 6f72 2074 6865  # # Wait for the
+0000ddb0: 206f 7065 7261 7469 6f6e 2074 6f20 6265   operation to be
+0000ddc0: 2063 6f6d 706c 6574 6564 2069 6e20 6261   completed in ba
+0000ddd0: 636b 656e 640a 2020 2020 2320 2320 4e6f  ckend.    # # No
+0000dde0: 7465 203a 206c 6f6f 7020 696e 7370 6972  te : loop inspir
+0000ddf0: 6564 2066 726f 6d20 5f73 696d 756c 6174  ed from _simulat
+0000de00: 696f 6e5f 6578 6563 7574 655f 6f70 6572  ion_execute_oper
+0000de10: 6174 696f 6e0a 2020 2020 2320 7768 696c  ation.    # whil
+0000de20: 6520 5472 7565 3a0a 2020 2020 2320 2020  e True:.    #   
+0000de30: 2020 2320 536c 6565 7020 6265 666f 7265    # Sleep before
+0000de40: 206e 6578 7420 6974 6572 6174 696f 6e0a   next iteration.
+0000de50: 2020 2020 2320 2020 2020 7469 6d65 2e73      #     time.s
+0000de60: 6c65 6570 2832 290a 0a20 2020 2023 2020  leep(2)..    #  
+0000de70: 2020 2023 2046 6574 6368 2074 6865 2063     # Fetch the c
+0000de80: 7572 7265 6e74 2073 7461 7475 7320 6f66  urrent status of
+0000de90: 2074 6865 206d 656d 6475 6d70 0a20 2020   the memdump.   
+0000dea0: 2023 2020 2020 2072 6573 756c 7420 3d20   #     result = 
+0000deb0: 5f67 6574 2866 222f 6e6f 6465 2f7b 6964  _get(f"/node/{id
+0000dec0: 5f6e 6f64 657d 2f6d 656d 6f72 7964 756d  _node}/memorydum
+0000ded0: 705f 7374 6174 7573 2229 0a0a 2020 2020  p_status")..    
+0000dee0: 2320 2020 2020 6966 2072 6573 756c 742e  #     if result.
+0000def0: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
+0000df00: 3030 3a0a 2020 2020 2320 2020 2020 2020  00:.    #       
+0000df10: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+0000df20: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
+0000df30: 6765 7420 7374 6174 7573 206f 6620 6e6f  get status of no
+0000df40: 6465 206d 656d 6f72 7920 6475 6d70 2066  de memory dump f
+0000df50: 726f 6d20 636f 7265 2041 5049 2229 0a0a  rom core API")..
+0000df60: 2020 2020 2320 2020 2020 7265 7375 6c74      #     result
+0000df70: 5f6a 736f 6e20 3d20 7265 7375 6c74 2e6a  _json = result.j
+0000df80: 736f 6e28 290a 2020 2020 2320 2020 2020  son().    #     
+0000df90: 7072 696e 7428 7265 7375 6c74 5f6a 736f  print(result_jso
+0000dfa0: 6e29 0a20 2020 2023 2020 2020 2069 6620  n).    #     if 
+0000dfb0: 6e6f 7420 280a 2020 2020 2320 2020 2020  not (.    #     
+0000dfc0: 2020 2020 616c 6c28 6b20 696e 2072 6573      all(k in res
+0000dfd0: 756c 745f 6a73 6f6e 2066 6f72 206b 2069  ult_json for k i
+0000dfe0: 6e20 2866 696c 655f 7061 7468 5f6b 6579  n (file_path_key
+0000dff0: 2c20 6669 6c65 5f73 697a 655f 6b65 792c  , file_size_key,
+0000e000: 2073 7461 7475 735f 6b65 7929 290a 2020   status_key)).  
+0000e010: 2020 2320 2020 2020 293a 0a20 2020 2023    #     ):.    #
+0000e020: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+0000e030: 7863 6570 7469 6f6e 280a 2020 2020 2320  xception(.    # 
+0000e040: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
+0000e050: 6e74 656e 7473 206f 6620 6d65 6d6f 7279  ntents of memory
+0000e060: 2064 756d 7020 7374 6174 7573 2075 7064   dump status upd
+0000e070: 6174 6520 6973 206e 6f74 2069 6e20 7468  ate is not in th
+0000e080: 6520 6578 7065 6374 6564 2066 6f72 6d61  e expected forma
+0000e090: 7420 2861 7474 7269 6275 7465 7320 277b  t (attributes '{
+0000e0a0: 6669 6c65 5f70 6174 685f 6b65 797d 272c  file_path_key}',
+0000e0b0: 2027 7b66 696c 655f 7369 7a65 5f6b 6579   '{file_size_key
+0000e0c0: 7d27 2061 6e64 2027 7b73 7461 7475 735f  }' and '{status_
+0000e0d0: 6b65 797d 2720 6578 7065 6374 6564 2922  key}' expected)"
+0000e0e0: 0a20 2020 2023 2020 2020 2020 2020 2029  .    #         )
+0000e0f0: 0a0a 2020 2020 2320 2020 2020 2320 4c6f  ..    #     # Lo
+0000e100: 6720 696e 666f 206f 6e20 7072 6f67 7265  g info on progre
+0000e110: 7373 696f 6e0a 2020 2020 2320 2020 2020  ssion.    #     
+0000e120: 6966 2072 6573 756c 745f 6a73 6f6e 5b73  if result_json[s
+0000e130: 7461 7475 735f 6b65 795d 203d 3d20 2253  tatus_key] == "S
+0000e140: 5441 5254 4544 223a 0a20 2020 2023 2020  TARTED":.    #  
+0000e150: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+0000e160: 2320 2020 2020 656c 6966 2072 6573 756c  #     elif resul
+0000e170: 745f 6a73 6f6e 5b73 7461 7475 735f 6b65  t_json[status_ke
+0000e180: 795d 203d 3d20 2250 524f 4752 4553 5322  y] == "PROGRESS"
+0000e190: 3a0a 2020 2020 2320 2020 2020 2020 2020  :.    #         
+0000e1a0: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+0000e1b0: 2023 2020 2020 2020 2020 2020 2020 2022   #             "
+0000e1c0: 2020 5b2b 5d20 4375 7272 656e 746c 7920    [+] Currently 
+0000e1d0: 7065 7266 6f72 6d69 6e67 206d 656d 6f72  performing memor
+0000e1e0: 7920 6475 6d70 206f 6620 6e6f 6465 2027  y dump of node '
+0000e1f0: 7b7d 2720 2863 7572 7265 6e74 2064 756d  {}' (current dum
+0000e200: 7020 6669 6c65 2073 697a 6520 6973 207b  p file size is {
+0000e210: 7d29 2e2e 2e22 2e66 6f72 6d61 7428 0a20  })...".format(. 
+0000e220: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0000e230: 2020 2020 2069 645f 6e6f 6465 2c20 6e61       id_node, na
+0000e240: 7475 7261 6c73 697a 6528 7265 7375 6c74  turalsize(result
+0000e250: 5f6a 736f 6e5b 6669 6c65 5f73 697a 655f  _json[file_size_
+0000e260: 6b65 795d 2c20 6269 6e61 7279 3d54 7275  key], binary=Tru
+0000e270: 6529 0a20 2020 2023 2020 2020 2020 2020  e).    #        
+0000e280: 2020 2020 2029 0a20 2020 2023 2020 2020       ).    #    
+0000e290: 2020 2020 2029 0a20 2020 2023 2020 2020       ).    #    
+0000e2a0: 2065 6c69 6620 7265 7375 6c74 5f6a 736f   elif result_jso
+0000e2b0: 6e5b 7374 6174 7573 5f6b 6579 5d20 3d3d  n[status_key] ==
+0000e2c0: 2022 5355 4343 4553 5322 3a0a 2020 2020   "SUCCESS":.    
+0000e2d0: 2320 2020 2020 2020 2020 6272 6561 6b0a  #         break.
+0000e2e0: 2020 2020 2320 2020 2020 656c 7365 3a0a      #     else:.
+0000e2f0: 2020 2020 2320 2020 2020 2020 2020 7261      #         ra
+0000e300: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
+0000e310: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0000e320: 2022 4572 726f 7220 6475 7269 6e67 206d   "Error during m
+0000e330: 656d 6f72 7920 6475 6d70 206f 6620 6e6f  emory dump of no
+0000e340: 6465 207b 7d20 6f70 6572 6174 696f 6e3a  de {} operation:
+0000e350: 2027 7b7d 2722 2e66 6f72 6d61 7428 0a20   '{}'".format(. 
+0000e360: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0000e370: 2020 2020 2069 645f 6e6f 6465 2c20 7265       id_node, re
+0000e380: 7375 6c74 5f6a 736f 6e5b 7374 6174 7573  sult_json[status
+0000e390: 5f6b 6579 5d0a 2020 2020 2320 2020 2020  _key].    #     
+0000e3a0: 2020 2020 2020 2020 290a 2020 2020 2320          ).    # 
+0000e3b0: 2020 2020 2020 2020 290a 0a20 2020 2023          )..    #
+0000e3c0: 206c 6f67 6765 722e 696e 666f 280a 2020   logger.info(.  
+0000e3d0: 2020 2320 2020 2020 225b 2b5d 204e 6f64    #     "[+] Nod
+0000e3e0: 6520 6d65 6d6f 7279 2064 756d 7020 2872  e memory dump (r
+0000e3f0: 6177 2064 756d 7020 7769 7468 206c 6962  aw dump with lib
+0000e400: 7669 7274 2920 6f62 7461 696e 6564 2c20  virt) obtained, 
+0000e410: 616e 6420 706c 6163 6564 2069 6e20 6669  and placed in fi
+0000e420: 6c65 207b 7d20 287b 7d29 206f 6e20 7468  le {} ({}) on th
+0000e430: 6520 7365 7276 6572 2e22 2e66 6f72 6d61  e server.".forma
+0000e440: 7428 0a20 2020 2023 2020 2020 2020 2020  t(.    #        
+0000e450: 2072 6573 756c 745f 6a73 6f6e 5b66 696c   result_json[fil
+0000e460: 655f 7061 7468 5f6b 6579 5d2c 0a20 2020  e_path_key],.   
+0000e470: 2023 2020 2020 2020 2020 206e 6174 7572   #         natur
+0000e480: 616c 7369 7a65 2872 6573 756c 745f 6a73  alsize(result_js
+0000e490: 6f6e 5b66 696c 655f 7369 7a65 5f6b 6579  on[file_size_key
+0000e4a0: 5d2c 2062 696e 6172 793d 5472 7565 292c  ], binary=True),
+0000e4b0: 0a20 2020 2023 2020 2020 2029 0a20 2020  .    #     ).   
+0000e4c0: 2023 2029 0a0a 2020 2020 2320 7265 7475   # )..    # retu
+0000e4d0: 726e 2072 6573 756c 745f 6a73 6f6e 5b66  rn result_json[f
+0000e4e0: 696c 655f 7061 7468 5f6b 6579 5d2c 2072  ile_path_key], r
+0000e4f0: 6573 756c 745f 6a73 6f6e 5b66 696c 655f  esult_json[file_
+0000e500: 7369 7a65 5f6b 6579 5d0a 0a0a 6465 6620  size_key]...def 
+0000e510: 6665 7463 685f 6e6f 6465 5f6e 6574 776f  fetch_node_netwo
+0000e520: 726b 5f69 6e74 6572 6661 6365 7328 6964  rk_interfaces(id
+0000e530: 5f6e 6f64 653a 2069 6e74 2920 2d3e 2041  _node: int) -> A
+0000e540: 6e79 3a0a 2020 2020 2222 2252 6574 7572  ny:.    """Retur
+0000e550: 6e20 6e65 7477 6f72 6b20 696e 7465 7266  n network interf
+0000e560: 6163 6573 206c 6973 7420 6769 7665 6e20  aces list given 
+0000e570: 6120 6e6f 6465 2049 442e 2222 220a 2020  a node ID.""".  
+0000e580: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
+0000e590: 6622 2f6e 6f64 652f 7b69 645f 6e6f 6465  f"/node/{id_node
+0000e5a0: 7d2f 6e65 7477 6f72 6b5f 696e 7465 7266  }/network_interf
+0000e5b0: 6163 6522 290a 0a20 2020 2069 6620 7265  ace")..    if re
+0000e5c0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+0000e5d0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+0000e5e0: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+0000e5f0: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+0000e600: 6574 7269 6576 6520 6e6f 6465 206e 6574  etrieve node net
+0000e610: 776f 726b 2069 6e74 6572 6661 6365 7322  work interfaces"
+0000e620: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
+0000e630: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
+0000e640: 6620 6665 7463 685f 7369 6d75 6c61 7469  f fetch_simulati
+0000e650: 6f6e 5f6e 6574 776f 726b 5f69 6e74 6572  on_network_inter
+0000e660: 6661 6365 7328 6964 5f73 696d 756c 6174  faces(id_simulat
+0000e670: 696f 6e3a 2069 6e74 2920 2d3e 2041 6e79  ion: int) -> Any
+0000e680: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
+0000e690: 6e65 7477 6f72 6b20 696e 7465 7266 6163  network interfac
+0000e6a0: 6573 206c 6973 7420 6769 7665 6e20 6120  es list given a 
+0000e6b0: 7369 6d75 6c61 7469 6f6e 2049 442e 2222  simulation ID.""
+0000e6c0: 220a 2020 2020 7265 7375 6c74 203d 205f  ".    result = _
+0000e6d0: 6765 7428 6622 2f73 696d 756c 6174 696f  get(f"/simulatio
+0000e6e0: 6e2f 7b69 645f 7369 6d75 6c61 7469 6f6e  n/{id_simulation
+0000e6f0: 7d2f 6e65 7477 6f72 6b5f 696e 7465 7266  }/network_interf
+0000e700: 6163 6522 290a 0a20 2020 2069 6620 7265  ace")..    if re
+0000e710: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+0000e720: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+0000e730: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+0000e740: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+0000e750: 6574 7269 6576 6520 7369 6d75 6c61 7469  etrieve simulati
+0000e760: 6f6e 206e 6574 776f 726b 2069 6e74 6572  on network inter
+0000e770: 6661 6365 7322 290a 0a20 2020 2072 6574  faces")..    ret
+0000e780: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
+0000e790: 290a 0a0a 6465 6620 6665 7463 685f 6e65  )...def fetch_ne
+0000e7a0: 7477 6f72 6b5f 696e 7465 7266 6163 655f  twork_interface_
+0000e7b0: 6279 5f6d 6163 2869 645f 7369 6d75 6c61  by_mac(id_simula
+0000e7c0: 7469 6f6e 3a20 696e 742c 206d 6163 5f61  tion: int, mac_a
+0000e7d0: 6464 7265 7373 3a20 7374 7229 202d 3e20  ddress: str) -> 
+0000e7e0: 416e 793a 0a20 2020 2022 2222 5265 7475  Any:.    """Retu
+0000e7f0: 726e 206e 6574 776f 726b 2069 6e74 6572  rn network inter
+0000e800: 6661 6365 206c 6973 7420 6769 7665 6e20  face list given 
+0000e810: 6120 6d61 6320 6164 6472 6573 732e 2222  a mac address.""
+0000e820: 220a 2020 2020 2320 4665 7463 6820 6e6f  ".    # Fetch no
+0000e830: 6465 206e 6574 776f 726b 2069 6e74 6572  de network inter
+0000e840: 6661 6365 730a 2020 2020 7265 7375 6c74  faces.    result
+0000e850: 203d 205f 6765 7428 6622 2f73 696d 756c   = _get(f"/simul
+0000e860: 6174 696f 6e2f 7b69 645f 7369 6d75 6c61  ation/{id_simula
+0000e870: 7469 6f6e 7d2f 6e65 7477 6f72 6b5f 696e  tion}/network_in
+0000e880: 7465 7266 6163 6522 290a 0a20 2020 2069  terface")..    i
+0000e890: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
+0000e8a0: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
+0000e8b0: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
+0000e8c0: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
+0000e8d0: 6f74 2072 6574 7269 6576 6520 6e65 7477  ot retrieve netw
+0000e8e0: 6f72 6b20 696e 7465 7266 6163 6573 2229  ork interfaces")
+0000e8f0: 0a0a 2020 2020 6e65 7477 6f72 6b5f 696e  ..    network_in
+0000e900: 7465 7266 6163 6573 203d 2072 6573 756c  terfaces = resul
+0000e910: 742e 6a73 6f6e 2829 0a0a 2020 2020 666f  t.json()..    fo
+0000e920: 7220 6e65 7477 6f72 6b5f 696e 7465 7266  r network_interf
+0000e930: 6163 6520 696e 206e 6574 776f 726b 5f69  ace in network_i
+0000e940: 6e74 6572 6661 6365 733a 0a20 2020 2020  nterfaces:.     
+0000e950: 2020 2069 6620 6e65 7477 6f72 6b5f 696e     if network_in
+0000e960: 7465 7266 6163 655b 226d 6163 5f61 6464  terface["mac_add
+0000e970: 7265 7373 225d 203d 3d20 6d61 635f 6164  ress"] == mac_ad
+0000e980: 6472 6573 733a 0a20 2020 2020 2020 2020  dress:.         
+0000e990: 2020 2072 6574 7572 6e20 6e65 7477 6f72     return networ
+0000e9a0: 6b5f 696e 7465 7266 6163 650a 2020 2020  k_interface.    
+0000e9b0: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
+0000e9c0: 7475 726e 204e 6f6e 650a 0a0a 6465 6620  turn None...def 
+0000e9d0: 6465 6c65 7465 5f6e 6574 776f 726b 5f69  delete_network_i
+0000e9e0: 6e74 6572 6661 6365 2869 645f 6e65 7477  nterface(id_netw
+0000e9f0: 6f72 6b5f 696e 7465 7266 6163 653a 2069  ork_interface: i
+0000ea00: 6e74 2920 2d3e 2041 6e79 3a0a 2020 2020  nt) -> Any:.    
+0000ea10: 2222 2244 656c 6574 6520 6e65 7477 6f72  """Delete networ
+0000ea20: 6b20 696e 7465 7266 6163 6520 6769 7665  k interface give
+0000ea30: 6e20 616e 2069 642e 2222 220a 2020 2020  n an id.""".    
+0000ea40: 7265 7375 6c74 203d 205f 6465 6c65 7465  result = _delete
+0000ea50: 2866 222f 6e65 7477 6f72 6b5f 696e 7465  (f"/network_inte
+0000ea60: 7266 6163 652f 7b69 645f 6e65 7477 6f72  rface/{id_networ
+0000ea70: 6b5f 696e 7465 7266 6163 657d 2229 0a0a  k_interface}")..
+0000ea80: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
+0000ea90: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
+0000eaa0: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
+0000eab0: 655f 6572 726f 7228 0a20 2020 2020 2020  e_error(.       
+0000eac0: 2020 2020 2072 6573 756c 742c 2022 4361       result, "Ca
+0000ead0: 6e6e 6f74 2072 6574 7269 6576 6520 6e6f  nnot retrieve no
+0000eae0: 6465 206e 6574 776f 726b 2069 6e74 6572  de network inter
+0000eaf0: 6661 6365 7320 6672 6f6d 2049 5420 5369  faces from IT Si
+0000eb00: 6d75 6c61 7469 6f6e 2041 5049 220a 2020  mulation API".  
+0000eb10: 2020 2020 2020 290a 0a20 2020 2072 6574        )..    ret
+0000eb20: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
+0000eb30: 290a 0a0a 6465 6620 7570 6461 7465 5f6e  )...def update_n
+0000eb40: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
+0000eb50: 280a 2020 2020 6964 5f6e 6574 776f 726b  (.    id_network
+0000eb60: 5f69 6e74 6572 6661 6365 3a20 696e 742c  _interface: int,
+0000eb70: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
+0000eb80: 6365 5f64 6963 743a 2064 6963 740a 2920  ce_dict: dict.) 
+0000eb90: 2d3e 2041 6e79 3a0a 2020 2020 2222 2255  -> Any:.    """U
+0000eba0: 7064 6174 6520 6e65 7477 6f72 6b20 696e  pdate network in
+0000ebb0: 7465 7266 6163 6520 696e 666f 726d 6174  terface informat
+0000ebc0: 696f 6e20 696e 666f 726d 6174 696f 6e20  ion information 
+0000ebd0: 6769 7665 6e20 6120 6e65 7477 6f72 6b20  given a network 
+0000ebe0: 696e 7465 7266 6163 6520 6964 2061 6e64  interface id and
+0000ebf0: 2061 0a20 2020 2064 6963 7420 636f 6e74   a.    dict cont
+0000ec00: 6169 6e69 6e67 206e 6574 776f 726b 2069  aining network i
+0000ec10: 6e66 6f2e 0a0a 2020 2020 2222 220a 2020  nfo...    """.  
+0000ec20: 2020 6461 7461 203d 206a 736f 6e2e 6475    data = json.du
+0000ec30: 6d70 7328 6e65 7477 6f72 6b5f 696e 7465  mps(network_inte
+0000ec40: 7266 6163 655f 6469 6374 290a 2020 2020  rface_dict).    
+0000ec50: 7265 7375 6c74 203d 205f 7075 7428 0a20  result = _put(. 
+0000ec60: 2020 2020 2020 2066 222f 6e65 7477 6f72         f"/networ
+0000ec70: 6b5f 696e 7465 7266 6163 652f 7b69 645f  k_interface/{id_
+0000ec80: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+0000ec90: 657d 222c 0a20 2020 2020 2020 2064 6174  e}",.        dat
+0000eca0: 613d 6461 7461 2c0a 2020 2020 2020 2020  a=data,.        
+0000ecb0: 6865 6164 6572 733d 7b22 436f 6e74 656e  headers={"Conten
+0000ecc0: 742d 5479 7065 223a 2022 6170 706c 6963  t-Type": "applic
+0000ecd0: 6174 696f 6e2f 6a73 6f6e 227d 2c0a 2020  ation/json"},.  
+0000ece0: 2020 290a 0a20 2020 2069 6620 7265 7375    )..    if resu
+0000ecf0: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
+0000ed00: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
+0000ed10: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
+0000ed20: 756c 742c 2022 4361 6e6e 6f74 2075 7064  ult, "Cannot upd
+0000ed30: 6174 6520 6e65 7477 6f72 6b20 696e 7465  ate network inte
+0000ed40: 7266 6163 6520 696e 666f 726d 6174 696f  rface informatio
+0000ed50: 6e22 290a 0a20 2020 2072 6574 7572 6e20  n")..    return 
+0000ed60: 7265 7375 6c74 2e6a 736f 6e28 290a 0a0a  result.json()...
+0000ed70: 6465 6620 6665 7463 685f 7072 6f62 6528  def fetch_probe(
+0000ed80: 7072 6f62 655f 6964 3a20 696e 7429 202d  probe_id: int) -
+0000ed90: 3e20 416e 793a 0a20 2020 2022 2222 5265  > Any:.    """Re
+0000eda0: 7475 726e 2061 2070 726f 6265 2067 6976  turn a probe giv
+0000edb0: 656e 2069 7473 2049 4422 2222 0a0a 2020  en its ID"""..  
+0000edc0: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
+0000edd0: 6622 2f70 726f 6265 2f7b 7072 6f62 655f  f"/probe/{probe_
+0000ede0: 6964 7d22 290a 0a20 2020 2069 6620 7265  id}")..    if re
+0000edf0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+0000ee00: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+0000ee10: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+0000ee20: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+0000ee30: 6574 7269 6576 6520 7072 6f62 6520 6672  etrieve probe fr
+0000ee40: 6f6d 2063 6f72 6520 4150 4922 290a 0a20  om core API").. 
+0000ee50: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0000ee60: 2e6a 736f 6e28 290a 0a0a 6465 6620 6665  .json()...def fe
+0000ee70: 7463 685f 7072 6f62 6573 2869 645f 7369  tch_probes(id_si
+0000ee80: 6d75 6c61 7469 6f6e 3a20 696e 7429 202d  mulation: int) -
+0000ee90: 3e20 416e 793a 0a20 2020 2022 2222 5265  > Any:.    """Re
+0000eea0: 7475 726e 2073 696d 756c 6174 696f 6e20  turn simulation 
+0000eeb0: 7072 6f62 6573 2064 6963 7420 6769 7665  probes dict give
+0000eec0: 6e0a 2020 2020 6120 7369 6d75 6c61 7469  n.    a simulati
+0000eed0: 6f6e 2049 442c 2077 6865 7265 206b 6579  on ID, where key
+0000eee0: 7320 6172 6520 7072 6f62 6573 2069 6473  s are probes ids
+0000eef0: 2e0a 2020 2020 2222 220a 0a20 2020 2072  ..    """..    r
+0000ef00: 6573 756c 7420 3d20 5f67 6574 2866 222f  esult = _get(f"/
+0000ef10: 7369 6d75 6c61 7469 6f6e 2f7b 6964 5f73  simulation/{id_s
+0000ef20: 696d 756c 6174 696f 6e7d 2f70 726f 6265  imulation}/probe
+0000ef30: 2229 0a0a 2020 2020 6966 2072 6573 756c  ")..    if resul
+0000ef40: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
+0000ef50: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
+0000ef60: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
+0000ef70: 6c74 2c20 2243 616e 6e6f 7420 7265 7472  lt, "Cannot retr
+0000ef80: 6965 7665 2073 696d 756c 6174 696f 6e20  ieve simulation 
+0000ef90: 7072 6f62 6573 2066 726f 6d20 636f 7265  probes from core
+0000efa0: 2041 5049 2229 0a0a 2020 2020 7265 7475   API")..    retu
+0000efb0: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
+0000efc0: 0a0a 0a64 6566 2063 7265 6174 655f 7072  ...def create_pr
+0000efd0: 6f62 6528 0a20 2020 2069 645f 7369 6d75  obe(.    id_simu
+0000efe0: 6c61 7469 6f6e 3a20 696e 742c 0a20 2020  lation: int,.   
+0000eff0: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
+0000f000: 6365 733a 204c 6973 745b 696e 745d 2c0a  ces: List[int],.
+0000f010: 2020 2020 6966 6163 653a 2073 7472 2c0a      iface: str,.
+0000f020: 2020 2020 7063 6170 3a20 626f 6f6c 2c0a      pcap: bool,.
+0000f030: 2020 2020 6669 6c74 6572 3a20 7374 722c      filter: str,
+0000f040: 0a20 2020 2064 6972 6563 7469 6f6e 3a20  .    direction: 
+0000f050: 7374 722c 0a29 202d 3e20 696e 743a 0a20  str,.) -> int:. 
+0000f060: 2020 2022 2222 4372 6561 7465 2061 206e     """Create a n
+0000f070: 6577 2070 726f 6265 2066 6f72 2074 6865  ew probe for the
+0000f080: 2073 696d 756c 6174 696f 6e20 6769 7665   simulation give
+0000f090: 6e20 6120 6469 6374 2063 6f6e 7461 696e  n a dict contain
+0000f0a0: 696e 6720 7072 6f62 6520 6461 7461 2222  ing probe data""
+0000f0b0: 220a 0a20 2020 2064 6174 615f 6469 6374  "..    data_dict
+0000f0c0: 203d 207b 0a20 2020 2020 2020 2022 6966   = {.        "if
+0000f0d0: 6163 6522 3a20 6966 6163 652c 0a20 2020  ace": iface,.   
+0000f0e0: 2020 2020 2022 7063 6170 223a 2070 6361       "pcap": pca
+0000f0f0: 702c 0a20 2020 2020 2020 2022 6669 6c74  p,.        "filt
+0000f100: 6572 223a 2066 696c 7465 722c 0a20 2020  er": filter,.   
+0000f110: 2020 2020 2022 6e65 7477 6f72 6b5f 696e       "network_in
+0000f120: 7465 7266 6163 6573 223a 206e 6574 776f  terfaces": netwo
+0000f130: 726b 5f69 6e74 6572 6661 6365 732c 0a20  rk_interfaces,. 
+0000f140: 2020 2020 2020 2022 6469 7265 6374 696f         "directio
+0000f150: 6e22 3a20 6469 7265 6374 696f 6e2c 0a20  n": direction,. 
+0000f160: 2020 207d 0a0a 2020 2020 6461 7461 203d     }..    data =
+0000f170: 206a 736f 6e2e 6475 6d70 7328 6461 7461   json.dumps(data
+0000f180: 5f64 6963 7429 0a20 2020 2072 6573 756c  _dict).    resul
+0000f190: 7420 3d20 5f70 6f73 7428 0a20 2020 2020  t = _post(.     
+0000f1a0: 2020 2066 222f 7369 6d75 6c61 7469 6f6e     f"/simulation
+0000f1b0: 2f7b 6964 5f73 696d 756c 6174 696f 6e7d  /{id_simulation}
+0000f1c0: 2f70 726f 6265 222c 0a20 2020 2020 2020  /probe",.       
+0000f1d0: 2064 6174 613d 6461 7461 2c0a 2020 2020   data=data,.    
+0000f1e0: 2020 2020 6865 6164 6572 733d 7b22 436f      headers={"Co
+0000f1f0: 6e74 656e 742d 5479 7065 223a 2022 6170  ntent-Type": "ap
+0000f200: 706c 6963 6174 696f 6e2f 6a73 6f6e 227d  plication/json"}
+0000f210: 2c0a 2020 2020 290a 0a20 2020 2069 6620  ,.    )..    if 
+0000f220: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
+0000f230: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
+0000f240: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+0000f250: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
+0000f260: 2063 7265 6174 6520 7072 6f62 6520 7769   create probe wi
+0000f270: 7468 2063 6f72 6520 4150 4922 290a 0a20  th core API").. 
+0000f280: 2020 2070 726f 6265 5f69 6420 3d20 7265     probe_id = re
+0000f290: 7375 6c74 2e6a 736f 6e28 295b 2269 6422  sult.json()["id"
+0000f2a0: 5d0a 0a20 2020 2072 6574 7572 6e20 7072  ]..    return pr
+0000f2b0: 6f62 655f 6964 0a0a 0a64 6566 2075 7064  obe_id...def upd
+0000f2c0: 6174 655f 7072 6f62 6528 7072 6f62 655f  ate_probe(probe_
+0000f2d0: 6964 3a20 696e 742c 2070 726f 6265 5f64  id: int, probe_d
+0000f2e0: 6963 743a 2064 6963 7429 202d 3e20 416e  ict: dict) -> An
+0000f2f0: 793a 0a20 2020 2022 2222 5570 6461 7465  y:.    """Update
+0000f300: 2070 726f 6265 2069 6e66 6f72 6d61 7469   probe informati
+0000f310: 6f6e 2067 6976 656e 2061 2070 726f 6265  on given a probe
+0000f320: 2069 6420 616e 6420 6120 6469 6374 2063   id and a dict c
+0000f330: 6f6e 7461 696e 696e 670a 2020 2020 7072  ontaining.    pr
+0000f340: 6f62 6520 6461 7461 2e0a 2020 2020 2222  obe data..    ""
+0000f350: 220a 0a20 2020 2064 6174 6120 3d20 6a73  "..    data = js
+0000f360: 6f6e 2e64 756d 7073 2870 726f 6265 5f64  on.dumps(probe_d
+0000f370: 6963 7429 0a20 2020 2072 6573 756c 7420  ict).    result 
+0000f380: 3d20 5f70 7574 280a 2020 2020 2020 2020  = _put(.        
+0000f390: 6622 2f70 726f 6265 2f7b 7072 6f62 655f  f"/probe/{probe_
+0000f3a0: 6964 7d22 2c0a 2020 2020 2020 2020 6461  id}",.        da
+0000f3b0: 7461 3d64 6174 612c 0a20 2020 2020 2020  ta=data,.       
+0000f3c0: 2068 6561 6465 7273 3d7b 2243 6f6e 7465   headers={"Conte
+0000f3d0: 6e74 2d54 7970 6522 3a20 2261 7070 6c69  nt-Type": "appli
+0000f3e0: 6361 7469 6f6e 2f6a 736f 6e22 7d2c 0a20  cation/json"},. 
+0000f3f0: 2020 2029 0a0a 2020 2020 6966 2072 6573     )..    if res
+0000f400: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
+0000f410: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
+0000f420: 5f68 616e 646c 655f 6572 726f 7228 7265  _handle_error(re
+0000f430: 7375 6c74 2c20 2243 616e 6e6f 7420 7570  sult, "Cannot up
+0000f440: 6461 7465 2070 726f 6265 2069 6e66 6f72  date probe infor
+0000f450: 6d61 7469 6f6e 2077 6974 6820 636f 7265  mation with core
+0000f460: 2041 5049 2229 0a0a 2020 2020 7265 7475   API")..    retu
+0000f470: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
+0000f480: 0a0a 0a64 6566 2064 656c 6574 655f 7072  ...def delete_pr
+0000f490: 6f62 6528 7072 6f62 655f 6964 3a20 696e  obe(probe_id: in
+0000f4a0: 7429 202d 3e20 416e 793a 0a20 2020 2022  t) -> Any:.    "
+0000f4b0: 2222 4465 6c65 7465 2073 696d 756c 6174  ""Delete simulat
+0000f4c0: 696f 6e20 7072 6f62 6520 6769 7665 6e20  ion probe given 
+0000f4d0: 6974 7320 4944 2e22 2222 0a0a 2020 2020  its ID."""..    
+0000f4e0: 2320 4465 6c65 7465 2070 726f 6265 0a20  # Delete probe. 
+0000f4f0: 2020 2072 6573 756c 7420 3d20 5f64 656c     result = _del
+0000f500: 6574 6528 6622 2f70 726f 6265 2f7b 7072  ete(f"/probe/{pr
+0000f510: 6f62 655f 6964 7d22 290a 0a20 2020 2069  obe_id}")..    i
+0000f520: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
+0000f530: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
+0000f540: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
+0000f550: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
+0000f560: 6f74 2064 656c 6574 6520 7072 6f62 6522  ot delete probe"
+0000f570: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
+0000f580: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
+0000f590: 6620 6665 7463 685f 6261 7365 626f 7865  f fetch_baseboxe
+0000f5a0: 7328 2920 2d3e 2041 6e79 3a0a 2020 2020  s() -> Any:.    
+0000f5b0: 2222 2252 6574 7572 6e20 6261 7365 626f  """Return basebo
+0000f5c0: 7865 7320 6c69 7374 2e22 2222 0a20 2020  xes list.""".   
+0000f5d0: 2072 6573 756c 7420 3d20 5f67 6574 2822   result = _get("
+0000f5e0: 2f62 6173 6562 6f78 2229 0a0a 2020 2020  /basebox")..    
+0000f5f0: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
+0000f600: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
+0000f610: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
+0000f620: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
+0000f630: 6e6f 7420 7265 7472 6965 7665 2062 6173  not retrieve bas
+0000f640: 6562 6f78 6573 206c 6973 7420 6672 6f6d  eboxes list from
+0000f650: 2049 5420 5369 6d75 6c61 7469 6f6e 2041   IT Simulation A
+0000f660: 5049 2229 0a0a 2020 2020 6261 7365 626f  PI")..    basebo
+0000f670: 7865 7320 3d20 7265 7375 6c74 2e6a 736f  xes = result.jso
+0000f680: 6e28 290a 2020 2020 7265 7475 726e 2062  n().    return b
+0000f690: 6173 6562 6f78 6573 0a0a 0a64 6566 2066  aseboxes...def f
+0000f6a0: 6574 6368 5f62 6173 6562 6f78 2869 645f  etch_basebox(id_
+0000f6b0: 6261 7365 626f 783a 2073 7472 2920 2d3e  basebox: str) ->
+0000f6c0: 2041 6e79 3a0a 2020 2020 2222 2252 6574   Any:.    """Ret
+0000f6d0: 7572 6e20 6261 7365 626f 7820 6769 7665  urn basebox give
+0000f6e0: 6e20 6120 6261 7365 626f 7820 6964 2e22  n a basebox id."
+0000f6f0: 2222 0a20 2020 2072 6573 756c 7420 3d20  "".    result = 
+0000f700: 5f67 6574 2866 222f 6261 7365 626f 782f  _get(f"/basebox/
+0000f710: 6964 2f7b 6964 5f62 6173 6562 6f78 7d22  id/{id_basebox}"
+0000f720: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
+0000f730: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
+0000f740: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
+0000f750: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
+0000f760: 742c 2022 4361 6e6e 6f74 2072 6574 7269  t, "Cannot retri
+0000f770: 6576 6520 6261 7365 626f 7820 696e 666f  eve basebox info
+0000f780: 2066 726f 6d20 4954 2053 696d 756c 6174   from IT Simulat
+0000f790: 696f 6e20 4150 4922 290a 0a20 2020 2062  ion API")..    b
+0000f7a0: 6173 6562 6f78 203d 2072 6573 756c 742e  asebox = result.
+0000f7b0: 6a73 6f6e 2829 0a20 2020 2072 6574 7572  json().    retur
+0000f7c0: 6e20 6261 7365 626f 780a 0a0a 6465 6620  n basebox...def 
+0000f7d0: 7265 6c6f 6164 5f62 6173 6562 6f78 6573  reload_baseboxes
+0000f7e0: 2829 202d 3e20 416e 793a 0a20 2020 2022  () -> Any:.    "
+0000f7f0: 2222 0a20 2020 2043 616c 6c20 7468 6520  "".    Call the 
+0000f800: 6379 6265 7220 7261 6e67 6520 4150 4920  cyber range API 
+0000f810: 746f 2072 656c 6f61 6420 7468 6520 6c69  to reload the li
+0000f820: 7374 206f 6620 6176 6169 6c61 626c 6520  st of available 
+0000f830: 6261 7365 626f 7865 732e 0a0a 2020 2020  baseboxes...    
+0000f840: 3a72 6574 7572 6e3a 0a20 2020 2022 2222  :return:.    """
+0000f850: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
+0000f860: 6574 2822 2f62 6173 6562 6f78 2f72 656c  et("/basebox/rel
+0000f870: 6f61 6422 290a 0a20 2020 2069 6620 7265  oad")..    if re
+0000f880: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+0000f890: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+0000f8a0: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+0000f8b0: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+0000f8c0: 6574 7269 6576 6520 6261 7365 626f 7820  etrieve basebox 
+0000f8d0: 696e 666f 2066 726f 6d20 4954 2053 696d  info from IT Sim
+0000f8e0: 756c 6174 696f 6e20 4150 4922 290a 0a20  ulation API").. 
+0000f8f0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0000f900: 2e6a 736f 6e28 290a 0a0a 6465 6620 7665  .json()...def ve
+0000f910: 7269 6679 5f62 6173 6562 6f78 5f72 6573  rify_basebox_res
+0000f920: 756c 7428 7461 736b 5f69 643a 2073 7472  ult(task_id: str
+0000f930: 2920 2d3e 2041 6e79 3a0a 2020 2020 2222  ) -> Any:.    ""
+0000f940: 220a 2020 2020 2043 616c 6c20 7468 6520  ".     Call the 
+0000f950: 4150 4920 746f 2067 6574 2074 6865 2072  API to get the r
+0000f960: 6573 756c 7420 7468 6520 6375 7272 656e  esult the curren
+0000f970: 7420 7665 7269 6669 6361 7469 6f6e 2e0a  t verification..
+0000f980: 0a20 2020 203a 7061 7261 6d20 7461 736b  .    :param task
+0000f990: 5f69 643a 2074 6865 2074 6173 6b20 6964  _id: the task id
+0000f9a0: 0a20 2020 203a 7265 7475 726e 3a20 7468  .    :return: th
+0000f9b0: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
+0000f9c0: 7665 7269 6669 6361 7469 6f6e 0a0a 2020  verification..  
+0000f9d0: 2020 2222 220a 0a20 2020 2064 6174 6120    """..    data 
+0000f9e0: 3d20 7b22 7461 736b 5f69 6422 3a20 7461  = {"task_id": ta
+0000f9f0: 736b 5f69 647d 0a0a 2020 2020 7472 793a  sk_id}..    try:
+0000fa00: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0000fa10: 3d20 5f70 6f73 7428 0a20 2020 2020 2020  = _post(.       
+0000fa20: 2020 2020 2022 2f62 6173 6562 6f78 2f72       "/basebox/r
+0000fa30: 6573 756c 745f 7665 7269 6679 222c 0a20  esult_verify",. 
+0000fa40: 2020 2020 2020 2020 2020 2064 6174 613d             data=
+0000fa50: 6461 7461 2c0a 2020 2020 2020 2020 290a  data,.        ).
+0000fa60: 0a20 2020 2020 2020 2069 6620 7265 7375  .        if resu
+0000fa70: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
+0000fa80: 3d20 3230 303a 0a20 2020 2020 2020 2020  = 200:.         
+0000fa90: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+0000faa0: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
+0000fab0: 2067 6574 2076 6572 6966 6963 6174 696f   get verificatio
+0000fac0: 6e20 7265 7375 6c74 2229 0a0a 2020 2020  n result")..    
+0000fad0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0000fae0: 742e 6a73 6f6e 2829 0a0a 2020 2020 6578  t.json()..    ex
+0000faf0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+0000fb00: 7320 653a 0a20 2020 2020 2020 2072 6169  s e:.        rai
+0000fb10: 7365 2045 7863 6570 7469 6f6e 2822 4973  se Exception("Is
+0000fb20: 7375 6520 7768 656e 2067 6574 7469 6e67  sue when getting
+0000fb30: 2076 6572 6966 6963 6174 696f 6e20 7265   verification re
+0000fb40: 7375 6c74 3a20 277b 7d27 222e 666f 726d  sult: '{}'".form
+0000fb50: 6174 2865 2929 0a0a 0a64 6566 2076 6572  at(e))...def ver
+0000fb60: 6966 795f 6261 7365 626f 785f 7374 6f70  ify_basebox_stop
+0000fb70: 2874 6173 6b5f 6964 3a20 7374 7229 202d  (task_id: str) -
+0000fb80: 3e20 416e 793a 0a20 2020 2022 2222 0a20  > Any:.    """. 
+0000fb90: 2020 2043 616c 6c20 7468 6520 4150 4920     Call the API 
+0000fba0: 746f 2073 746f 7020 7468 6520 6375 7272  to stop the curr
+0000fbb0: 656e 7420 7665 7269 6669 6361 7469 6f6e  ent verification
+0000fbc0: 0a20 2020 203a 7265 7475 726e 3a0a 2020  .    :return:.  
+0000fbd0: 2020 2222 220a 2020 2020 6461 7461 203d    """.    data =
+0000fbe0: 207b 2274 6173 6b5f 6964 223a 2074 6173   {"task_id": tas
+0000fbf0: 6b5f 6964 7d0a 0a20 2020 2072 6573 756c  k_id}..    resul
+0000fc00: 7420 3d20 5f70 6f73 7428 222f 6261 7365  t = _post("/base
+0000fc10: 626f 782f 7374 6f70 5f76 6572 6966 7922  box/stop_verify"
+0000fc20: 2c20 6461 7461 3d64 6174 6129 0a0a 2020  , data=data)..  
+0000fc30: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
+0000fc40: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
+0000fc50: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
+0000fc60: 6572 726f 7228 7265 7375 6c74 2c20 2243  error(result, "C
+0000fc70: 616e 6e6f 7420 7374 6f70 2076 6572 6966  annot stop verif
+0000fc80: 6963 6174 696f 6e20 7461 736b 2229 0a0a  ication task")..
+0000fc90: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0000fca0: 742e 6a73 6f6e 2829 0a0a 0a64 6566 2076  t.json()...def v
+0000fcb0: 6572 6966 795f 6261 7365 626f 785f 7374  erify_basebox_st
+0000fcc0: 6174 7573 2874 6173 6b5f 6964 3a20 7374  atus(task_id: st
+0000fcd0: 7229 202d 3e20 416e 793a 0a20 2020 2022  r) -> Any:.    "
+0000fce0: 2222 0a20 2020 2043 616c 6c20 7468 6520  "".    Call the 
+0000fcf0: 4150 4920 746f 2067 6574 2074 6865 2073  API to get the s
+0000fd00: 7461 7475 7320 6f66 2063 7572 7265 6e74  tatus of current
+0000fd10: 2076 6572 6966 6963 6174 696f 6e0a 2020   verification.  
+0000fd20: 2020 3a72 6574 7572 6e3a 0a20 2020 2022    :return:.    "
+0000fd30: 2222 0a20 2020 2064 6174 6120 3d20 7b22  "".    data = {"
+0000fd40: 7461 736b 5f69 6422 3a20 7461 736b 5f69  task_id": task_i
+0000fd50: 647d 0a0a 2020 2020 7472 793a 0a20 2020  d}..    try:.   
+0000fd60: 2020 2020 2072 6573 756c 7420 3d20 5f70       result = _p
+0000fd70: 6f73 7428 222f 6261 7365 626f 782f 7374  ost("/basebox/st
+0000fd80: 6174 7573 5f76 6572 6966 7922 2c20 6461  atus_verify", da
+0000fd90: 7461 3d64 6174 6129 0a0a 2020 2020 2020  ta=data)..      
+0000fda0: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
+0000fdb0: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
+0000fdc0: 2020 2020 2020 2020 2020 2020 5f68 616e              _han
+0000fdd0: 646c 655f 6572 726f 7228 7265 7375 6c74  dle_error(result
+0000fde0: 2c20 2243 616e 6e6f 7420 6765 7420 7665  , "Cannot get ve
+0000fdf0: 7269 6679 2073 7461 7475 7322 290a 0a20  rify status").. 
+0000fe00: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000fe10: 7375 6c74 2e6a 736f 6e28 290a 0a20 2020  sult.json()..   
+0000fe20: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0000fe30: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+0000fe40: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+0000fe50: 2249 7373 7565 2077 6865 6e20 6765 7474  "Issue when gett
+0000fe60: 696e 6720 7665 7269 6679 2073 7461 7475  ing verify statu
+0000fe70: 733a 2027 7b7d 2722 2e66 6f72 6d61 7428  s: '{}'".format(
+0000fe80: 6529 290a 0a0a 6465 6620 7665 7269 6679  e))...def verify
+0000fe90: 5f62 6173 6562 6f78 2869 645f 6261 7365  _basebox(id_base
+0000fea0: 626f 783a 2069 6e74 2920 2d3e 2041 6e79  box: int) -> Any
+0000feb0: 3a0a 2020 2020 2222 220a 2020 2020 4361  :.    """.    Ca
+0000fec0: 6c6c 2074 6865 2041 5049 2074 6f20 7665  ll the API to ve
+0000fed0: 7269 6679 2074 6865 2063 6865 636b 7375  rify the checksu
+0000fee0: 6d20 6f66 2074 6865 2067 6976 656e 2062  m of the given b
+0000fef0: 6173 6562 6f78 0a20 2020 203a 7061 7261  asebox.    :para
+0000ff00: 6d20 6964 5f62 6173 6562 6f78 3a20 7468  m id_basebox: th
+0000ff10: 6520 6964 206f 6620 7468 6520 6261 7365  e id of the base
+0000ff20: 626f 7820 746f 2076 6572 6966 790a 2020  box to verify.  
+0000ff30: 2020 3a72 6574 7572 6e3a 0a20 2020 2022    :return:.    "
+0000ff40: 2222 0a20 2020 2072 6573 756c 7420 3d20  "".    result = 
+0000ff50: 5f67 6574 2866 222f 6261 7365 626f 782f  _get(f"/basebox/
+0000ff60: 7665 7269 6679 2f7b 6964 5f62 6173 6562  verify/{id_baseb
+0000ff70: 6f78 7d22 290a 0a20 2020 2069 6620 7265  ox}")..    if re
+0000ff80: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+0000ff90: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+0000ffa0: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+0000ffb0: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+0000ffc0: 6574 7269 6576 6520 6261 7365 626f 7820  etrieve basebox 
+0000ffd0: 696e 666f 2066 726f 6d20 4954 2053 696d  info from IT Sim
+0000ffe0: 756c 6174 696f 6e20 4150 4922 290a 0a20  ulation API").. 
+0000fff0: 2020 2072 6573 756c 7420 3d20 7265 7375     result = resu
+00010000: 6c74 2e6a 736f 6e28 290a 2020 2020 7461  lt.json().    ta
+00010010: 736b 5f69 6420 3d20 7265 7375 6c74 5b22  sk_id = result["
+00010020: 7461 736b 5f69 6422 5d0a 2020 2020 7375  task_id"].    su
+00010030: 6363 6573 7320 3d20 7265 7375 6c74 5b22  ccess = result["
+00010040: 7265 7375 6c74 225d 203d 3d20 2253 5441  result"] == "STA
+00010050: 5254 4544 220a 0a20 2020 2069 6620 6e6f  RTED"..    if no
+00010060: 7420 7375 6363 6573 733a 0a20 2020 2020  t success:.     
+00010070: 2020 205f 7261 6973 655f 6572 726f 725f     _raise_error_
+00010080: 6d73 6728 7265 7375 6c74 290a 0a20 2020  msg(result)..   
+00010090: 206c 6f67 6765 722e 696e 666f 2866 225b   logger.info(f"[
+000100a0: 2b5d 2056 6572 6966 6963 6174 696f 6e20  +] Verification 
+000100b0: 7461 736b 2049 443a 207b 7461 736b 5f69  task ID: {task_i
+000100c0: 647d 2229 0a0a 2020 2020 7265 7375 6c74  d}")..    result
+000100d0: 203d 205f 5f68 616e 646c 655f 7761 6974   = __handle_wait
+000100e0: 280a 2020 2020 2020 2020 7761 6974 3d54  (.        wait=T
+000100f0: 7275 652c 2074 6173 6b5f 6964 3d74 6173  rue, task_id=tas
+00010100: 6b5f 6964 2c20 6c6f 675f 7375 6666 6978  k_id, log_suffix
+00010110: 3d69 645f 6261 7365 626f 782c 2074 696d  =id_basebox, tim
+00010120: 656f 7574 3d33 3630 300a 2020 2020 290a  eout=3600.    ).
+00010130: 0a20 2020 2072 6574 7572 6e20 7b0a 2020  .    return {.  
+00010140: 2020 2020 2020 2273 7563 6365 7373 223a        "success":
+00010150: 2072 6573 756c 745b 2272 6573 756c 7422   result["result"
+00010160: 5d5b 2273 7563 6365 7373 225d 2c0a 2020  ]["success"],.  
+00010170: 2020 2020 2020 2274 6173 6b5f 6964 223a        "task_id":
+00010180: 2074 6173 6b5f 6964 2c0a 2020 2020 2020   task_id,.      
+00010190: 2020 2276 616c 6964 5f63 6865 636b 7375    "valid_checksu
+000101a0: 6d22 3a20 7265 7375 6c74 5b22 7265 7375  m": result["resu
+000101b0: 6c74 225d 5b22 7661 6c69 645f 6368 6563  lt"]["valid_chec
+000101c0: 6b73 756d 225d 2c0a 2020 2020 7d0a 0a0a  ksum"],.    }...
+000101d0: 6465 6620 7665 7269 6679 5f62 6173 6562  def verify_baseb
+000101e0: 6f78 6573 2829 202d 3e20 416e 793a 0a20  oxes() -> Any:. 
+000101f0: 2020 2022 2222 0a20 2020 2043 616c 6c20     """.    Call 
+00010200: 7468 6520 4150 4920 746f 2076 6572 6966  the API to verif
+00010210: 7920 7468 6520 6368 6563 6b73 756d 206f  y the checksum o
+00010220: 6620 616c 6c20 6261 7365 626f 7865 730a  f all baseboxes.
+00010230: 2020 2020 3a72 6574 7572 6e3a 0a20 2020      :return:.   
+00010240: 2022 2222 0a20 2020 2072 6573 756c 7420   """.    result 
+00010250: 3d20 5f67 6574 2822 2f62 6173 6562 6f78  = _get("/basebox
+00010260: 2f76 6572 6966 792f 2229 0a0a 2020 2020  /verify/")..    
+00010270: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
+00010280: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
+00010290: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
+000102a0: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
+000102b0: 6e6f 7420 7265 7472 6965 7665 2062 6173  not retrieve bas
+000102c0: 6562 6f78 2069 6e66 6f20 6672 6f6d 2049  ebox info from I
+000102d0: 5420 5369 6d75 6c61 7469 6f6e 2041 5049  T Simulation API
+000102e0: 2229 0a0a 2020 2020 7265 7375 6c74 203d  ")..    result =
+000102f0: 2072 6573 756c 742e 6a73 6f6e 2829 0a20   result.json(). 
+00010300: 2020 2074 6173 6b5f 6964 203d 2072 6573     task_id = res
+00010310: 756c 745b 2274 6173 6b5f 6964 225d 0a20  ult["task_id"]. 
+00010320: 2020 2073 7563 6365 7373 203d 2072 6573     success = res
+00010330: 756c 745b 2272 6573 756c 7422 5d20 3d3d  ult["result"] ==
+00010340: 2022 5354 4152 5445 4422 0a0a 2020 2020   "STARTED"..    
+00010350: 6966 206e 6f74 2073 7563 6365 7373 3a0a  if not success:.
+00010360: 2020 2020 2020 2020 5f72 6169 7365 5f65          _raise_e
+00010370: 7272 6f72 5f6d 7367 2872 6573 756c 7429  rror_msg(result)
+00010380: 0a0a 2020 2020 6c6f 6767 6572 2e69 6e66  ..    logger.inf
+00010390: 6f28 6622 5b2b 5d20 5665 7269 6669 6361  o(f"[+] Verifica
+000103a0: 7469 6f6e 2074 6173 6b20 4944 3a20 7b74  tion task ID: {t
+000103b0: 6173 6b5f 6964 7d22 290a 0a20 2020 2072  ask_id}")..    r
+000103c0: 6573 756c 7420 3d20 5f5f 6861 6e64 6c65  esult = __handle
+000103d0: 5f77 6169 7428 0a20 2020 2020 2020 2077  _wait(.        w
+000103e0: 6169 743d 5472 7565 2c20 7461 736b 5f69  ait=True, task_i
+000103f0: 643d 7461 736b 5f69 642c 206c 6f67 5f73  d=task_id, log_s
+00010400: 7566 6669 783d 2261 6c6c 2062 6173 6562  uffix="all baseb
+00010410: 6f78 6573 222c 2074 696d 656f 7574 3d33  oxes", timeout=3
+00010420: 3630 300a 2020 2020 290a 0a20 2020 2072  600.    )..    r
+00010430: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+00010440: 2273 7563 6365 7373 223a 2072 6573 756c  "success": resul
+00010450: 745b 2272 6573 756c 7422 5d5b 2273 7563  t["result"]["suc
+00010460: 6365 7373 225d 2c0a 2020 2020 2020 2020  cess"],.        
+00010470: 2274 6173 6b5f 6964 223a 2074 6173 6b5f  "task_id": task_
+00010480: 6964 2c0a 2020 2020 2020 2020 2272 6573  id,.        "res
+00010490: 756c 7422 3a20 7265 7375 6c74 5b22 7265  ult": result["re
+000104a0: 7375 6c74 225d 5b22 7661 6c69 645f 6368  sult"]["valid_ch
+000104b0: 6563 6b73 756d 225d 2c0a 2020 2020 7d0a  ecksum"],.    }.
+000104c0: 0a0a 6465 6620 6665 7463 685f 646f 6d61  ..def fetch_doma
+000104d0: 696e 7328 2920 2d3e 2044 6963 745b 7374  ins() -> Dict[st
+000104e0: 722c 2073 7472 5d3a 0a20 2020 2022 2222  r, str]:.    """
+000104f0: 5265 7475 726e 7320 7468 6520 6d61 7070  Returns the mapp
+00010500: 696e 6720 646f 6d61 696e 2d3e 4950 2222  ing domain->IP""
+00010510: 220a 0a20 2020 2023 2046 4958 4d45 286d  "..    # FIXME(m
+00010520: 756c 7469 2d74 656e 616e 7429 3a20 7765  ulti-tenant): we
+00010530: 2073 686f 756c 6420 7265 7472 6965 7665   should retrieve
+00010540: 2064 6f6d 6169 6e73 2061 6363 6f72 6469   domains accordi
+00010550: 6e67 2074 6f20 6120 7369 6d75 6c61 7469  ng to a simulati
+00010560: 6f6e 2069 640a 2020 2020 7265 7375 6c74  on id.    result
+00010570: 203d 205f 6765 7428 222f 6e65 7477 6f72   = _get("/networ
+00010580: 6b5f 696e 7465 7266 6163 652f 646f 6d61  k_interface/doma
+00010590: 696e 7322 290a 0a20 2020 2069 6620 7265  ins")..    if re
+000105a0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+000105b0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+000105c0: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+000105d0: 6573 756c 742c 2022 4572 726f 7220 7768  esult, "Error wh
+000105e0: 696c 6520 6665 7463 6869 6e67 2064 6f6d  ile fetching dom
+000105f0: 6169 6e73 2229 0a0a 2020 2020 7265 7475  ains")..    retu
+00010600: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
+00010610: 0a0a 0a64 6566 2066 6574 6368 5f77 6562  ...def fetch_web
+00010620: 7369 7465 7328 2920 2d3e 2041 6e79 3a0a  sites() -> Any:.
+00010630: 2020 2020 2222 2252 6574 7572 6e20 7765      """Return we
+00010640: 6273 6974 6573 206c 6973 742e 2222 220a  bsites list.""".
+00010650: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
+00010660: 7428 222f 7765 6273 6974 6522 290a 0a20  t("/website").. 
+00010670: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+00010680: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+00010690: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+000106a0: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
+000106b0: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
+000106c0: 7765 6273 6974 6573 206c 6973 7420 6672  websites list fr
+000106d0: 6f6d 2049 5420 5369 6d75 6c61 7469 6f6e  om IT Simulation
+000106e0: 2041 5049 2229 0a0a 2020 2020 7765 6273   API")..    webs
+000106f0: 6974 6573 203d 2072 6573 756c 742e 6a73  ites = result.js
+00010700: 6f6e 2829 0a20 2020 2072 6574 7572 6e20  on().    return 
+00010710: 7765 6273 6974 6573 0a0a 0a64 6566 2074  websites...def t
+00010720: 6f70 6f6c 6f67 795f 6164 645f 7765 6273  opology_add_webs
+00010730: 6974 6573 280a 2020 2020 746f 706f 6c6f  ites(.    topolo
+00010740: 6779 5f79 616d 6c3a 2073 7472 2c20 7765  gy_yaml: str, we
+00010750: 6273 6974 6573 3a20 4c69 7374 5b73 7472  bsites: List[str
+00010760: 5d2c 2073 7769 7463 685f 6e61 6d65 3a20  ], switch_name: 
+00010770: 7374 720a 2920 2d3e 2073 7472 3a0a 2020  str.) -> str:.  
+00010780: 2020 2222 2241 6464 2064 6f63 6b65 7220    """Add docker 
+00010790: 7765 6273 6974 6573 206e 6f64 6520 746f  websites node to
+000107a0: 2061 2067 6976 656e 2074 6f70 6f6c 6f67   a given topolog
+000107b0: 792c 2061 6e64 2072 6574 7572 6e20 7468  y, and return th
+000107c0: 6520 7570 6461 7465 6420 746f 706f 6c6f  e updated topolo
+000107d0: 6779 2e22 2222 0a0a 2020 2020 6461 7461  gy."""..    data
+000107e0: 5f64 6963 7420 3d20 7b0a 2020 2020 2020  _dict = {.      
+000107f0: 2020 2274 6f70 6f6c 6f67 795f 7961 6d6c    "topology_yaml
+00010800: 223a 2074 6f70 6f6c 6f67 795f 7961 6d6c  ": topology_yaml
+00010810: 2c0a 2020 2020 2020 2020 2277 6562 7369  ,.        "websi
+00010820: 7465 7322 3a20 7765 6273 6974 6573 2c0a  tes": websites,.
+00010830: 2020 2020 2020 2020 2273 7769 7463 685f          "switch_
+00010840: 6e61 6d65 223a 2073 7769 7463 685f 6e61  name": switch_na
+00010850: 6d65 2c0a 2020 2020 7d0a 2020 2020 6461  me,.    }.    da
+00010860: 7461 203d 206a 736f 6e2e 6475 6d70 7328  ta = json.dumps(
+00010870: 6461 7461 5f64 6963 7429 0a20 2020 2072  data_dict).    r
+00010880: 6573 756c 7420 3d20 5f70 6f73 7428 0a20  esult = _post(. 
+00010890: 2020 2020 2020 2022 2f74 6f70 6f6c 6f67         "/topolog
+000108a0: 792f 6164 645f 7765 6273 6974 6573 222c  y/add_websites",
+000108b0: 0a20 2020 2020 2020 2064 6174 613d 6461  .        data=da
+000108c0: 7461 2c0a 2020 2020 2020 2020 6865 6164  ta,.        head
+000108d0: 6572 733d 7b22 436f 6e74 656e 742d 5479  ers={"Content-Ty
+000108e0: 7065 223a 2022 6170 706c 6963 6174 696f  pe": "applicatio
+000108f0: 6e2f 6a73 6f6e 227d 2c0a 2020 2020 290a  n/json"},.    ).
+00010900: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
+00010910: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+00010920: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
+00010930: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
+00010940: 2022 4572 726f 7220 7768 696c 6520 6164   "Error while ad
+00010950: 6469 6e67 2077 6562 7369 7465 7320 746f  ding websites to
+00010960: 2061 2074 6f70 6f6c 6f67 7922 290a 0a20   a topology").. 
+00010970: 2020 2074 6f70 6f6c 6f67 795f 7961 6d6c     topology_yaml
+00010980: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
+00010990: 5b22 746f 706f 6c6f 6779 5f79 616d 6c22  ["topology_yaml"
+000109a0: 5d0a 0a20 2020 2072 6574 7572 6e20 746f  ]..    return to
+000109b0: 706f 6c6f 6779 5f79 616d 6c0a 0a0a 6465  pology_yaml...de
+000109c0: 6620 746f 706f 6c6f 6779 5f61 6464 5f64  f topology_add_d
+000109d0: 6761 280a 2020 2020 746f 706f 6c6f 6779  ga(.    topology
+000109e0: 5f79 616d 6c3a 2073 7472 2c0a 2020 2020  _yaml: str,.    
+000109f0: 616c 676f 7269 7468 6d3a 2073 7472 2c0a  algorithm: str,.
+00010a00: 2020 2020 7377 6974 6368 5f6e 616d 653a      switch_name:
+00010a10: 2073 7472 2c0a 2020 2020 6e75 6d62 6572   str,.    number
+00010a20: 3a20 696e 742c 0a20 2020 2072 6573 6f75  : int,.    resou
+00010a30: 7263 6573 5f64 6972 3a20 7374 722c 0a29  rces_dir: str,.)
+00010a40: 202d 3e20 5475 706c 655b 7374 722c 204c   -> Tuple[str, L
+00010a50: 6973 745b 7374 725d 5d3a 0a20 2020 2022  ist[str]]:.    "
+00010a60: 2222 4164 6420 646f 636b 6572 2065 6d70  ""Add docker emp
+00010a70: 7479 2077 6562 7369 7465 7320 7769 7468  ty websites with
+00010a80: 2044 4741 206e 6f64 6520 746f 2061 2067   DGA node to a g
+00010a90: 6976 656e 2074 6f70 6f6c 6f67 792c 2061  iven topology, a
+00010aa0: 6e64 2072 6574 7572 6e20 7468 6520 7570  nd return the up
+00010ab0: 6461 7465 6420 746f 706f 6c6f 6779 0a20  dated topology. 
+00010ac0: 2020 2061 7373 6f63 6961 7465 6420 7769     associated wi
+00010ad0: 7468 2074 6865 2064 6f6d 6169 6e73 2e22  th the domains."
+00010ae0: 2222 0a0a 2020 2020 6461 7461 5f64 6963  ""..    data_dic
+00010af0: 7420 3d20 7b0a 2020 2020 2020 2020 2274  t = {.        "t
+00010b00: 6f70 6f6c 6f67 795f 7961 6d6c 223a 2074  opology_yaml": t
+00010b10: 6f70 6f6c 6f67 795f 7961 6d6c 2c0a 2020  opology_yaml,.  
+00010b20: 2020 2020 2020 2261 6c67 6f72 6974 686d        "algorithm
+00010b30: 223a 2061 6c67 6f72 6974 686d 2c0a 2020  ": algorithm,.  
+00010b40: 2020 2020 2020 2273 7769 7463 685f 6e61        "switch_na
+00010b50: 6d65 223a 2073 7769 7463 685f 6e61 6d65  me": switch_name
+00010b60: 2c0a 2020 2020 2020 2020 226e 756d 6265  ,.        "numbe
+00010b70: 7222 3a20 6e75 6d62 6572 2c0a 2020 2020  r": number,.    
+00010b80: 2020 2020 2272 6573 6f75 7263 6573 5f64      "resources_d
+00010b90: 6972 223a 2072 6573 6f75 7263 6573 5f64  ir": resources_d
+00010ba0: 6972 2c0a 2020 2020 7d0a 2020 2020 6461  ir,.    }.    da
+00010bb0: 7461 203d 206a 736f 6e2e 6475 6d70 7328  ta = json.dumps(
+00010bc0: 6461 7461 5f64 6963 7429 0a20 2020 2072  data_dict).    r
+00010bd0: 6573 756c 7420 3d20 5f70 6f73 7428 0a20  esult = _post(. 
+00010be0: 2020 2020 2020 2022 2f74 6f70 6f6c 6f67         "/topolog
+00010bf0: 792f 6164 645f 6467 6122 2c0a 2020 2020  y/add_dga",.    
+00010c00: 2020 2020 6461 7461 3d64 6174 612c 0a20      data=data,. 
+00010c10: 2020 2020 2020 2068 6561 6465 7273 3d7b         headers={
+00010c20: 2243 6f6e 7465 6e74 2d54 7970 6522 3a20  "Content-Type": 
+00010c30: 2261 7070 6c69 6361 7469 6f6e 2f6a 736f  "application/jso
+00010c40: 6e22 7d2c 0a20 2020 2029 0a0a 2020 2020  n"},.    )..    
+00010c50: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
+00010c60: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
+00010c70: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
+00010c80: 726f 7228 7265 7375 6c74 2c20 2245 7272  ror(result, "Err
+00010c90: 6f72 2077 6869 6c65 2061 6464 696e 6720  or while adding 
+00010ca0: 7765 6273 6974 6573 2074 6f20 6120 746f  websites to a to
+00010cb0: 706f 6c6f 6779 2229 0a0a 2020 2020 746f  pology")..    to
+00010cc0: 706f 6c6f 6779 5f79 616d 6c20 3d20 7265  pology_yaml = re
+00010cd0: 7375 6c74 2e6a 736f 6e28 295b 2274 6f70  sult.json()["top
+00010ce0: 6f6c 6f67 795f 7961 6d6c 225d 0a20 2020  ology_yaml"].   
+00010cf0: 2064 6f6d 6169 6e73 203d 2072 6573 756c   domains = resul
+00010d00: 742e 6a73 6f6e 2829 5b22 646f 6d61 696e  t.json()["domain
+00010d10: 7322 5d0a 0a20 2020 2072 6574 7572 6e20  s"]..    return 
+00010d20: 746f 706f 6c6f 6779 5f79 616d 6c2c 2064  topology_yaml, d
+00010d30: 6f6d 6169 6e73 0a0a 0a64 6566 2074 6f70  omains...def top
+00010d40: 6f6c 6f67 795f 6164 645f 646e 735f 7365  ology_add_dns_se
+00010d50: 7276 6572 280a 2020 2020 746f 706f 6c6f  rver(.    topolo
+00010d60: 6779 5f79 616d 6c3a 2073 7472 2c0a 2020  gy_yaml: str,.  
+00010d70: 2020 7377 6974 6368 5f6e 616d 653a 2073    switch_name: s
+00010d80: 7472 2c0a 2020 2020 7265 736f 7572 6365  tr,.    resource
+00010d90: 735f 6469 723a 2073 7472 2c0a 2920 2d3e  s_dir: str,.) ->
+00010da0: 2054 7570 6c65 5b73 7472 2c20 7374 725d   Tuple[str, str]
+00010db0: 3a0a 2020 2020 6461 7461 5f64 6963 7420  :.    data_dict 
+00010dc0: 3d20 7b0a 2020 2020 2020 2020 2274 6f70  = {.        "top
+00010dd0: 6f6c 6f67 795f 7961 6d6c 223a 2074 6f70  ology_yaml": top
+00010de0: 6f6c 6f67 795f 7961 6d6c 2c0a 2020 2020  ology_yaml,.    
+00010df0: 2020 2020 2273 7769 7463 685f 6e61 6d65      "switch_name
+00010e00: 223a 2073 7769 7463 685f 6e61 6d65 2c0a  ": switch_name,.
+00010e10: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00010e20: 6573 5f64 6972 223a 2072 6573 6f75 7263  es_dir": resourc
+00010e30: 6573 5f64 6972 2c0a 2020 2020 7d0a 2020  es_dir,.    }.  
+00010e40: 2020 6461 7461 203d 206a 736f 6e2e 6475    data = json.du
+00010e50: 6d70 7328 6461 7461 5f64 6963 7429 0a20  mps(data_dict). 
+00010e60: 2020 2072 6573 756c 7420 3d20 5f70 6f73     result = _pos
+00010e70: 7428 0a20 2020 2020 2020 2022 2f74 6f70  t(.        "/top
+00010e80: 6f6c 6f67 792f 6164 645f 646e 735f 7365  ology/add_dns_se
+00010e90: 7276 6572 222c 0a20 2020 2020 2020 2064  rver",.        d
+00010ea0: 6174 613d 6461 7461 2c0a 2020 2020 2020  ata=data,.      
+00010eb0: 2020 6865 6164 6572 733d 7b22 436f 6e74    headers={"Cont
+00010ec0: 656e 742d 5479 7065 223a 2022 6170 706c  ent-Type": "appl
+00010ed0: 6963 6174 696f 6e2f 6a73 6f6e 227d 2c0a  ication/json"},.
+00010ee0: 2020 2020 290a 0a20 2020 2069 6620 7265      )..    if re
+00010ef0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+00010f00: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+00010f10: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+00010f20: 6573 756c 742c 2022 4572 726f 7220 7768  esult, "Error wh
+00010f30: 696c 6520 6164 6469 6e67 2061 2044 4e53  ile adding a DNS
+00010f40: 2073 6572 7665 7220 746f 2061 2074 6f70   server to a top
+00010f50: 6f6c 6f67 7922 290a 0a20 2020 2074 6f70  ology")..    top
+00010f60: 6f6c 6f67 795f 7961 6d6c 203d 2072 6573  ology_yaml = res
+00010f70: 756c 742e 6a73 6f6e 2829 5b22 746f 706f  ult.json()["topo
+00010f80: 6c6f 6779 5f79 616d 6c22 5d0a 2020 2020  logy_yaml"].    
+00010f90: 646e 735f 636f 6e66 203d 2072 6573 756c  dns_conf = resul
+00010fa0: 742e 6a73 6f6e 2829 5b22 646e 735f 636f  t.json()["dns_co
+00010fb0: 6e66 225d 0a0a 2020 2020 7265 7475 726e  nf"]..    return
+00010fc0: 2074 6f70 6f6c 6f67 795f 7961 6d6c 2c20   topology_yaml, 
+00010fd0: 646e 735f 636f 6e66 0a0a 0a64 6566 2074  dns_conf...def t
+00010fe0: 6f6f 6c73 5f67 656e 6572 6174 655f 646f  ools_generate_do
+00010ff0: 6d61 696e 7328 0a20 2020 2061 6c67 6f72  mains(.    algor
+00011000: 6974 686d 3a20 7374 722c 0a20 2020 206e  ithm: str,.    n
+00011010: 756d 6265 723a 2069 6e74 2c0a 2920 2d3e  umber: int,.) ->
+00011020: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
+00011030: 2222 220a 2020 2020 4765 6e65 7261 7465  """.    Generate
+00011040: 2064 6f6d 6169 6e20 6e61 6d65 7320 6163   domain names ac
+00011050: 636f 7264 696e 6720 746f 2074 6865 2067  cording to the g
+00011060: 6976 656e 2061 6c67 6f72 6974 686d 0a20  iven algorithm. 
+00011070: 2020 203a 7061 7261 6d20 616c 676f 7269     :param algori
+00011080: 7468 6d3a 2061 6c67 6f72 6974 686d 2074  thm: algorithm t
+00011090: 6f20 7573 650a 2020 2020 3a70 6172 616d  o use.    :param
+000110a0: 206e 756d 6265 723a 206e 756d 6265 7220   number: number 
+000110b0: 6f66 2064 6f6d 6169 6e73 2074 6f20 6765  of domains to ge
+000110c0: 6e65 7261 7465 0a20 2020 203a 7265 7475  nerate.    :retu
+000110d0: 726e 3a20 4120 6c69 7374 206f 6620 646f  rn: A list of do
+000110e0: 6d61 696e 730a 2020 2020 2222 220a 2020  mains.    """.  
+000110f0: 2020 6461 7461 5f64 6963 7420 3d20 7b0a    data_dict = {.
+00011100: 2020 2020 2020 2020 2261 6c67 6f72 6974          "algorit
+00011110: 686d 223a 2061 6c67 6f72 6974 686d 2c0a  hm": algorithm,.
+00011120: 2020 2020 2020 2020 226e 756d 6265 7222          "number"
+00011130: 3a20 6e75 6d62 6572 2c0a 2020 2020 7d0a  : number,.    }.
+00011140: 2020 2020 6461 7461 203d 206a 736f 6e2e      data = json.
+00011150: 6475 6d70 7328 6461 7461 5f64 6963 7429  dumps(data_dict)
+00011160: 0a20 2020 2072 6573 756c 7420 3d20 5f70  .    result = _p
+00011170: 6f73 7428 0a20 2020 2020 2020 2022 2f64  ost(.        "/d
+00011180: 6f6d 6169 6e2f 6765 6e65 7261 7465 5f64  omain/generate_d
+00011190: 6f6d 6169 6e73 222c 0a20 2020 2020 2020  omains",.       
+000111a0: 2064 6174 613d 6461 7461 2c0a 2020 2020   data=data,.    
+000111b0: 2020 2020 6865 6164 6572 733d 7b22 436f      headers={"Co
+000111c0: 6e74 656e 742d 5479 7065 223a 2022 6170  ntent-Type": "ap
+000111d0: 706c 6963 6174 696f 6e2f 6a73 6f6e 227d  plication/json"}
+000111e0: 2c0a 2020 2020 290a 0a20 2020 2069 6620  ,.    )..    if 
+000111f0: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
+00011200: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
+00011210: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+00011220: 2872 6573 756c 742c 2022 4572 726f 7220  (result, "Error 
+00011230: 7768 696c 6520 6765 6e65 7261 7469 6e67  while generating
+00011240: 2064 6f6d 6169 6e73 2229 0a0a 2020 2020   domains")..    
+00011250: 646f 6d61 696e 7320 3d20 7265 7375 6c74  domains = result
+00011260: 2e6a 736f 6e28 295b 2264 6f6d 6169 6e73  .json()["domains
+00011270: 225d 0a0a 2020 2020 7265 7475 726e 2064  "]..    return d
+00011280: 6f6d 6169 6e73 0a0a 0a64 6566 2066 6574  omains...def fet
+00011290: 6368 5f74 6f70 6f6c 6f67 6965 7328 2920  ch_topologies() 
+000112a0: 2d3e 2041 6e79 3a0a 2020 2020 2222 2252  -> Any:.    """R
+000112b0: 6574 7572 6e20 746f 706f 6c6f 6769 6573  eturn topologies
+000112c0: 206c 6973 742e 2222 220a 2020 2020 7265   list.""".    re
+000112d0: 7375 6c74 203d 205f 6765 7428 222f 746f  sult = _get("/to
+000112e0: 706f 6c6f 6779 2229 0a0a 2020 2020 6966  pology")..    if
+000112f0: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
+00011300: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
+00011310: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
+00011320: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
+00011330: 7420 7265 7472 6965 7665 2074 6f70 6f6c  t retrieve topol
+00011340: 6f67 6965 7320 6c69 7374 2066 726f 6d20  ogies list from 
+00011350: 4954 2053 696d 756c 6174 696f 6e20 4150  IT Simulation AP
+00011360: 4922 290a 0a20 2020 2074 6f70 6f6c 6f67  I")..    topolog
+00011370: 6965 7320 3d20 7265 7375 6c74 2e6a 736f  ies = result.jso
+00011380: 6e28 290a 2020 2020 7265 7475 726e 2074  n().    return t
+00011390: 6f70 6f6c 6f67 6965 730a 0a0a 2323 230a  opologies...###.
+000113a0: 2320 5369 6d75 6c61 7469 6f6e 2063 6f6d  # Simulation com
+000113b0: 6d61 6e64 730a 2323 230a 0a0a 6465 6620  mands.###...def 
+000113c0: 7374 6172 745f 7369 6d75 6c61 7469 6f6e  start_simulation
+000113d0: 280a 2020 2020 6964 5f73 696d 756c 6174  (.    id_simulat
+000113e0: 696f 6e3a 2069 6e74 2c0a 2020 2020 7573  ion: int,.    us
+000113f0: 655f 696e 7374 616c 6c5f 7469 6d65 3a20  e_install_time: 
+00011400: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00011410: 2020 7469 6d65 6f75 743a 2069 6e74 203d    timeout: int =
+00011420: 2033 3030 2c0a 2020 2020 6e6f 6465 733a   300,.    nodes:
+00011430: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00011440: 7472 5d5d 203d 204e 6f6e 652c 0a29 202d  tr]] = None,.) -
+00011450: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2253  > None:.    """S
+00011460: 7461 7274 2074 6865 2073 696d 756c 6174  tart the simulat
+00011470: 696f 6e2c 2077 6974 6820 6375 7272 656e  ion, with curren
+00011480: 7420 7469 6d65 2028 6279 2064 6566 6175  t time (by defau
+00011490: 6c74 2920 6f72 2074 696d 6520 7768 6572  lt) or time wher
+000114a0: 650a 2020 2020 7468 6520 564d 2077 6173  e.    the VM was
+000114b0: 2063 7265 6174 6564 2028 7573 655f 696e   created (use_in
+000114c0: 7374 616c 6c5f 7469 6d65 3d54 7275 6529  stall_time=True)
+000114d0: 2e20 4974 2069 7320 706f 7373 6962 6c65  . It is possible
+000114e0: 2074 6f0a 2020 2020 7370 6563 6966 7920   to.    specify 
+000114f0: 7468 6520 6e6f 6465 7320 746f 2073 7461  the nodes to sta
+00011500: 7274 2e20 4279 2064 6566 6175 6c74 2c20  rt. By default, 
+00011510: 616c 6c20 6e6f 6465 7320 6172 6520 7374  all nodes are st
+00011520: 6172 7465 642e 0a0a 2020 2020 2222 220a  arted...    """.
+00011530: 2020 2020 2320 4368 6563 6b20 7468 6174      # Check that
+00011540: 206e 6f20 6f74 6865 7220 7369 6d75 6c61   no other simula
+00011550: 7469 6f6e 2069 7320 7275 6e6e 696e 670a  tion is running.
+00011560: 2020 2020 7369 6d75 6c61 7469 6f6e 5f6c      simulation_l
+00011570: 6973 7420 3d20 6665 7463 685f 7369 6d75  ist = fetch_simu
+00011580: 6c61 7469 6f6e 7328 290a 2020 2020 666f  lations().    fo
+00011590: 7220 7369 6d75 6c61 7469 6f6e 2069 6e20  r simulation in 
+000115a0: 7369 6d75 6c61 7469 6f6e 5f6c 6973 743a  simulation_list:
+000115b0: 0a20 2020 2020 2020 2069 6620 7369 6d75  .        if simu
+000115c0: 6c61 7469 6f6e 5b22 6964 225d 2021 3d20  lation["id"] != 
+000115d0: 6964 5f73 696d 756c 6174 696f 6e20 616e  id_simulation an
+000115e0: 6420 7369 6d75 6c61 7469 6f6e 5b22 7374  d simulation["st
+000115f0: 6174 7573 225d 203d 3d20 2252 554e 4e49  atus"] == "RUNNI
+00011600: 4e47 223a 0a20 2020 2020 2020 2020 2020  NG":.           
+00011610: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+00011620: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00011630: 2020 2243 616e 6e6f 7420 7374 6172 7420    "Cannot start 
+00011640: 6120 6e65 7720 7369 6d75 6c61 7469 6f6e  a new simulation
+00011650: 2c20 6173 2074 6865 2073 696d 756c 6174  , as the simulat
+00011660: 696f 6e20 277b 7d27 2069 7320 220a 2020  ion '{}' is ".  
+00011670: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00011680: 6c72 6561 6479 2072 756e 6e69 6e67 222e  lready running".
+00011690: 666f 726d 6174 2873 696d 756c 6174 696f  format(simulatio
+000116a0: 6e5b 2269 6422 5d29 0a20 2020 2020 2020  n["id"]).       
+000116b0: 2020 2020 2029 0a0a 2020 2020 2320 496e       )..    # In
+000116c0: 6974 6961 7465 2074 6865 2073 696d 756c  itiate the simul
+000116d0: 6174 696f 6e0a 2020 2020 6966 206e 6f64  ation.    if nod
+000116e0: 6573 2069 7320 4e6f 6e65 3a0a 2020 2020  es is None:.    
+000116f0: 2020 2020 6e6f 6465 7320 3d20 5b5d 0a20      nodes = []. 
+00011700: 2020 2070 6f73 745f 6461 7461 203d 207b     post_data = {
+00011710: 226e 6f64 6573 223a 206e 6f64 6573 7d0a  "nodes": nodes}.
+00011720: 0a20 2020 205f 7369 6d75 6c61 7469 6f6e  .    _simulation
+00011730: 5f65 7865 6375 7465 5f6f 7065 7261 7469  _execute_operati
+00011740: 6f6e 280a 2020 2020 2020 2020 2270 6f73  on(.        "pos
+00011750: 7422 2c0a 2020 2020 2020 2020 2273 7461  t",.        "sta
+00011760: 7274 222c 0a20 2020 2020 2020 2069 645f  rt",.        id_
+00011770: 7369 6d75 6c61 7469 6f6e 2c0a 2020 2020  simulation,.    
+00011780: 2020 2020 2253 5441 5254 494e 4722 2c0a      "STARTING",.
+00011790: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+000117a0: 5f70 6172 616d 313d 7573 655f 696e 7374  _param1=use_inst
+000117b0: 616c 6c5f 7469 6d65 2c0a 2020 2020 2020  all_time,.      
+000117c0: 2020 6f70 7469 6f6e 616c 5f70 6172 616d    optional_param
+000117d0: 323d 7469 6d65 6f75 742c 0a20 2020 2020  2=timeout,.     
+000117e0: 2020 2070 6f73 745f 6461 7461 3d70 6f73     post_data=pos
+000117f0: 745f 6461 7461 2c0a 2020 2020 290a 0a0a  t_data,.    )...
+00011800: 6465 6620 7061 7573 655f 7369 6d75 6c61  def pause_simula
+00011810: 7469 6f6e 2869 645f 7369 6d75 6c61 7469  tion(id_simulati
+00011820: 6f6e 3a20 696e 7429 202d 3e20 4e6f 6e65  on: int) -> None
+00011830: 3a0a 2020 2020 2222 2250 6175 7365 2061  :.    """Pause a
+00011840: 2073 696d 756c 6174 696f 6e20 2863 616c   simulation (cal
+00011850: 6c73 206c 6962 7669 7274 2073 7573 7065  ls libvirt suspe
+00011860: 6e64 2041 5049 292e 2222 220a 2020 2020  nd API).""".    
+00011870: 5f73 696d 756c 6174 696f 6e5f 6578 6563  _simulation_exec
+00011880: 7574 655f 6f70 6572 6174 696f 6e28 2267  ute_operation("g
+00011890: 6574 222c 2022 7061 7573 6522 2c20 6964  et", "pause", id
+000118a0: 5f73 696d 756c 6174 696f 6e2c 2022 5041  _simulation, "PA
+000118b0: 5553 494e 4722 290a 0a0a 6465 6620 756e  USING")...def un
+000118c0: 7061 7573 655f 7369 6d75 6c61 7469 6f6e  pause_simulation
+000118d0: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
+000118e0: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+000118f0: 2020 2222 2255 6e70 6175 7365 2061 2073    """Unpause a s
+00011900: 696d 756c 6174 696f 6e20 2863 616c 6c73  imulation (calls
+00011910: 206c 6962 7669 7274 2072 6573 756d 6520   libvirt resume 
+00011920: 4150 4929 2e22 2222 0a20 2020 205f 7369  API).""".    _si
+00011930: 6d75 6c61 7469 6f6e 5f65 7865 6375 7465  mulation_execute
+00011940: 5f6f 7065 7261 7469 6f6e 2822 6765 7422  _operation("get"
+00011950: 2c20 2275 6e70 6175 7365 222c 2069 645f  , "unpause", id_
+00011960: 7369 6d75 6c61 7469 6f6e 2c20 2255 4e50  simulation, "UNP
+00011970: 4155 5349 4e47 2229 0a0a 0a64 6566 2063  AUSING")...def c
+00011980: 7265 6174 655f 6261 636b 7570 5f73 696d  reate_backup_sim
+00011990: 756c 6174 696f 6e28 0a20 2020 2069 645f  ulation(.    id_
+000119a0: 7369 6d75 6c61 7469 6f6e 3a20 696e 742c  simulation: int,
+000119b0: 0a20 2020 206e 6f64 6573 3a20 4f70 7469  .    nodes: Opti
+000119c0: 6f6e 616c 5b4c 6973 745b 7374 725d 5d20  onal[List[str]] 
+000119d0: 3d20 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e  = None,.) -> Non
+000119e0: 653a 0a20 2020 2022 2222 4372 6561 7465  e:.    """Create
+000119f0: 2062 6163 6b75 7020 6f66 2061 2073 696d   backup of a sim
+00011a00: 756c 6174 696f 6e2e 2049 7420 6973 2070  ulation. It is p
+00011a10: 6f73 7369 626c 6520 746f 2073 7065 6369  ossible to speci
+00011a20: 6679 2074 6865 206e 6f64 6573 0a20 2020  fy the nodes.   
+00011a30: 2074 6f20 6261 636b 7570 2e20 4279 2064   to backup. By d
+00011a40: 6566 6175 6c74 2c20 616c 6c20 6e6f 6465  efault, all node
+00011a50: 7320 6172 6520 6261 636b 6564 2075 702e  s are backed up.
+00011a60: 0a0a 2020 2020 2222 220a 0a20 2020 2069  ..    """..    i
+00011a70: 6620 6e6f 6465 7320 6973 204e 6f6e 653a  f nodes is None:
+00011a80: 0a20 2020 2020 2020 206e 6f64 6573 203d  .        nodes =
+00011a90: 205b 5d0a 2020 2020 706f 7374 5f64 6174   [].    post_dat
+00011aa0: 6120 3d20 7b22 6e6f 6465 7322 3a20 6e6f  a = {"nodes": no
+00011ab0: 6465 737d 0a0a 2020 2020 5f73 696d 756c  des}..    _simul
+00011ac0: 6174 696f 6e5f 6578 6563 7574 655f 6f70  ation_execute_op
+00011ad0: 6572 6174 696f 6e28 0a20 2020 2020 2020  eration(.       
+00011ae0: 2022 706f 7374 222c 2022 6372 6561 7465   "post", "create
+00011af0: 5f62 6163 6b75 7022 2c20 6964 5f73 696d  _backup", id_sim
+00011b00: 756c 6174 696f 6e2c 2022 5052 4550 4152  ulation, "PREPAR
+00011b10: 494e 4722 2c20 706f 7374 5f64 6174 613d  ING", post_data=
+00011b20: 706f 7374 5f64 6174 610a 2020 2020 290a  post_data.    ).
+00011b30: 0a0a 6465 6620 7265 7374 6f72 655f 6261  ..def restore_ba
+00011b40: 636b 7570 5f73 696d 756c 6174 696f 6e28  ckup_simulation(
+00011b50: 0a20 2020 2069 645f 7369 6d75 6c61 7469  .    id_simulati
+00011b60: 6f6e 3a20 696e 742c 0a20 2020 206e 6f64  on: int,.    nod
+00011b70: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
+00011b80: 745b 7374 725d 5d20 3d20 4e6f 6e65 2c0a  t[str]] = None,.
+00011b90: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+00011ba0: 2222 5265 7374 6f72 6520 6261 636b 7570  ""Restore backup
+00011bb0: 206f 6620 6120 7369 6d75 6c61 7469 6f6e   of a simulation
+00011bc0: 2e20 4974 2069 7320 706f 7373 6962 6c65  . It is possible
+00011bd0: 2074 6f20 7370 6563 6966 7920 7468 6520   to specify the 
+00011be0: 6e6f 6465 730a 2020 2020 746f 2072 6573  nodes.    to res
+00011bf0: 746f 7265 2e20 4279 2064 6566 6175 6c74  tore. By default
+00011c00: 2c20 616c 6c20 6e6f 6465 7320 6172 6520  , all nodes are 
+00011c10: 7265 7374 6f72 6564 2e0a 0a20 2020 2022  restored...    "
+00011c20: 2222 0a0a 2020 2020 6966 206e 6f64 6573  ""..    if nodes
+00011c30: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00011c40: 2020 6e6f 6465 7320 3d20 5b5d 0a20 2020    nodes = [].   
+00011c50: 2070 6f73 745f 6461 7461 203d 207b 226e   post_data = {"n
+00011c60: 6f64 6573 223a 206e 6f64 6573 7d0a 0a20  odes": nodes}.. 
+00011c70: 2020 205f 7369 6d75 6c61 7469 6f6e 5f65     _simulation_e
+00011c80: 7865 6375 7465 5f6f 7065 7261 7469 6f6e  xecute_operation
+00011c90: 280a 2020 2020 2020 2020 2270 6f73 7422  (.        "post"
+00011ca0: 2c20 2272 6573 746f 7265 5f62 6163 6b75  , "restore_backu
+00011cb0: 7022 2c20 6964 5f73 696d 756c 6174 696f  p", id_simulatio
+00011cc0: 6e2c 2022 5052 4550 4152 494e 4722 2c20  n, "PREPARING", 
+00011cd0: 706f 7374 5f64 6174 613d 706f 7374 5f64  post_data=post_d
+00011ce0: 6174 610a 2020 2020 290a 0a0a 6465 6620  ata.    )...def 
+00011cf0: 6861 6c74 5f73 696d 756c 6174 696f 6e28  halt_simulation(
+00011d00: 0a20 2020 2069 645f 7369 6d75 6c61 7469  .    id_simulati
+00011d10: 6f6e 3a20 696e 742c 206e 6f64 6573 3a20  on: int, nodes: 
+00011d20: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+00011d30: 725d 5d20 3d20 4e6f 6e65 0a29 202d 3e20  r]] = None.) -> 
+00011d40: 4f70 7469 6f6e 616c 5b75 7569 642e 5555  Optional[uuid.UU
+00011d50: 4944 5d3a 0a20 2020 2022 2222 5072 6f70  ID]:.    """Prop
+00011d60: 6572 6c79 2073 746f 7020 6120 7369 6d75  erly stop a simu
+00011d70: 6c61 7469 6f6e 2c20 6279 2073 656e 6469  lation, by sendi
+00011d80: 6e67 2061 2073 6875 7464 6f77 6e20 7369  ng a shutdown si
+00011d90: 676e 616c 2074 6f20 7468 650a 2020 2020  gnal to the.    
+00011da0: 6f70 6572 6174 696e 6720 7379 7374 656d  operating system
+00011db0: 732e 2049 7420 6973 2070 6f73 7369 626c  s. It is possibl
+00011dc0: 6520 746f 2073 7065 6369 6679 2074 6865  e to specify the
+00011dd0: 206e 6f64 6573 2074 6f0a 2020 2020 7374   nodes to.    st
+00011de0: 6172 742e 2042 7920 6465 6661 756c 742c  art. By default,
+00011df0: 2061 6c6c 206e 6f64 6573 2061 7265 2073   all nodes are s
+00011e00: 7461 7274 6564 2e0a 0a20 2020 2022 2222  tarted...    """
+00011e10: 0a20 2020 2069 6620 6e6f 6465 7320 6973  .    if nodes is
+00011e20: 204e 6f6e 653a 0a20 2020 2020 2020 206e   None:.        n
+00011e30: 6f64 6573 203d 205b 5d0a 2020 2020 706f  odes = [].    po
+00011e40: 7374 5f64 6174 6120 3d20 7b22 6e6f 6465  st_data = {"node
+00011e50: 7322 3a20 6e6f 6465 737d 0a0a 2020 2020  s": nodes}..    
+00011e60: 5f73 696d 756c 6174 696f 6e5f 6578 6563  _simulation_exec
+00011e70: 7574 655f 6f70 6572 6174 696f 6e28 0a20  ute_operation(. 
+00011e80: 2020 2020 2020 2022 706f 7374 222c 0a20         "post",. 
+00011e90: 2020 2020 2020 2022 7374 6f70 222c 0a20         "stop",. 
+00011ea0: 2020 2020 2020 2069 645f 7369 6d75 6c61         id_simula
+00011eb0: 7469 6f6e 2c0a 2020 2020 2020 2020 2253  tion,.        "S
+00011ec0: 544f 5050 494e 4722 2c0a 2020 2020 2020  TOPPING",.      
+00011ed0: 2020 706f 7374 5f64 6174 613d 706f 7374    post_data=post
+00011ee0: 5f64 6174 612c 0a20 2020 2029 0a0a 0a64  _data,.    )...d
+00011ef0: 6566 2064 6573 7472 6f79 5f73 696d 756c  ef destroy_simul
+00011f00: 6174 696f 6e28 6964 5f73 696d 756c 6174  ation(id_simulat
+00011f10: 696f 6e3a 2069 6e74 2c20 6e6f 6465 733a  ion: int, nodes:
+00011f20: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00011f30: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
+00011f40: 4e6f 6e65 3a0a 2020 2020 2222 2253 746f  None:.    """Sto
+00011f50: 7020 6120 7369 6d75 6c61 7469 6f6e 2074  p a simulation t
+00011f60: 6872 6f75 6768 2061 2068 6172 6420 7265  hrough a hard re
+00011f70: 7365 742e 2222 220a 0a20 2020 2069 6620  set."""..    if 
+00011f80: 6e6f 6465 7320 6973 204e 6f6e 653a 0a20  nodes is None:. 
+00011f90: 2020 2020 2020 206e 6f64 6573 203d 205b         nodes = [
+00011fa0: 5d0a 2020 2020 706f 7374 5f64 6174 6120  ].    post_data 
+00011fb0: 3d20 7b22 6e6f 6465 7322 3a20 6e6f 6465  = {"nodes": node
+00011fc0: 737d 0a0a 2020 2020 5f73 696d 756c 6174  s}..    _simulat
+00011fd0: 696f 6e5f 6578 6563 7574 655f 6f70 6572  ion_execute_oper
+00011fe0: 6174 696f 6e28 0a20 2020 2020 2020 2022  ation(.        "
+00011ff0: 706f 7374 222c 2022 6465 7374 726f 7922  post", "destroy"
+00012000: 2c20 6964 5f73 696d 756c 6174 696f 6e2c  , id_simulation,
+00012010: 2022 5354 4f50 5049 4e47 222c 2070 6f73   "STOPPING", pos
+00012020: 745f 6461 7461 3d70 6f73 745f 6461 7461  t_data=post_data
+00012030: 0a20 2020 2029 0a0a 0a64 6566 2063 6c6f  .    )...def clo
+00012040: 6e65 5f73 696d 756c 6174 696f 6e28 6964  ne_simulation(id
+00012050: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
+00012060: 2920 2d3e 2069 6e74 3a0a 2020 2020 2222  ) -> int:.    ""
+00012070: 2243 6c6f 6e65 2061 2073 696d 756c 6174  "Clone a simulat
+00012080: 696f 6e20 616e 6420 6372 6561 7465 2061  ion and create a
+00012090: 206e 6577 2073 696d 756c 6174 696f 6e2c   new simulation,
+000120a0: 2061 6e64 2072 6574 7572 6e20 7468 6520   and return the 
+000120b0: 6e65 7720 4944 2e22 2222 0a20 2020 2069  new ID.""".    i
+000120c0: 645f 6e65 775f 7369 6d75 6c61 7469 6f6e  d_new_simulation
+000120d0: 203d 205f 7369 6d75 6c61 7469 6f6e 5f65   = _simulation_e
+000120e0: 7865 6375 7465 5f6f 7065 7261 7469 6f6e  xecute_operation
+000120f0: 280a 2020 2020 2020 2020 2267 6574 222c  (.        "get",
+00012100: 2022 636c 6f6e 6522 2c20 6964 5f73 696d   "clone", id_sim
+00012110: 756c 6174 696f 6e2c 2022 434c 4f4e 494e  ulation, "CLONIN
+00012120: 4722 0a20 2020 2029 0a20 2020 2072 6574  G".    ).    ret
+00012130: 7572 6e20 6964 5f6e 6577 5f73 696d 756c  urn id_new_simul
+00012140: 6174 696f 6e0a 0a0a 6465 6620 6e65 745f  ation...def net_
+00012150: 6372 6561 7465 5f70 726f 6265 2820 2023  create_probe(  #
+00012160: 206e 6f71 613a 2043 3930 310a 2020 2020   noqa: C901.    
+00012170: 6964 5f73 696d 756c 6174 696f 6e3a 2069  id_simulation: i
+00012180: 6e74 2c0a 2020 2020 7369 6d75 5f6e 6f64  nt,.    simu_nod
+00012190: 6573 3a20 4469 6374 2c0a 2020 2020 6966  es: Dict,.    if
+000121a0: 6163 653a 204f 7074 696f 6e61 6c5b 7374  ace: Optional[st
+000121b0: 725d 203d 204e 6f6e 652c 0a20 2020 2070  r] = None,.    p
+000121c0: 6361 703a 204f 7074 696f 6e61 6c5b 626f  cap: Optional[bo
+000121d0: 6f6c 5d20 3d20 4661 6c73 652c 0a20 2020  ol] = False,.   
+000121e0: 2066 696c 7465 723a 204f 7074 696f 6e61   filter: Optiona
+000121f0: 6c5b 7374 725d 203d 2022 222c 0a20 2020  l[str] = "",.   
+00012200: 2064 6972 6563 7469 6f6e 3a20 4f70 7469   direction: Opti
+00012210: 6f6e 616c 5b73 7472 5d20 3d20 2262 6f74  onal[str] = "bot
+00012220: 6822 2c0a 2920 2d3e 2069 6e74 3a0a 2020  h",.) -> int:.  
+00012230: 2020 2222 2243 7265 6174 6520 6120 6e65    """Create a ne
+00012240: 7720 7072 6f62 6520 616e 6420 636f 6e66  w probe and conf
+00012250: 6967 7572 6520 6869 7320 6e65 7477 6f72  igure his networ
+00012260: 6b20 636f 6c6c 6563 7469 6f6e 7320 706f  k collections po
+00012270: 696e 7473 2e0a 0a20 2020 203a 7061 7261  ints...    :para
+00012280: 6d20 6964 5f73 696d 756c 6174 696f 6e3a  m id_simulation:
+00012290: 2054 6865 2069 6420 6f66 2074 6865 2073   The id of the s
+000122a0: 696d 756c 6174 696f 6e2e 0a20 2020 203a  imulation..    :
+000122b0: 7061 7261 6d20 7369 6d75 5f6e 6f64 6573  param simu_nodes
+000122c0: 3a20 4120 6469 6374 696f 6e61 7279 2073  : A dictionary s
+000122d0: 746f 7269 6e67 2074 6865 2063 6f6c 6c65  toring the colle
+000122e0: 6374 696f 6e20 706f 696e 7473 2074 6f20  ction points to 
+000122f0: 6361 7074 7572 652e 0a20 2020 203a 7061  capture..    :pa
+00012300: 7261 6d20 6966 6163 653a 2049 6e74 6572  ram iface: Inter
+00012310: 6661 6365 2077 6865 7265 2074 6865 2074  face where the t
+00012320: 7261 6666 6963 2069 7320 6d69 7272 6f72  raffic is mirror
+00012330: 6564 2074 6f2e 0a20 2020 203a 7061 7261  ed to..    :para
+00012340: 6d20 7063 6170 3a20 4120 626f 6f6c 6561  m pcap: A boolea
+00012350: 6e20 696e 6469 6361 7469 6e67 2069 6620  n indicating if 
+00012360: 7468 6520 6361 7074 7572 6520 7368 6f75  the capture shou
+00012370: 6c64 2062 6520 7361 7665 6420 6f6e 2064  ld be saved on d
+00012380: 6973 6b20 696e 2061 2070 6361 7020 6669  isk in a pcap fi
+00012390: 6c65 2028 746f 2062 6520 696e 636c 7564  le (to be includ
+000123a0: 6564 2069 6e20 6461 7461 7365 7429 0a20  ed in dataset). 
+000123b0: 2020 203a 7061 7261 6d20 6669 6c74 6572     :param filter
+000123c0: 3a20 5374 7269 6e67 2066 696c 7465 7269  : String filteri
+000123d0: 6e67 2074 6370 6475 6d70 2063 6170 7475  ng tcpdump captu
+000123e0: 7265 0a20 2020 203a 7061 7261 6d20 6469  re.    :param di
+000123f0: 7265 6374 696f 6e3a 2053 656c 6563 7420  rection: Select 
+00012400: 7768 6963 6820 7472 6166 6669 6320 746f  which traffic to
+00012410: 206d 6f6e 6974 6f72 206f 6e20 7468 6520   monitor on the 
+00012420: 6d69 7272 6f72 6564 2069 6e74 6572 6661  mirrored interfa
+00012430: 6365 2873 293a 2065 6974 6865 7220 2769  ce(s): either 'i
+00012440: 6e67 7265 7373 272c 2027 6567 7265 7373  ngress', 'egress
+00012450: 2720 6f72 2027 626f 7468 272e 0a0a 2020  ' or 'both'...  
+00012460: 2020 3a74 7970 6520 6964 5f73 696d 756c    :type id_simul
+00012470: 6174 696f 6e3a 203a 636c 6173 733a 6069  ation: :class:`i
+00012480: 6e74 602c 2065 7820 3a20 310a 2020 2020  nt`, ex : 1.    
+00012490: 3a74 7970 6520 7369 6d75 5f6e 6f64 6573  :type simu_nodes
+000124a0: 3a20 3a63 6c61 7373 3a60 4469 6374 602c  : :class:`Dict`,
+000124b0: 2065 7820 3a20 7b27 7377 6974 6368 7327   ex : {'switchs'
+000124c0: 3a20 5b5b 2773 7769 7463 6831 272c 2027  : [['switch1', '
+000124d0: 636c 6965 6e74 3127 5d5d 2c20 276e 6f64  client1']], 'nod
+000124e0: 6573 273a 205b 2763 6c69 656e 7432 275d  es': ['client2']
+000124f0: 7d0a 2020 2020 3a74 7970 6520 6966 6163  }.    :type ifac
+00012500: 653a 203a 636c 6173 733a 6073 7472 602c  e: :class:`str`,
+00012510: 2065 7820 3a20 6475 6d6d 7930 0a20 2020   ex : dummy0.   
+00012520: 203a 7479 7065 2070 6361 703a 203a 636c   :type pcap: :cl
+00012530: 6173 733a 6062 6f6f 6c60 2c20 6578 203a  ass:`bool`, ex :
+00012540: 2074 7275 650a 2020 2020 3a74 7970 6520   true.    :type 
+00012550: 6669 6c74 6572 3a20 3a63 6c61 7373 3a60  filter: :class:`
+00012560: 7374 7260 2c20 6578 203a 2074 6370 2070  str`, ex : tcp p
+00012570: 6f72 7420 3830 0a20 2020 203a 7479 7065  ort 80.    :type
+00012580: 2064 6972 6563 7469 6f6e 3a20 3a63 6c61   direction: :cla
+00012590: 7373 3a60 7374 7260 2c20 6578 203a 2069  ss:`str`, ex : i
+000125a0: 6e67 7265 7373 0a20 2020 2022 2222 0a0a  ngress.    """..
+000125b0: 2020 2020 6e65 7477 6f72 6b5f 696e 7465      network_inte
+000125c0: 7266 6163 6573 203d 205b 5d0a 0a20 2020  rfaces = []..   
+000125d0: 2069 6620 7369 6d75 5f6e 6f64 6573 5b22   if simu_nodes["
+000125e0: 7377 6974 6368 7322 5d20 6973 204e 6f6e  switchs"] is Non
+000125f0: 6520 616e 6420 7369 6d75 5f6e 6f64 6573  e and simu_nodes
+00012600: 5b22 6e6f 6465 7322 5d20 6973 204e 6f6e  ["nodes"] is Non
+00012610: 653a 0a20 2020 2020 2020 2023 2043 6f6e  e:.        # Con
+00012620: 7369 6465 7220 616c 6c20 6e6f 6465 206f  sider all node o
+00012630: 6620 7468 6520 7369 6d75 6c61 7469 6f6e  f the simulation
+00012640: 2028 6578 6365 7074 2072 6f75 7465 7273   (except routers
+00012650: 2074 6861 7420 6172 650a 2020 2020 2020   that are.      
+00012660: 2020 2320 4f56 4e20 6162 7374 7261 6374    # OVN abstract
+00012670: 206f 626a 6563 7473 206f 6e20 7768 6963   objects on whic
+00012680: 6820 6974 2069 7320 6e6f 7420 706f 7373  h it is not poss
+00012690: 6962 6c65 2074 6f20 6361 7074 7572 650a  ible to capture.
+000126a0: 2020 2020 2020 2020 2320 7472 6166 6669          # traffi
+000126b0: 6329 0a20 2020 2020 2020 2066 6f72 206e  c).        for n
+000126c0: 6f64 6520 696e 2066 6574 6368 5f6e 6f64  ode in fetch_nod
+000126d0: 6573 2869 645f 7369 6d75 6c61 7469 6f6e  es(id_simulation
+000126e0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+000126f0: 6620 6e6f 6465 5b22 7479 7065 225d 2021  f node["type"] !
+00012700: 3d20 2272 6f75 7465 7222 3a0a 2020 2020  = "router":.    
+00012710: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00012720: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+00012730: 6520 696e 206e 6f64 655b 226e 6574 776f  e in node["netwo
+00012740: 726b 5f69 6e74 6572 6661 6365 7322 5d3a  rk_interfaces"]:
+00012750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012760: 2020 2020 206e 6574 776f 726b 5f69 6e74       network_int
+00012770: 6572 6661 6365 732e 6170 7065 6e64 286e  erfaces.append(n
+00012780: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
+00012790: 5b22 6d61 635f 6164 6472 6573 7322 5d29  ["mac_address"])
+000127a0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+000127b0: 2020 2069 6620 7369 6d75 5f6e 6f64 6573     if simu_nodes
+000127c0: 5b22 7377 6974 6368 7322 5d20 6973 206e  ["switchs"] is n
+000127d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000127e0: 2020 2020 2023 204d 6972 726f 7220 7472       # Mirror tr
+000127f0: 6166 6669 6320 6672 6f6d 206e 6f64 6520  affic from node 
+00012800: 696e 7465 7266 6163 6573 2063 6f6e 6e65  interfaces conne
+00012810: 6374 6564 2074 6f20 7468 6520 7370 6563  cted to the spec
+00012820: 6966 6965 6420 7377 6974 6368 730a 2020  ified switchs.  
+00012830: 2020 2020 2020 2020 2020 666f 7220 7377            for sw
+00012840: 6974 6368 5f6e 6f64 6573 2069 6e20 7369  itch_nodes in si
+00012850: 6d75 5f6e 6f64 6573 5b22 7377 6974 6368  mu_nodes["switch
+00012860: 7322 5d3a 0a20 2020 2020 2020 2020 2020  s"]:.           
+00012870: 2020 2020 2073 7769 7463 6820 3d20 6665       switch = fe
+00012880: 7463 685f 6e6f 6465 5f62 795f 6e61 6d65  tch_node_by_name
+00012890: 2869 645f 7369 6d75 6c61 7469 6f6e 2c20  (id_simulation, 
+000128a0: 7377 6974 6368 5f6e 6f64 6573 5b30 5d29  switch_nodes[0])
+000128b0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000128c0: 2020 2320 4368 6563 6b20 6966 2073 7065    # Check if spe
+000128d0: 6369 6669 6320 6e6f 6465 7320 6172 6520  cific nodes are 
+000128e0: 6465 6669 6e65 642c 2066 6f72 2074 6869  defined, for thi
+000128f0: 7320 7377 6974 6368 0a20 2020 2020 2020  s switch.       
+00012900: 2020 2020 2020 2020 2069 6620 7377 6974           if swit
+00012910: 6368 5f6e 6f64 6573 5b31 3a5d 3a0a 2020  ch_nodes[1:]:.  
+00012920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012930: 2020 666f 7220 6e6f 6465 5f6e 616d 6520    for node_name 
+00012940: 696e 2073 7769 7463 685f 6e6f 6465 735b  in switch_nodes[
+00012950: 313a 5d3a 0a20 2020 2020 2020 2020 2020  1:]:.           
+00012960: 2020 2020 2020 2020 2020 2020 206e 6f64               nod
+00012970: 6520 3d20 6665 7463 685f 6e6f 6465 5f62  e = fetch_node_b
+00012980: 795f 6e61 6d65 2869 645f 7369 6d75 6c61  y_name(id_simula
+00012990: 7469 6f6e 2c20 6e6f 6465 5f6e 616d 6529  tion, node_name)
+000129a0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000129b0: 2020 2020 2020 2020 2020 666f 7220 6e65            for ne
+000129c0: 7477 6f72 6b5f 696e 7465 7266 6163 6520  twork_interface 
+000129d0: 696e 206e 6f64 655b 226e 6574 776f 726b  in node["network
+000129e0: 5f69 6e74 6572 6661 6365 7322 5d3a 0a20  _interfaces"]:. 
+000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a00: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
+00012a10: 7477 6f72 6b5f 696e 7465 7266 6163 655b  twork_interface[
+00012a20: 2273 7769 7463 685f 6e61 6d65 225d 203d  "switch_name"] =
+00012a30: 3d20 7377 6974 6368 5b22 6e61 6d65 225d  = switch["name"]
+00012a40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a60: 2020 6e65 7477 6f72 6b5f 696e 7465 7266    network_interf
+00012a70: 6163 6573 2e61 7070 656e 6428 0a20 2020  aces.append(.   
+00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012aa0: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
+00012ab0: 6365 5b22 6d61 635f 6164 6472 6573 7322  ce["mac_address"
+00012ac0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ae0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b00: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b20: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b40: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+00012b50: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00012b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b70: 2020 2020 2022 5468 6520 6e6f 6465 2027       "The node '
+00012b80: 7b7d 2720 6973 6e27 7420 6c69 6e6b 6564  {}' isn't linked
+00012b90: 2077 6974 6820 7468 6520 7377 6974 6368   with the switch
+00012ba0: 2027 7b7d 2722 2e66 6f72 6d61 7428 0a20   '{}'".format(. 
+00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 2020 206e 6f64 655f 6e61 6d65 2c20 7377     node_name, sw
+00012be0: 6974 6368 5b22 6e61 6d65 225d 0a20 2020  itch["name"].   
+00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c00: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00012c30: 2020 2020 2020 2020 2020 2020 2023 2045               # E
+00012c40: 6c73 652c 2063 6f6e 7369 6465 7220 616c  lse, consider al
+00012c50: 6c20 6e6f 6465 7320 636f 6e6e 6563 7465  l nodes connecte
+00012c60: 6420 746f 2074 6865 2073 7769 7463 680a  d to the switch.
+00012c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c80: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00012c90: 2020 2020 2020 2020 2020 666f 7220 6e6f            for no
+00012ca0: 6465 2069 6e20 6665 7463 685f 6e6f 6465  de in fetch_node
+00012cb0: 7328 6964 5f73 696d 756c 6174 696f 6e29  s(id_simulation)
+00012cc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012cd0: 2020 2020 2020 2020 2020 6966 206e 6f64            if nod
+00012ce0: 655b 2274 7970 6522 5d20 213d 2022 726f  e["type"] != "ro
+00012cf0: 7574 6572 223a 0a20 2020 2020 2020 2020  uter":.         
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2020 2066 6f72 206e 6574 776f 726b 5f69     for network_i
+00012d20: 6e74 6572 6661 6365 2069 6e20 6e6f 6465  nterface in node
+00012d30: 5b22 6e65 7477 6f72 6b5f 696e 7465 7266  ["network_interf
+00012d40: 6163 6573 225d 3a0a 2020 2020 2020 2020  aces"]:.        
+00012d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d60: 2020 2020 2020 2020 6966 206e 6574 776f          if netwo
+00012d70: 726b 5f69 6e74 6572 6661 6365 5b22 7377  rk_interface["sw
+00012d80: 6974 6368 5f6e 616d 6522 5d20 3d3d 2073  itch_name"] == s
+00012d90: 7769 7463 685b 226e 616d 6522 5d3a 0a20  witch["name"]:. 
+00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012dc0: 2020 206e 6574 776f 726b 5f69 6e74 6572     network_inter
+00012dd0: 6661 6365 732e 6170 7065 6e64 280a 2020  faces.append(.  
+00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e00: 2020 2020 2020 6e65 7477 6f72 6b5f 696e        network_in
+00012e10: 7465 7266 6163 655b 226d 6163 5f61 6464  terface["mac_add
+00012e20: 7265 7373 225d 0a20 2020 2020 2020 2020  ress"].         
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e40: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00012e50: 2020 2020 2020 6966 2073 696d 755f 6e6f        if simu_no
+00012e60: 6465 735b 226e 6f64 6573 225d 2069 7320  des["nodes"] is 
+00012e70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00012e80: 2020 2020 2020 2320 4d69 7272 6f72 2074        # Mirror t
+00012e90: 7261 6666 6963 206f 6e20 616c 6c20 696e  raffic on all in
+00012ea0: 7465 7266 6163 6573 2066 726f 6d20 7468  terfaces from th
+00012eb0: 6520 7370 6563 6966 6965 6420 6e6f 6465  e specified node
+00012ec0: 730a 2020 2020 2020 2020 2020 2020 666f  s.            fo
+00012ed0: 7220 6e6f 6465 5f6e 616d 6520 696e 2073  r node_name in s
+00012ee0: 696d 755f 6e6f 6465 735b 226e 6f64 6573  imu_nodes["nodes
+00012ef0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+00012f00: 2020 2020 666f 7220 6e65 7477 6f72 6b5f      for network_
+00012f10: 696e 7465 7266 6163 6520 696e 2066 6574  interface in fet
+00012f20: 6368 5f6e 6f64 655f 6279 5f6e 616d 6528  ch_node_by_name(
+00012f30: 6964 5f73 696d 756c 6174 696f 6e2c 206e  id_simulation, n
+00012f40: 6f64 655f 6e61 6d65 295b 0a20 2020 2020  ode_name)[.     
+00012f50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00012f60: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+00012f70: 6573 220a 2020 2020 2020 2020 2020 2020  es".            
+00012f80: 2020 2020 5d3a 0a20 2020 2020 2020 2020      ]:.         
+00012f90: 2020 2020 2020 2020 2020 206e 6574 776f             netwo
+00012fa0: 726b 5f69 6e74 6572 6661 6365 732e 6170  rk_interfaces.ap
+00012fb0: 7065 6e64 286e 6574 776f 726b 5f69 6e74  pend(network_int
+00012fc0: 6572 6661 6365 5b22 6d61 635f 6164 6472  erface["mac_addr
+00012fd0: 6573 7322 5d29 0a0a 2020 2020 7072 6f62  ess"])..    prob
+00012fe0: 655f 6964 203d 2063 7265 6174 655f 7072  e_id = create_pr
+00012ff0: 6f62 6528 0a20 2020 2020 2020 2069 645f  obe(.        id_
+00013000: 7369 6d75 6c61 7469 6f6e 2c20 6e65 7477  simulation, netw
+00013010: 6f72 6b5f 696e 7465 7266 6163 6573 2c20  ork_interfaces, 
+00013020: 6966 6163 652c 2070 6361 702c 2066 696c  iface, pcap, fil
+00013030: 7465 722c 2064 6972 6563 7469 6f6e 0a20  ter, direction. 
+00013040: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
+00013050: 2070 726f 6265 5f69 640a 0a0a 6465 6620   probe_id...def 
+00013060: 6e65 745f 7374 6172 745f 7072 6f62 6528  net_start_probe(
+00013070: 6964 5f73 696d 756c 6174 696f 6e3a 2069  id_simulation: i
+00013080: 6e74 2c20 7072 6f62 655f 6964 3a20 696e  nt, probe_id: in
+00013090: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+000130a0: 2222 2252 6564 6972 6563 7420 6e65 7477  """Redirect netw
+000130b0: 6f72 6b20 7472 6166 6669 6320 746f 2074  ork traffic to t
+000130c0: 6865 2070 726f 6265 2069 6e74 6572 6661  he probe interfa
+000130d0: 6365 2e0a 0a20 2020 203a 7061 7261 6d20  ce...    :param 
+000130e0: 6964 5f73 696d 756c 6174 696f 6e3a 2054  id_simulation: T
+000130f0: 6865 2069 6420 6f66 2074 6865 2073 696d  he id of the sim
+00013100: 756c 6174 696f 6e2e 0a20 2020 203a 7061  ulation..    :pa
+00013110: 7261 6d20 7072 6f62 655f 6964 3a20 5468  ram probe_id: Th
+00013120: 6520 6964 206f 6620 7468 6520 7072 6f62  e id of the prob
+00013130: 650a 0a20 2020 203a 7479 7065 2069 645f  e..    :type id_
+00013140: 7369 6d75 6c61 7469 6f6e 3a20 3a63 6c61  simulation: :cla
+00013150: 7373 3a60 696e 7460 2c20 6578 203a 2031  ss:`int`, ex : 1
+00013160: 0a20 2020 203a 7479 7065 2070 726f 6265  .    :type probe
+00013170: 5f69 643a 203a 636c 6173 733a 6069 6e74  _id: :class:`int
+00013180: 602c 2065 7820 3a20 310a 0a20 2020 2022  `, ex : 1..    "
+00013190: 2222 0a0a 2020 2020 7265 7375 6c74 203d  ""..    result =
+000131a0: 205f 6765 7428 6622 2f73 696d 756c 6174   _get(f"/simulat
+000131b0: 696f 6e2f 7b69 645f 7369 6d75 6c61 7469  ion/{id_simulati
+000131c0: 6f6e 7d2f 7072 6f62 652f 7b70 726f 6265  on}/probe/{probe
+000131d0: 5f69 647d 2229 0a0a 2020 2020 6966 2072  _id}")..    if r
+000131e0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
+000131f0: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
+00013200: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+00013210: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00013220: 756c 742c 2022 4361 6e6e 6f74 2061 6374  ult, "Cannot act
+00013230: 6976 6174 6520 6e65 7477 6f72 6b20 7472  ivate network tr
+00013240: 6166 6669 6320 7265 6469 7265 6374 696f  affic redirectio
+00013250: 6e20 6672 6f6d 2049 5420 5369 6d75 6c61  n from IT Simula
+00013260: 7469 6f6e 2041 5049 220a 2020 2020 2020  tion API".      
+00013270: 2020 290a 0a0a 6465 6620 6e65 745f 7374    )...def net_st
+00013280: 6f70 5f70 726f 6265 2869 645f 7369 6d75  op_probe(id_simu
+00013290: 6c61 7469 6f6e 3a20 696e 742c 2070 726f  lation: int, pro
+000132a0: 6265 5f69 643a 2069 6e74 2920 2d3e 204e  be_id: int) -> N
+000132b0: 6f6e 653a 0a20 2020 2022 2222 5374 6f70  one:.    """Stop
+000132c0: 2072 6564 6972 6563 7469 6f6e 206f 6620   redirection of 
+000132d0: 6e65 7477 6f72 6b20 7472 6166 6669 6320  network traffic 
+000132e0: 746f 2074 6865 2070 726f 6265 2069 6e74  to the probe int
+000132f0: 6572 6661 6365 2e0a 0a20 2020 203a 7061  erface...    :pa
+00013300: 7261 6d20 6964 5f73 696d 756c 6174 696f  ram id_simulatio
+00013310: 6e3a 2054 6865 2069 6420 6f66 2074 6865  n: The id of the
+00013320: 2073 696d 756c 6174 696f 6e2e 0a20 2020   simulation..   
+00013330: 203a 7061 7261 6d20 7072 6f62 655f 6964   :param probe_id
+00013340: 3a20 5468 6520 6964 206f 6620 7468 6520  : The id of the 
+00013350: 7072 6f62 650a 0a20 2020 203a 7479 7065  probe..    :type
+00013360: 2069 645f 7369 6d75 6c61 7469 6f6e 3a20   id_simulation: 
+00013370: 3a63 6c61 7373 3a60 696e 7460 2c20 6578  :class:`int`, ex
+00013380: 203a 2031 0a20 2020 203a 7479 7065 2070   : 1.    :type p
+00013390: 726f 6265 5f69 643a 203a 636c 6173 733a  robe_id: :class:
+000133a0: 6069 6e74 602c 2065 7820 3a20 310a 0a20  `int`, ex : 1.. 
+000133b0: 2020 2022 2222 0a0a 2020 2020 7265 7375     """..    resu
+000133c0: 6c74 203d 205f 6765 7428 6622 2f73 696d  lt = _get(f"/sim
+000133d0: 756c 6174 696f 6e2f 7b69 645f 7369 6d75  ulation/{id_simu
+000133e0: 6c61 7469 6f6e 7d2f 7374 6f70 5f70 726f  lation}/stop_pro
+000133f0: 6265 2f7b 7072 6f62 655f 6964 7d22 290a  be/{probe_id}").
+00013400: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
+00013410: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+00013420: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
+00013430: 6c65 5f65 7272 6f72 280a 2020 2020 2020  le_error(.      
+00013440: 2020 2020 2020 7265 7375 6c74 2c20 2243        result, "C
+00013450: 616e 6e6f 7420 7374 6f70 206e 6574 776f  annot stop netwo
+00013460: 726b 2074 7261 6666 6963 2072 6564 6972  rk traffic redir
+00013470: 6563 7469 6f6e 2066 726f 6d20 4954 2053  ection from IT S
+00013480: 696d 756c 6174 696f 6e20 4150 4922 0a20  imulation API". 
+00013490: 2020 2020 2020 2029 0a0a 0a64 6566 2066         )...def f
+000134a0: 6574 6368 5f6c 6973 745f 7072 6f62 6573  etch_list_probes
+000134b0: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
+000134c0: 696e 7429 202d 3e20 4469 6374 3a0a 2020  int) -> Dict:.  
+000134d0: 2020 2222 2252 6574 7572 6e20 7468 6520    """Return the 
+000134e0: 6c69 7374 206f 6620 7072 6f62 6573 2077  list of probes w
+000134f0: 6974 6820 7468 6569 7220 6461 7461 0a0a  ith their data..
+00013500: 2020 2020 3a70 6172 616d 2069 645f 7369      :param id_si
+00013510: 6d75 6c61 7469 6f6e 3a20 5468 6520 6964  mulation: The id
+00013520: 206f 6620 7468 6520 7369 6d75 6c61 7469   of the simulati
+00013530: 6f6e 0a0a 2020 2020 3a74 7970 6520 6964  on..    :type id
+00013540: 5f73 696d 756c 6174 696f 6e3a 203a 636c  _simulation: :cl
+00013550: 6173 733a 6069 6e74 602c 2065 7820 3a20  ass:`int`, ex : 
+00013560: 310a 0a20 2020 203a 7265 7475 726e 3a20  1..    :return: 
+00013570: 4120 6c69 7374 206f 6620 7072 6f62 6573  A list of probes
+00013580: 2077 6974 6820 7468 6569 7220 6461 7461   with their data
+00013590: 0a20 2020 2022 2222 0a0a 2020 2020 7265  .    """..    re
+000135a0: 7375 6c74 203d 207b 7d0a 0a20 2020 2070  sult = {}..    p
+000135b0: 726f 6265 7320 3d20 6665 7463 685f 7072  robes = fetch_pr
+000135c0: 6f62 6573 2869 645f 7369 6d75 6c61 7469  obes(id_simulati
+000135d0: 6f6e 290a 2020 2020 666f 7220 7072 6f62  on).    for prob
+000135e0: 6520 696e 2070 726f 6265 733a 0a20 2020  e in probes:.   
+000135f0: 2020 2020 2072 6573 756c 745b 7072 6f62       result[prob
+00013600: 655b 2269 6422 5d5d 203d 207b 0a20 2020  e["id"]] = {.   
+00013610: 2020 2020 2020 2020 2022 636f 6c6c 6563           "collec
+00013620: 7469 6e67 5f70 6f69 6e74 7322 3a20 6665  ting_points": fe
+00013630: 7463 685f 7072 6f62 655f 636f 6c6c 6563  tch_probe_collec
+00013640: 7469 6e67 5f70 6f69 6e74 7328 6964 5f73  ting_points(id_s
+00013650: 696d 756c 6174 696f 6e2c 2070 726f 6265  imulation, probe
+00013660: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
+00013670: 6966 6163 6522 3a20 7072 6f62 655b 2269  iface": probe["i
+00013680: 6661 6365 225d 2c0a 2020 2020 2020 2020  face"],.        
+00013690: 2020 2020 2270 6361 7022 3a20 7072 6f62      "pcap": prob
+000136a0: 655b 2270 6361 7022 5d2c 0a20 2020 2020  e["pcap"],.     
+000136b0: 2020 2020 2020 2022 6669 6c74 6572 223a         "filter":
+000136c0: 2070 726f 6265 5b22 6669 6c74 6572 225d   probe["filter"]
+000136d0: 2c0a 2020 2020 2020 2020 2020 2020 2263  ,.            "c
+000136e0: 6170 7475 7265 5f69 6e5f 7072 6f67 7265  apture_in_progre
+000136f0: 7373 223a 2070 726f 6265 5b22 6361 7074  ss": probe["capt
+00013700: 7572 655f 696e 5f70 726f 6772 6573 7322  ure_in_progress"
+00013710: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+00013720: 6469 7265 6374 696f 6e22 3a20 7072 6f62  direction": prob
+00013730: 655b 2264 6972 6563 7469 6f6e 225d 2c0a  e["direction"],.
+00013740: 2020 2020 2020 2020 7d0a 0a20 2020 2072          }..    r
+00013750: 6574 7572 6e20 7265 7375 6c74 0a0a 0a64  eturn result...d
+00013760: 6566 2066 6574 6368 5f70 726f 6265 5f63  ef fetch_probe_c
+00013770: 6f6c 6c65 6374 696e 675f 706f 696e 7473  ollecting_points
+00013780: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
+00013790: 696e 742c 2070 726f 6265 3a20 4469 6374  int, probe: Dict
+000137a0: 2920 2d3e 2041 6e79 3a0a 2020 2020 2222  ) -> Any:.    ""
+000137b0: 2252 6574 7572 6e20 7468 6520 6c69 7374  "Return the list
+000137c0: 206f 6620 636f 6c6c 6563 7469 6e67 2070   of collecting p
+000137d0: 6f69 6e74 7320 7573 6564 2074 6f20 6361  oints used to ca
+000137e0: 7074 7572 6520 7468 6520 6e65 7477 6f72  pture the networ
+000137f0: 6b20 7472 6166 6669 6320 746f 2061 2067  k traffic to a g
+00013800: 6976 656e 2070 726f 6265 206f 6620 6120  iven probe of a 
+00013810: 7369 6d75 6c61 7469 6f6e 2e0a 0a20 2020  simulation...   
+00013820: 203a 7061 7261 6d20 6964 5f73 696d 756c   :param id_simul
+00013830: 6174 696f 6e3a 2054 6865 2069 6420 6f66  ation: The id of
+00013840: 2074 6865 2073 696d 756c 6174 696f 6e2e   the simulation.
+00013850: 0a20 2020 203a 7061 7261 6d20 7072 6f62  .    :param prob
+00013860: 653a 2054 6865 2067 6976 656e 2070 726f  e: The given pro
+00013870: 6265 206f 6620 7468 6520 7369 6d75 6c61  be of the simula
+00013880: 7469 6f6e 0a0a 2020 2020 3a74 7970 6520  tion..    :type 
+00013890: 6964 5f73 696d 756c 6174 696f 6e3a 203a  id_simulation: :
+000138a0: 636c 6173 733a 6069 6e74 602c 2065 7820  class:`int`, ex 
+000138b0: 3a20 310a 2020 2020 3a74 7970 6520 7072  : 1.    :type pr
+000138c0: 6f62 653a 203a 636c 6173 733a 6063 6c61  obe: :class:`cla
+000138d0: 7373 603a 6044 6963 7460 2c20 6578 203a  ss`:`Dict`, ex :
+000138e0: 207b 2769 6661 6365 273a 2027 6475 6d6d   {'iface': 'dumm
+000138f0: 7930 272c 2027 6964 273a 2031 2c20 2770  y0', 'id': 1, 'p
+00013900: 6361 7027 3a20 5472 7565 2c20 2763 6170  cap': True, 'cap
+00013910: 7475 7265 5f69 6e5f 7072 6f67 7265 7373  ture_in_progress
+00013920: 273a 2046 616c 7365 2c20 2766 696c 7465  ': False, 'filte
+00013930: 7227 3a20 2774 6370 2070 6f72 7420 3830  r': 'tcp port 80
+00013940: 272c 2027 7369 6d75 6c61 7469 6f6e 5f69  ', 'simulation_i
+00013950: 6427 3a20 312c 2027 6e65 7477 6f72 6b5f  d': 1, 'network_
+00013960: 696e 7465 7266 6163 6573 273a 205b 2730  interfaces': ['0
+00013970: 303a 3231 3a61 313a 3037 3a37 643a 6265  0:21:a1:07:7d:be
+00013980: 275d 2c20 2764 6972 6563 7469 6f6e 273a  '], 'direction':
+00013990: 2027 696e 6772 6573 7327 7d0a 0a20 2020   'ingress'}..   
+000139a0: 2022 2222 0a0a 2020 2020 636f 6c6c 6563   """..    collec
+000139b0: 7469 6e67 5f70 6f69 6e74 7320 3d20 7b22  ting_points = {"
+000139c0: 7377 6974 6368 7322 3a20 7b7d 2c20 226e  switchs": {}, "n
+000139d0: 6f64 6573 223a 205b 5d7d 0a0a 2020 2020  odes": []}..    
+000139e0: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+000139f0: 6573 203d 205b 0a20 2020 2020 2020 2066  es = [.        f
+00013a00: 6574 6368 5f6e 6574 776f 726b 5f69 6e74  etch_network_int
+00013a10: 6572 6661 6365 5f62 795f 6d61 6328 6964  erface_by_mac(id
+00013a20: 5f73 696d 756c 6174 696f 6e2c 206e 290a  _simulation, n).
+00013a30: 2020 2020 2020 2020 666f 7220 6e20 696e          for n in
+00013a40: 2070 726f 6265 5b22 6e65 7477 6f72 6b5f   probe["network_
+00013a50: 696e 7465 7266 6163 6573 225d 0a20 2020  interfaces"].   
+00013a60: 205d 0a0a 2020 2020 6e6f 6465 735f 746f   ]..    nodes_to
+00013a70: 5f63 6170 7475 7265 203d 205b 5d0a 2020  _capture = [].  
+00013a80: 2020 666f 7220 6e65 7477 6f72 6b5f 696e    for network_in
+00013a90: 7465 7266 6163 6520 696e 206e 6574 776f  terface in netwo
+00013aa0: 726b 5f69 6e74 6572 6661 6365 733a 0a20  rk_interfaces:. 
+00013ab0: 2020 2020 2020 206e 6f64 6520 3d20 6665         node = fe
+00013ac0: 7463 685f 6e6f 6465 286e 6574 776f 726b  tch_node(network
+00013ad0: 5f69 6e74 6572 6661 6365 5b22 6e6f 6465  _interface["node
+00013ae0: 5f69 6422 5d29 0a20 2020 2020 2020 2069  _id"]).        i
+00013af0: 6620 6e6f 6465 206e 6f74 2069 6e20 6e6f  f node not in no
+00013b00: 6465 735f 746f 5f63 6170 7475 7265 3a0a  des_to_capture:.
+00013b10: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+00013b20: 735f 746f 5f63 6170 7475 7265 2e61 7070  s_to_capture.app
+00013b30: 656e 6428 6e6f 6465 290a 0a20 2020 2023  end(node)..    #
+00013b40: 2052 6574 7572 6e20 4e6f 6e65 2069 6620   Return None if 
+00013b50: 7468 6572 6520 6973 206e 6f74 6869 6e67  there is nothing
+00013b60: 2074 6f20 6361 7074 7572 650a 2020 2020   to capture.    
+00013b70: 6966 206e 6f64 6573 5f74 6f5f 6361 7074  if nodes_to_capt
+00013b80: 7572 6520 3d3d 205b 5d3a 0a20 2020 2020  ure == []:.     
+00013b90: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00013ba0: 2020 2020 2320 5265 7475 726e 207b 7d20      # Return {} 
+00013bb0: 6966 2065 7665 7279 206e 6f64 6520 6d75  if every node mu
+00013bc0: 7374 2062 6520 6361 7074 7572 6564 0a20  st be captured. 
+00013bd0: 2020 2069 6620 6c65 6e28 6e65 7477 6f72     if len(networ
+00013be0: 6b5f 696e 7465 7266 6163 6573 2920 3d3d  k_interfaces) ==
+00013bf0: 206c 656e 280a 2020 2020 2020 2020 6665   len(.        fe
+00013c00: 7463 685f 7369 6d75 6c61 7469 6f6e 5f6e  tch_simulation_n
+00013c10: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
+00013c20: 7328 6964 5f73 696d 756c 6174 696f 6e29  s(id_simulation)
+00013c30: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00013c40: 7265 7475 726e 207b 7d0a 0a20 2020 2066  return {}..    f
+00013c50: 6f72 206e 6f64 6520 696e 206e 6f64 6573  or node in nodes
+00013c60: 5f74 6f5f 6361 7074 7572 653a 0a0a 2020  _to_capture:..  
+00013c70: 2020 2020 2020 2320 4966 2065 7665 7279        # If every
+00013c80: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
+00013c90: 6365 2066 726f 6d20 6120 6e6f 6465 2069  ce from a node i
+00013ca0: 7320 6361 7074 7572 6564 2c20 6974 2067  s captured, it g
+00013cb0: 6f65 7320 746f 2074 6865 2022 6e6f 6465  oes to the "node
+00013cc0: 7322 2064 6963 740a 2020 2020 2020 2020  s" dict.        
+00013cd0: 6361 7074 7572 655f 616c 6c5f 6e65 7477  capture_all_netw
+00013ce0: 6f72 6b5f 696e 7465 7266 6163 6573 203d  ork_interfaces =
+00013cf0: 2054 7275 650a 2020 2020 2020 2020 666f   True.        fo
+00013d00: 7220 6e6f 6465 5f6e 6574 776f 726b 5f69  r node_network_i
+00013d10: 6e74 6572 6661 6365 2069 6e20 6e6f 6465  nterface in node
+00013d20: 5b22 6e65 7477 6f72 6b5f 696e 7465 7266  ["network_interf
+00013d30: 6163 6573 225d 3a0a 2020 2020 2020 2020  aces"]:.        
+00013d40: 2020 2020 6361 7074 7572 655f 616c 6c5f      capture_all_
+00013d50: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+00013d60: 6573 203d 2063 6170 7475 7265 5f61 6c6c  es = capture_all
+00013d70: 5f6e 6574 776f 726b 5f69 6e74 6572 6661  _network_interfa
+00013d80: 6365 7320 616e 6420 280a 2020 2020 2020  ces and (.      
+00013d90: 2020 2020 2020 2020 2020 6e6f 6465 5f6e            node_n
+00013da0: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
+00013db0: 2069 6e20 6e65 7477 6f72 6b5f 696e 7465   in network_inte
+00013dc0: 7266 6163 6573 0a20 2020 2020 2020 2020  rfaces.         
+00013dd0: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+00013de0: 2063 6170 7475 7265 5f61 6c6c 5f6e 6574   capture_all_net
+00013df0: 776f 726b 5f69 6e74 6572 6661 6365 733a  work_interfaces:
+00013e00: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+00013e10: 6c65 6374 696e 675f 706f 696e 7473 5b22  lecting_points["
+00013e20: 6e6f 6465 7322 5d2e 6170 7065 6e64 286e  nodes"].append(n
+00013e30: 6f64 655b 226e 616d 6522 5d29 0a20 2020  ode["name"]).   
+00013e40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00013e50: 2020 2020 2020 2023 2045 6c73 652c 2069         # Else, i
+00013e60: 7420 676f 6573 2074 6f20 7468 6520 2273  t goes to the "s
+00013e70: 7769 7463 6873 2220 6469 6374 0a20 2020  witchs" dict.   
+00013e80: 2020 2020 2020 2020 2066 6f72 206e 6f64           for nod
+00013e90: 655f 6e65 7477 6f72 6b5f 696e 7465 7266  e_network_interf
+00013ea0: 6163 6520 696e 206e 6f64 655b 226e 6574  ace in node["net
+00013eb0: 776f 726b 5f69 6e74 6572 6661 6365 7322  work_interfaces"
+00013ec0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00013ed0: 2020 2069 6620 6e6f 6465 5f6e 6574 776f     if node_netwo
+00013ee0: 726b 5f69 6e74 6572 6661 6365 2069 6e20  rk_interface in 
+00013ef0: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+00013f00: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00013f10: 2020 2020 2020 2020 7377 6974 6368 203d          switch =
+00013f20: 207b 226e 616d 6522 3a20 6e6f 6465 5f6e   {"name": node_n
+00013f30: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
+00013f40: 5b22 7377 6974 6368 5f6e 616d 6522 5d7d  ["switch_name"]}
+00013f50: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013f60: 2020 2020 2020 6966 2073 7769 7463 685b        if switch[
+00013f70: 226e 616d 6522 5d20 6e6f 7420 696e 2063  "name"] not in c
+00013f80: 6f6c 6c65 6374 696e 675f 706f 696e 7473  ollecting_points
+00013f90: 5b22 7377 6974 6368 7322 5d2e 6b65 7973  ["switchs"].keys
+00013fa0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00013fb0: 2020 2020 2020 2020 2020 2020 636f 6c6c              coll
+00013fc0: 6563 7469 6e67 5f70 6f69 6e74 735b 2273  ecting_points["s
+00013fd0: 7769 7463 6873 225d 5b73 7769 7463 685b  witchs"][switch[
+00013fe0: 226e 616d 6522 5d5d 203d 205b 5d0a 2020  "name"]] = [].  
+00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014000: 2020 636f 6c6c 6563 7469 6e67 5f70 6f69    collecting_poi
+00014010: 6e74 735b 2273 7769 7463 6873 225d 5b73  nts["switchs"][s
+00014020: 7769 7463 685b 226e 616d 6522 5d5d 2e61  witch["name"]].a
+00014030: 7070 656e 6428 6e6f 6465 5b22 6e61 6d65  ppend(node["name
+00014040: 225d 290a 0a20 2020 2072 6574 7572 6e20  "])..    return 
+00014050: 636f 6c6c 6563 7469 6e67 5f70 6f69 6e74  collecting_point
+00014060: 730a 0a0a 6465 6620 736e 6170 7368 6f74  s...def snapshot
+00014070: 5f73 696d 756c 6174 696f 6e28 6964 5f73  _simulation(id_s
+00014080: 696d 756c 6174 696f 6e3a 2069 6e74 2920  imulation: int) 
+00014090: 2d3e 2073 7472 3a0a 2020 2020 2222 2243  -> str:.    """C
+000140a0: 7265 6174 6520 6120 736e 6170 7368 6f74  reate a snapshot
+000140b0: 206f 6620 6120 7369 6d75 6c61 7469 6f6e   of a simulation
+000140c0: 2e0a 0a20 2020 2041 6c6c 2074 6865 2066  ...    All the f
+000140d0: 696c 6573 2077 696c 6c20 6265 2073 746f  iles will be sto
+000140e0: 7265 6420 746f 0a20 2020 202f 6379 6265  red to.    /cybe
+000140f0: 722d 7261 6e67 652d 6361 7461 6c6f 672f  r-range-catalog/
+00014100: 7369 6d75 6c61 7469 6f6e 732f 3c68 6173  simulations/<has
+00014110: 6820 6361 6d70 6169 676e 3e2f 3c74 696d  h campaign>/<tim
+00014120: 6573 7461 6d70 3e2f 0a0a 2020 2020 5468  estamp>/..    Th
+00014130: 6973 2041 5049 2063 616c 6c20 7265 7475  is API call retu
+00014140: 726e 7320 7468 6520 7061 7468 2077 6865  rns the path whe
+00014150: 7265 2074 6865 2074 6f70 6f6c 6f67 7920  re the topology 
+00014160: 6669 6c65 2077 696c 6c20 6265 2073 746f  file will be sto
+00014170: 7265 642e 0a0a 2020 2020 5061 7261 6d65  red...    Parame
+00014180: 7465 7273 3a0a 0a20 2020 2069 645f 7369  ters:..    id_si
+00014190: 6d75 6c61 7469 6f6e 3a20 696e 740a 2020  mulation: int.  
+000141a0: 2020 2020 2020 5369 6d75 6c61 7469 6f6e        Simulation
+000141b0: 2074 6f20 736e 6170 7368 6f74 0a0a 2020   to snapshot..  
+000141c0: 2020 2222 220a 0a20 2020 2023 2073 696d    """..    # sim
+000141d0: 755f 736e 6170 2063 616e 206f 6e6c 7920  u_snap can only 
+000141e0: 6265 2064 6f6e 6520 6f6e 2061 2052 554e  be done on a RUN
+000141f0: 4e49 4e47 2073 696d 756c 6174 696f 6e0a  NING simulation.
+00014200: 2020 2020 6966 2073 696d 756c 6174 696f      if simulatio
+00014210: 6e5f 7374 6174 7573 2869 645f 7369 6d75  n_status(id_simu
+00014220: 6c61 7469 6f6e 2920 213d 2022 5255 4e4e  lation) != "RUNN
+00014230: 494e 4722 3a0a 2020 2020 2020 2020 7261  ING":.        ra
+00014240: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
+00014250: 2020 2020 2020 2020 2020 2022 4361 6e6e             "Cann
+00014260: 6f74 2063 7265 6174 6520 6120 736e 6170  ot create a snap
+00014270: 7368 6f74 206f 6620 7468 6520 7369 6d75  shot of the simu
+00014280: 6c61 7469 6f6e 2c20 6173 2074 6865 2073  lation, as the s
+00014290: 696d 756c 6174 696f 6e20 277b 7d27 2069  imulation '{}' i
+000142a0: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
+000142b0: 226e 6f74 2072 756e 6e69 6e67 222e 666f  "not running".fo
+000142c0: 726d 6174 2869 645f 7369 6d75 6c61 7469  rmat(id_simulati
+000142d0: 6f6e 290a 2020 2020 2020 2020 290a 0a20  on).        ).. 
+000142e0: 2020 2023 2043 616c 6c20 736e 6170 7368     # Call snapsh
+000142f0: 6f74 2041 5049 0a20 2020 2072 6573 756c  ot API.    resul
+00014300: 7420 3d20 5f70 6f73 7428 6622 2f73 696d  t = _post(f"/sim
+00014310: 756c 6174 696f 6e2f 7b69 645f 7369 6d75  ulation/{id_simu
+00014320: 6c61 7469 6f6e 7d2f 736e 6170 7368 6f74  lation}/snapshot
+00014330: 2229 0a20 2020 2069 6620 7265 7375 6c74  ").    if result
+00014340: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
+00014350: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
+00014360: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
+00014370: 742c 2022 4572 726f 7220 7768 696c 6520  t, "Error while 
+00014380: 6372 6561 7469 6e67 2073 6e61 7073 686f  creating snapsho
+00014390: 7422 290a 0a20 2020 2079 616d 6c3a 2073  t")..    yaml: s
+000143a0: 7472 203d 2072 6573 756c 742e 6a73 6f6e  tr = result.json
+000143b0: 2829 0a0a 2020 2020 6c6f 6767 6572 2e69  ()..    logger.i
+000143c0: 6e66 6f28 6622 5b2b 5d20 5374 6172 7469  nfo(f"[+] Starti
+000143d0: 6e67 2074 6865 2073 6e61 7073 686f 7420  ng the snapshot 
+000143e0: 6f66 2073 696d 756c 6174 696f 6e20 7b69  of simulation {i
+000143f0: 645f 7369 6d75 6c61 7469 6f6e 7d2e 2e2e  d_simulation}...
+00014400: 2229 0a20 2020 2077 6869 6c65 2073 696d  ").    while sim
+00014410: 756c 6174 696f 6e5f 7374 6174 7573 2869  ulation_status(i
+00014420: 645f 7369 6d75 6c61 7469 6f6e 2920 213d  d_simulation) !=
+00014430: 2022 534e 4150 5348 4f54 223a 0a20 2020   "SNAPSHOT":.   
+00014440: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+00014450: 3129 0a0a 2020 2020 2020 2020 7369 6d75  1)..        simu
+00014460: 6c61 7469 6f6e 5f64 6963 7420 3d20 6665  lation_dict = fe
+00014470: 7463 685f 7369 6d75 6c61 7469 6f6e 2869  tch_simulation(i
+00014480: 645f 7369 6d75 6c61 7469 6f6e 290a 2020  d_simulation).  
+00014490: 2020 2020 2020 6375 7272 656e 745f 7374        current_st
+000144a0: 6174 7573 203d 2073 696d 756c 6174 696f  atus = simulatio
+000144b0: 6e5f 6469 6374 5b22 7374 6174 7573 225d  n_dict["status"]
+000144c0: 0a20 2020 2020 2020 2069 6620 6375 7272  .        if curr
+000144d0: 656e 745f 7374 6174 7573 203d 3d20 2245  ent_status == "E
+000144e0: 5252 4f52 223a 0a20 2020 2020 2020 2020  RROR":.         
+000144f0: 2020 2065 7272 6f72 5f6d 6573 7361 6765     error_message
+00014500: 203d 2073 696d 756c 6174 696f 6e5f 6469   = simulation_di
+00014510: 6374 5b22 6572 726f 725f 6d73 6722 5d0a  ct["error_msg"].
+00014520: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00014530: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
+00014540: 2020 2020 2020 2020 2020 2020 2022 4572               "Er
+00014550: 726f 7220 6475 7269 6e67 2073 696d 756c  ror during simul
+00014560: 6174 696f 6e20 736e 6170 7368 6f74 3a20  ation snapshot: 
+00014570: 277b 7d27 222e 666f 726d 6174 2865 7272  '{}'".format(err
+00014580: 6f72 5f6d 6573 7361 6765 290a 2020 2020  or_message).    
+00014590: 2020 2020 2020 2020 290a 0a20 2020 206c          )..    l
+000145a0: 6f67 6765 722e 696e 666f 2822 5b2b 5d20  ogger.info("[+] 
+000145b0: 536e 6170 7368 6f74 2070 726f 6365 7373  Snapshot process
+000145c0: 2068 6173 2073 7461 7274 6564 2229 0a0a   has started")..
+000145d0: 2020 2020 7768 696c 6520 7369 6d75 6c61      while simula
+000145e0: 7469 6f6e 5f73 7461 7475 7328 6964 5f73  tion_status(id_s
+000145f0: 696d 756c 6174 696f 6e29 2021 3d20 2252  imulation) != "R
+00014600: 4541 4459 223a 0a20 2020 2020 2020 206c  EADY":.        l
+00014610: 6f67 6765 722e 696e 666f 2822 2020 5b2b  ogger.info("  [+
+00014620: 5d20 536e 6170 7368 6f74 2069 6e20 7072  ] Snapshot in pr
+00014630: 6f67 7265 7373 2e2e 2e22 290a 2020 2020  ogress...").    
+00014640: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
+00014650: 290a 0a20 2020 2020 2020 2073 696d 756c  )..        simul
+00014660: 6174 696f 6e5f 6469 6374 203d 2066 6574  ation_dict = fet
+00014670: 6368 5f73 696d 756c 6174 696f 6e28 6964  ch_simulation(id
+00014680: 5f73 696d 756c 6174 696f 6e29 0a20 2020  _simulation).   
+00014690: 2020 2020 2063 7572 7265 6e74 5f73 7461       current_sta
+000146a0: 7475 7320 3d20 7369 6d75 6c61 7469 6f6e  tus = simulation
+000146b0: 5f64 6963 745b 2273 7461 7475 7322 5d0a  _dict["status"].
+000146c0: 2020 2020 2020 2020 6966 2063 7572 7265          if curre
+000146d0: 6e74 5f73 7461 7475 7320 3d3d 2022 4552  nt_status == "ER
+000146e0: 524f 5222 3a0a 2020 2020 2020 2020 2020  ROR":.          
+000146f0: 2020 6572 726f 725f 6d65 7373 6167 6520    error_message 
+00014700: 3d20 7369 6d75 6c61 7469 6f6e 5f64 6963  = simulation_dic
+00014710: 745b 2265 7272 6f72 5f6d 7367 225d 0a20  t["error_msg"]. 
+00014720: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00014730: 2045 7863 6570 7469 6f6e 280a 2020 2020   Exception(.    
+00014740: 2020 2020 2020 2020 2020 2020 2245 7272              "Err
+00014750: 6f72 2064 7572 696e 6720 7369 6d75 6c61  or during simula
+00014760: 7469 6f6e 2073 6e61 7073 686f 743a 2027  tion snapshot: '
+00014770: 7b7d 2722 2e66 6f72 6d61 7428 6572 726f  {}'".format(erro
+00014780: 725f 6d65 7373 6167 6529 0a20 2020 2020  r_message).     
+00014790: 2020 2020 2020 2029 0a0a 2020 2020 7265         )..    re
+000147a0: 7475 726e 2079 616d 6c0a 0a0a 6465 6620  turn yaml...def 
+000147b0: 636f 6d70 7574 655f 696e 6672 6173 7472  compute_infrastr
+000147c0: 7563 7475 7265 5f73 7461 7475 7328 2920  ucture_status() 
+000147d0: 2d3e 2041 6e79 3a0a 2020 2020 2222 2247  -> Any:.    """G
+000147e0: 6574 2076 6972 7463 6c69 656e 7420 7365  et virtclient se
+000147f0: 7276 6963 6520 7374 6174 7573 2e22 2222  rvice status."""
+00014800: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
+00014810: 6574 2822 2f73 696d 756c 6174 696f 6e2f  et("/simulation/
+00014820: 636f 6d70 7574 655f 696e 6672 6173 7472  compute_infrastr
+00014830: 7563 7475 7265 5f73 7461 7475 7322 290a  ucture_status").
+00014840: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
+00014850: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+00014860: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
+00014870: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
+00014880: 2022 4361 6e6e 6f74 2067 6574 2063 6f6d   "Cannot get com
+00014890: 7075 7465 2069 6e66 7261 7374 7275 6374  pute infrastruct
+000148a0: 7572 6520 7374 6174 7573 2229 0a0a 2020  ure status")..  
+000148b0: 2020 7369 6d75 6c61 7469 6f6e 5f64 6963    simulation_dic
+000148c0: 7420 3d20 7265 7375 6c74 2e6a 736f 6e28  t = result.json(
+000148d0: 290a 2020 2020 7265 7475 726e 2073 696d  ).    return sim
+000148e0: 756c 6174 696f 6e5f 6469 6374 0a0a 0a64  ulation_dict...d
+000148f0: 6566 2061 6464 5f64 6e73 5f65 6e74 7269  ef add_dns_entri
+00014900: 6573 2869 645f 7369 6d75 6c61 7469 6f6e  es(id_simulation
+00014910: 3a20 696e 742c 2064 6e73 5f65 6e74 7269  : int, dns_entri
+00014920: 6573 3a20 4469 6374 5b73 7472 2c20 7374  es: Dict[str, st
+00014930: 725d 2920 2d3e 2073 7472 3a0a 2020 2020  r]) -> str:.    
+00014940: 2222 2241 6464 2076 6f6c 6174 696c 6520  """Add volatile 
+00014950: 444e 5320 656e 7472 6965 7320 746f 2074  DNS entries to t
+00014960: 6865 2063 7572 7265 6e74 2073 696d 756c  he current simul
+00014970: 6174 696f 6e2e 2056 6f6c 6174 696c 6520  ation. Volatile 
+00014980: 6d65 616e 7320 7468 6174 2069 7420 6973  means that it is
+00014990: 206e 6f74 0a20 2020 2073 746f 7265 6420   not.    stored 
+000149a0: 696e 2064 6174 6162 6173 652e 0a0a 2020  in database...  
+000149b0: 2020 2222 220a 0a20 2020 2064 6174 6120    """..    data 
+000149c0: 3d20 6a73 6f6e 2e64 756d 7073 2864 6e73  = json.dumps(dns
+000149d0: 5f65 6e74 7269 6573 290a 2020 2020 7265  _entries).    re
+000149e0: 7375 6c74 203d 205f 706f 7374 280a 2020  sult = _post(.  
+000149f0: 2020 2020 2020 6622 2f73 696d 756c 6174        f"/simulat
+00014a00: 696f 6e2f 7b69 645f 7369 6d75 6c61 7469  ion/{id_simulati
+00014a10: 6f6e 7d2f 6164 645f 646e 735f 656e 7472  on}/add_dns_entr
+00014a20: 6965 7322 2c0a 2020 2020 2020 2020 6461  ies",.        da
+00014a30: 7461 3d64 6174 612c 0a20 2020 2020 2020  ta=data,.       
+00014a40: 2068 6561 6465 7273 3d7b 2243 6f6e 7465   headers={"Conte
+00014a50: 6e74 2d54 7970 6522 3a20 2261 7070 6c69  nt-Type": "appli
+00014a60: 6361 7469 6f6e 2f6a 736f 6e22 7d2c 0a20  cation/json"},. 
+00014a70: 2020 2029 0a0a 2020 2020 6966 2072 6573     )..    if res
+00014a80: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
+00014a90: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
+00014aa0: 5f68 616e 646c 655f 6572 726f 7228 7265  _handle_error(re
+00014ab0: 7375 6c74 2c20 2245 7272 6f72 2077 6869  sult, "Error whi
+00014ac0: 6c65 2061 6464 696e 6720 444e 5320 656e  le adding DNS en
+00014ad0: 7472 6965 7322 290a 0a0a 6465 6620 636f  tries")...def co
+00014ae0: 6e6e 6563 745f 686f 7374 2869 645f 7369  nnect_host(id_si
+00014af0: 6d75 6c61 7469 6f6e 3a20 696e 7429 202d  mulation: int) -
+00014b00: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2243  > None:.    """C
+00014b10: 6f6e 6e65 6374 2074 6865 2068 6f73 7420  onnect the host 
+00014b20: 696e 7465 7266 6163 6520 746f 2074 6865  interface to the
+00014b30: 2063 7572 7265 6e74 2073 696d 756c 6174   current simulat
+00014b40: 696f 6e2e 2222 220a 0a20 2020 2072 6573  ion."""..    res
+00014b50: 756c 7420 3d20 5f67 6574 2866 222f 7369  ult = _get(f"/si
+00014b60: 6d75 6c61 7469 6f6e 2f7b 6964 5f73 696d  mulation/{id_sim
+00014b70: 756c 6174 696f 6e7d 2f63 6f6e 6e65 6374  ulation}/connect
+00014b80: 5f68 6f73 7422 290a 0a20 2020 2069 6620  _host")..    if 
+00014b90: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
+00014ba0: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
+00014bb0: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+00014bc0: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+00014bd0: 7375 6c74 2c0a 2020 2020 2020 2020 2020  sult,.          
+00014be0: 2020 6622 4361 6e6e 6f74 2065 7865 6375    f"Cannot execu
+00014bf0: 7465 206f 7065 7261 7469 6f6e 2027 636f  te operation 'co
+00014c00: 6e6e 6563 745f 686f 7374 2720 6f6e 2073  nnect_host' on s
+00014c10: 696d 756c 6174 696f 6e20 277b 6964 5f73  imulation '{id_s
+00014c20: 696d 756c 6174 696f 6e7d 272e 222c 0a20  imulation}'.",. 
+00014c30: 2020 2020 2020 2029 0a0a 0a64 6566 2064         )...def d
+00014c40: 6973 636f 6e6e 6563 745f 686f 7374 2869  isconnect_host(i
+00014c50: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
+00014c60: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+00014c70: 2222 2244 6973 636f 6e6e 6563 7420 7468  """Disconnect th
+00014c80: 6520 686f 7374 2069 6e74 6572 6661 6365  e host interface
+00014c90: 2074 6f20 7468 6520 6375 7272 656e 7420   to the current 
+00014ca0: 7369 6d75 6c61 7469 6f6e 2e22 2222 0a0a  simulation."""..
+00014cb0: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
+00014cc0: 7428 6622 2f73 696d 756c 6174 696f 6e2f  t(f"/simulation/
+00014cd0: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d2f  {id_simulation}/
+00014ce0: 6469 7363 6f6e 6e65 6374 5f68 6f73 7422  disconnect_host"
+00014cf0: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
+00014d00: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
+00014d10: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
+00014d20: 6e64 6c65 5f65 7272 6f72 280a 2020 2020  ndle_error(.    
+00014d30: 2020 2020 2020 2020 7265 7375 6c74 2c0a          result,.
+00014d40: 2020 2020 2020 2020 2020 2020 6622 4361              f"Ca
+00014d50: 6e6e 6f74 2065 7865 6375 7465 206f 7065  nnot execute ope
+00014d60: 7261 7469 6f6e 2027 6469 7363 6f6e 6e65  ration 'disconne
+00014d70: 6374 5f68 6f73 7427 206f 6e20 7369 6d75  ct_host' on simu
+00014d80: 6c61 7469 6f6e 2027 7b69 645f 7369 6d75  lation '{id_simu
+00014d90: 6c61 7469 6f6e 7d27 2e22 2c0a 2020 2020  lation}'.",.    
+00014da0: 2020 2020 290a 0a0a 6465 6620 6765 6e65      )...def gene
+00014db0: 7261 7465 5f6d 616c 6963 696f 7573 5f64  rate_malicious_d
+00014dc0: 6f6d 6169 6e73 2861 6c67 6f72 6974 686d  omains(algorithm
+00014dd0: 3a20 7374 7220 3d20 4e6f 6e65 2c20 6e75  : str = None, nu
+00014de0: 6d62 6572 3a20 696e 7420 3d20 3129 202d  mber: int = 1) -
+00014df0: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
+00014e00: 2022 2222 4765 6e65 7261 7465 2061 6e64   """Generate and
+00014e10: 2072 6574 7572 6e20 6120 6c69 7374 206f   return a list o
+00014e20: 6620 6d61 6c69 6369 6f75 7320 646f 6d61  f malicious doma
+00014e30: 696e 732e 2222 220a 0a20 2020 2064 6174  ins."""..    dat
+00014e40: 615f 6469 6374 203d 207b 0a20 2020 2020  a_dict = {.     
+00014e50: 2020 2022 616c 676f 7269 7468 6d22 3a20     "algorithm": 
+00014e60: 616c 676f 7269 7468 6d2c 0a20 2020 2020  algorithm,.     
+00014e70: 2020 2022 6e75 6d62 6572 223a 206e 756d     "number": num
+00014e80: 6265 722c 0a20 2020 207d 0a20 2020 2064  ber,.    }.    d
+00014e90: 6174 6120 3d20 6a73 6f6e 2e64 756d 7073  ata = json.dumps
+00014ea0: 2864 6174 615f 6469 6374 290a 0a20 2020  (data_dict)..   
+00014eb0: 2072 6573 756c 7420 3d20 5f70 6f73 7428   result = _post(
+00014ec0: 0a20 2020 2020 2020 2022 2f74 6f70 6f6c  .        "/topol
+00014ed0: 6f67 792f 6765 6e65 7261 7465 5f6d 616c  ogy/generate_mal
+00014ee0: 6963 696f 7573 5f64 6f6d 6169 6e73 222c  icious_domains",
+00014ef0: 0a20 2020 2020 2020 2064 6174 613d 6461  .        data=da
+00014f00: 7461 2c0a 2020 2020 2020 2020 6865 6164  ta,.        head
+00014f10: 6572 733d 7b22 436f 6e74 656e 742d 5479  ers={"Content-Ty
+00014f20: 7065 223a 2022 6170 706c 6963 6174 696f  pe": "applicatio
+00014f30: 6e2f 6a73 6f6e 227d 2c0a 2020 2020 290a  n/json"},.    ).
+00014f40: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
+00014f50: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+00014f60: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
+00014f70: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
+00014f80: 2022 4572 726f 7220 7768 696c 6520 6164   "Error while ad
+00014f90: 6469 6e67 2044 4e53 2065 6e74 7269 6573  ding DNS entries
+00014fa0: 2229 0a0a 2020 2020 646f 6d61 696e 7320  ")..    domains 
+00014fb0: 3d20 7265 7375 6c74 2e6a 736f 6e28 290a  = result.json().
+00014fc0: 2020 2020 7265 7475 726e 2064 6f6d 6169      return domai
+00014fd0: 6e73 5b22 646f 6d61 696e 7322 5d0a 0a0a  ns["domains"]...
+00014fe0: 6465 6620 6372 6561 7465 5f64 6174 6173  def create_datas
+00014ff0: 6574 280a 2020 2020 6964 5f73 696d 756c  et(.    id_simul
+00015000: 6174 696f 6e3a 2069 6e74 2c20 646f 6e74  ation: int, dont
+00015010: 5f63 6865 636b 5f6c 6f67 735f 7061 7468  _check_logs_path
+00015020: 3a20 626f 6f6c 203d 2046 616c 7365 0a29  : bool = False.)
+00015030: 202d 3e20 4f70 7469 6f6e 616c 5b75 7569   -> Optional[uui
+00015040: 642e 5555 4944 5d3a 0a20 2020 2022 2222  d.UUID]:.    """
+00015050: 0a20 2020 2048 616e 646c 6573 2074 6865  .    Handles the
+00015060: 2063 7265 6174 696f 6e20 6f66 2074 6865   creation of the
+00015070: 2064 6174 6173 6574 2061 6674 6572 2074   dataset after t
+00015080: 6865 2065 6e64 206f 6620 6120 7369 6d75  he end of a simu
+00015090: 6c61 7469 6f6e 0a0a 2020 2020 4d75 7374  lation..    Must
+000150a0: 2062 6520 6361 6c6c 6564 2061 6674 6572   be called after
+000150b0: 2061 2053 544f 5020 6f70 6572 6174 696f   a STOP operatio
+000150c0: 6e2c 2061 6e64 206f 6e63 6520 616c 6c20  n, and once all 
+000150d0: 636f 6d70 7574 6520 7365 7276 6572 730a  compute servers.
+000150e0: 2020 2020 2876 6972 7463 6c69 656e 7429      (virtclient)
+000150f0: 2068 6176 6520 6675 6c6c 7920 7374 6f70   have fully stop
+00015100: 7065 642e 0a0a 2020 2020 4261 7369 6361  ped...    Basica
+00015110: 6c6c 792c 2074 6869 7320 6675 6e63 7469  lly, this functi
+00015120: 6f6e 2063 6f6d 6d75 6e69 6361 7465 7320  on communicates 
+00015130: 7769 7468 2074 6865 2074 6865 2063 6f72  with the the cor
+00015140: 6520 4150 492c 2077 6869 6368 2069 7473  e API, which its
+00015150: 656c 660a 2020 2020 636f 6d6d 756e 6963  elf.    communic
+00015160: 6174 6573 2077 6974 6820 7468 6520 7075  ates with the pu
+00015170: 626c 6973 6820 7365 7276 6572 2773 2022  blish server's "
+00015180: 6261 636b 656e 6422 2041 5049 2e0a 0a20  backend" API... 
+00015190: 2020 203a 7061 7261 6d20 6964 5f73 696d     :param id_sim
+000151a0: 756c 6174 696f 6e3a 2074 6865 2073 696d  ulation: the sim
+000151b0: 756c 6174 696f 6e20 7768 6963 6820 7761  ulation which wa
+000151c0: 7320 6a75 7374 2073 746f 7070 6564 2061  s just stopped a
+000151d0: 6e64 2066 726f 6d20 7768 6963 6820 6f75  nd from which ou
+000151e0: 7470 7574 2074 6865 2064 6174 6173 6574  tput the dataset
+000151f0: 2073 686f 756c 6420 6265 2063 7265 6174   should be creat
+00015200: 6564 0a20 2020 203a 7265 7475 726e 3a20  ed.    :return: 
+00015210: 7468 6520 6e65 7720 6461 7461 7365 7420  the new dataset 
+00015220: 6964 0a20 2020 2022 2222 0a0a 2020 2020  id.    """..    
+00015230: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+00015240: 2020 2020 2022 5b2b 5d20 476f 696e 6720       "[+] Going 
+00015250: 746f 2063 7265 6174 6520 6461 7461 7365  to create datase
+00015260: 7420 6261 7365 6420 6f6e 2064 6174 6120  t based on data 
+00015270: 7072 6f64 7563 6564 2062 7920 7369 6d75  produced by simu
+00015280: 6c61 7469 6f6e 2049 4420 277b 7d27 222e  lation ID '{}'".
+00015290: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+000152a0: 2020 2020 6964 5f73 696d 756c 6174 696f      id_simulatio
+000152b0: 6e0a 2020 2020 2020 2020 290a 2020 2020  n.        ).    
+000152c0: 290a 0a20 2020 2069 6620 646f 6e74 5f63  )..    if dont_c
+000152d0: 6865 636b 5f6c 6f67 735f 7061 7468 2069  heck_logs_path i
+000152e0: 7320 4661 6c73 653a 0a20 2020 2020 2020  s False:.       
+000152f0: 2069 6620 5f63 6865 636b 5f6c 6f67 735f   if _check_logs_
+00015300: 7061 7468 2869 645f 7369 6d75 6c61 7469  path(id_simulati
+00015310: 6f6e 293a 0a20 2020 2020 2020 2020 2020  on):.           
+00015320: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00015330: 2020 2320 4173 6b20 7468 6520 636f 7265    # Ask the core
+00015340: 2041 5049 2074 6f20 636f 6e74 6163 7420   API to contact 
+00015350: 7468 6520 2f62 6163 6b65 6e64 2f20 7075  the /backend/ pu
+00015360: 626c 6973 6820 7365 7276 6572 2041 5049  blish server API
+00015370: 0a20 2020 2023 2069 6e20 6f72 6465 7220  .    # in order 
+00015380: 746f 2073 7461 7274 2074 6865 2064 6174  to start the dat
+00015390: 6173 6574 2063 7265 6174 696f 6e20 7072  aset creation pr
+000153a0: 6f63 6573 730a 2020 2020 7265 7375 6c74  ocess.    result
+000153b0: 203d 205f 706f 7374 2866 222f 6372 6561   = _post(f"/crea
+000153c0: 7465 5f64 6174 6173 6574 2f7b 6964 5f73  te_dataset/{id_s
+000153d0: 696d 756c 6174 696f 6e7d 2229 0a20 2020  imulation}").   
+000153e0: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+000153f0: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+00015400: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+00015410: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
+00015420: 6e6e 6f74 2069 6e69 7469 6174 6520 7468  nnot initiate th
+00015430: 6520 6372 6561 7469 6f6e 206f 6620 7468  e creation of th
+00015440: 6520 6461 7461 7365 7422 290a 0a20 2020  e dataset")..   
+00015450: 2064 6174 6173 6574 5f69 6420 3d20 7265   dataset_id = re
+00015460: 7375 6c74 2e6a 736f 6e28 295b 2264 6174  sult.json()["dat
+00015470: 6173 6574 5f69 6422 5d0a 0a20 2020 206c  aset_id"]..    l
+00015480: 6f67 6765 722e 696e 666f 2866 2220 205b  ogger.info(f"  [
+00015490: 2b5d 2044 6174 6173 6574 2070 7265 2d63  +] Dataset pre-c
+000154a0: 7265 6174 6564 2077 6974 6820 6461 7461  reated with data
+000154b0: 7365 7420 6964 207b 6461 7461 7365 745f  set id {dataset_
+000154c0: 6964 7d22 290a 0a20 2020 2023 2053 7461  id}")..    # Sta
+000154d0: 7274 2061 6e20 6163 7469 7665 2077 6169  rt an active wai
+000154e0: 7469 6e67 206c 6f6f 7020 756e 7469 6c20  ting loop until 
+000154f0: 7468 6520 6461 7461 7365 7420 6372 6561  the dataset crea
+00015500: 7469 6f6e 2069 6620 6675 6c6c 7920 636f  tion if fully co
+00015510: 6d70 6c65 7465 0a20 2020 2023 2049 6e64  mplete.    # Ind
+00015520: 6565 642c 2064 6174 6173 6574 2063 7265  eed, dataset cre
+00015530: 6174 696f 6e20 696e 766f 6c76 6573 2074  ation involves t
+00015540: 6865 2064 6f77 6e6c 6f61 6420 6f66 2070  he download of p
+00015550: 6f74 656e 7469 616c 6c79 206c 6172 6765  otentially large
+00015560: 0a20 2020 2023 2066 696c 6573 206f 7665  .    # files ove
+00015570: 7273 2074 6865 206e 6574 776f 726b 2c20  rs the network, 
+00015580: 7768 6963 6820 6361 6e20 7461 6b65 2073  which can take s
+00015590: 6f6d 6520 7469 6d65 210a 2020 2020 6d61  ome time!.    ma
+000155a0: 785f 7265 7472 6965 7320 3d20 350a 2020  x_retries = 5.  
+000155b0: 2020 7265 7472 6965 7320 3d20 6d61 785f    retries = max_
+000155c0: 7265 7472 6965 730a 2020 2020 7768 696c  retries.    whil
+000155d0: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
+000155e0: 7469 6d65 2e73 6c65 6570 2832 290a 0a20  time.sleep(2).. 
+000155f0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00015600: 5f67 6574 2866 222f 6372 6561 7465 5f64  _get(f"/create_d
+00015610: 6174 6173 6574 2f73 7461 7475 732f 7b64  ataset/status/{d
+00015620: 6174 6173 6574 5f69 647d 2229 0a20 2020  ataset_id}").   
+00015630: 2020 2020 2069 6620 7265 7375 6c74 2e73       if result.s
+00015640: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+00015650: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
+00015660: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00015670: 2020 2020 7265 7375 6c74 2e68 6561 6465      result.heade
+00015680: 7273 2e67 6574 2822 636f 6e74 656e 742d  rs.get("content-
+00015690: 7479 7065 2229 203d 3d20 2261 7070 6c69  type") == "appli
+000156a0: 6361 7469 6f6e 2f6a 736f 6e22 0a20 2020  cation/json".   
+000156b0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+000156c0: 2022 6d65 7373 6167 6522 2069 6e20 7265   "message" in re
+000156d0: 7375 6c74 2e6a 736f 6e28 290a 2020 2020  sult.json().    
+000156e0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+000156f0: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00015700: 5f6d 7367 203d 2072 6573 756c 742e 6a73  _msg = result.js
+00015710: 6f6e 2829 5b22 6d65 7373 6167 6522 5d0a  on()["message"].
+00015720: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00015730: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015740: 2020 6572 726f 725f 6d73 6720 3d20 7265    error_msg = re
+00015750: 7375 6c74 2e74 6578 740a 0a20 2020 2020  sult.text..     
+00015760: 2020 2020 2020 2023 2052 6574 7279 2074         # Retry t
+00015770: 6f20 6765 7420 7468 6520 7374 6174 7573  o get the status
+00015780: 2061 2063 6f75 706c 6520 6f66 2074 696d   a couple of tim
+00015790: 6573 2062 6566 6f72 6520 7173 656e 6469  es before qsendi
+000157a0: 6e67 2062 6163 6b20 616e 2065 7272 6f72  ng back an error
+000157b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000157c0: 7265 7472 6965 7320 3d3d 2030 3a0a 2020  retries == 0:.  
+000157d0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000157e0: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
+000157f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015800: 2020 2022 4572 726f 7220 6475 7269 6e67     "Error during
+00015810: 2063 7265 6174 696f 6e20 6f66 2064 6174   creation of dat
+00015820: 6173 6574 207b 7d3a 2063 6f75 6c64 206e  aset {}: could n
+00015830: 6f74 2067 6574 2073 7461 7475 7320 6f66  ot get status of
+00015840: 2074 6865 2064 6174 6173 6574 2063 7265   the dataset cre
+00015850: 6174 696f 6e20 6166 7465 7220 7b7d 2074  ation after {} t
+00015860: 7269 6573 2e20 436f 7265 2041 5049 2048  ries. Core API H
+00015870: 5454 5020 7374 6174 7573 3a20 7b7d 2e20  TTP status: {}. 
+00015880: 5265 7370 6f6e 7365 3a20 7b7d 2022 2e66  Response: {} ".f
+00015890: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+000158a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000158b0: 6174 6173 6574 5f69 642c 206d 6178 5f72  ataset_id, max_r
+000158c0: 6574 7269 6573 2c20 7265 7375 6c74 2e73  etries, result.s
+000158d0: 7461 7475 735f 636f 6465 2c20 6572 726f  tatus_code, erro
+000158e0: 725f 6d73 670a 2020 2020 2020 2020 2020  r_msg.          
+000158f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00015900: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00015910: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00015920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015930: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
+00015940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015950: 2020 2020 2220 205b 2b5d 2043 6f75 6c64      "  [+] Could
+00015960: 206e 6f74 2067 6574 2073 7461 7475 7320   not get status 
+00015970: 6f66 2064 6174 6173 6574 2063 7265 6174  of dataset creat
+00015980: 696f 6e20 2852 6574 7269 6573 206c 6566  ion (Retries lef
+00015990: 743a 207b 7d2e 2043 6f72 6520 4150 4920  t: {}. Core API 
+000159a0: 4854 5450 2073 7461 7475 733a 207b 7d2e  HTTP status: {}.
+000159b0: 2052 6573 706f 6e73 653a 207b 7d29 222e   Response: {})".
+000159c0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+000159d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159e0: 7265 7472 6965 732c 2072 6573 756c 742e  retries, result.
+000159f0: 7374 6174 7573 5f63 6f64 652c 2065 7272  status_code, err
+00015a00: 6f72 5f6d 7367 0a20 2020 2020 2020 2020  or_msg.         
+00015a10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00015a20: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00015a30: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00015a40: 6574 7269 6573 202d 3d20 310a 2020 2020  etries -= 1.    
+00015a50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00015a60: 2020 2020 2020 2320 5265 7365 7420 7468        # Reset th
+00015a70: 6520 6e75 6d62 6572 206f 6620 7265 7472  e number of retr
+00015a80: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
+00015a90: 7265 7472 6965 7320 3d20 6d61 785f 7265  retries = max_re
+00015aa0: 7472 6965 730a 0a20 2020 2020 2020 2020  tries..         
+00015ab0: 2020 2023 2047 6574 2074 6865 2073 7461     # Get the sta
+00015ac0: 7475 7320 616e 6420 6d65 7373 6167 650a  tus and message.
+00015ad0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00015ae0: 7365 745f 6372 6561 7469 6f6e 5f73 7461  set_creation_sta
+00015af0: 7475 7320 3d20 7265 7375 6c74 2e6a 736f  tus = result.jso
+00015b00: 6e28 295b 2273 7461 7475 7322 5d0a 2020  n()["status"].  
+00015b10: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+00015b20: 745f 6372 6561 7469 6f6e 5f6d 6573 7361  t_creation_messa
+00015b30: 6765 203d 2072 6573 756c 742e 6a73 6f6e  ge = result.json
+00015b40: 2829 5b22 6d65 7373 6167 6522 5d0a 0a20  ()["message"].. 
+00015b50: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00015b60: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
+00015b70: 2020 2020 2020 2020 2220 205b 2b5d 2044          "  [+] D
+00015b80: 6174 6173 6574 2063 7265 6174 696f 6e20  ataset creation 
+00015b90: 696e 2070 726f 6772 6573 7320 2853 7461  in progress (Sta
+00015ba0: 7475 733a 207b 7d29 222e 666f 726d 6174  tus: {})".format
+00015bb0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00015bc0: 2020 2020 2020 6461 7461 7365 745f 6372        dataset_cr
+00015bd0: 6561 7469 6f6e 5f73 7461 7475 730a 2020  eation_status.  
+00015be0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00015bf0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00015c00: 2020 2020 2020 2020 2020 2069 6620 6461             if da
+00015c10: 7461 7365 745f 6372 6561 7469 6f6e 5f73  taset_creation_s
+00015c20: 7461 7475 7320 3d3d 2022 4649 4e49 5348  tatus == "FINISH
+00015c30: 4544 223a 0a20 2020 2020 2020 2020 2020  ED":.           
+00015c40: 2020 2020 2023 2041 6c6c 2077 656e 7420       # All went 
+00015c50: 7765 6c6c 0a20 2020 2020 2020 2020 2020  well.           
+00015c60: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+00015c70: 2020 2020 2020 2065 6c69 6620 6461 7461         elif data
+00015c80: 7365 745f 6372 6561 7469 6f6e 5f73 7461  set_creation_sta
+00015c90: 7475 7320 3d3d 2022 4649 4e49 5348 4544  tus == "FINISHED
+00015ca0: 5f45 5252 4f52 223a 0a20 2020 2020 2020  _ERROR":.       
+00015cb0: 2020 2020 2020 2020 2023 2054 6865 2064           # The d
+00015cc0: 6174 6173 6574 2063 7265 6174 696f 6e20  ataset creation 
+00015cd0: 656e 636f 756e 7465 7265 6420 6572 726f  encountered erro
+00015ce0: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
+00015cf0: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+00015d00: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00015d10: 2020 2020 2020 2020 2245 7272 6f72 2064          "Error d
+00015d20: 7572 696e 6720 6372 6561 7469 6f6e 206f  uring creation o
+00015d30: 6620 6461 7461 7365 7420 7b7d 3a20 6461  f dataset {}: da
+00015d40: 7461 7365 7420 6372 6561 7469 6f6e 2065  taset creation e
+00015d50: 6e64 6564 2077 6974 6820 6572 726f 7273  nded with errors
+00015d60: 2028 277b 7d27 292e 222e 666f 726d 6174   ('{}').".format
+00015d70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00015d80: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+00015d90: 745f 6964 2c20 6461 7461 7365 745f 6372  t_id, dataset_cr
+00015da0: 6561 7469 6f6e 5f6d 6573 7361 6765 0a20  eation_message. 
+00015db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015dc0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00015dd0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00015de0: 2020 2023 204f 7468 6572 7769 7365 2c20     # Otherwise, 
+00015df0: 6461 7461 7365 7420 6372 6561 7469 6f6e  dataset creation
+00015e00: 2069 7320 6e6f 7420 6669 6e69 7368 6564   is not finished
+00015e10: 2c20 6a75 7374 206c 6f6f 700a 0a20 2020  , just loop..   
+00015e20: 206c 6f67 6765 722e 696e 666f 2822 5b2b   logger.info("[+
+00015e30: 5d20 4461 7461 7365 7420 6372 6561 7469  ] Dataset creati
+00015e40: 6f6e 2077 6173 2063 6f72 7265 6374 6c79  on was correctly
+00015e50: 2065 7865 6375 7465 6422 290a 0a20 2020   executed")..   
+00015e60: 2023 2053 6574 2074 6865 2073 696d 756c   # Set the simul
+00015e70: 6174 696f 6e20 7374 6174 7573 2074 6f20  ation status to 
+00015e80: 5245 4144 590a 2020 2020 7570 6461 7465  READY.    update
+00015e90: 5f73 696d 756c 6174 696f 6e28 6964 5f73  _simulation(id_s
+00015ea0: 696d 756c 6174 696f 6e2c 207b 2273 7461  imulation, {"sta
+00015eb0: 7475 7322 3a20 2252 4541 4459 227d 290a  tus": "READY"}).
+00015ec0: 0a20 2020 2073 696d 756c 6174 696f 6e20  .    simulation 
+00015ed0: 3d20 6665 7463 685f 7369 6d75 6c61 7469  = fetch_simulati
+00015ee0: 6f6e 2869 645f 7369 6d75 6c61 7469 6f6e  on(id_simulation
+00015ef0: 290a 2020 2020 6c6f 6767 6572 2e69 6e66  ).    logger.inf
+00015f00: 6f28 225b 2b5d 2043 7572 7265 6e74 2073  o("[+] Current s
+00015f10: 696d 756c 6174 696f 6e20 7374 6174 7573  imulation status
+00015f20: 3a20 277b 7d27 222e 666f 726d 6174 2873  : '{}'".format(s
+00015f30: 696d 756c 6174 696f 6e5b 2273 7461 7475  imulation["statu
+00015f40: 7322 5d29 290a 0a20 2020 2072 6574 7572  s"]))..    retur
+00015f50: 6e20 7575 6964 2e55 5549 4428 6461 7461  n uuid.UUID(data
+00015f60: 7365 745f 6964 290a 0a0a 6465 6620 5f63  set_id)...def _c
+00015f70: 6865 636b 5f6c 6f67 735f 7061 7468 2869  heck_logs_path(i
+00015f80: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
+00015f90: 7429 202d 3e20 626f 6f6c 3a0a 2020 2020  t) -> bool:.    
+00015fa0: 2222 220a 2020 2020 5265 7475 726e 2074  """.    Return t
+00015fb0: 7275 6520 6966 2061 2062 6164 2070 6174  rue if a bad pat
+00015fc0: 6820 7761 7320 7365 7420 666f 7220 7468  h was set for th
+00015fd0: 6520 7273 7973 6c6f 6727 7320 6c6f 6720  e rsyslog's log 
+00015fe0: 766f 6c75 6d65 0a0a 2020 2020 446f 2061  volume..    Do a
+00015ff0: 2073 6d61 6c6c 2063 6865 636b 2066 6f72   small check for
+00016000: 2074 6865 2073 616b 6520 6f66 2068 656c   the sake of hel
+00016010: 7069 6e67 2074 6865 2075 7365 7220 616e  ping the user an
+00016020: 6420 6769 7669 6e67 2062 6574 7465 720a  d giving better.
+00016030: 2020 2020 7573 6572 2065 7870 6572 6965      user experie
+00016040: 6e63 653a 2063 6865 636b 2069 6620 7468  nce: check if th
+00016050: 6520 7273 7973 6c6f 6720 646f 636b 6572  e rsyslog docker
+00016060: 2028 7768 6963 6820 636f 6c6c 6563 7473   (which collects
+00016070: 206c 6f67 7329 0a20 2020 2069 7320 696e   logs).    is in
+00016080: 7369 6465 2074 6865 2074 6f70 6f6c 6f67  side the topolog
+00016090: 792c 2061 6e64 2069 6620 736f 2c20 6368  y, and if so, ch
+000160a0: 6563 6b20 7468 6520 2268 6f73 745f 7061  eck the "host_pa
+000160b0: 7468 2220 666f 7220 6c6f 6773 0a20 2020  th" for logs.   
+000160c0: 2028 6120 7370 6563 6966 6963 2070 6174   (a specific pat
+000160d0: 6820 6973 2065 7870 6563 7465 642c 2061  h is expected, a
+000160e0: 6e64 2069 7320 6861 7264 636f 6465 6420  nd is hardcoded 
+000160f0: 696e 2069 745f 7369 6d75 6c61 7469 6f6e  in it_simulation
+00016100: 290a 2020 2020 2222 220a 2020 2020 2320  ).    """.    # 
+00016110: 544f 444f 2843 5244 293a 2074 6869 7320  TODO(CRD): this 
+00016120: 6368 6563 6b20 7769 6c6c 2061 6c77 6179  check will alway
+00016130: 7320 6661 696c 2077 6865 6e20 6372 5f61  s fail when cr_a
+00016140: 7069 5f63 6c69 656e 742c 2074 6865 0a20  pi_client, the. 
+00016150: 2020 2023 2069 745f 7369 6d75 6c61 7469     # it_simulati
+00016160: 6f6e 2064 6f63 6b65 722c 2061 6e64 2074  on docker, and t
+00016170: 6865 2072 7379 736c 6f67 2064 6f63 6b65  he rsyslog docke
+00016180: 7220 6172 6520 6e6f 7420 6f6e 2074 6865  r are not on the
+00016190: 2073 616d 6520 6d61 6368 696e 650a 0a20   same machine.. 
+000161a0: 2020 2074 6f70 6f6c 6f67 7920 3d20 5941     topology = YA
+000161b0: 4d4c 2829 2e6c 6f61 6428 6665 7463 685f  ML().load(fetch_
+000161c0: 7369 6d75 6c61 7469 6f6e 5f74 6f70 6f6c  simulation_topol
+000161d0: 6f67 795f 7961 6d6c 2869 645f 7369 6d75  ogy_yaml(id_simu
+000161e0: 6c61 7469 6f6e 2929 0a0a 2020 2020 2320  lation))..    # 
+000161f0: 5468 6520 7061 7468 206f 6620 7468 6520  The path of the 
+00016200: 6c6f 6773 2c20 6f6e 2074 6865 2063 6f6d  logs, on the com
+00016210: 7075 7465 2073 6572 7665 7220 6669 6c65  pute server file
+00016220: 2073 7973 7465 6d20 7368 6f75 6c64 2041   system should A
+00016230: 4c57 4159 5320 6265 2061 7320 666f 6c6c  LWAYS be as foll
+00016240: 6f77 730a 2020 2020 7273 7973 6c6f 675f  ows.    rsyslog_
+00016250: 646f 636b 6572 5f70 7265 7365 6e74 3a20  docker_present: 
+00016260: 626f 6f6c 203d 2046 616c 7365 0a20 2020  bool = False.   
+00016270: 2070 6f74 656e 7469 616c 5f6c 6f67 735f   potential_logs_
+00016280: 6162 736f 6c75 7465 5f70 6174 683a 204c  absolute_path: L
+00016290: 6973 745b 5061 7468 5d20 3d20 5b5d 0a20  ist[Path] = []. 
+000162a0: 2020 2066 6f72 206e 6f64 6520 696e 2074     for node in t
+000162b0: 6f70 6f6c 6f67 795b 226e 6f64 6573 225d  opology["nodes"]
+000162c0: 3a0a 2020 2020 2020 2020 6966 2028 0a20  :.        if (. 
+000162d0: 2020 2020 2020 2020 2020 206e 6f64 655b             node[
+000162e0: 2274 7970 6522 5d20 3d3d 2022 646f 636b  "type"] == "dock
+000162f0: 6572 220a 2020 2020 2020 2020 2020 2020  er".            
+00016300: 616e 6420 2272 7379 736c 6f67 2220 696e  and "rsyslog" in
+00016310: 206e 6f64 655b 2262 6173 655f 696d 6167   node["base_imag
+00016320: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+00016330: 616e 6420 2276 6f6c 756d 6573 2220 696e  and "volumes" in
+00016340: 206e 6f64 650a 2020 2020 2020 2020 293a   node.        ):
+00016350: 0a20 2020 2020 2020 2020 2020 2072 7379  .            rsy
+00016360: 736c 6f67 5f64 6f63 6b65 725f 7072 6573  slog_docker_pres
+00016370: 656e 7420 3d20 5472 7565 0a20 2020 2020  ent = True.     
+00016380: 2020 2020 2020 2066 6f72 2076 6f6c 756d         for volum
+00016390: 6520 696e 206e 6f64 655b 2276 6f6c 756d  e in node["volum
+000163a0: 6573 225d 3a0a 2020 2020 2020 2020 2020  es"]:.          
+000163b0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+000163c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000163d0: 686f 7374 5f70 6174 6822 2069 6e20 766f  host_path" in vo
+000163e0: 6c75 6d65 0a20 2020 2020 2020 2020 2020  lume.           
+000163f0: 2020 2020 2020 2020 2061 6e64 2022 7772           and "wr
+00016400: 6974 6162 6c65 2220 696e 2076 6f6c 756d  itable" in volum
+00016410: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00016420: 2020 2020 2020 616e 6420 766f 6c75 6d65        and volume
+00016430: 5b22 7772 6974 6162 6c65 225d 0a20 2020  ["writable"].   
+00016440: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+00016450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016460: 2020 2020 706f 7465 6e74 6961 6c5f 6c6f      potential_lo
+00016470: 6773 5f61 6273 6f6c 7574 655f 7061 7468  gs_absolute_path
+00016480: 2e61 7070 656e 6428 5061 7468 2876 6f6c  .append(Path(vol
+00016490: 756d 655b 2268 6f73 745f 7061 7468 225d  ume["host_path"]
+000164a0: 2929 0a0a 2020 2020 2320 4966 206e 6f20  ))..    # If no 
+000164b0: 7273 7973 6c6f 6720 646f 636b 6572 2069  rsyslog docker i
+000164c0: 7320 7072 6573 656e 742c 206a 7375 7420  s present, jsut 
+000164d0: 6973 7375 6520 6120 6e6f 6e2d 626c 6f63  issue a non-bloc
+000164e0: 6b69 6e67 2077 6172 6e69 6e67 0a20 2020  king warning.   
+000164f0: 2069 6620 6e6f 7420 7273 7973 6c6f 675f   if not rsyslog_
+00016500: 646f 636b 6572 5f70 7265 7365 6e74 3a0a  docker_present:.
+00016510: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
+00016520: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
+00016530: 2020 2020 2220 205b 2b5d 2054 6865 2063      "  [+] The c
+00016540: 6f6c 6c65 6374 696f 6e20 6f66 206c 6f67  ollection of log
+00016550: 7320 7761 7320 6e6f 7420 6163 7469 7661  s was not activa
+00016560: 7465 6420 666f 7220 7468 6520 7369 6d75  ted for the simu
+00016570: 6c61 7469 6f6e 2028 7468 6520 7273 7973  lation (the rsys
+00016580: 6c6f 6720 646f 636b 6572 2069 7320 6e6f  log docker is no
+00016590: 7420 7072 6573 656e 7420 696e 2074 6865  t present in the
+000165a0: 2074 6f70 6f6c 6f67 7929 2e20 4e6f 206c   topology). No l
+000165b0: 6f67 2077 696c 6c20 6265 2069 6e63 6c75  og will be inclu
+000165c0: 6465 6420 696e 2074 6865 2064 6174 6173  ded in the datas
+000165d0: 6574 2e22 0a20 2020 2020 2020 2029 0a20  et.".        ). 
+000165e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000165f0: 2077 726f 6e67 5f68 6f73 745f 7061 7468   wrong_host_path
+00016600: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00016610: 666f 7220 7020 696e 2070 6f74 656e 7469  for p in potenti
+00016620: 616c 5f6c 6f67 735f 6162 736f 6c75 7465  al_logs_absolute
+00016630: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
+00016640: 2020 2069 6620 6e6f 7420 702e 6973 5f61     if not p.is_a
+00016650: 6273 6f6c 7574 6528 2920 616e 6420 7020  bsolute() and p 
+00016660: 3d3d 2050 6174 6828 2273 6861 7265 645f  == Path("shared_
+00016670: 7265 736f 7572 6365 732f 7273 7973 6c6f  resources/rsyslo
+00016680: 672f 6c6f 6773 2229 3a0a 2020 2020 2020  g/logs"):.      
+00016690: 2020 2020 2020 2020 2020 7772 6f6e 675f            wrong_
+000166a0: 686f 7374 5f70 6174 6820 3d20 4661 6c73  host_path = Fals
+000166b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000166c0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+000166d0: 2020 2020 656c 6966 2070 2e69 735f 6162      elif p.is_ab
+000166e0: 736f 6c75 7465 2829 2061 6e64 2050 6174  solute() and Pat
+000166f0: 6828 7374 7228 7029 5b31 3a5d 2920 3d3d  h(str(p)[1:]) ==
+00016700: 2050 6174 6828 0a20 2020 2020 2020 2020   Path(.         
+00016710: 2020 2020 2020 2022 7368 6172 6564 5f72         "shared_r
+00016720: 6573 6f75 7263 6573 2f72 7379 736c 6f67  esources/rsyslog
+00016730: 2f6c 6f67 7322 0a20 2020 2020 2020 2020  /logs".         
+00016740: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00016750: 2020 2020 2020 7772 6f6e 675f 686f 7374        wrong_host
+00016760: 5f70 6174 6820 3d20 4661 6c73 650a 2020  _path = False.  
+00016770: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00016780: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00016790: 656c 6966 2070 2e69 735f 6162 736f 6c75  elif p.is_absolu
+000167a0: 7465 2829 2061 6e64 2070 203d 3d20 5061  te() and p == Pa
+000167b0: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
+000167c0: 2020 2020 222f 6379 6265 722d 7261 6e67      "/cyber-rang
+000167d0: 652d 6361 7461 6c6f 672f 7369 6d75 6c61  e-catalog/simula
+000167e0: 7469 6f6e 735f 7265 736f 7572 6365 732f  tions_resources/
+000167f0: 312f 7368 6172 6564 5f72 6573 6f75 7263  1/shared_resourc
+00016800: 6573 2f72 7379 736c 6f67 2f6c 6f67 7322  es/rsyslog/logs"
+00016810: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
+00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016830: 7772 6f6e 675f 686f 7374 5f70 6174 6820  wrong_host_path 
+00016840: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00016850: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
+00016860: 2020 2020 2020 2069 6620 7772 6f6e 675f         if wrong_
+00016870: 686f 7374 5f70 6174 683a 0a20 2020 2020  host_path:.     
+00016880: 2020 2020 2020 206c 6f67 6765 722e 6572         logger.er
+00016890: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+000168a0: 2020 2020 2022 2020 5b2b 5d20 4974 2073       "  [+] It s
+000168b0: 6565 6d73 2074 6861 7420 7468 6520 7369  eems that the si
+000168c0: 6d75 6c61 7469 6f6e 2069 6e63 6c75 6465  mulation include
+000168d0: 7320 7468 6520 2772 7379 736c 6f67 2720  s the 'rsyslog' 
+000168e0: 646f 636b 6572 2074 6861 7420 636f 6c6c  docker that coll
+000168f0: 6563 7473 2074 6865 206c 6f67 732c 2062  ects the logs, b
+00016900: 7574 2064 6f65 7320 6e6f 7420 7370 6563  ut does not spec
+00016910: 6966 7920 7468 6520 6170 7072 6f70 7269  ify the appropri
+00016920: 6174 6520 686f 7374 5f70 6174 6820 666f  ate host_path fo
+00016930: 7220 7468 6520 6c6f 6773 2e20 4974 2069  r the logs. It i
+00016940: 7320 6578 7065 6374 6564 2074 6861 7420  s expected that 
+00016950: 7468 6520 7273 7973 6c6f 6720 646f 636b  the rsyslog dock
+00016960: 6572 206e 6f64 6520 7370 6563 6966 6965  er node specifie
+00016970: 7320 6120 2877 7269 7461 626c 6529 2076  s a (writable) v
+00016980: 6f6c 756d 6520 7769 7468 2061 2068 6f73  olume with a hos
+00016990: 745f 7061 7468 2065 7175 616c 2074 6f20  t_path equal to 
+000169a0: 272f 7368 6172 6564 5f72 6573 6f75 7263  '/shared_resourc
+000169b0: 6573 2f72 7379 736c 6f67 2f6c 6f67 7327  es/rsyslog/logs'
+000169c0: 2e20 4361 6e64 6964 6174 6573 2061 7265  . Candidates are
+000169d0: 2027 7b7d 2720 696e 7374 6561 642e 222e   '{}' instead.".
+000169e0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+000169f0: 2020 2020 2020 2020 2020 2020 5b73 7472              [str
+00016a00: 2870 2920 666f 7220 7020 696e 2070 6f74  (p) for p in pot
+00016a10: 656e 7469 616c 5f6c 6f67 735f 6162 736f  ential_logs_abso
+00016a20: 6c75 7465 5f70 6174 685d 2c0a 2020 2020  lute_path],.    
+00016a30: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00016a40: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00016a50: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
+00016a60: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00016a70: 2020 2020 2020 2220 5b2b 5d20 4461 7461        " [+] Data
+00016a80: 7365 7420 6372 6561 7469 6f6e 2061 626f  set creation abo
+00016a90: 7274 6564 2e20 596f 7520 6d61 7920 7769  rted. You may wi
+00016aa0: 7368 2074 6f20 6d6f 7665 2074 6865 206c  sh to move the l
+00016ab0: 6f67 2066 696c 6573 2074 6f20 7468 6520  og files to the 
+00016ac0: 6170 7072 6f70 7269 6174 6520 666f 6c64  appropriate fold
+00016ad0: 6572 206f 6e20 7468 6520 636f 6d70 7574  er on the comput
+00016ae0: 6520 7365 7276 6572 2873 292c 2061 6e64  e server(s), and
+00016af0: 2074 6865 6e20 7265 7472 792e 2041 6c74   then retry. Alt
+00016b00: 6572 6e61 7469 7665 6c79 2c20 796f 7520  ernatively, you 
+00016b10: 6361 6e20 6279 7061 7373 2074 6869 7320  can bypass this 
+00016b20: 6368 6563 6b20 7769 7468 2074 6865 2064  check with the d
+00016b30: 6f6e 745f 6368 6563 6b5f 6c6f 675f 7061  ont_check_log_pa
+00016b40: 7468 206f 7074 696f 6e2e 220a 2020 2020  th option.".    
+00016b50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00016b60: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00016b70: 650a 0a0a 6465 6620 7374 6f70 5f64 6174  e...def stop_dat
+00016b80: 6173 6574 5f63 7265 6174 696f 6e28 6461  aset_creation(da
+00016b90: 7461 7365 745f 6964 3a20 7575 6964 2e55  taset_id: uuid.U
+00016ba0: 5549 4429 202d 3e20 416e 793a 0a20 2020  UID) -> Any:.   
+00016bb0: 2022 2222 0a20 2020 2053 746f 7073 2f61   """.    Stops/a
+00016bc0: 626f 7274 7320 7468 6520 6372 6561 7469  borts the creati
+00016bd0: 6f6e 206f 6620 6120 6461 7461 7365 7420  on of a dataset 
+00016be0: 7468 6174 2069 7320 696e 2074 6865 2070  that is in the p
+00016bf0: 726f 6365 7373 206f 6620 6265 696e 6720  rocess of being 
+00016c00: 6372 6561 7465 642e 0a0a 2020 2020 5468  created...    Th
+00016c10: 6973 2066 756e 6374 696f 6e20 7368 6f75  is function shou
+00016c20: 6c64 2062 6520 7573 6564 2c20 666f 7220  ld be used, for 
+00016c30: 696e 7374 616e 6365 2c20 6966 2061 2064  instance, if a d
+00016c40: 6174 6173 6574 2063 7265 6174 696f 6e20  ataset creation 
+00016c50: 6861 7320 6265 656e 0a20 2020 2061 7574  has been.    aut
+00016c60: 6f6d 6174 6963 616c 6c79 2073 7461 7274  omatically start
+00016c70: 6564 2061 6c74 686f 7567 6820 7468 6520  ed although the 
+00016c80: 7573 6572 2064 6f65 7320 6e6f 7420 7761  user does not wa
+00016c90: 6e74 2061 2064 6174 6173 6574 2c20 616e  nt a dataset, an
+00016ca0: 6420 7468 6520 6461 7461 7365 740a 2020  d the dataset.  
+00016cb0: 2020 6372 6561 7469 6f6e 2070 726f 6365    creation proce
+00016cc0: 7373 2069 7320 7461 6b69 6e67 2074 6f6f  ss is taking too
+00016cd0: 206d 7563 6820 7469 6d65 2e0a 0a20 2020   much time...   
+00016ce0: 2057 4152 4e49 4e47 3a20 6166 7465 7220   WARNING: after 
+00016cf0: 7374 6f70 7069 6e67 2074 6865 2064 6174  stopping the dat
+00016d00: 6173 6574 2063 7265 6174 696f 6e2c 2069  aset creation, i
+00016d10: 7420 6973 2061 6476 6973 6564 2074 6f20  t is advised to 
+00016d20: 6465 6c65 7465 206f 7220 6174 206c 6561  delete or at lea
+00016d30: 7374 0a20 2020 2072 6570 6169 7220 7468  st.    repair th
+00016d40: 6520 6461 7461 7365 742e 0a0a 2020 2020  e dataset...    
+00016d50: 3a70 6172 616d 2064 6174 6173 6574 5f69  :param dataset_i
+00016d60: 643a 2074 6865 2064 6174 6173 6574 2077  d: the dataset w
+00016d70: 6869 6368 2069 7320 696e 2074 6865 2070  hich is in the p
+00016d80: 726f 6365 7373 206f 6620 6265 696e 6720  rocess of being 
+00016d90: 6372 6561 7465 6420 616e 6420 7468 6174  created and that
+00016da0: 206d 7573 7420 6265 2061 626f 7274 6564   must be aborted
+00016db0: 0a20 2020 203a 7265 7475 726e 3a20 7265  .    :return: re
+00016dc0: 7475 726e 2074 6865 206a 736f 6e20 626f  turn the json bo
+00016dd0: 6479 206f 6620 7468 6520 636f 7265 2041  dy of the core A
+00016de0: 5049 2072 6573 706f 6e73 650a 2020 2020  PI response.    
+00016df0: 2222 220a 2020 2020 2320 5369 6d70 6c79  """.    # Simply
+00016e00: 2063 616c 6c73 2074 6865 2063 6f72 6520   calls the core 
+00016e10: 4150 4920 7768 6963 6820 6974 7365 6c66  API which itself
+00016e20: 2061 736b 7320 7468 6520 7075 626c 6973   asks the publis
+00016e30: 680a 2020 2020 2320 7365 7276 6572 2028  h.    # server (
+00016e40: 6261 636b 656e 6429 2074 6f20 7374 6f70  backend) to stop
+00016e50: 206f 6620 7468 6520 6461 7461 7365 7420   of the dataset 
+00016e60: 6372 6561 7469 6f6e 2070 726f 6365 7373  creation process
+00016e70: 2e0a 0a20 2020 2072 6573 756c 7420 3d20  ...    result = 
+00016e80: 5f70 7574 2822 2f63 7265 6174 655f 6461  _put("/create_da
+00016e90: 7461 7365 742f 7374 6f70 2f7b 7d22 2e66  taset/stop/{}".f
+00016ea0: 6f72 6d61 7428 7374 7228 6461 7461 7365  ormat(str(datase
+00016eb0: 745f 6964 2929 290a 0a20 2020 2069 6620  t_id)))..    if 
+00016ec0: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
+00016ed0: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
+00016ee0: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+00016ef0: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
+00016f00: 2073 746f 7020 6461 7461 7365 7420 6372   stop dataset cr
+00016f10: 6561 7469 6f6e 2074 6872 6f75 6768 2063  eation through c
+00016f20: 6f72 6520 4150 4922 290a 0a20 2020 2072  ore API")..    r
+00016f30: 6574 7572 6e20 7265 7375 6c74 2e6a 736f  eturn result.jso
+00016f40: 6e28 290a 0a0a 6465 6620 6665 7463 685f  n()...def fetch_
+00016f50: 636f 6d70 7574 655f 7365 7276 6572 2863  compute_server(c
+00016f60: 6f6d 7075 7465 5f73 6572 7665 725f 6964  ompute_server_id
+00016f70: 3a20 696e 7429 202d 3e20 416e 793a 0a20  : int) -> Any:. 
+00016f80: 2020 2022 2222 5265 7475 726e 2061 2063     """Return a c
+00016f90: 6f6d 7075 7465 2073 6572 7665 7220 6769  ompute server gi
+00016fa0: 7665 6e20 6974 7320 4944 2222 220a 2020  ven its ID""".  
+00016fb0: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
+00016fc0: 6622 2f63 6f6d 7075 7465 5f73 6572 7665  f"/compute_serve
+00016fd0: 7273 2f7b 636f 6d70 7574 655f 7365 7276  rs/{compute_serv
+00016fe0: 6572 5f69 647d 2229 0a0a 2020 2020 6966  er_id}")..    if
+00016ff0: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
+00017000: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
+00017010: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
+00017020: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
+00017030: 7420 7265 7472 6965 7665 206e 6f64 6520  t retrieve node 
+00017040: 6672 6f6d 2049 5420 5369 6d75 6c61 7469  from IT Simulati
+00017050: 6f6e 2041 5049 2229 0a0a 2020 2020 7265  on API")..    re
+00017060: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
+00017070: 2829 0a0a 0a64 6566 2066 6574 6368 5f63  ()...def fetch_c
+00017080: 6f6d 7075 7465 5f73 6572 7665 725f 6279  ompute_server_by
+00017090: 5f6e 6f64 655f 6964 286e 6f64 655f 6964  _node_id(node_id
+000170a0: 3a20 696e 7429 202d 3e20 416e 793a 0a20  : int) -> Any:. 
+000170b0: 2020 2022 2222 5265 7475 726e 2061 2063     """Return a c
+000170c0: 6f6d 7075 7465 2073 6572 7665 7220 7768  ompute server wh
+000170d0: 6572 6520 6120 6e6f 6465 2049 4420 6973  ere a node ID is
+000170e0: 2072 756e 6e69 6e67 2222 220a 2020 2020   running""".    
+000170f0: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
+00017100: 2f63 6f6d 7075 7465 5f73 6572 7665 7273  /compute_servers
+00017110: 2f6e 6f64 652f 7b6e 6f64 655f 6964 7d22  /node/{node_id}"
+00017120: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
+00017130: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
+00017140: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
+00017150: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
+00017160: 742c 2022 4361 6e6e 6f74 2072 6574 7269  t, "Cannot retri
+00017170: 6576 6520 6e6f 6465 2066 726f 6d20 4954  eve node from IT
+00017180: 2053 696d 756c 6174 696f 6e20 4150 4922   Simulation API"
+00017190: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
+000171a0: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
+000171b0: 6620 6665 7463 685f 636f 6d70 7574 655f  f fetch_compute_
+000171c0: 7365 7276 6572 7328 2920 2d3e 204c 6973  servers() -> Lis
+000171d0: 745b 4469 6374 5b73 7472 2c20 416e 795d  t[Dict[str, Any]
+000171e0: 5d3a 0a20 2020 2022 2222 0a20 2020 2052  ]:.    """.    R
+000171f0: 6574 7572 6e20 7468 6520 6c69 7374 206f  eturn the list o
+00017200: 6620 636f 6d70 7574 6520 7365 7276 6572  f compute server
+00017210: 7320 6173 206b 6e6f 776e 2069 6e20 6461  s as known in da
+00017220: 7461 6261 7365 0a20 2020 2022 2222 0a20  tabase.    """. 
+00017230: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
+00017240: 2822 2f63 6f6d 7075 7465 5f73 6572 7665  ("/compute_serve
+00017250: 7273 2f22 290a 0a20 2020 2069 6620 7265  rs/")..    if re
+00017260: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+00017270: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+00017280: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+00017290: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+000172a0: 6574 7269 6576 6520 636f 6d70 7574 6520  etrieve compute 
+000172b0: 7365 7276 6572 7320 6672 6f6d 2049 5420  servers from IT 
+000172c0: 5369 6d75 6c61 7469 6f6e 2041 5049 2229  Simulation API")
+000172d0: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+000172e0: 756c 742e 6a73 6f6e 2829 0a0a 0a64 6566  ult.json()...def
+000172f0: 2064 656c 6574 655f 636f 6d70 7574 655f   delete_compute_
+00017300: 7365 7276 6572 2863 6f6d 7075 7465 5f73  server(compute_s
+00017310: 6572 7665 725f 6964 3a20 696e 7429 202d  erver_id: int) -
+00017320: 3e20 4e6f 6e65 3a0a 2020 2020 2222 220a  > None:.    """.
+00017330: 2020 2020 4465 6c65 7465 7320 6120 636f      Deletes a co
+00017340: 6d70 7574 6520 7365 7276 6572 2069 6e20  mpute server in 
+00017350: 6461 7461 6261 7365 2075 7369 6e67 2069  database using i
+00017360: 7473 2069 640a 0a20 2020 2043 6f6d 7075  ts id..    Compu
+00017370: 7465 2073 6572 7665 7273 2069 6473 2063  te servers ids c
+00017380: 616e 2062 6520 6f62 7461 696e 6564 2074  an be obtained t
+00017390: 6872 6f75 6768 2060 6379 6265 725f 7261  hrough `cyber_ra
+000173a0: 6e67 6520 7374 6174 7573 60c2 a06f 7220  nge status`..or 
+000173b0: 3a66 756e 633a 6066 6574 6368 5f63 6f6d  :func:`fetch_com
+000173c0: 7075 7465 5f73 6572 7665 7260 2e0a 2020  pute_server`..  
+000173d0: 2020 2222 220a 2020 2020 7265 7375 6c74    """.    result
+000173e0: 203d 205f 6465 6c65 7465 2866 222f 636f   = _delete(f"/co
+000173f0: 6d70 7574 655f 7365 7276 6572 732f 7b63  mpute_servers/{c
+00017400: 6f6d 7075 7465 5f73 6572 7665 725f 6964  ompute_server_id
+00017410: 7d22 290a 0a20 2020 2069 6620 7265 7375  }")..    if resu
+00017420: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
+00017430: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
+00017440: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
+00017450: 756c 742c 2022 4361 6e6e 6f74 2064 656c  ult, "Cannot del
+00017460: 6574 6520 636f 6d70 7574 6520 7365 7276  ete compute serv
+00017470: 6572 2069 6e20 636f 7265 2041 5049 2229  er in core API")
+00017480: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+00017490: 756c 742e 6a73 6f6e 2829 0a              ult.json().
```

### Comparing `cr_api_client-3.1.0/cr_api_client/cyber_range.py` & `cr_api_client-4.0.0/cr_api_client/cyber_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,17 @@
 class Version:
     def __init__(self, str_vers: str) -> None:
         try:
             self.major, self.minor, self.patch = str_vers.split(".")
         except Exception as e:
             raise Exception(
                 "Bad version format for '{}': 'X.Y.Z' expected. Error: {}".format(
-                    str_vers, e))
+                    str_vers, e
+                )
+            )
 
 
 #
 # 'status' related functions
 #
 def status_handler(args: Any) -> None:  # noqa: C901
     """Get platform status."""
@@ -261,39 +263,29 @@
                     compute_server["api_status"] = colored("NOK", "white", "on_red")
             else:
                 compute_server["api"] = "deactivated"
                 compute_server["api_status"] = colored("NA", "white", "on_grey")
 
             # Libvirt is special: it is always installed and must be responding, even
             # if it is not used activly to run VMs on the compute server
-            if compute_server["libvirt_transport_mode"] == "tcp":
-                compute_server["libvirt"] = "on tcp:" + str(
-                    compute_server["libvirt_port"]
-                )
-            else:
-                compute_server["libvirt"] = (
-                    "on " + compute_server["libvirt_transport_mode"]
-                )
+            compute_server["libvirt"] = "on tcp: {}".format(
+                compute_server["libvirt_port"]
+            )
             if compute_server["libvirt_ping"] is True:
                 compute_server["libvirt_status"] = colored("OK", "grey", "on_green")
             else:
                 compute_server["libvirt_status"] = colored("NOK", "white", "on_red")
 
             if not compute_server["libvirt_activate"]:
                 compute_server["libvirt_status"] += " (deactivated)"
 
             if compute_server["docker_activate"]:
-                if compute_server["docker_transport_mode"] == "tcp":
-                    compute_server["docker"] = "on tcp:" + str(
-                        compute_server["docker_port"]
-                    )
-                else:
-                    compute_server["docker"] = (
-                        "on " + compute_server["docker_transport_mode"]
-                    )
+                compute_server["docker"] = "on tcp: {}".format(
+                    compute_server["docker_port"]
+                )
                 if compute_server["docker_ping"] is True:
                     compute_server["docker_status"] = colored("OK", "grey", "on_green")
                 else:
                     compute_server["docker_status"] = colored("NOK", "white", "on_red")
             else:
                 compute_server["docker"] = "deactivated"
                 compute_server["docker_status"] = colored("NA", "white", "on_grey")
@@ -465,31 +457,29 @@
     # Trick to order the system_type set
     system_type_list = sorted(list(system_type_list))
 
     # Display baseboxes ordered by system_type and operating_system
     for current_system_type in system_type_list:
         logger.info("  [+] " + colored(f"{current_system_type}", attrs=["bold"]))
 
-        for (system_type, operating_system_list) in operating_system_dict.items():
+        for system_type, operating_system_list in operating_system_dict.items():
             if current_system_type == system_type:
-
                 # Trick to order the operating_system_list set
                 operating_system_list = sorted(list(operating_system_list))
 
                 for operating_system in operating_system_list:
                     logger.info(
                         "    [+] " + colored(f"{operating_system}", attrs=["bold"])
                     )
 
                     for basebox in baseboxes:
                         if (
                             basebox["system_type"] == current_system_type
                             and basebox["operating_system"] == operating_system
                         ):
-
                             # Check if basebox is in local catalog
                             logger.info(
                                 "      [+] '{}': {} (role: {}, language: {})".format(
                                     basebox["id"],
                                     basebox["description"],
                                     basebox["role"],
                                     basebox["language"],
@@ -1054,14 +1044,15 @@
             for node in nodes:
                 logger.info(
                     "    [+] ID: {}, name: {}, type: {}".format(
                         node["id"], node["name"], node["type"]
                     )
                 )
                 logger.info("      [+] status: {}".format(node["status"]))
+                logger.info("      [+] start: {}".format(node["node_start_time"]))
 
                 if node["active"] is False:
                     logger.info("      [+] active: {}".format(node["active"]))
                     continue
 
                 if node["type"] == "virtual_machine":
                     logger.info(
@@ -1223,15 +1214,14 @@
         cs_used_resources[k]["cpu"] += node["nb_proc"]
         cs_used_resources[k]["mem"] += node["memory_size"]
 
     for cs in compute_servers:
         cs_id_to_cs[cs["id"]] = cs
 
     for cs_id, cs_nodes in cs_to_nodes.items():
-
         if cs_id is None:
             logger.info("[+] Not allocated")
         else:
             logger.info(
                 "[+] On compute server {name} (IP {ip_address})".format(
                     **(cs_id_to_cs[cs_id])
                 )
@@ -1974,20 +1964,20 @@
             logger.info("    [+] IP address: {ip_address}".format(**compute_server))
             logger.info(
                 "    [+] API is active ? {api_activate}. On port {api_port}".format(
                     **compute_server
                 )
             )
             logger.info(
-                "    [+] Libvirt is active ? {libvirt_activate}. With transport '{libvirt_transport_mode}', and (tcp) port {libvirt_port}".format(
+                "    [+] Libvirt is active ? {libvirt_activate}. With (tcp) port {libvirt_port}".format(
                     **compute_server
                 )
             )
             logger.info(
-                "    [+] Docker is active ? {docker_activate}. With transport '{docker_transport_mode}', and (tcp) port {docker_port}".format(
+                "    [+] Docker is active ? {docker_activate}. With (tcp) port {docker_port}".format(
                     **compute_server
                 )
             )
             logger.info(
                 "    [+] is_down {is_down}, last_heartbeat={last_heartbeat_timestamp}".format(
                     **compute_server
                 )
@@ -2135,15 +2125,14 @@
 
     knowledge = redteam_api.attack_knowledge()
 
     filter_count = 0
 
     # Show available attacks by attack sessions
     for session in attack_sessions:
-
         # Try to find IP of compromised host on which the attack session is active
         compromised_host_ip = None
         if "hosts" in knowledge:
             for host in knowledge["hosts"]:
                 for nic in host:
                     if (
                         nic is not None
@@ -2177,16 +2166,23 @@
             if filter_status is not None:
                 select = False
                 if filter_status.lower() == attack["status"].lower():
                     select = True
                     filter_count += 1
 
             if select:
+
+                # Retrieve attacks values, after removing redondant attack session infos
+                attack_values = dict_values.copy()
+                attack_values.pop("attack_session_type", None)
+                attack_values.pop("attack_session_source", None)
+                attack_values.pop("attack_session_id", None)
+
                 logger.info(
-                    f"    [+] {attack['idAttack']} - {attack['worker']['mitre_data']['technique']['id']} - {attack['worker']['mitre_data']['technique']['name']} - {attack['worker']['id']} - {attack['worker']['name']} - {attack['status']}"
+                    f"    [+] {attack['idAttack']} - {attack['worker']['id']} - {attack['worker']['mitre_data']['technique']['name']} - {attack['worker']['name']} - {attack['status']} - values:{attack_values}"
                 )
 
     # Show available attacks not tied to an attack session
     logger.info("  [+] direct attacks (no attack session)")
     for attack in attacks:
         # Find attacks with no attack session
         in_attack_session = True
@@ -2196,16 +2192,20 @@
         if not isinstance(dict_values, dict):
             in_attack_session = False
         else:
             if "attack_session_id" not in dict_values:
                 in_attack_session = False
 
         if in_attack_session is False:
+
+            # Retrieve attacks values, after removing redondant attack session infos
+            attack_values = dict_values.copy()
+
             logger.info(
-                f"    [+] {attack['idAttack']} - {attack['worker']['mitre_data']['technique']['id']} - {attack['worker']['mitre_data']['technique']['name']} - {attack['worker']['id']} - {attack['worker']['name']} - {attack['status']}"
+                f"    [+] {attack['idAttack']} - {attack['worker']['id']} - {attack['worker']['mitre_data']['technique']['name']} - {attack['worker']['name']} - {attack['status']} - values:{attack_values}"
             )
 
     logger.info("====")
     logger.info(f"  [+] Number of available attacks: {len(attacks)}")
 
     if filter_status is not None:
         logger.info(f"  [+] Number of filtered attacks: {filter_count}")
@@ -2232,15 +2232,15 @@
 #
 def redteam_knowledge_handler(args: Any) -> None:
     """Get the attack knowledge (attack hosts and sessions)."""
 
     logger.info("[+] Attack knowledge")
     knowledge = redteam_api.attack_knowledge()
 
-    pp = pprint.PrettyPrinter(depth=4, compact=True, width=160)
+    pp = pprint.PrettyPrinter(compact=True, width=160)
     pp.pprint(knowledge)
 
 
 #
 # 'redteam_sessions' related functions
 #
 def redteam_sessions_handler(args: Any) -> None:
@@ -2290,15 +2290,15 @@
     debug = args.debug_mode
 
     logger.info(f"[+] Play attack ID {id_attack}")
 
     # Retrieve attack name
     # TODO: attack_name seems to be useless in this API. Only the id_attack is necessary.
     redteam_api.execute_attack(
-        id_attack, "j'attends le patch TLS", waiting_worker=wait, debug=debug
+        id_attack, "ATTACK_NAME", waiting_worker=wait, debug=debug
     )
 
     logger.info("[+] Attack executed")
 
 
 #
 # 'redteam_reset' related functions
@@ -2317,15 +2317,15 @@
     """Get logs from redteam workers."""
 
     logger.info("[+] Logs from redteam workers")
     redteam_logs = redteam_api.logs()
 
     attacks = redteam_api.list_attacks()
 
-    for (id_source_log, logs) in redteam_logs.items():
+    for id_source_log, logs in redteam_logs.items():
         print("")  # Empty print to enhance visibility of log separation
 
         for attack in attacks:
             if str(attack["idAttack"]) == str(id_source_log):
                 logger.warning(
                     f"  [+] Source log: {id_source_log} - attack: {attack['worker']['id']}"
                 )
@@ -2344,15 +2344,15 @@
 #
 def redteam_report_handler(args: Any) -> None:
     """Get the redteam report."""
 
     logger.info("[+] Report from redteam API")
     report = redteam_api.scenario_result()
 
-    pp = pprint.PrettyPrinter(depth=4, width=160)
+    pp = pprint.PrettyPrinter(width=160)
     pp.pprint(report)
 
 
 def main() -> None:
     parser = argparse.ArgumentParser()
 
     # Config file argument
```

### Comparing `cr_api_client-3.1.0/cr_api_client/provisioning_api.py` & `cr_api_client-4.0.0/cr_api_client/provisioning_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
     machines_file: Optional[str] = None,
     playbook_path: Optional[str] = None,
     target_roles: Optional[List[str]] = None,
     target_system_types: Optional[List[str]] = None,
     target_operating_systems: Optional[List[str]] = None,
     target_names: Optional[List[str]] = None,
     host_vars: Optional[List[str]] = None,
-    extra_vars: Optional[str] = None,
+    extra_vars: Optional[Any] = None,
     gather_facts: Optional[bool] = None,
     debug: bool = False,
     wait: bool = True,
     timeout: int = 3600,
 ) -> Tuple[bool, Optional[str]]:
     """Apply ansible playbooks on specified target(s). The ``wait`` parameter defines if
     the function wait for task to complete or not.
@@ -261,14 +261,16 @@
         target_system_types = []
     if target_operating_systems is None:
         target_operating_systems = []
     if target_names is None:
         target_names = []
     if host_vars is None:
         host_vars = []
+    extra_vars_str = str(extra_vars)
+    extra_vars_str = extra_vars_str.replace("\\\\", "\\")
 
     if playbook_path is None:
         raise Exception("provisioning_file parameter cannot be None")
 
     if (id_simulation is None and machines_file is None) or (
         id_simulation is not None and machines_file is not None
     ):
@@ -330,15 +332,15 @@
     ):
         logger.warning("Target lists are empty. No provisioning will be done.")
         return (False, None)
 
     data = {
         "id_simulation": id_simulation,
         "machines_yaml": machines_yaml,
-        "extra_vars": extra_vars,
+        "extra_vars": extra_vars_str,
         "target_roles": target_roles,
         "target_system_types": target_system_types,
         "target_operating_systems": target_operating_systems,
         "target_names": target_names,
         "host_vars": host_vars,
         "gather_facts": gather_facts,
         "debug": debug,
```

### Comparing `cr_api_client-3.1.0/cr_api_client/publish_api.py` & `cr_api_client-4.0.0/cr_api_client/publish_api.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/redteam_api.py` & `cr_api_client-4.0.0/cr_api_client/redteam_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 import json
 import os
 import pprint
 import time
+from typing import Any
+from typing import Callable
 from typing import Dict
 from typing import List
-from typing import Optional, Callable, Any
+from typing import Optional
 from typing import Tuple
 
 import requests
 from colorama import Fore
 from loguru import logger
 
 from cr_api_client.config import cr_api_client_config
@@ -111,29 +113,30 @@
 
 def reset_redteam() -> None:
     """Reset redteam platform (init knowledge_database and delete all workers).
 
     :return: None
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
 
     """
     result = _delete("/platform")
     result.raise_for_status()
 
 
 def logs() -> Dict:
     """Get redteam API logs.
 
     :return: str
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.logs()
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.logs()  # doctest: +SKIP
+    {}
 
     """
     url = "/logs"
 
     result = _get(url, headers={}, data={})
 
     if result.status_code != 200:
@@ -145,17 +148,17 @@
 def list_tactics() -> List[dict]:
     """List all available tactics (based on MITRE ATT&CK).
 
     :return: Available tactics in JSON format.
     :rtype: :class:`List`
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.list_tactics()
-    []
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.list_tactics()  # doctest: +SKIP
+    [{'id': 'TA0001', 'name': 'Initial Access'}, {'id': 'TA0002', 'name': 'Execution'}, {'id': 'TA0003', 'name': 'Persistence'}, {'id': 'TA0004', 'name': 'Privilege Escalation'}, {'id': 'TA0005', 'name': 'Defense Evasion'}, {'id': 'TA0006', 'name': 'Credential Access'}, {'id': 'TA0007', 'name': 'Discovery'}, {'id': 'TA0008', 'name': 'Lateral Movement'}, {'id': 'TA0009', 'name': 'Collection'}, {'id': 'TA0010', 'name': 'Exfiltration'}, {'id': 'TA0011', 'name': 'Command and Control'}, {'id': 'TA0040', 'name': 'Impact'}, {'id': 'TA0042', 'name': 'Resource Development'}, {'id': 'TA0043', 'name': 'Reconnaissance'}]
 
     """
     url = "/tactic"
 
     result = _get(url, headers={}, data={})
 
     if result.status_code != 200:
@@ -167,17 +170,17 @@
 def list_workers() -> List[dict]:
     """List all available workers.
 
     :return: Available workers in JSON format.
     :rtype: :class:`List`
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.list_workers()
-    []
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.list_workers()  # doctest: +SKIP
+    [{...}]
 
     """
     url = "/worker"
 
     result = _get(url, headers={}, data={})
 
     if result.status_code != 200:
@@ -189,17 +192,17 @@
 def worker_infos(id_worker: str) -> dict:
     """Retrieve worker info from its ID.
 
     :return: Worker info in JSON format.
     :rtype: :class:`List`
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.worker_info()
-    []
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.worker_infos("1021_006_002")  # doctest: +SKIP
+    {'id': '1021_006_002', 'name': 'winrm_session', ...}
 
     """
     url = f"/worker/{id_worker}"
 
     result = _get(url, headers={}, data={})
 
     if result.status_code != 200:
@@ -214,16 +217,16 @@
     :param status: The status (success, failed, error, running, runnable) to filter.
     :type status: :class:`str`
 
     :return: List all attacks in JSON format.
     :rtype: :class:`List`
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.list_attacks(status="success")
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.list_attacks(status="success")  # doctest: +SKIP
     []
 
     """
     url = "/attack"
 
     if status:
         url = url + "?status=" + status
@@ -241,16 +244,16 @@
     :param id_attack: The attack identifier.
     :type id_attack: :class:`int`
 
     :return: Status of attack and output data.
     :rtype: :class:`str`, :class:`Dict`
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.attack_infos(id_attack=1)
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.attack_infos(id_attack=1)  # doctest: +SKIP
     ('runnable', None)
 
     """
     url = "/attack/" + str(id_attack)
 
     result = _get(url, headers={}, data={})
     if result.status_code != 200:
@@ -323,15 +326,15 @@
     debug_env = os.getenv("CR_DEBUG", "0")
 
     # Debug value can either be set from var env or from function parameter
     if debug or debug_env == "1":
         # Show attack report
         scenario_report = scenario_result()
 
-        pp = pprint.PrettyPrinter(depth=4, width=160)
+        pp = pprint.PrettyPrinter(width=160)
 
         if len(scenario_report) > 0:
             logger.info("[+] Attack report")
 
             for attack_report in scenario_report:
                 if str(attack_report["id"]) == str(id_attack):
                     pp.pprint(attack_report)
@@ -361,15 +364,15 @@
     :param waiting_worker: Wait attack status become "success" or "failed".
     :type waiting_worker: :class:`bool`, optional
 
     :return: The ID of attack.
     :rtype: :class:`str`
 
     """
-    url = "/attack/" + str(id_attack) + "?action=start"
+    url = "/attack/" + str(id_attack) + "/play"
     payload = {}
     headers = {}
     result = _get(url, headers=headers, data=payload)
 
     if result.status_code != 200:
         _handle_error(result, "Cannot start attack from redteam API")
 
@@ -416,14 +419,15 @@
 
 def execute_attack_name_by_values(
     attack_name: str,
     retries: int = 3,
     attack_session_identifier: Optional[str] = None,
     attack_values_dict: Optional[Dict[str, Any]] = None,
     attack_values_callback: Optional[Callable[[Dict[str, Any]], bool]] = None,
+    waiting_worker: bool = True,
 ) -> Optional[str]:
     attack = None
     for _ in range(retries):
         attack = get_attack_by_values(
             attack_name,
             attack_session_identifier=attack_session_identifier,
             attack_values_dict=attack_values_dict,
@@ -439,50 +443,51 @@
 
         if attack_session_identifier:
             message += f", for attack session id {attack_session_identifier}."
 
         if attack_values_dict and not attack_values_callback:
             message += f", for attack values {attack_values_dict}."
         elif not attack_values_dict and attack_values_callback:
-            message += (
-                ", for attack values selected by a callback."
-            )
+            message += ", for attack values selected by a callback."
         elif attack_values_dict and attack_values_callback:
             message += f", for attack values {attack_values_dict} and further selected by a callback."
 
         raise Exception(message)
 
-    return execute_attack(attack["idAttack"], attack["worker"]["name"])
+    return execute_attack(
+        attack["idAttack"], attack["worker"]["name"], waiting_worker=waiting_worker
+    )
 
 
 def get_attack_by_values(
     attack_name: str,
     attack_session_identifier: Optional[str] = None,
     attack_values_dict: Optional[Dict[str, Any]] = None,
     attack_values_callback: Optional[Callable[[Dict[str, Any]], bool]] = None,
 ) -> Dict[str, Any]:
     """
     Helper function to find an attack for a specific attack session or for specific attack values
 
     Allows to search for an available an attack based on its name, and several optional criteria.
-    The selection can be done based one: 
-    
-    * the ID of the attack session to use 
+    The selection can be done based one:
+
+    * the ID of the attack session to use
     * specific, exact keys/values in the attack values
     * a custom callback, for more complex selection
 
     The three selection methods can be combined. If two or all three parameters are used
     (`attack_session_identifier`, `attack_values_dict`, `attack_values_callback`), an attack is
     searched that matches all three parameters.
 
-    Example: 
+    Example:
+    >>> from cr_api_client import redteam_api
     >>> attack_session_id = "d5f7a6a3-54c7-4666-9e9d-31cbc404c21b"
     >>> attack_values_dict = {"target_ip": "1.2.3.4", "param1": 42}
-    >>> attack_values_callback = lambda values: "param2" in values and "substring" values["param2]
-    >>> redteam_api.attack_by_session("my_worker_name", attack_session_id, attack_values_dict, attack_values_callback)
+    >>> attack_values_callback = lambda values: "param2" in values and "substring" in values["param2"]
+    >>> redteam_api.get_attack_by_values("my_worker_name", attack_session_id, attack_values_dict, attack_values_callback)  # doctest: +SKIP
     {'idAttack': 23, 'worker': {'id': '1487_000_001', 'name': 'my_worker_name', 'description':
     'XXX', 'cve': [],'stability': 'CRASH_SAFE', 'reliability': 'UNIQUE', 'side_effect':
     'NETWORK_CONNECTION', 'killchain_step': 'EXECUTION', 'repeatable': False, 'mitre_data':
     {'technique': {'id': 'T1487', 'name': 'Techname'}, 'subtechnique': {}, 'tactics': [{'id':
     'TA0002', 'name': 'Execution'}]}}, 'status': 'runnable', 'created_date':
     '2023-03-09T17:12:00+01:00', 'started_date': '', 'last_update': '', 'commands': None, 'values':
     '{"target_ip": "1.2.3.4", "param3": "value3", "param2: "this string contains a substring, it
@@ -534,16 +539,14 @@
                 )
 
             # If all constraints are respected, the attack is the right one
             if attack_values_match:
                 return attack
 
 
-
-
 def __execute_attack_with_value(
     attack_name: str,
     waiting_worker: bool = True,
     values: Optional[Dict] = None,
     debug: bool = False,
 ) -> Optional[str]:
     url = "/attack"
@@ -577,16 +580,16 @@
 def init_knowledge(data: List[dict]) -> bool:
     """
     Insert data in knowledge database.
 
     :return: boolean
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.init_knowledge([{"host": {"host_ip": "x.x.x.x", "host": {"netbios_name": "WIN"}, "roles": []}}])
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.init_knowledge([{"host": {"host_ip": "x.x.x.x", "host": {"netbios_name": "WIN"}, "roles": []}}])  # doctest: +SKIP
     True
 
     """
     output = {}
 
     for elt in data:
         key = list(elt)[0]
@@ -605,16 +608,16 @@
 def scenario_result() -> str:
     """
     Generate json report about all attack actions.
 
     :return: List all attacks done and runnning.
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.scenario_result()
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.scenario_result()  # doctest: +SKIP
     []
 
     """
 
     url = "/report"
 
     result = _get(url, headers={}, data={})
@@ -628,17 +631,17 @@
 def attack_knowledge() -> str:
     """
     Get the attack knowledge (attack hosts and sessions).
 
     :return: Attack hosts and sessions.
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.attack_knowledge()
-    {'hosts': [], 'attack_sessions': [], 'infrastructures': []}
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.attack_knowledge()  # doctest: +SKIP
+    {'hosts': [], 'network_interfaces': [], 'services': [], 'softwares': [], 'credentials': [], 'payloads': [], 'files': [], 'ad_groups': []}
 
     """
 
     url = "/attack_knowledge"
 
     result = _get(url, headers={}, data={})
     if result.status_code != 200:
@@ -655,16 +658,16 @@
 def attack_sessions() -> str:
     """
     Show available redteam attack sessions.
 
     :return: Attack sessions.
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.attack_sessions()
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.attack_sessions()  # doctest: +SKIP
     []
 
     """
 
     url = "/attack_sessions"
 
     result = _get(url, headers={}, data={})
@@ -692,16 +695,16 @@
 def infrastructures() -> str:
     """
     Show redteam attack infrastructures.
 
     :return: Attack infractructures.
 
     >>> from cr_api_client import redteam_api
-    >>> redteam_api.reset_redteam()
-    >>> redteam_api.infrastructures()
+    >>> redteam_api.reset_redteam()  # doctest: +SKIP
+    >>> redteam_api.infrastructures()  # doctest: +SKIP
     []
 
     """
 
     url = "/attack_infrastructures"
 
     result = _get(url, headers={}, data={})
```

### Comparing `cr_api_client-3.1.0/cr_api_client/topology/TopologyElements.py` & `cr_api_client-4.0.0/cr_api_client/topology/TopologyElements.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/topology/TopologyGenerator.py` & `cr_api_client-4.0.0/cr_api_client/topology/TopologyGenerator.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/topology/TopologyLinksGenerator.py` & `cr_api_client-4.0.0/cr_api_client/topology/TopologyLinksGenerator.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/topology/TopologyNodeGenerator.py` & `cr_api_client-4.0.0/cr_api_client/topology/TopologyNodeGenerator.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/topology/TopologyNodesGenerator.py` & `cr_api_client-4.0.0/cr_api_client/topology/TopologyNodesGenerator.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/topology/validator/common.py` & `cr_api_client-4.0.0/cr_api_client/topology/validator/common.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/topology/validator/link.py` & `cr_api_client-4.0.0/cr_api_client/topology/validator/link.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/topology/validator/node.py` & `cr_api_client-4.0.0/cr_api_client/topology/validator/node.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/topology/validator/topology.py` & `cr_api_client-4.0.0/cr_api_client/topology/validator/topology.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/user_activity_api.py` & `cr_api_client-4.0.0/cr_api_client/user_activity_api.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/cr_api_client/yaml_helper.py` & `cr_api_client-4.0.0/cr_api_client/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-3.1.0/pyproject.toml` & `cr_api_client-4.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cr_api_client"
-version = "3.1.0"
+version = "4.0.0"
 description = "AMOSSYS Cyber Range client API"
 readme = "README.md"
 authors = ["AMOSSYS"]
 packages = [
     { include = "cr_api_client" },
 ]
 license = "MIT"
@@ -23,18 +23,19 @@
 pypsrp = "~0.5.0" # Needed to play ./data/scenarios*
 pydantic = "~1.10.2" # Needed to play ./data/scenarios*
 markupsafe = "2.0.1" # Need to fix version to resolve 'soft_unicode' needed by jinja2
 omegaconf = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 cr_dataset_model = {path = "../libs/cr_dataset_model", develop = true}
-coverage = "6.4"
-pytest = "6.2.2"
-pytest-env = "0.6.2"
-pytest-mock = "3.5.1"
+coverage = "7.2.5"
+pytest = "7.3.1"
+pytest-env = "0.8.1"
+pytest-mock = "3.10.0"
+pytest-cov = "4.0.0"
 sh = "1.14.2"
 commitizen = "~2.35.0"
 mypy = "^0.961"
 allure-pytest = "^2.12.0"
 
 [tool.poetry.scripts]
 cyber_range = "cr_api_client.cyber_range:main"
```

### Comparing `cr_api_client-3.1.0/setup.py` & `cr_api_client-4.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,416 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cr-api-client
+Version: 4.0.0
+Summary: AMOSSYS Cyber Range client API
+License: MIT
+Author: AMOSSYS
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=2.11.3,<2.12.0)
+Requires-Dist: argcomplete (>=1.12.1,<1.13.0)
+Requires-Dist: colorama (>=0.4.4,<0.5.0)
+Requires-Dist: humanize (>=3.13.1,<4.0.0)
+Requires-Dist: loguru (>=0.5.3,<0.6.0)
+Requires-Dist: markupsafe (==2.0.1)
+Requires-Dist: omegaconf (>=2.2.2,<3.0.0)
+Requires-Dist: pydantic (>=1.10.2,<1.11.0)
+Requires-Dist: pypsrp (>=0.5.0,<0.6.0)
+Requires-Dist: requests (>=2.24.0,<3.0.0)
+Requires-Dist: ruamel.yaml (>=0.16.10,<0.17.0)
+Requires-Dist: setuptools (==44.0.0)
+Requires-Dist: termcolor (>=1.1.0,<1.2.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['cr_api_client', 'cr_api_client.topology', 'cr_api_client.topology.validator']
+# AMOSSYS Cyber Range client API
 
-package_data = \
-{'': ['*']}
+## Installation
 
-install_requires = \
-['Jinja2>=2.11.3,<2.12.0',
- 'argcomplete>=1.12.1,<1.13.0',
- 'colorama>=0.4.4,<0.5.0',
- 'humanize>=3.13.1,<4.0.0',
- 'loguru>=0.5.3,<0.6.0',
- 'markupsafe==2.0.1',
- 'omegaconf>=2.2.2,<3.0.0',
- 'pydantic>=1.10.2,<1.11.0',
- 'pypsrp>=0.5.0,<0.6.0',
- 'requests>=2.24.0,<3.0.0',
- 'ruamel.yaml>=0.16.10,<0.17.0',
- 'setuptools==44.0.0',
- 'termcolor>=1.1.0,<1.2.0']
-
-entry_points = \
-{'console_scripts': ['cyber_range = cr_api_client.cyber_range:main']}
-
-setup_kwargs = {
-    'name': 'cr-api-client',
-    'version': '3.1.0',
-    'description': 'AMOSSYS Cyber Range client API',
-    'long_description': '# AMOSSYS Cyber Range client API\n\n## Installation\n\nNote: it is recommanded to install the package in a virtualenv in order to avoid conflicts with version dependencies of other packages.\n\n```sh\npython3 setup.py install\n```\n\n## Configuration\n\nAccess to the Cyber Range is possible with either of the following configuration methods.\n\n### Configuration through configuration file (CLI only)\n\nIt is possible to configure access to the Cyber Range through a configuration file, specified with the `--config` command line parameter:\n\n```sh\n$ cyber_range --help\n(...)\n--config CONFIG       Configuration file\n(...)\n```\n\nConfiguration file content should be of the form `--key = value` (without quotes in values), as in the following exemple:\n\n```\n[DEFAULT]\n--core-url = https://[CORE-URL-API]\n--user_activity-url = https://[USER-ACTIVITY-URL-API]\n--provisioning-url = https://[PROVISIONING-URL-API]\n--redteam-url = https://[REDTEAM-URL-API]\n--cacert = <PATH TO CA CERT>\n--cert = <PATH TO CLIENT CERT>\n--key = <PATH TO CLIENT PRIVATE KEY>\n```\n\n### Configuration through command line arguments (CLI only)\n\nIt is possible to configure access to the Cyber Range through command line arguments. See `cyber_range --help` command line output for available parameters:\n\n```sh\n$ cyber_range\n(...)\n  --core-url CORE_API_URL\n                        Set core API URL (default: \'http://127.0.0.1:5000\')\n  --user_activity-url USER_ACTIVITY_API_URL\n                        Set user activity API URL (default: \'http://127.0.0.1:5002\')\n  --provisioning-url PROVISIONING_API_URL\n                        Set provisioning API URL (default: \'http://127.0.0.1:5003\')\n  --redteam-url REDTEAM_API_URL\n                        Set redteam API URL (default: \'http://127.0.0.1:5004\')\n  --cacert CACERT       Set path to CA certs (default: None)\n  --cert CERT           Set path to client cert (default: None)\n  --key KEY             Set path to client key (default: None)\n```\n\n### Configuration through programmatic means\n\nIt is possible to configure access to the Cyber Range programmatically in Python:\n\n```python\nimport cr_api_client.config import cr_api_client_config\n\n# Set URL API\ncr_api_client_config.core_api_url = "https://[CORE-URL-API]"\ncr_api_client_config.user_activity_api_url = "https://[USER-ACTIVITY-URL-API]"\ncr_api_client_config.provisioning_api_url = "https://[PROVISIONING-URL-API]"\ncr_api_client_config.publish_api_url = "https://[PUBLISH-URL-API]"\ncr_api_client_config.redteam_api_url = "https://[REDTEAM-URL-API]"\n\n# Set server and client certificates for Core API\ncr_api_client_config.cacert = "<PATH TO CA CERT>"\ncr_api_client_config.cert = "<PATH TO CLIENT CERT>"\ncr_api_client_config.key = "<PATH TO CLIENT PRIVATE KEY>"\n```\n\nOr by using environment variable before calling a script depending on\n`cr_api_client` python library:\n\n```bash\nexport CORE_API_URL="https://[CORE-URL-API]"\nexport USER_ACTIVITY_API_URL="https://[USER-ACTIVITY-URL-API]"\nexport PROVISIONING_API_URL="https://[PROVISIONING-URL-API]"\nexport PUBLISH_API_URL="https://[PUBLISH-URL-API]"\nexport REDTEAM_API_URL="https://[REDTEAM-URL-API]"\n\n./my_custom_client\n```\n\n## CLI usage\n\nSee `cyber_range --help` command line output for available parameters:\n\n```sh\n$ cyber_range --help\n(...)\n```\n\n## Programmatic usage\n\n### Platform initialization API\n\nBefore starting a new simulation, the platform has to be initialized:\n\n```python\ncore_api.reset()\nredteam_api.reset_redteam()\n```\n\n### Simulation API\n\n```python\n# Create a simulation from a topology\ncore_api.create_simulation_from_topology(topology_file: str)\n\n# Create a simulation from a basebox ID\ncore_api.create_simulation_from_basebox(basebox_id: str)\n\n# Start the simulation, with current time (by default) or time where the VM was created (use_vm_time=True)\ncore_api.start_simulation(id_simulation: int, use_vm_time: bool)\n\n# Pause a simulation (calls libvirt suspend API)\ncore_api.pause_simulation(id_simulation: int)\n\n# Unpause a simulation (calls libvirt resume API)\ncore_api.unpause_simulation(id_simulation: int)\n\n# Properly stop a simulation, by sending a shutdown signal to the operating systems\ncore_api.halt_simulation(id_simulation: int)\n\n# Stop a simulation through a hard reset\ncore_api.destroy_simulation(id_simulation: int)\n\n# Clone a simulation and create a new simulation, and return the new ID\ncore_api.clone_simulation(id_simulation: int) -> int\n\n# Delete a simulation in database\ncore_api.delete_simulation(id_simulation: int)\n```\n\n### Provisioning API\n\n```python\n# Apply provisioning configuration defined in YAML file on simulation defined in argument ID OR on machines defined in file\n# ``wait`` parameter defines if the function wait for task to complete or not.\n\nprovisioning_execute(id_simulation: int = None,\n                     machines_file: str = None,\n                     provisioning_file: str,\n                     debug: bool = False,\n                     wait: bool = True,\n                     ) -> Tuple[bool, str]:\n\n# Apply ansible playbooks on specified target(s):\n# ``wait`` parameter defines if the function wait for task to complete or not.\n\ndef provisioning_ansible(id_simulation: int = None,\n                         machines_file: str = None,\n                         playbook_path: str = None,\n                         target_roles: List[str] = [],\n                         target_system_types: List[str] = [],\n                         target_operating_systems: List[str] = [],\n                         target_names: List[str] = [],\n                         extra_vars: str = None,\n                         debug: bool = False,\n                         wait: bool = True,\n                         ) -> Tuple[bool, str]:\n\n# Get status on targeted simulation\nprovisioning_api.provisioning_status(id_simulation: int)\n\n# Get provisioning result on targeted simulation\nprovisioning_api.provisioning_result(id_simulation: int)\n```\n\n### User activity API\n\n```python\nuser_activity_api.user_activity_play(id_simulation: int, user_activity_path: str,\n                              debug_mode: str = \'off\', speed: str = \'normal\',\n                              user_activity_file_results: str = None)\n```\n\nThis method makes it possible to play user activities defined in ``user activity path`` on simulation defined in ``id_simulation``.\nThese parameters are **mandatory**.\n\nThe following parameters are optional:\n\n* ``debug_mode``: This parameter has to be used for **debug** only. It corresponds to the level of verbosity of the debug traces generated during the execution of user actions:\n  * ``\'off\'``: no debug traces,\n  * ``\'on\'``:  with debug traces,\n  * ``\'full\'``: with maximum debug traces.\n\n  The default is ``\'off\'``. Debug traces are generated **on the server side only**.\n\n* ``speed``: This parameter affects the speed of typing keys on the keyboard and the speed of mouse movement:\n  * ``\'slow\'``: slow speed,\n  * ``\'normal\'``:  normal speed,\n  * ``\'fast\'``: fast speed.\n\n  The default is ``\'normal\'``.\n\n* ``user_activity_file_results``: This parameter makes it possible to get the user activity results (of user actions) in a file.\n  Results are stored using a json format. The file name should be absolute (``\'/tmp/results.json\'`` for example).\n\n  Here an example:\n\n  ```json\n  {\n    "success": true,\n    "scenario_results": [\n        {\n            "name": "user_activity.py",\n            "success": true,\n            "target": {\n                "name": "CLIENT1",\n                "role": "client",\n                "basebox_id": 70,\n                "ip_address": "localhost",\n                "vnc_port": 5901\n            },\n            "action_packs": {\n                "operating_system": "operating_system/windows7"\n            },\n            "action_list": [\n                {\n                    "name": "open_session",\n                    "parameters": {\n                        "password": "7h7JMc67",\n                        "password_error": "false",\n                        "login": "John"\n                    },\n                    "start_time": "2021-03-01 12:39:25.119",\n                    "end_time": "2021-03-01 12:39:57.325",\n                    "success": true,\n                    "implemented": true\n                },\n                {\n                    "name": "close_session",\n                    "parameters": {},\n                    "start_time": "2021-03-01 12:40:02.330",\n                    "end_time": "2021-03-01 12:40:09.303",\n                    "success": true,\n                    "implemented": true\n                }\n            ]\n        }\n    ]\n  }\n  ```\n\nHere are some examples of calling this method:\n\n```python\nuser_activity_api.user_activity_play(1, \'./user_activity/my_scenario\') # this is the common way\n\nuser_activity_api.user_activity_play(1, \'./user_activity/my_scenario\', scenario_file_results=\'/tmp/results.json\')\n\nuser_activity_api.user_activity_play(1, \'./user_activity/my_scenario\', debug_mode=\'full\', speed=\'fast\')\n```\n\n### Redteam API\n\n```python\nredteam_api.execute_scenario(attack_list: str)\n```\n\nThis method executes sequentially each attack in list.\nFor each attack this method displays started time and ending time (last_update).\n\n```python\nredteam_api.execute_attack_name(attack_name: str,  waiting_worker: bool = True)\n```\n\nThis method execute one attack, selected by name.\n\n```python\ndef init_knowledge(data: List[dict])\n```\n\nLoad data into knowledge database.\n\nExample :\n```\n[\n  {"software":\n    {"host_ip": "192.168.33.11",\n    "software": {"category": "os"},\n    "credentials":[{"username": "Administrateur", "password": "123pass"}]\n    }\n  }\n]\n```\n\n```python\ndef attack_infos(id_attack: str)\n```\n\nGet status and output for attack.\n\nExample :\n```\nstatus = "success",\noutput = [\n  {\n  "attack_session": {\n   "idAttackSession": 1,\n   "source": "vffxlcationgreedinessb.com",\n   "type": "powershell",\n   "identifier": "d67672cb-8f64-420a-a7ba-1d33d7b7fd45",\n   "privilege_level": 1,\n   "idHost": 1\n  }\n }\n]\n\n```\n\n```python\nredteam_api.list_workers()\n```\n\nThis method list all workers availabe in platform.\nList of attributes :\n* stability\n* reliability\n* side_effect\n* killchain_step : step in MITRE ATT&CK killchain\n\n```json\n{\n  "worker_id":"1548_002_001",\n  "name":"uac_bypass",\n  "description":"Use Metasploit uac bypass",\n  "stability":"CRASH_SAFE",\n  "reliability":"ALWAYS",\n  "side_effect":"NETWORK_CONNECTION",\n  "killchain_step":"privilege_escalation",\n  "repeatable":false\n}\n```\n\n\n```python\nredteam_api.list_attacks()\n```\n\nThis method return all attack (available, successed or failed) with time information and origin.\nList of attributes :\n* idAttack : Identifier for attack action\n* status : Attack status (failed, success or runnable)\n* created_date\n* started_date\n* last_update : End time\n* values : Values send to the worker\n* output : Data generated by this attack\n* source: idAttack that created it\n\nHere an example :\n```json\n{\n  "idAttack":13,\n  "worker":\n  {\n    "worker_id":"1548_002_001",\n    "name":"uac_bypass",\n    "description":"Use Metasploit uac bypass",\n    "stability":"FIRST_ATTEMPT_FAIL",\n    "reliability":"ALWAYS",\n    "side_effect":"NETWORK_CONNECTION",\n    "killchain_step":"privilege_escalation",\n    "repeatable":false\n    },\n  "status":"success",\n  "created_date":"2021-04-21 10:33:00",\n  "started_date":"2021-04-21 10:37:04",\n  "last_update":"2021-04-21 10:37:06",\n  "values":"{\\"Host.ip\\": \\"192.168.2.101\\", \\"AttackSession.type\\": \\"windows/x64/meterpreter/reverse_tcp\\", \\"AttackSession.source\\": \\"192.168.2.66\\", \\"AttackSession.identifier\\": \\"1\\"}",\n  "output": "",\n  "source":1}\n```\n\n\n*In progress*\n',
-    'author': 'AMOSSYS',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+Note: it is recommanded to install the package in a virtualenv in order to avoid conflicts with version dependencies of other packages.
+
+```sh
+python3 setup.py install
+```
+
+## Configuration
+
+Access to the Cyber Range is possible with either of the following configuration methods.
+
+### Configuration through configuration file (CLI only)
+
+It is possible to configure access to the Cyber Range through a configuration file, specified with the `--config` command line parameter:
+
+```sh
+$ cyber_range --help
+(...)
+--config CONFIG       Configuration file
+(...)
+```
+
+Configuration file content should be of the form `--key = value` (without quotes in values), as in the following exemple:
+
+```
+[DEFAULT]
+--core-url = https://[CORE-URL-API]
+--user_activity-url = https://[USER-ACTIVITY-URL-API]
+--provisioning-url = https://[PROVISIONING-URL-API]
+--redteam-url = https://[REDTEAM-URL-API]
+--cacert = <PATH TO CA CERT>
+--cert = <PATH TO CLIENT CERT>
+--key = <PATH TO CLIENT PRIVATE KEY>
+```
+
+### Configuration through command line arguments (CLI only)
+
+It is possible to configure access to the Cyber Range through command line arguments. See `cyber_range --help` command line output for available parameters:
+
+```sh
+$ cyber_range
+(...)
+  --core-url CORE_API_URL
+                        Set core API URL (default: 'http://127.0.0.1:5000')
+  --user_activity-url USER_ACTIVITY_API_URL
+                        Set user activity API URL (default: 'http://127.0.0.1:5002')
+  --provisioning-url PROVISIONING_API_URL
+                        Set provisioning API URL (default: 'http://127.0.0.1:5003')
+  --redteam-url REDTEAM_API_URL
+                        Set redteam API URL (default: 'http://127.0.0.1:5004')
+  --cacert CACERT       Set path to CA certs (default: None)
+  --cert CERT           Set path to client cert (default: None)
+  --key KEY             Set path to client key (default: None)
+```
+
+### Configuration through programmatic means
+
+It is possible to configure access to the Cyber Range programmatically in Python:
+
+```python
+import cr_api_client.config import cr_api_client_config
+
+# Set URL API
+cr_api_client_config.core_api_url = "https://[CORE-URL-API]"
+cr_api_client_config.user_activity_api_url = "https://[USER-ACTIVITY-URL-API]"
+cr_api_client_config.provisioning_api_url = "https://[PROVISIONING-URL-API]"
+cr_api_client_config.publish_api_url = "https://[PUBLISH-URL-API]"
+cr_api_client_config.redteam_api_url = "https://[REDTEAM-URL-API]"
+
+# Set server and client certificates for Core API
+cr_api_client_config.cacert = "<PATH TO CA CERT>"
+cr_api_client_config.cert = "<PATH TO CLIENT CERT>"
+cr_api_client_config.key = "<PATH TO CLIENT PRIVATE KEY>"
+```
+
+Or by using environment variable before calling a script depending on
+`cr_api_client` python library:
+
+```bash
+export CORE_API_URL="https://[CORE-URL-API]"
+export USER_ACTIVITY_API_URL="https://[USER-ACTIVITY-URL-API]"
+export PROVISIONING_API_URL="https://[PROVISIONING-URL-API]"
+export PUBLISH_API_URL="https://[PUBLISH-URL-API]"
+export REDTEAM_API_URL="https://[REDTEAM-URL-API]"
+
+./my_custom_client
+```
+
+## CLI usage
+
+See `cyber_range --help` command line output for available parameters:
+
+```sh
+$ cyber_range --help
+(...)
+```
+
+## Programmatic usage
+
+### Platform initialization API
+
+Before starting a new simulation, the platform has to be initialized:
+
+```python
+core_api.reset()
+redteam_api.reset_redteam()
+```
+
+### Simulation API
+
+```python
+# Create a simulation from a topology
+core_api.create_simulation_from_topology(topology_file: str)
+
+# Create a simulation from a basebox ID
+core_api.create_simulation_from_basebox(basebox_id: str)
+
+# Start the simulation, with current time (by default) or time where the VM was created (use_vm_time=True)
+core_api.start_simulation(id_simulation: int, use_vm_time: bool)
+
+# Pause a simulation (calls libvirt suspend API)
+core_api.pause_simulation(id_simulation: int)
+
+# Unpause a simulation (calls libvirt resume API)
+core_api.unpause_simulation(id_simulation: int)
+
+# Properly stop a simulation, by sending a shutdown signal to the operating systems
+core_api.halt_simulation(id_simulation: int)
+
+# Stop a simulation through a hard reset
+core_api.destroy_simulation(id_simulation: int)
+
+# Clone a simulation and create a new simulation, and return the new ID
+core_api.clone_simulation(id_simulation: int) -> int
+
+# Delete a simulation in database
+core_api.delete_simulation(id_simulation: int)
+```
+
+### Provisioning API
+
+```python
+# Apply provisioning configuration defined in YAML file on simulation defined in argument ID OR on machines defined in file
+# ``wait`` parameter defines if the function wait for task to complete or not.
+
+provisioning_execute(id_simulation: int = None,
+                     machines_file: str = None,
+                     provisioning_file: str,
+                     debug: bool = False,
+                     wait: bool = True,
+                     ) -> Tuple[bool, str]:
+
+# Apply ansible playbooks on specified target(s):
+# ``wait`` parameter defines if the function wait for task to complete or not.
+
+def provisioning_ansible(id_simulation: int = None,
+                         machines_file: str = None,
+                         playbook_path: str = None,
+                         target_roles: List[str] = [],
+                         target_system_types: List[str] = [],
+                         target_operating_systems: List[str] = [],
+                         target_names: List[str] = [],
+                         extra_vars: str = None,
+                         debug: bool = False,
+                         wait: bool = True,
+                         ) -> Tuple[bool, str]:
+
+# Get status on targeted simulation
+provisioning_api.provisioning_status(id_simulation: int)
+
+# Get provisioning result on targeted simulation
+provisioning_api.provisioning_result(id_simulation: int)
+```
+
+### User activity API
+
+```python
+user_activity_api.user_activity_play(id_simulation: int, user_activity_path: str,
+                              debug_mode: str = 'off', speed: str = 'normal',
+                              user_activity_file_results: str = None)
+```
+
+This method makes it possible to play user activities defined in ``user activity path`` on simulation defined in ``id_simulation``.
+These parameters are **mandatory**.
+
+The following parameters are optional:
+
+* ``debug_mode``: This parameter has to be used for **debug** only. It corresponds to the level of verbosity of the debug traces generated during the execution of user actions:
+  * ``'off'``: no debug traces,
+  * ``'on'``:  with debug traces,
+  * ``'full'``: with maximum debug traces.
+
+  The default is ``'off'``. Debug traces are generated **on the server side only**.
+
+* ``speed``: This parameter affects the speed of typing keys on the keyboard and the speed of mouse movement:
+  * ``'slow'``: slow speed,
+  * ``'normal'``:  normal speed,
+  * ``'fast'``: fast speed.
+
+  The default is ``'normal'``.
+
+* ``user_activity_file_results``: This parameter makes it possible to get the user activity results (of user actions) in a file.
+  Results are stored using a json format. The file name should be absolute (``'/tmp/results.json'`` for example).
+
+  Here an example:
+
+  ```json
+  {
+    "success": true,
+    "scenario_results": [
+        {
+            "name": "user_activity.py",
+            "success": true,
+            "target": {
+                "name": "CLIENT1",
+                "role": "client",
+                "basebox_id": 70,
+                "ip_address": "localhost",
+                "vnc_port": 5901
+            },
+            "action_packs": {
+                "operating_system": "operating_system/windows7"
+            },
+            "action_list": [
+                {
+                    "name": "open_session",
+                    "parameters": {
+                        "password": "7h7JMc67",
+                        "password_error": "false",
+                        "login": "John"
+                    },
+                    "start_time": "2021-03-01 12:39:25.119",
+                    "end_time": "2021-03-01 12:39:57.325",
+                    "success": true,
+                    "implemented": true
+                },
+                {
+                    "name": "close_session",
+                    "parameters": {},
+                    "start_time": "2021-03-01 12:40:02.330",
+                    "end_time": "2021-03-01 12:40:09.303",
+                    "success": true,
+                    "implemented": true
+                }
+            ]
+        }
+    ]
+  }
+  ```
+
+Here are some examples of calling this method:
+
+```python
+user_activity_api.user_activity_play(1, './user_activity/my_scenario') # this is the common way
+
+user_activity_api.user_activity_play(1, './user_activity/my_scenario', scenario_file_results='/tmp/results.json')
+
+user_activity_api.user_activity_play(1, './user_activity/my_scenario', debug_mode='full', speed='fast')
+```
+
+### Redteam API
+
+```python
+redteam_api.execute_scenario(attack_list: str)
+```
+
+This method executes sequentially each attack in list.
+For each attack this method displays started time and ending time (last_update).
+
+```python
+redteam_api.execute_attack_name(attack_name: str,  waiting_worker: bool = True)
+```
+
+This method execute one attack, selected by name.
+
+```python
+def init_knowledge(data: List[dict])
+```
+
+Load data into knowledge database.
+
+Example :
+```
+[
+  {"software":
+    {"host_ip": "192.168.33.11",
+    "software": {"category": "os"},
+    "credentials":[{"username": "Administrateur", "password": "123pass"}]
+    }
+  }
+]
+```
+
+```python
+def attack_infos(id_attack: str)
+```
+
+Get status and output for attack.
+
+Example :
+```
+status = "success",
+output = [
+  {
+  "attack_session": {
+   "idAttackSession": 1,
+   "source": "vffxlcationgreedinessb.com",
+   "type": "powershell",
+   "identifier": "d67672cb-8f64-420a-a7ba-1d33d7b7fd45",
+   "privilege_level": 1,
+   "idHost": 1
+  }
+ }
+]
+
+```
+
+```python
+redteam_api.list_workers()
+```
+
+This method list all workers availabe in platform.
+List of attributes :
+* stability
+* reliability
+* side_effect
+* killchain_step : step in MITRE ATT&CK killchain
+
+```json
+{
+  "worker_id":"1548_002_001",
+  "name":"uac_bypass",
+  "description":"Use Metasploit uac bypass",
+  "stability":"CRASH_SAFE",
+  "reliability":"ALWAYS",
+  "side_effect":"NETWORK_CONNECTION",
+  "killchain_step":"privilege_escalation",
+  "repeatable":false
 }
+```
+
+
+```python
+redteam_api.list_attacks()
+```
+
+This method return all attack (available, successed or failed) with time information and origin.
+List of attributes :
+* idAttack : Identifier for attack action
+* status : Attack status (failed, success or runnable)
+* created_date
+* started_date
+* last_update : End time
+* values : Values send to the worker
+* output : Data generated by this attack
+* source: idAttack that created it
+
+Here an example :
+```json
+{
+  "idAttack":13,
+  "worker":
+  {
+    "worker_id":"1548_002_001",
+    "name":"uac_bypass",
+    "description":"Use Metasploit uac bypass",
+    "stability":"FIRST_ATTEMPT_FAIL",
+    "reliability":"ALWAYS",
+    "side_effect":"NETWORK_CONNECTION",
+    "killchain_step":"privilege_escalation",
+    "repeatable":false
+    },
+  "status":"success",
+  "created_date":"2021-04-21 10:33:00",
+  "started_date":"2021-04-21 10:37:04",
+  "last_update":"2021-04-21 10:37:06",
+  "values":"{\"Host.ip\": \"192.168.2.101\", \"AttackSession.type\": \"windows/x64/meterpreter/reverse_tcp\", \"AttackSession.source\": \"192.168.2.66\", \"AttackSession.identifier\": \"1\"}",
+  "output": "",
+  "source":1}
+```
+
 
+*In progress*
 
-setup(**setup_kwargs)
```

