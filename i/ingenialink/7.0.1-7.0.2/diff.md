# Comparing `tmp/ingenialink-7.0.1.tar.gz` & `tmp/ingenialink-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingenialink-7.0.1.tar", last modified: Tue Apr  4 15:30:31 2023, max compression
+gzip compressed data, was "ingenialink-7.0.2.tar", last modified: Mon May 22 08:59:47 2023, max compression
```

## Comparing `ingenialink-7.0.1.tar` & `ingenialink-7.0.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.414935 ingenialink-7.0.1/
--rw-rw-rw-   0        0        0    17630 2023-04-04 15:29:27.000000 ingenialink-7.0.1/LICENSE.md
--rw-rw-rw-   0        0        0       35 2023-04-04 15:29:27.000000 ingenialink-7.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2080 2023-04-04 15:30:31.399185 ingenialink-7.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1343 2023-04-04 15:29:27.000000 ingenialink-7.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.286814 ingenialink-7.0.1/examples/
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.318071 ingenialink-7.0.1/examples/canopen/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/canopen/__init__.py
--rw-rw-rw-   0        0        0      977 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/canopen/can_connection.py
--rw-rw-rw-   0        0        0     2983 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/canopen/can_disturbance.py
--rw-rw-rw-   0        0        0     2239 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/canopen/can_load_firmware.py
--rw-rw-rw-   0        0        0     1364 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/canopen/can_load_save_config.py
--rw-rw-rw-   0        0        0     4125 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/canopen/can_monitoring.py
--rw-rw-rw-   0        0        0     1609 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/canopen/can_store_restore.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.318071 ingenialink-7.0.1/examples/ethercat/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/ethercat/__init__.py
--rw-rw-rw-   0        0        0      330 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/ethercat/ecat_load_firmware.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.333698 ingenialink-7.0.1/examples/ethernet/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/ethernet/__init__.py
--rw-rw-rw-   0        0        0      549 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/ethernet/eth_connection.py
--rw-rw-rw-   0        0        0      334 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/ethernet/eth_load_firmware.py
--rw-rw-rw-   0        0        0     1264 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/ethernet/eth_load_save_config.py
--rw-rw-rw-   0        0        0     3959 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/ethernet/eth_monitoring.py
--rw-rw-rw-   0        0        0     1276 2023-04-04 15:29:27.000000 ingenialink-7.0.1/examples/ethernet/eth_store_restore.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.333698 ingenialink-7.0.1/ingenialink/
--rw-rw-rw-   0        0        0     1410 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.350609 ingenialink-7.0.1/ingenialink/bin/
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.350609 ingenialink-7.0.1/ingenialink/bin/FoE/
--rw-rw-rw-   0        0        0       23 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/bin/FoE/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.350609 ingenialink-7.0.1/ingenialink/bin/FoE/win_64x/
--rwxrwxrwx   0        0        0    44032 2023-04-04 15:28:42.000000 ingenialink-7.0.1/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/bin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.350609 ingenialink-7.0.1/ingenialink/canopen/
--rw-rw-rw-   0        0        0       90 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/canopen/__init__.py
--rw-rw-rw-   0        0        0     1527 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/canopen/dictionary.py
--rw-rw-rw-   0        0        0    38430 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/canopen/network.py
--rw-rw-rw-   0        0        0     2434 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/canopen/register.py
--rw-rw-rw-   0        0        0     5333 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/canopen/servo.py
--rw-rw-rw-   0        0        0      902 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/constants.py
--rw-rw-rw-   0        0        0    13716 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/dictionary.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.366298 ingenialink-7.0.1/ingenialink/enums/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/enums/__init__.py
--rw-rw-rw-   0        0        0     1172 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/enums/register.py
--rw-rw-rw-   0        0        0     2892 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/enums/servo.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.366298 ingenialink-7.0.1/ingenialink/eoe/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/eoe/__init__.py
--rw-rw-rw-   0        0        0    12305 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/eoe/network.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.366298 ingenialink-7.0.1/ingenialink/ethercat/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/ethercat/__init__.py
--rw-rw-rw-   0        0        0     3040 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/ethercat/network.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.366298 ingenialink-7.0.1/ingenialink/ethernet/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/ethernet/__init__.py
--rw-rw-rw-   0        0        0     1392 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/ethernet/dictionary.py
--rw-rw-rw-   0        0        0    10972 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/ethernet/network.py
--rw-rw-rw-   0        0        0     2432 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/ethernet/register.py
--rw-rw-rw-   0        0        0     5636 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/ethernet/servo.py
--rw-rw-rw-   0        0        0     3572 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/exceptions.py
--rw-rw-rw-   0        0        0     1765 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/network.py
--rw-rw-rw-   0        0        0     7615 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/poller.py
--rw-rw-rw-   0        0        0     7824 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/register.py
--rw-rw-rw-   0        0        0    41950 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/servo.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.382821 ingenialink-7.0.1/ingenialink/utils/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/utils/__init__.py
--rw-rw-rw-   0        0        0     7856 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/utils/_utils.py
--rw-rw-rw-   0        0        0     4486 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/utils/constants.py
--rw-rw-rw-   0        0        0      684 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/utils/errors.py
--rw-rw-rw-   0        0        0     6983 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/utils/mcb.py
--rw-rw-rw-   0        0        0     4263 2023-04-04 15:29:27.000000 ingenialink-7.0.1/ingenialink/utils/udp.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.350609 ingenialink-7.0.1/ingenialink.egg-info/
--rw-rw-rw-   0        0        0     2080 2023-04-04 15:30:31.000000 ingenialink-7.0.1/ingenialink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2355 2023-04-04 15:30:31.000000 ingenialink-7.0.1/ingenialink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 15:30:31.000000 ingenialink-7.0.1/ingenialink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      294 2023-04-04 15:30:31.000000 ingenialink-7.0.1/ingenialink.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-04 15:30:31.000000 ingenialink-7.0.1/ingenialink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-04-04 15:29:27.000000 ingenialink-7.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 15:30:31.414935 ingenialink-7.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1783 2023-04-04 15:29:27.000000 ingenialink-7.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.382821 ingenialink-7.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.399185 ingenialink-7.0.1/tests/canopen/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/canopen/__init__.py
--rw-rw-rw-   0        0        0     3688 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/canopen/test_canopen_dictionary.py
--rw-rw-rw-   0        0        0     4009 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/canopen/test_canopen_network.py
--rw-rw-rw-   0        0        0     3470 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/canopen/test_canopen_register.py
--rw-rw-rw-   0        0        0      262 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/canopen/test_canopen_servo.py
--rw-rw-rw-   0        0        0     3246 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.399185 ingenialink-7.0.1/tests/ethercat/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/ethercat/__init__.py
--rw-rw-rw-   0        0        0     1619 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/ethercat/test_ethercat_network.py
-drwxrwxrwx   0        0        0        0 2023-04-04 15:30:31.399185 ingenialink-7.0.1/tests/ethernet/
--rw-rw-rw-   0        0        0        0 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/ethernet/__init__.py
--rw-rw-rw-   0        0        0     3376 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/ethernet/test_ethernet_dictionary.py
--rw-rw-rw-   0        0        0     4511 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/ethernet/test_ethernet_network.py
--rw-rw-rw-   0        0        0     2057 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/ethernet/test_ethernet_register.py
--rw-rw-rw-   0        0        0      712 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/ethernet/test_ethernet_servo.py
--rw-rw-rw-   0        0        0     3103 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/test_mcb.py
--rw-rw-rw-   0        0        0     5594 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/test_register.py
--rw-rw-rw-   0        0        0    16261 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/test_servo.py
--rw-rw-rw-   0        0        0     4744 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/test_virtual_drive.py
--rw-rw-rw-   0        0        0    16613 2023-04-04 15:29:27.000000 ingenialink-7.0.1/tests/virtual_drive.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.599449 ingenialink-7.0.2/
+-rw-rw-rw-   0        0        0    17630 2023-05-22 08:58:33.000000 ingenialink-7.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0       35 2023-05-22 08:58:33.000000 ingenialink-7.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2080 2023-05-22 08:59:47.599449 ingenialink-7.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1343 2023-05-22 08:58:33.000000 ingenialink-7.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.458792 ingenialink-7.0.2/examples/
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.490076 ingenialink-7.0.2/examples/canopen/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/canopen/__init__.py
+-rw-rw-rw-   0        0        0      977 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/canopen/can_connection.py
+-rw-rw-rw-   0        0        0     2983 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/canopen/can_disturbance.py
+-rw-rw-rw-   0        0        0     2239 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/canopen/can_load_firmware.py
+-rw-rw-rw-   0        0        0     1364 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/canopen/can_load_save_config.py
+-rw-rw-rw-   0        0        0     4125 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/canopen/can_monitoring.py
+-rw-rw-rw-   0        0        0     1609 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/canopen/can_store_restore.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.505668 ingenialink-7.0.2/examples/ethercat/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/ethercat/__init__.py
+-rw-rw-rw-   0        0        0      330 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/ethercat/ecat_load_firmware.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.521334 ingenialink-7.0.2/examples/ethernet/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/ethernet/__init__.py
+-rw-rw-rw-   0        0        0      549 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/ethernet/eth_connection.py
+-rw-rw-rw-   0        0        0      334 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/ethernet/eth_load_firmware.py
+-rw-rw-rw-   0        0        0     1264 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/ethernet/eth_load_save_config.py
+-rw-rw-rw-   0        0        0     3959 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/ethernet/eth_monitoring.py
+-rw-rw-rw-   0        0        0     1276 2023-05-22 08:58:33.000000 ingenialink-7.0.2/examples/ethernet/eth_store_restore.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.536952 ingenialink-7.0.2/ingenialink/
+-rw-rw-rw-   0        0        0     1410 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.536952 ingenialink-7.0.2/ingenialink/bin/
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.536952 ingenialink-7.0.2/ingenialink/bin/FoE/
+-rw-rw-rw-   0        0        0       23 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/bin/FoE/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.536952 ingenialink-7.0.2/ingenialink/bin/FoE/win_64x/
+-rwxrwxrwx   0        0        0    44032 2023-05-22 08:57:48.000000 ingenialink-7.0.2/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/bin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.552569 ingenialink-7.0.2/ingenialink/canopen/
+-rw-rw-rw-   0        0        0       90 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/canopen/__init__.py
+-rw-rw-rw-   0        0        0     1527 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/canopen/dictionary.py
+-rw-rw-rw-   0        0        0    38430 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/canopen/network.py
+-rw-rw-rw-   0        0        0     2434 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/canopen/register.py
+-rw-rw-rw-   0        0        0     5333 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/canopen/servo.py
+-rw-rw-rw-   0        0        0      902 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/constants.py
+-rw-rw-rw-   0        0        0    13716 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/dictionary.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.552569 ingenialink-7.0.2/ingenialink/enums/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/enums/__init__.py
+-rw-rw-rw-   0        0        0     1172 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/enums/register.py
+-rw-rw-rw-   0        0        0     2892 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/enums/servo.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.552569 ingenialink-7.0.2/ingenialink/eoe/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/eoe/__init__.py
+-rw-rw-rw-   0        0        0    12305 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/eoe/network.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.552569 ingenialink-7.0.2/ingenialink/ethercat/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/ethercat/__init__.py
+-rw-rw-rw-   0        0        0     3051 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/ethercat/network.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.568186 ingenialink-7.0.2/ingenialink/ethernet/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/ethernet/__init__.py
+-rw-rw-rw-   0        0        0     1392 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/ethernet/dictionary.py
+-rw-rw-rw-   0        0        0    11068 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/ethernet/network.py
+-rw-rw-rw-   0        0        0     2432 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/ethernet/register.py
+-rw-rw-rw-   0        0        0     5636 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/ethernet/servo.py
+-rw-rw-rw-   0        0        0     3572 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/exceptions.py
+-rw-rw-rw-   0        0        0     1765 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/network.py
+-rw-rw-rw-   0        0        0     7615 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/poller.py
+-rw-rw-rw-   0        0        0     7824 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/register.py
+-rw-rw-rw-   0        0        0    41930 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/servo.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.568186 ingenialink-7.0.2/ingenialink/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/utils/__init__.py
+-rw-rw-rw-   0        0        0     7856 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/utils/_utils.py
+-rw-rw-rw-   0        0        0     4486 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/utils/constants.py
+-rw-rw-rw-   0        0        0      684 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/utils/errors.py
+-rw-rw-rw-   0        0        0     7004 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/utils/mcb.py
+-rw-rw-rw-   0        0        0     4263 2023-05-22 08:58:33.000000 ingenialink-7.0.2/ingenialink/utils/udp.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.536952 ingenialink-7.0.2/ingenialink.egg-info/
+-rw-rw-rw-   0        0        0     2080 2023-05-22 08:59:47.000000 ingenialink-7.0.2/ingenialink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2355 2023-05-22 08:59:47.000000 ingenialink-7.0.2/ingenialink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:59:47.000000 ingenialink-7.0.2/ingenialink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2023-05-22 08:59:47.000000 ingenialink-7.0.2/ingenialink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-22 08:59:47.000000 ingenialink-7.0.2/ingenialink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-05-22 08:58:33.000000 ingenialink-7.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 08:59:47.599449 ingenialink-7.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1744 2023-05-22 08:58:33.000000 ingenialink-7.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.583830 ingenialink-7.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.599449 ingenialink-7.0.2/tests/canopen/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/canopen/__init__.py
+-rw-rw-rw-   0        0        0     3688 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/canopen/test_canopen_dictionary.py
+-rw-rw-rw-   0        0        0     4009 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/canopen/test_canopen_network.py
+-rw-rw-rw-   0        0        0     3470 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/canopen/test_canopen_register.py
+-rw-rw-rw-   0        0        0      262 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/canopen/test_canopen_servo.py
+-rw-rw-rw-   0        0        0     3246 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.599449 ingenialink-7.0.2/tests/ethercat/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/ethercat/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/ethercat/test_ethercat_network.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:59:47.599449 ingenialink-7.0.2/tests/ethernet/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/ethernet/__init__.py
+-rw-rw-rw-   0        0        0     3376 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/ethernet/test_ethernet_dictionary.py
+-rw-rw-rw-   0        0        0     4511 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/ethernet/test_ethernet_network.py
+-rw-rw-rw-   0        0        0     2057 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/ethernet/test_ethernet_register.py
+-rw-rw-rw-   0        0        0      712 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/ethernet/test_ethernet_servo.py
+-rw-rw-rw-   0        0        0     3157 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/test_mcb.py
+-rw-rw-rw-   0        0        0     5594 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/test_register.py
+-rw-rw-rw-   0        0        0    16261 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/test_servo.py
+-rw-rw-rw-   0        0        0     4744 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/test_virtual_drive.py
+-rw-rw-rw-   0        0        0    16613 2023-05-22 08:58:33.000000 ingenialink-7.0.2/tests/virtual_drive.py
```

### Comparing `ingenialink-7.0.1/LICENSE.md` & `ingenialink-7.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/PKG-INFO` & `ingenialink-7.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ingenialink
-Version: 7.0.1
+Version: 7.0.2
 Summary: IngeniaLink Communications Library
 Home-page: https://www.ingeniamc.com
 Author: Ingenia Motion Control
 Author-email: support@ingeniamc.com
 License: UNKNOWN
-Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.0.1
+Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.0.2
 Project-URL: Source, https://github.com/ingeniamc/ingenialink-python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications
```

### Comparing `ingenialink-7.0.1/README.rst` & `ingenialink-7.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/canopen/can_connection.py` & `ingenialink-7.0.2/examples/canopen/can_connection.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/canopen/can_disturbance.py` & `ingenialink-7.0.2/examples/canopen/can_disturbance.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/canopen/can_load_firmware.py` & `ingenialink-7.0.2/examples/canopen/can_load_firmware.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/canopen/can_load_save_config.py` & `ingenialink-7.0.2/examples/canopen/can_load_save_config.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/canopen/can_monitoring.py` & `ingenialink-7.0.2/examples/canopen/can_monitoring.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/canopen/can_store_restore.py` & `ingenialink-7.0.2/examples/canopen/can_store_restore.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/ethernet/eth_connection.py` & `ingenialink-7.0.2/examples/ethernet/eth_connection.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/ethernet/eth_load_save_config.py` & `ingenialink-7.0.2/examples/ethernet/eth_load_save_config.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/ethernet/eth_monitoring.py` & `ingenialink-7.0.2/examples/ethernet/eth_monitoring.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/examples/ethernet/eth_store_restore.py` & `ingenialink-7.0.2/examples/ethernet/eth_store_restore.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/__init__.py` & `ingenialink-7.0.2/ingenialink/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,8 +50,8 @@
     "CAN_BAUDRATE",
     "CanopenServo",
     "CanopenRegister",
     "Poller",
     "CanopenDictionary",
 ]
 
