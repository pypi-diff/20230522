# Comparing `tmp/bdsim-1.1.0.tar.gz` & `tmp/bdsim-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdsim-1.1.0.tar", last modified: Sun May 14 00:13:45 2023, max compression
+gzip compressed data, was "bdsim-1.1.1.tar", last modified: Mon May 22 09:59:40 2023, max compression
```

## Comparing `bdsim-1.1.0.tar` & `bdsim-1.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.693340 bdsim-1.1.0/
--rw-rw----   0 corkep     (503) staff       (20)     1068 2022-11-21 06:57:48.000000 bdsim-1.1.0/LICENSE
--rw-rw----   0 corkep     (503) staff       (20)    22336 2023-05-14 00:13:45.692638 bdsim-1.1.0/PKG-INFO
--rw-r--r--   0 corkep     (503) staff       (20)    20379 2023-05-14 00:02:13.000000 bdsim-1.1.0/README.md
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.626771 bdsim-1.1.0/bdsim/
--rw-rw----   0 corkep     (503) staff       (20)      462 2023-03-12 00:27:33.000000 bdsim-1.1.0/bdsim/__init__.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.658078 bdsim-1.1.0/bdsim/bdedit/
--rw-rw----   0 corkep     (503) staff       (20)   214076 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/Icons.py
--rw-rw----   0 corkep     (503) staff       (20)      550 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/__init__.py
--rwxrwx---   0 corkep     (503) staff       (20)     6767 2023-01-22 22:15:43.000000 bdsim-1.1.0/bdsim/bdedit/bdedit.py
--rw-rw----   0 corkep     (503) staff       (20)    46296 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block.py
--rw-rw----   0 corkep     (503) staff       (20)     3493 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_connector_block.py
--rw-rw----   0 corkep     (503) staff       (20)    27281 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_graphics_block.py
--rw-rw----   0 corkep     (503) staff       (20)    16144 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_graphics_socket.py
--rw-rw----   0 corkep     (503) staff       (20)    65171 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_graphics_wire.py
--rw-rw----   0 corkep     (503) staff       (20)    26025 2023-01-22 22:16:45.000000 bdsim-1.1.0/bdsim/bdedit/block_importer.py
--rw-rw----   0 corkep     (503) staff       (20)     1681 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_main_block.py
--rw-rw----   0 corkep     (503) staff       (20)    56804 2023-03-12 00:27:34.000000 bdsim-1.1.0/bdsim/bdedit/block_param_window.py
--rw-rw----   0 corkep     (503) staff       (20)    10984 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_socket.py
--rw-rw----   0 corkep     (503) staff       (20)    22093 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_wire.py
--rw-rw----   0 corkep     (503) staff       (20)     8773 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/floating_label.py
--rw-rw----   0 corkep     (503) staff       (20)     6662 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/floating_label_graphics.py
--rw-rw----   0 corkep     (503) staff       (20)     3482 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/grouping_box.py
--rw-rw----   0 corkep     (503) staff       (20)    13971 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/grouping_box_graphics.py
--rw-rw----   0 corkep     (503) staff       (20)    35012 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface.py
--rw-rw----   0 corkep     (503) staff       (20)    20471 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_graphics_scene.py
--rw-rw----   0 corkep     (503) staff       (20)    36974 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_graphics_view.py
--rw-rw----   0 corkep     (503) staff       (20)    41772 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_manager.py
--rw-rw----   0 corkep     (503) staff       (20)    21061 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_scene.py
--rw-rw----   0 corkep     (503) staff       (20)     7608 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_scene_history.py
--rw-rw----   0 corkep     (503) staff       (20)     1645 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_serialize.py
--rwxrwx---   0 corkep     (503) staff       (20)     8230 2023-05-12 03:20:38.000000 bdsim-1.1.0/bdsim/bdrun.py
--rw-r--r--   0 corkep     (503) staff       (20)    47042 2023-05-11 10:20:38.000000 bdsim-1.1.0/bdsim/blockdiagram.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.672358 bdsim-1.1.0/bdsim/blocks/
--rw-rw----   0 corkep     (503) staff       (20)      291 2023-04-03 00:16:30.000000 bdsim-1.1.0/bdsim/blocks/__init__.py
--rw-r--r--   0 corkep     (503) staff       (20)    15328 2023-04-19 22:21:12.000000 bdsim-1.1.0/bdsim/blocks/connections.py
--rw-r--r--   0 corkep     (503) staff       (20)    12585 2023-05-01 04:27:59.000000 bdsim-1.1.0/bdsim/blocks/discrete.py
--rw-r--r--   0 corkep     (503) staff       (20)    17776 2023-05-13 23:27:14.000000 bdsim-1.1.0/bdsim/blocks/displays.py
--rw-r--r--   0 corkep     (503) staff       (20)    23971 2023-04-28 05:08:21.000000 bdsim-1.1.0/bdsim/blocks/functions.py
--rw-rw----   0 corkep     (503) staff       (20)     2444 2023-04-30 21:23:08.000000 bdsim-1.1.0/bdsim/blocks/io.py
--rw-r--r--   0 corkep     (503) staff       (20)    14257 2023-04-19 21:49:23.000000 bdsim-1.1.0/bdsim/blocks/linalg.py
--rw-r--r--   0 corkep     (503) staff       (20)     7432 2023-04-19 20:51:16.000000 bdsim-1.1.0/bdsim/blocks/sinks.py
--rw-r--r--   0 corkep     (503) staff       (20)    13423 2023-04-28 02:23:28.000000 bdsim-1.1.0/bdsim/blocks/sources.py
--rw-r--r--   0 corkep     (503) staff       (20)     5439 2023-04-19 22:41:09.000000 bdsim-1.1.0/bdsim/blocks/spatial.py
--rw-r--r--   0 corkep     (503) staff       (20)    17072 2023-04-30 04:30:47.000000 bdsim-1.1.0/bdsim/blocks/transfers.py
--rw-rw----   0 corkep     (503) staff       (20)      442 2022-11-21 06:57:49.000000 bdsim-1.1.0/bdsim/blocks/vision.py
--rw-r--r--   0 corkep     (503) staff       (20)    67747 2023-05-01 04:23:25.000000 bdsim-1.1.0/bdsim/components.py
--rw-r--r--   0 corkep     (503) staff       (20)    10214 2023-04-30 00:39:07.000000 bdsim-1.1.0/bdsim/graphics.py
--rw-r--r--   0 corkep     (503) staff       (20)      855 2023-01-22 06:20:05.000000 bdsim-1.1.0/bdsim/newplots.py
--rw-r--r--   0 corkep     (503) staff       (20)    12653 2023-04-12 03:39:20.000000 bdsim-1.1.0/bdsim/run_realtime.py
--rw-r--r--   0 corkep     (503) staff       (20)    58796 2023-05-11 09:44:42.000000 bdsim-1.1.0/bdsim/run_sim.py
--rw-r--r--   0 corkep     (503) staff       (20)      190 2023-03-14 04:44:13.000000 bdsim-1.1.0/bdsim/test-stubs.py
--rwxrwx---   0 corkep     (503) staff       (20)     5104 2023-04-18 08:13:58.000000 bdsim-1.1.0/bdsim/tex2icon.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.630706 bdsim-1.1.0/bdsim.egg-info/
--rw-rw----   0 corkep     (503) staff       (20)    22336 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/PKG-INFO
--rw-rw----   0 corkep     (503) staff       (20)     1723 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/SOURCES.txt
--rw-rw----   0 corkep     (503) staff       (20)        1 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/dependency_links.txt
--rw-rw----   0 corkep     (503) staff       (20)      113 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/entry_points.txt
--rw-rw----   0 corkep     (503) staff       (20)      287 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/requires.txt
--rw-rw----   0 corkep     (503) staff       (20)        6 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/top_level.txt
--rw-rw----   0 corkep     (503) staff       (20)     1805 2023-04-25 06:02:55.000000 bdsim-1.1.0/pyproject.toml
--rw-rw----   0 corkep     (503) staff       (20)       38 2023-05-14 00:13:45.693542 bdsim-1.1.0/setup.cfg
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.689737 bdsim-1.1.0/tests/
--rw-rw----   0 corkep     (503) staff       (20)     3818 2023-04-10 12:13:42.000000 bdsim-1.1.0/tests/test_bdsim.py
--rw-rw----   0 corkep     (503) staff       (20)    19421 2023-04-18 09:41:18.000000 bdsim-1.1.0/tests/test_blockdiagram.py
--rw-r--r--   0 corkep     (503) staff       (20)     8576 2023-04-15 00:55:21.000000 bdsim-1.1.0/tests/test_components.py
--rwxrwx---   0 corkep     (503) staff       (20)     1085 2022-11-21 06:57:49.000000 bdsim-1.1.0/tests/test_connections.py
--rw-rw----   0 corkep     (503) staff       (20)     2796 2023-05-01 04:28:27.000000 bdsim-1.1.0/tests/test_discrete.py
--rwxrwx---   0 corkep     (503) staff       (20)     7673 2023-01-22 08:44:29.000000 bdsim-1.1.0/tests/test_functions.py
--rw-rw----   0 corkep     (503) staff       (20)     4312 2022-11-21 06:57:49.000000 bdsim-1.1.0/tests/test_linalg.py
--rw-r--r--   0 corkep     (503) staff       (20)     3850 2023-04-14 22:15:25.000000 bdsim-1.1.0/tests/test_sinks.py
--rw-r--r--   0 corkep     (503) staff       (20)     8519 2023-04-14 21:42:24.000000 bdsim-1.1.0/tests/test_sources.py
--rw-rw----   0 corkep     (503) staff       (20)     1145 2022-11-21 06:57:49.000000 bdsim-1.1.0/tests/test_spatial.py
--rw-rw----   0 corkep     (503) staff       (20)     3659 2023-01-22 08:44:29.000000 bdsim-1.1.0/tests/test_transfers.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-22 09:59:40.733311 bdsim-1.1.1/
+-rw-rw----   0 corkep     (503) staff       (20)     1068 2022-11-21 06:57:48.000000 bdsim-1.1.1/LICENSE
+-rw-rw----   0 corkep     (503) staff       (20)    22336 2023-05-22 09:59:40.732757 bdsim-1.1.1/PKG-INFO
+-rw-r--r--   0 corkep     (503) staff       (20)    20379 2023-05-14 00:02:13.000000 bdsim-1.1.1/README.md
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-22 09:59:40.676483 bdsim-1.1.1/bdsim/
+-rw-rw----   0 corkep     (503) staff       (20)      462 2023-03-12 00:27:33.000000 bdsim-1.1.1/bdsim/__init__.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-22 09:59:40.696705 bdsim-1.1.1/bdsim/bdedit/
+-rw-rw----   0 corkep     (503) staff       (20)   214076 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/Icons.py
+-rw-rw----   0 corkep     (503) staff       (20)      550 2023-01-22 08:44:29.000000 bdsim-1.1.1/bdsim/bdedit/__init__.py
+-rwxrwx---   0 corkep     (503) staff       (20)     6767 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/bdedit.py
+-rw-rw----   0 corkep     (503) staff       (20)    46296 2023-01-22 08:44:29.000000 bdsim-1.1.1/bdsim/bdedit/block.py
+-rw-rw----   0 corkep     (503) staff       (20)     3493 2023-01-22 08:44:29.000000 bdsim-1.1.1/bdsim/bdedit/block_connector_block.py
+-rw-rw----   0 corkep     (503) staff       (20)    27281 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/block_graphics_block.py
+-rw-rw----   0 corkep     (503) staff       (20)    16144 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/block_graphics_socket.py
+-rw-rw----   0 corkep     (503) staff       (20)    65171 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/block_graphics_wire.py
+-rw-rw----   0 corkep     (503) staff       (20)    26025 2023-01-22 22:16:45.000000 bdsim-1.1.1/bdsim/bdedit/block_importer.py
+-rw-rw----   0 corkep     (503) staff       (20)     1681 2023-01-22 08:44:29.000000 bdsim-1.1.1/bdsim/bdedit/block_main_block.py
+-rw-rw----   0 corkep     (503) staff       (20)    56804 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/block_param_window.py
+-rw-rw----   0 corkep     (503) staff       (20)    10984 2023-01-22 08:44:29.000000 bdsim-1.1.1/bdsim/bdedit/block_socket.py
+-rw-rw----   0 corkep     (503) staff       (20)    22093 2023-01-22 08:44:29.000000 bdsim-1.1.1/bdsim/bdedit/block_wire.py
+-rw-rw----   0 corkep     (503) staff       (20)     8773 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/floating_label.py
+-rw-rw----   0 corkep     (503) staff       (20)     6662 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/floating_label_graphics.py
+-rw-rw----   0 corkep     (503) staff       (20)     3482 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/grouping_box.py
+-rw-rw----   0 corkep     (503) staff       (20)    13971 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/grouping_box_graphics.py
+-rw-rw----   0 corkep     (503) staff       (20)    35012 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/interface.py
+-rw-rw----   0 corkep     (503) staff       (20)    20471 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/interface_graphics_scene.py
+-rw-rw----   0 corkep     (503) staff       (20)    36974 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/interface_graphics_view.py
+-rw-rw----   0 corkep     (503) staff       (20)    41772 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/interface_manager.py
+-rw-rw----   0 corkep     (503) staff       (20)    21061 2023-05-22 09:58:16.000000 bdsim-1.1.1/bdsim/bdedit/interface_scene.py
+-rw-rw----   0 corkep     (503) staff       (20)     7608 2023-01-22 08:44:29.000000 bdsim-1.1.1/bdsim/bdedit/interface_scene_history.py
+-rw-rw----   0 corkep     (503) staff       (20)     1645 2023-01-22 08:44:29.000000 bdsim-1.1.1/bdsim/bdedit/interface_serialize.py
+-rwxrwx---   0 corkep     (503) staff       (20)     8230 2023-05-12 03:20:38.000000 bdsim-1.1.1/bdsim/bdrun.py
+-rw-r--r--   0 corkep     (503) staff       (20)    47042 2023-05-11 10:20:38.000000 bdsim-1.1.1/bdsim/blockdiagram.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-22 09:59:40.703571 bdsim-1.1.1/bdsim/blocks/
+-rw-rw----   0 corkep     (503) staff       (20)      291 2023-04-03 00:16:30.000000 bdsim-1.1.1/bdsim/blocks/__init__.py
+-rw-r--r--   0 corkep     (503) staff       (20)    15328 2023-04-19 22:21:12.000000 bdsim-1.1.1/bdsim/blocks/connections.py
+-rw-r--r--   0 corkep     (503) staff       (20)    12585 2023-05-01 04:27:59.000000 bdsim-1.1.1/bdsim/blocks/discrete.py
+-rw-r--r--   0 corkep     (503) staff       (20)    17776 2023-05-13 23:27:14.000000 bdsim-1.1.1/bdsim/blocks/displays.py
+-rw-r--r--   0 corkep     (503) staff       (20)    23971 2023-04-28 05:08:21.000000 bdsim-1.1.1/bdsim/blocks/functions.py
+-rw-rw----   0 corkep     (503) staff       (20)     2444 2023-04-30 21:23:08.000000 bdsim-1.1.1/bdsim/blocks/io.py
+-rw-r--r--   0 corkep     (503) staff       (20)    14257 2023-04-19 21:49:23.000000 bdsim-1.1.1/bdsim/blocks/linalg.py
+-rw-r--r--   0 corkep     (503) staff       (20)     7432 2023-04-19 20:51:16.000000 bdsim-1.1.1/bdsim/blocks/sinks.py
+-rw-r--r--   0 corkep     (503) staff       (20)    13423 2023-04-28 02:23:28.000000 bdsim-1.1.1/bdsim/blocks/sources.py
+-rw-r--r--   0 corkep     (503) staff       (20)     5439 2023-04-19 22:41:09.000000 bdsim-1.1.1/bdsim/blocks/spatial.py
+-rw-r--r--   0 corkep     (503) staff       (20)    17072 2023-04-30 04:30:47.000000 bdsim-1.1.1/bdsim/blocks/transfers.py
+-rw-rw----   0 corkep     (503) staff       (20)      442 2022-11-21 06:57:49.000000 bdsim-1.1.1/bdsim/blocks/vision.py
+-rw-r--r--   0 corkep     (503) staff       (20)    67747 2023-05-01 04:23:25.000000 bdsim-1.1.1/bdsim/components.py
+-rw-r--r--   0 corkep     (503) staff       (20)    10214 2023-04-30 00:39:07.000000 bdsim-1.1.1/bdsim/graphics.py
+-rw-r--r--   0 corkep     (503) staff       (20)      855 2023-01-22 06:20:05.000000 bdsim-1.1.1/bdsim/newplots.py
+-rw-r--r--   0 corkep     (503) staff       (20)    12653 2023-04-12 03:39:20.000000 bdsim-1.1.1/bdsim/run_realtime.py
+-rw-r--r--   0 corkep     (503) staff       (20)    58796 2023-05-11 09:44:42.000000 bdsim-1.1.1/bdsim/run_sim.py
+-rw-r--r--   0 corkep     (503) staff       (20)      190 2023-03-14 04:44:13.000000 bdsim-1.1.1/bdsim/test-stubs.py
+-rwxrwx---   0 corkep     (503) staff       (20)     5104 2023-04-18 08:13:58.000000 bdsim-1.1.1/bdsim/tex2icon.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-22 09:59:40.679581 bdsim-1.1.1/bdsim.egg-info/
+-rw-rw----   0 corkep     (503) staff       (20)    22336 2023-05-22 09:59:40.000000 bdsim-1.1.1/bdsim.egg-info/PKG-INFO
+-rw-rw----   0 corkep     (503) staff       (20)     1723 2023-05-22 09:59:40.000000 bdsim-1.1.1/bdsim.egg-info/SOURCES.txt
+-rw-rw----   0 corkep     (503) staff       (20)        1 2023-05-22 09:59:40.000000 bdsim-1.1.1/bdsim.egg-info/dependency_links.txt
+-rw-rw----   0 corkep     (503) staff       (20)      113 2023-05-22 09:59:40.000000 bdsim-1.1.1/bdsim.egg-info/entry_points.txt
+-rw-rw----   0 corkep     (503) staff       (20)      281 2023-05-22 09:59:40.000000 bdsim-1.1.1/bdsim.egg-info/requires.txt
+-rw-rw----   0 corkep     (503) staff       (20)        6 2023-05-22 09:59:40.000000 bdsim-1.1.1/bdsim.egg-info/top_level.txt
+-rw-rw----   0 corkep     (503) staff       (20)     1792 2023-05-22 09:59:24.000000 bdsim-1.1.1/pyproject.toml
+-rw-rw----   0 corkep     (503) staff       (20)       38 2023-05-22 09:59:40.733430 bdsim-1.1.1/setup.cfg
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-22 09:59:40.732082 bdsim-1.1.1/tests/
+-rw-rw----   0 corkep     (503) staff       (20)     3818 2023-04-10 12:13:42.000000 bdsim-1.1.1/tests/test_bdsim.py
+-rw-rw----   0 corkep     (503) staff       (20)    19421 2023-04-18 09:41:18.000000 bdsim-1.1.1/tests/test_blockdiagram.py
+-rw-r--r--   0 corkep     (503) staff       (20)     8576 2023-04-15 00:55:21.000000 bdsim-1.1.1/tests/test_components.py
+-rwxrwx---   0 corkep     (503) staff       (20)     1085 2022-11-21 06:57:49.000000 bdsim-1.1.1/tests/test_connections.py
+-rw-rw----   0 corkep     (503) staff       (20)     2796 2023-05-01 04:28:27.000000 bdsim-1.1.1/tests/test_discrete.py
+-rwxrwx---   0 corkep     (503) staff       (20)     7673 2023-01-22 08:44:29.000000 bdsim-1.1.1/tests/test_functions.py
+-rw-rw----   0 corkep     (503) staff       (20)     4312 2022-11-21 06:57:49.000000 bdsim-1.1.1/tests/test_linalg.py
+-rw-r--r--   0 corkep     (503) staff       (20)     3850 2023-04-14 22:15:25.000000 bdsim-1.1.1/tests/test_sinks.py
+-rw-r--r--   0 corkep     (503) staff       (20)     8519 2023-04-14 21:42:24.000000 bdsim-1.1.1/tests/test_sources.py
+-rw-rw----   0 corkep     (503) staff       (20)     1145 2022-11-21 06:57:49.000000 bdsim-1.1.1/tests/test_spatial.py
+-rw-rw----   0 corkep     (503) staff       (20)     3659 2023-01-22 08:44:29.000000 bdsim-1.1.1/tests/test_transfers.py
```

### Comparing `bdsim-1.1.0/LICENSE` & `bdsim-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/PKG-INFO` & `bdsim-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdsim
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simulate dynamic systems expressed in block diagram form using Python
 Author-email: Peter Corke <rvc@petercorke.com>
 License: MIT License
         
         Copyright (c) 2020 Peter Corke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bdsim Version: 1.1.0 Summary: Simulate dynamic