-__version__ = "7.0.1"
+__version__ = "7.0.2"
```

### Comparing `ingenialink-7.0.1/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe` & `ingenialink-7.0.2/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/canopen/dictionary.py` & `ingenialink-7.0.2/ingenialink/canopen/dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/canopen/network.py` & `ingenialink-7.0.2/ingenialink/canopen/network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/canopen/register.py` & `ingenialink-7.0.2/ingenialink/canopen/register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/canopen/servo.py` & `ingenialink-7.0.2/ingenialink/canopen/servo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/constants.py` & `ingenialink-7.0.2/ingenialink/constants.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/dictionary.py` & `ingenialink-7.0.2/ingenialink/dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/enums/register.py` & `ingenialink-7.0.2/ingenialink/enums/register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/enums/servo.py` & `ingenialink-7.0.2/ingenialink/enums/servo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/eoe/network.py` & `ingenialink-7.0.2/ingenialink/eoe/network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/ethercat/network.py` & `ingenialink-7.0.2/ingenialink/ethercat/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import os
 import sys
 import platform
 import subprocess
-
-try:
-    import importlib.resources as pkg_resources
-except ImportError:
-    import importlib_resources as pkg_resources
+import inspect
 
 import ingenialogger
 
 from ingenialink.network import NET_PROT
 from ingenialink.exceptions import ILFirmwareLoadError
 from ingenialink import bin as bin_module
 