+Metadata-Version: 2.1 Name: bdsim Version: 1.1.1 Summary: Simulate dynamic
 systems expressed in block diagram form using Python Author-email: Peter Corke
 petercorke.com> License: MIT License Copyright (c) 2020 Peter Corke Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `bdsim-1.1.0/README.md` & `bdsim-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/Icons.py` & `bdsim-1.1.1/bdsim/bdedit/Icons.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/__init__.py` & `bdsim-1.1.1/bdsim/bdedit/__init__.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/bdedit.py` & `bdsim-1.1.1/bdsim/bdedit/bdedit.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block.py` & `bdsim-1.1.1/bdsim/bdedit/block.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block_connector_block.py` & `bdsim-1.1.1/bdsim/bdedit/block_connector_block.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block_graphics_block.py` & `bdsim-1.1.1/bdsim/bdedit/block_graphics_block.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block_graphics_socket.py` & `bdsim-1.1.1/bdsim/bdedit/block_graphics_socket.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block_graphics_wire.py` & `bdsim-1.1.1/bdsim/bdedit/block_graphics_wire.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block_importer.py` & `bdsim-1.1.1/bdsim/bdedit/block_importer.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block_main_block.py` & `bdsim-1.1.1/bdsim/bdedit/block_main_block.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block_param_window.py` & `bdsim-1.1.1/bdsim/bdedit/block_param_window.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block_socket.py` & `bdsim-1.1.1/bdsim/bdedit/block_socket.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/block_wire.py` & `bdsim-1.1.1/bdsim/bdedit/block_wire.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/floating_label.py` & `bdsim-1.1.1/bdsim/bdedit/floating_label.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/floating_label_graphics.py` & `bdsim-1.1.1/bdsim/bdedit/floating_label_graphics.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/grouping_box.py` & `bdsim-1.1.1/bdsim/bdedit/grouping_box.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/grouping_box_graphics.py` & `bdsim-1.1.1/bdsim/bdedit/grouping_box_graphics.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/interface.py` & `bdsim-1.1.1/bdsim/bdedit/interface.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/interface_graphics_scene.py` & `bdsim-1.1.1/bdsim/bdedit/interface_graphics_scene.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/interface_graphics_view.py` & `bdsim-1.1.1/bdsim/bdedit/interface_graphics_view.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/interface_manager.py` & `bdsim-1.1.1/bdsim/bdedit/interface_manager.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/interface_scene.py` & `bdsim-1.1.1/bdsim/bdedit/interface_scene.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/interface_scene_history.py` & `bdsim-1.1.1/bdsim/bdedit/interface_scene_history.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdedit/interface_serialize.py` & `bdsim-1.1.1/bdsim/bdedit/interface_serialize.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/bdrun.py` & `bdsim-1.1.1/bdsim/bdrun.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blockdiagram.py` & `bdsim-1.1.1/bdsim/blockdiagram.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/connections.py` & `bdsim-1.1.1/bdsim/blocks/connections.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/discrete.py` & `bdsim-1.1.1/bdsim/blocks/discrete.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/displays.py` & `bdsim-1.1.1/bdsim/blocks/displays.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/functions.py` & `bdsim-1.1.1/bdsim/blocks/functions.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/io.py` & `bdsim-1.1.1/bdsim/blocks/io.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/linalg.py` & `bdsim-1.1.1/bdsim/blocks/linalg.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/sinks.py` & `bdsim-1.1.1/bdsim/blocks/sinks.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/sources.py` & `bdsim-1.1.1/bdsim/blocks/sources.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/spatial.py` & `bdsim-1.1.1/bdsim/blocks/spatial.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/blocks/transfers.py` & `bdsim-1.1.1/bdsim/blocks/transfers.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/components.py` & `bdsim-1.1.1/bdsim/components.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/graphics.py` & `bdsim-1.1.1/bdsim/graphics.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/newplots.py` & `bdsim-1.1.1/bdsim/newplots.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/run_realtime.py` & `bdsim-1.1.1/bdsim/run_realtime.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/run_sim.py` & `bdsim-1.1.1/bdsim/run_sim.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim/tex2icon.py` & `bdsim-1.1.1/bdsim/tex2icon.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/bdsim.egg-info/PKG-INFO` & `bdsim-1.1.1/bdsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdsim
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simulate dynamic systems expressed in block diagram form using Python
 Author-email: Peter Corke <rvc@petercorke.com>
 License: MIT License
         
         Copyright (c) 2020 Peter Corke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bdsim Version: 1.1.0 Summary: Simulate dynamic
+Metadata-Version: 2.1 Name: bdsim Version: 1.1.1 Summary: Simulate dynamic
 systems expressed in block diagram form using Python Author-email: Peter Corke
 petercorke.com> License: MIT License Copyright (c) 2020 Peter Corke Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `bdsim-1.1.0/bdsim.egg-info/SOURCES.txt` & `bdsim-1.1.1/bdsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/pyproject.toml` & `bdsim-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [project]
 name = "bdsim"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Peter Corke", email="rvc@petercorke.com" },
 ]
 
 dependencies = [
     "numpy>=1.17.4",
     "scipy", 
     "matplotlib", 
     "spatialmath-python",
     "ansitable",
     "progress",
-    "PyQt5",
 ]
 license = { file = "LICENSE" }
 
 description = "Simulate dynamic systems expressed in block diagram form using Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `bdsim-1.1.0/tests/test_bdsim.py` & `bdsim-1.1.1/tests/test_bdsim.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_blockdiagram.py` & `bdsim-1.1.1/tests/test_blockdiagram.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_components.py` & `bdsim-1.1.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_connections.py` & `bdsim-1.1.1/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_discrete.py` & `bdsim-1.1.1/tests/test_discrete.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_functions.py` & `bdsim-1.1.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_linalg.py` & `bdsim-1.1.1/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_sinks.py` & `bdsim-1.1.1/tests/test_sinks.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_sources.py` & `bdsim-1.1.1/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_spatial.py` & `bdsim-1.1.1/tests/test_spatial.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.1.0/tests/test_transfers.py` & `bdsim-1.1.1/tests/test_transfers.py`

 * *Files identical despite different names*