@@ -63,18 +59,23 @@
         sys_name = sys.platform
         app_path = self.FOE_APPLICATION.get(sys_name, {}).get(arch, None)
         if app_path is None:
             raise NotImplementedError(
                 "Load FW by ECAT is not implemented for this OS and architecture:"
                 f" {sys_name} {arch}"
             )
-        exec_path = os.path.join(str(pkg_resources.files(bin_module)), app_path)
+        exec_path = os.path.join(os.path.dirname(inspect.getfile(bin_module)), app_path)
         logger.debug(f"Call FoE application for {sys_name}-{arch}")
         try:
-            subprocess.run([exec_path, self.interface_name, f"{slave_id}", fw_file], check=True)
+            subprocess.run(
+                [exec_path, self.interface_name, f"{slave_id}", fw_file],
+                check=True,
+                shell=True,
+                encoding="utf-8",
+            )
         except subprocess.CalledProcessError as e:
             foe_return_error = self.FOE_ERRORS.get(e.returncode, self.UNKNOWN_FOE_ERROR)
             raise ILFirmwareLoadError(
                 f"The firmware file could not be loaded correctly. {foe_return_error}"
             ) from e
         logger.info("Firmware updated successfully")
```

### Comparing `ingenialink-7.0.1/ingenialink/ethernet/dictionary.py` & `ingenialink-7.0.2/ingenialink/ethernet/dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/ethernet/network.py` & `ingenialink-7.0.2/ingenialink/ethernet/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,40 +35,41 @@
     """Network status listener thread to check if the drive is alive.
 
     Args:
         network (EthernetNetwork): Network instance of the Ethernet communication.
 
     """
 
-    def __init__(self, network):
+    def __init__(self, network, refresh_time=0.25):
         super(NetStatusListener, self).__init__()
         self.__network = network
+        self.__refresh_time = refresh_time
         self.__stop = False
         self.__max_unsuccessful_pings = MAX_NUM_UNSUCCESSFUL_PINGS
 
     def run(self):
         while not self.__stop:
             for servo in self.__network.servos:
                 unsuccessful_pings = 0
                 servo_ip = servo.ip_address
                 servo_state = self.__network._get_servo_state(servo_ip)
                 while unsuccessful_pings < self.__max_unsuccessful_pings:
-                    response = ping(servo_ip, timeout=1)
-                    if not isinstance(response, float):
+                    response = servo.is_alive()  # TODO: Use ping after CAP-924 is fixed
+                    if response == False:
                         unsuccessful_pings += 1
                     else:
                         break
                 ping_response = unsuccessful_pings != self.__max_unsuccessful_pings
                 if servo_state == NET_STATE.CONNECTED and not ping_response:
                     self.__network._notify_status(servo_ip, NET_DEV_EVT.REMOVED)
                     self.__network._set_servo_state(servo_ip, NET_STATE.DISCONNECTED)
                 if servo_state == NET_STATE.DISCONNECTED and ping_response:
                     self.__network._notify_status(servo_ip, NET_DEV_EVT.ADDED)
                     self.__network._set_servo_state(servo_ip, NET_STATE.CONNECTED)
-            time.sleep(0.25)
+            time.sleep(self.__refresh_time)
 
     def stop(self):
         self.__stop = True
 
 
 class EthernetNetwork(Network):
     """Network for all Ethernet communications."""
```

### Comparing `ingenialink-7.0.1/ingenialink/ethernet/register.py` & `ingenialink-7.0.2/ingenialink/ethernet/register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/ethernet/servo.py` & `ingenialink-7.0.2/ingenialink/ethernet/servo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/exceptions.py` & `ingenialink-7.0.2/ingenialink/exceptions.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/network.py` & `ingenialink-7.0.2/ingenialink/network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/poller.py` & `ingenialink-7.0.2/ingenialink/poller.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/register.py` & `ingenialink-7.0.2/ingenialink/register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/servo.py` & `ingenialink-7.0.2/ingenialink/servo.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         while not self.__stop:
             for subnode in range(1, self.__servo.subnodes):
                 try:
                     current_state = self.__servo.get_state(subnode)
                     if subnode not in previous_states or previous_states[subnode] != current_state:
                         previous_states[subnode] = current_state
                         self.__servo._notify_state(current_state, subnode)
-                except (ILIOError, ILTimeoutError) as e:
+                except ILError as e:
                     logger.error("Error getting drive status. Exception : %s", e)
             time.sleep(1.5)
 
     def stop(self):
         """Stops the loop that reads the status word register"""
         self.__stop = True
```

### Comparing `ingenialink-7.0.1/ingenialink/utils/_utils.py` & `ingenialink-7.0.2/ingenialink/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/utils/constants.py` & `ingenialink-7.0.2/ingenialink/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/utils/errors.py` & `ingenialink-7.0.2/ingenialink/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink/utils/mcb.py` & `ingenialink-7.0.2/ingenialink/utils/mcb.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
         Returns:
             bytes: data contained in frame.
         """
         recv_add, _, cmd, data = cls.read_mcb_frame(frame)
 
         if cmd != MCB_CMD_ACK:
-            err_code_little = int.from_bytes(data, byteorder="little")
+            err_code_little = int.from_bytes(data[: cls.ERR_CODE_SIZE], byteorder="little")
             err_code_big = err_code_little.to_bytes(cls.ERR_CODE_SIZE, byteorder="big")
             raise ILNACKError(f"Communications error (NACK -> 0x{err_code_big.hex().upper()})")
         if expected_address != recv_add:
             raise ILWrongRegisterError(
                 f"Received address: {hex(recv_add)} does "
                 "not match expected address: "
                 f"{hex(expected_address)}"
```

### Comparing `ingenialink-7.0.1/ingenialink/utils/udp.py` & `ingenialink-7.0.2/ingenialink/utils/udp.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/ingenialink.egg-info/PKG-INFO` & `ingenialink-7.0.2/ingenialink.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ingenialink
-Version: 7.0.1
+Version: 7.0.2
 Summary: IngeniaLink Communications Library
 Home-page: https://www.ingeniamc.com
 Author: Ingenia Motion Control
 Author-email: support@ingeniamc.com
 License: UNKNOWN
-Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.0.1
+Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.0.2
 Project-URL: Source, https://github.com/ingeniamc/ingenialink-python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications
```

### Comparing `ingenialink-7.0.1/ingenialink.egg-info/SOURCES.txt` & `ingenialink-7.0.2/ingenialink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/setup.py` & `ingenialink-7.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         'Topic :: Communications',
         'Topic :: Software Development :: Libraries'
     ],
     install_requires=[
         'canopen==1.2.1',
         'python-can==3.3.4',
         'ingenialogger>=0.2.1',
-        'ping3==4.0.3',
-        'importlib-resources==5.4.0'
+        'ping3==4.0.3'
     ],
     extras_require={
         "dev": [
             "sphinx==3.5.4",
             "sphinx-rtd-theme==1.0.0",
             "sphinxcontrib-bibtex==2.4.1",
             "nbsphinx==0.8.6",
```

### Comparing `ingenialink-7.0.1/tests/canopen/test_canopen_dictionary.py` & `ingenialink-7.0.2/tests/canopen/test_canopen_dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/canopen/test_canopen_network.py` & `ingenialink-7.0.2/tests/canopen/test_canopen_network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/canopen/test_canopen_register.py` & `ingenialink-7.0.2/tests/canopen/test_canopen_register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/conftest.py` & `ingenialink-7.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/ethercat/test_ethercat_network.py` & `ingenialink-7.0.2/tests/ethercat/test_ethercat_network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/ethernet/test_ethernet_dictionary.py` & `ingenialink-7.0.2/tests/ethernet/test_ethernet_dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/ethernet/test_ethernet_network.py` & `ingenialink-7.0.2/tests/ethernet/test_ethernet_network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/ethernet/test_ethernet_register.py` & `ingenialink-7.0.2/tests/ethernet/test_ethernet_register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/ethernet/test_ethernet_servo.py` & `ingenialink-7.0.2/tests/ethernet/test_ethernet_servo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/test_mcb.py` & `ingenialink-7.0.2/tests/test_mcb.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,18 @@
     frame = f"{frame[-4:]}0000"
     frame_byte_arr = bytearray.fromhex(frame)
     with pytest.raises(ILWrongCRCError):
         MCB.read_mcb_data(expected_address, frame_byte_arr)
 
 
 @pytest.mark.no_connection
-@pytest.mark.parametrize("expected_address, frame", [(0x11, "a1001c0100000106000000009ad7")])
+@pytest.mark.parametrize(
+    "expected_address, frame",
+    [(0x11, "a1001c0100000106000000009ad7"), (0x11, "a1001c01772f2f3a00004650608b")],
+)
 def test_read_mcb_frame_nack(expected_address, frame):
     frame_byte_arr = bytearray.fromhex(frame)
     with pytest.raises(ILNACKError):
         MCB.read_mcb_data(expected_address, frame_byte_arr)
 
 
 @pytest.mark.no_connection
```

### Comparing `ingenialink-7.0.1/tests/test_register.py` & `ingenialink-7.0.2/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/test_servo.py` & `ingenialink-7.0.2/tests/test_servo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/test_virtual_drive.py` & `ingenialink-7.0.2/tests/test_virtual_drive.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.0.1/tests/virtual_drive.py` & `ingenialink-7.0.2/tests/virtual_drive.py`

 * *Files identical despite different names*

