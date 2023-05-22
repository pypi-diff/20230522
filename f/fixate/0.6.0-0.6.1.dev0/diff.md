# Comparing `tmp/fixate-0.6.0.tar.gz` & `tmp/fixate-0.6.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixate-0.6.0.tar", last modified: Sat Oct 22 02:14:04 2022, max compression
+gzip compressed data, was "fixate-0.6.1.dev0.tar", last modified: Mon May 22 01:16:37 2023, max compression
```

## Comparing `fixate-0.6.0.tar` & `fixate-0.6.1.dev0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.969425 fixate-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 02:13:53.000000 fixate-0.6.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-10-22 02:13:53.000000 fixate-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2022-10-22 02:14:04.969425 fixate-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2022-10-22 02:13:53.000000 fixate-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-22 02:13:53.000000 fixate-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-10-22 02:14:04.969425 fixate-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.961425 fixate-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.961425 fixate-0.6.0/src/fixate/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13363 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.961425 fixate-0.6.0/src/fixate/config/
--rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/config/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.965425 fixate-0.6.0/src/fixate/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6272 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/core/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)    13721 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/core/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    15292 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/core/config_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4924 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/core/control.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    26866 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/core/jig_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     7672 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/core/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.965425 fixate-0.6.0/src/fixate/drivers/
--rw-r--r--   0 runner    (1001) docker     (121)     6518 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.965425 fixate-0.6.0/src/fixate/drivers/daq/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21977 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/daq/daqmx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.965425 fixate-0.6.0/src/fixate/drivers/dmm/
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/dmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12095 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/dmm/fluke_8846a.py
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/dmm/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.965425 fixate-0.6.0/src/fixate/drivers/dso/
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/dso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    37958 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/dso/agilent_mso_x.py
--rw-r--r--   0 runner    (1001) docker     (121)    22955 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/dso/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    13555 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/ftdi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.965425 fixate-0.6.0/src/fixate/drivers/funcgen/
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/funcgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25449 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/funcgen/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    18360 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/funcgen/keysight_33500b.py
--rw-r--r--   0 runner    (1001) docker     (121)    26615 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/funcgen/rigol_dg1022.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.965425 fixate-0.6.0/src/fixate/drivers/lcr/
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/lcr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7721 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/lcr/agilent_u1732c.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/lcr/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.965425 fixate-0.6.0/src/fixate/drivers/pps/
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/pps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11885 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/pps/bk_178x.py
--rw-r--r--   0 runner    (1001) docker     (121)     5555 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/pps/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    10859 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/drivers/pps/siglent_spd_3303X.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.969425 fixate-0.6.0/src/fixate/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/examples/function_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5311 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/examples/multi_level_design.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/examples/programmable_power_supply.py
--rw-r--r--   0 runner    (1001) docker     (121)     8389 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/examples/test_script.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/examples/tiny.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/examples/tiny_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/examples/tiny_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.969425 fixate-0.6.0/src/fixate/reporting/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14236 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/reporting/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)    13939 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/sequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.969425 fixate-0.6.0/src/fixate/ui_cmdline/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/ui_cmdline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14144 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/ui_cmdline/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/ui_cmdline/kbhit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.969425 fixate-0.6.0/src/fixate/ui_gui_qt/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/ui_gui_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25114 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/ui_gui_qt/layout.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/ui_gui_qt/subclassed_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    41970 2022-10-22 02:13:53.000000 fixate-0.6.0/src/fixate/ui_gui_qt/ui_gui_qt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.961425 fixate-0.6.0/src/fixate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2022-10-22 02:14:04.000000 fixate-0.6.0/src/fixate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-10-22 02:14:04.000000 fixate-0.6.0/src/fixate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-22 02:14:04.000000 fixate-0.6.0/src/fixate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-22 02:14:04.000000 fixate-0.6.0/src/fixate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-22 02:14:04.000000 fixate-0.6.0/src/fixate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-22 02:14:04.000000 fixate-0.6.0/src/fixate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-22 02:14:04.000000 fixate-0.6.0/src/fixate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 02:14:04.969425 fixate-0.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-10-22 02:13:53.000000 fixate-0.6.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.344973 fixate-0.6.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-22 01:16:37.344973 fixate-0.6.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-22 01:16:37.344973 fixate-0.6.1.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.312971 fixate-0.6.1.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.320972 fixate-0.6.1.dev0/src/fixate/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14402 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.324972 fixate-0.6.1.dev0/src/fixate/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/config/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.328972 fixate-0.6.1.dev0/src/fixate/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/config_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26866 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/jig_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.328972 fixate-0.6.1.dev0/src/fixate/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.328972 fixate-0.6.1.dev0/src/fixate/drivers/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/daq/daqmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.328972 fixate-0.6.1.dev0/src/fixate/drivers/dmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dmm/fluke_8846a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dmm/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dmm/keithley_6500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.332973 fixate-0.6.1.dev0/src/fixate/drivers/dso/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37958 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dso/agilent_mso_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dso/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/ftdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.332973 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25449 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/keysight_33500b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26615 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/rigol_dg1022.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.332973 fixate-0.6.1.dev0/src/fixate/drivers/lcr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/lcr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/lcr/agilent_u1732c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/lcr/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.336973 fixate-0.6.1.dev0/src/fixate/drivers/pps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/pps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/pps/bk_178x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/pps/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/pps/siglent_spd_3303X.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/src/fixate/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/function_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/multi_level_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/programmable_power_supply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/tiny_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/tiny_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/src/fixate/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/reporting/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/src/fixate/ui_cmdline/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_cmdline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_cmdline/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_cmdline/kbhit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25114 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/subclassed_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38562 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/ui_gui_qt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.324972 fixate-0.6.1.dev0/src/fixate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/test/test_config.py
```

### Comparing `fixate-0.6.0/LICENSE.txt` & `fixate-0.6.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/PKG-INFO` & `fixate-0.6.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixate
-Version: 0.6.0
+Version: 0.6.1.dev0
 Summary: Framework for hardware test fixtures and automated test environments
 Home-page: http://pyfixate.com/
 Author: Ryan Parry-Jones
 Author-email: ryanspj+github@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fixate-0.6.0/README.md` & `fixate-0.6.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/setup.cfg` & `fixate-0.6.1.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/__main__.py` & `fixate-0.6.1.dev0/src/fixate/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 import logging
 import logging.handlers
 import os
 import sys
+from enum import Enum
 from argparse import ArgumentParser, RawTextHelpFormatter
 from functools import partial
 from importlib.machinery import SourceFileLoader
 from zipimport import zipimporter
 from pubsub import pub
 import fixate.config
 from fixate.core.exceptions import SequenceAbort
-from fixate.core.ui import user_serial, user_ok
+from fixate.core.ui import user_info_important, user_serial, user_ok
 from fixate.reporting import register_csv, unregister_csv
 from fixate.ui_cmdline import register_cmd_line, unregister_cmd_line
 import fixate.sequencer
 
 parser = ArgumentParser(
     description="""
 Fixate Command Line Interface
 
 """,
     formatter_class=RawTextHelpFormatter,
 )
 
 logger = logging.getLogger(__name__)
 
+
+class ReturnCodes(int, Enum):
+    """Fixate Return codes"""
+
+    PASS = 5
+    FAIL = 10
+    ABORTED = 11
+    ERROR = 12
+
+
 # Optional Arguments
 mutex_group = parser.add_mutually_exclusive_group()
 mutex_group.add_argument(
     "-p",
     "--path",
     help="""Path to the directory where the script file is located. 
                          This is mutually exclusive with --zip""",
@@ -106,15 +117,15 @@
     help="The sequencer will not prompt for retries.",
 )
 parser.add_argument(
     "--disable-logs", action="store_true", help="Turn off diagnostic logs"
 )
 
 
-def load_test_suite(script_path, zip_path, zip_selector):
+def load_test_suite(script_path: str, zip_path: str, zip_selector: str):
     """
     Attempts to load a Fixate Script file from an absolute path.
     Try loading from zip, then direct script otherwise
     :param script_path:
     :param zip_path:
     :param zip_selector:
     :return:
@@ -208,15 +219,15 @@
             )
 
     def run_fixate(self):
         return self.controller.fixate_exec()
 
 
 class FixateWorker:
-    def __init__(self, sequencer, test_script_path, args):
+    def __init__(self, sequencer: fixate.sequencer.Sequencer, test_script_path, args):
         self.sequencer = sequencer
         self.test_script_path = test_script_path
         self.args = args
         self.start = False
         self.clean = False
         self.config = None
 
@@ -232,34 +243,42 @@
     def stop(self):
         """This function is called in case of unusual termination, and runs in the main thread"""
         self.sequencer._handle_sequence_abort()
         pub.sendMessage(
             "Sequence_Abort", exception=SequenceAbort("Application Closing")
         )
 
-        return 11
+        return ReturnCodes.ABORTED
 
     def ui_run(self):
 
         serial_number = None
+        serial_response = None
         test_selector = None
         self.start = True
 
         try:
             # args = parser.parse_args()
             if self.args.dev:
                 fixate.config.DEBUG = True
 
             if self.args.serial_number is None:
-                serial_number = user_serial("Please enter serial number")
-                self.sequencer.context_data["serial_number"] = serial_number[1]
-                if serial_number == "ABORT_FORCE":
-                    return
+                serial_response = user_serial("Please enter serial number")
+                if serial_response == "ABORT_FORCE":
+                    return ReturnCodes.ABORTED
+                elif serial_response[0] == "Exception":
+                    # Should be tuple: ("Exception", <Exception>)
+                    raise serial_response[1]
+                else:
+                    # Should be tuple: ("Result", serial_number)
+                    serial_number = serial_response[1]
+                    self.sequencer.context_data["serial_number"] = serial_number
             else:
-                self.sequencer.context_data["serial_number"] = self.args.serial_number
+                serial_number = self.args.serial_number
+                self.sequencer.context_data["serial_number"] = serial_number
 
             if self.test_script_path is None:
                 self.test_script_path = self.args.path
 
             if self.args.non_interactive:
                 self.sequencer.non_interactive = True
 
@@ -289,30 +308,35 @@
             self.sequencer.run_sequence()
             if not self.sequencer.non_interactive:
                 user_ok("Finished testing")
 
         except BaseException:
             import traceback
 
+            user_info_important("Exception - see terminal for details")
             input(traceback.print_exc())
             raise
         finally:
             unregister_csv()
-            if serial_number == "ABORT_FORCE" or test_selector == "ABORT_FORCE":
-                return 11
+            if serial_response == "ABORT_FORCE" or test_selector == "ABORT_FORCE":
+                return ReturnCodes.ABORTED
+            if serial_number is None:
+                # Error at serial number input stage
+                return ReturnCodes.ERROR
             # Let the supervisor know that the program is finishing normally
             self.clean = True
             if self.sequencer.end_status == "FAILED":
-                return 10
+                return ReturnCodes.FAIL
             elif self.sequencer.status == "Aborted":
-                return 11
-            elif self.sequencer.end_status == "ERROR":
-                return 12
+                return ReturnCodes.ABORTED
+            elif self.sequencer.end_status == "PASSED":
+                return ReturnCodes.PASS
             else:
-                return 5
+                # Default to Error
+                return ReturnCodes.ERROR
 
 
 def retrieve_test_data(test_suite, index):
     """
     Tries to retrieve test data from the loaded test_suite module
     :param test_suite: Imported module with tests available
     :param index: index of test_data for getting the sequence
@@ -374,14 +398,15 @@
         )
         root_logger = logging.getLogger()
         root_logger.addHandler(handler)
         root_logger.setLevel(logging.DEBUG)
 
     fixate.config.load_config(args.config)
     fixate.config.load_dict_config({"log_file": args.log_file})
+    # Could this be replaced with a simple log_file variable in fixate.config ^ ?
     supervisor = FixateSupervisor(test_script_path, args)
     exit(supervisor.run_fixate())
 
 
 # Setup configuration
 if __name__ == "__main__":
     run_main_program()
```

### Comparing `fixate-0.6.0/src/fixate/config/__init__.py` & `fixate-0.6.1.dev0/src/fixate/config/__init__.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/config/helper.py` & `fixate-0.6.1.dev0/src/fixate/config/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/core/common.py` & `fixate-0.6.1.dev0/src/fixate/core/common.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/core/config_util.py` & `fixate-0.6.1.dev0/src/fixate/core/config_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,14 @@
     the result of the idn command as a string.
     :param visa_resource_name:
     :return:
     """
     instr = pyvisa.ResourceManager().open_resource(visa_resource_name, query_delay=0.1)
     # 1 s timeout is overly conservative. But if we call clear() that can take a while for some instruments
     instr.timeout = 1000
-    # instr.clear()
     resp = instr.query("*IDN?")
 
     if resp:
         instr.close()
         return resp.strip()
 
     # At least one instrument (Siglent SPD3303X power supply) only responds
```

### Comparing `fixate-0.6.0/src/fixate/core/control.py` & `fixate-0.6.1.dev0/src/fixate/core/control.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/core/exceptions.py` & `fixate-0.6.1.dev0/src/fixate/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/core/jig_mapping.py` & `fixate-0.6.1.dev0/src/fixate/core/jig_mapping.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/core/ui.py` & `fixate-0.6.1.dev0/src/fixate/core/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         user response
     """
     # TODO - fix validation, bring it all into one method?? or move validation into target function for consistency
     return _user_req_input(msg)
 
 
 def _float_validate(entry):
+    """Requires float entry"""
     try:
         return float(entry)
     except ValueError:
         user_info("Please enter a number")
         return False
 
 
@@ -204,14 +205,15 @@
         for choice in choices:
             if choice.startswith(response.upper()):
                 return choice
     return False
 
 
 def _ten_digit_serial(response):
+    """Requires 10-digit integer"""
     return (len(response) == 10) and int(response)
 
 
 def user_serial(msg, target=_ten_digit_serial, attempts=5):
     serial = _user_req_input(msg, attempts=attempts, target=target)
     return serial
```

### Comparing `fixate-0.6.0/src/fixate/drivers/__init__.py` & `fixate-0.6.1.dev0/src/fixate/drivers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 import pubsub.pub
 
 
 class InstrumentNotFoundError(Exception):
     pass
 
 
+class InstrumentOpenError(Exception):
+    pass
+
+
 class DriverProtocol(Protocol):
     REGEX_ID: str
 
     def get_identity(self) -> str:
         """Query the instrument for it identity.
 
         For visa instruments, this is generally the results of the idn? command.
```

### Comparing `fixate-0.6.0/src/fixate/drivers/daq/daqmx.py` & `fixate-0.6.1.dev0/src/fixate/drivers/daq/daqmx.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/drivers/dmm/__init__.py` & `fixate-0.6.1.dev0/src/fixate/drivers/lcr/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """
-dmm is the digital multimeter driver.
+lcr is the lcr meter driver.
 
-Use dmm.open to connect to a connected digital multi meter
-Functions are dictacted by the metaclass in helper.py
+Use lcr.open to connect to a connected digital multi meter
+Functions are dictated by the metaclass in helper.py
 
-dmm.measure(*mode, **mode_params)
-dmm.reset()
 """
 import pyvisa
+
 import fixate.drivers
-from fixate.drivers.dmm.helper import DMM
-from fixate.drivers.dmm.fluke_8846a import Fluke8846A
 from fixate.config import find_instrument_by_id
+from fixate.drivers import InstrumentNotFoundError, InstrumentOpenError
+from fixate.drivers.lcr.agilent_u1732c import AgilentU1732C
+from fixate.drivers.lcr.helper import LCR
 
 
-def open() -> DMM:
-    instrument = find_instrument_by_id(Fluke8846A.REGEX_ID)
+def open() -> LCR:
+    instrument = find_instrument_by_id(AgilentU1732C.REGEX_ID)
     if instrument is not None:
-        # we've found a connected instrument so open and return it
+        # We've found a configured instrument so try to open it
         rm = pyvisa.ResourceManager()
-        # open_resource could raise visa.VisaIOError?
-        driver = Fluke8846A(rm.open_resource(instrument.address))
+        try:
+            resource = rm.open_resource(instrument.address)
+        except pyvisa.VisaIOError as e:
+            raise InstrumentOpenError(
+                f"Unable to open LCR: {instrument.address}"
+            ) from e
+        # Instantiate driver with connected instrument
+        driver = AgilentU1732C(resource)
         fixate.drivers.log_instrument_open(driver)
         return driver
-    raise fixate.drivers.InstrumentNotFoundError
+    raise InstrumentNotFoundError
```

### Comparing `fixate-0.6.0/src/fixate/drivers/dmm/fluke_8846a.py` & `fixate-0.6.1.dev0/src/fixate/drivers/dmm/fluke_8846a.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,31 @@
 from threading import Lock
 from pyvisa import constants
 from fixate.core.exceptions import InstrumentError, ParameterError
 from fixate.core.common import mode_builder, deprecated
 from fixate.drivers.dmm.helper import DMM
 import time
 
-MODES = {
-    ":VOLTage": {
-        ":DC": {"[:RATio]": {}, " [{range}]": {", [{resolution}]": {}}},
-        ":AC": {" [{range}]": {", [{resolution}]": {}}},
-    },
-    ":CURRent": {
-        ":DC": {" [{range}]": {", [{resolution}]": {}}},
-        ":AC": {" [{range}]": {", [{resolution}]": {}}},
-    },
-    ":RESistance": {" [{range}]": {", [{resolution}]": {}}},
-    ":FRESistance": {" [{range}]": {", [{resolution}]": {}}},
-    ":FREQuency": {" [{range}]": {", [{resolution}]": {}}},
-    ":PERiod": {" [{range}]": {", [{resolution}]": {}}},
-    ":CAPacitance": {" [{range}]": {", [{resolution}]": {}}},
-    ":TEMPerature": {":FRTD": {" [{RTD_type}]": {}}, ":RTD": {" [{RTD_type}]": {}}},
-    ":CONTinuity": {},
-    ":DIODe": {" [{low_current}]": {", [{high_voltage}]": {}}},
-}
-
-FILTERS = {
-    "[SENSe:VOLTage]": {
-        "[:DC]:FILTer:STATe ON; VOLTage:DC:FILTEr:DIGital:STATe OFF": {},
-        ":AC:BANDwidth 20": {},
-    },
-    "[SENSe:CURRent]": {
-        "[:DC]:FILTer:STATe ON; CURRent:DC:FILTEr:DIGital:STATe OFF": {},
-        ":AC:BANDwidth 20": {},
-    },
-    "[SENSe:RESistance]:FILTer:STATe ON; RESistance:FILTEr:DIGital:STATe OFF": {},
-    "[SENSe:FRESistance]:FILTer:STATe ON; FRESistance:FILTEr:DIGital:STATe OFF": {},
-}
-
 
 class Fluke8846A(DMM):
     REGEX_ID = "FLUKE,8846A"
     INSTR_TYPE = "VISA"
 
     def __init__(self, instrument, *args, **kwargs):
         self.instrument = instrument
         instrument.rtscts = 1
         self.lock = Lock()
         self.display = "on"
-        # del self.instrument.timeout
         self.instrument.timeout = 10000
-        self.instrument.query_delay = 0
+        self.instrument.query_delay = 0  # Delay between write and read in a query
         self.instrument.delay = 0
         self.is_connected = True
         self.reset()
+        self._manual_trigger = False
         self._samples = 1
-        self._CLEAN_UP_FLAG = False
-        self._ANALOG_FLAG = False
-        self._DIGITAL_FLAG = False
         self._range_string = ""
         self._bandwidth = None
         self._mode = None
         # Set to True to have explicit error checks on each read
         self.legacy_mode = False
         self._modes = {
             "voltage_ac": "CONF:VOLTage:AC",
@@ -101,18 +66,44 @@
 
     @property
     def samples(self):
         return self._samples
 
     @samples.setter
     def samples(self, val):
-        self._write(["SAMP:COUN {}".format(self.samples)])
+        self._write(f"SAMP:COUN {val}")
         self._is_error()
         self._samples = val
 
+    def local(self):
+        self._write("SYST:LOC")
+
+    def remote(self):
+        self._write("SYST:REM")
+
+    def set_manual_trigger(self, samples=1):
+        MAX_TRIGGER_COUNT = 5000
+        self._manual_trigger = True
+        self.samples = samples
+        # set DMM to remote trigger
+        self._write("TRIG:SOUR BUS")
+        # Set number of samples to maximum:
+        self._write(f"TRIG:COUN {int(MAX_TRIGGER_COUNT/samples)}")
+        self._write("INIT")  # Wait for trigger
+        self._is_error()  # Catch possible insufficient memory error (and others)
+
+    def trigger(self):
+        """
+        Manually trigger a measurement and store in instrument buffer.
+        """
+        if self._manual_trigger == False:
+            raise InstrumentError("Manual trigger mode not set.")
+        self._write("*TRG")  # Send trigger to instrument
+        self._is_error()  # Catch errors. This might slow things down
+
     def measurement(self):
         """
         Sets up DMM triggering, creates list of measurements from the read buffer
         returns: a single value as a float
         """
         return self.measurements()[0]
 
@@ -125,16 +116,15 @@
 
     def reset(self):
         """
         Checks for errors and then returns DMM to power up state
         """
         with self.lock:
             self._is_error(silent=True)
-            self._write(["*rst", "SYST:REM", "*cls", "disp {}".format(self.display)])
-            self._CLEAN_UP_FLAG = False
+            self._write(["*rst", "SYST:REM", "*cls", f"disp {self.display}"])
             self._is_error()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.instrument.close()
@@ -144,32 +134,41 @@
         """
         Writes data to the DMM
         raise: ParameterError if called with no data string
         """
         if data:
             if isinstance(data, str):
                 self.instrument.write(data)
-                time.sleep(0.05)
-            else:
+                time.sleep(0.05)  # Sleep to stop DMM crashes
+            elif isinstance(data, list) and all([isinstance(itm, str) for itm in data]):
                 for itm in data:
                     self.instrument.write(itm)
-                time.sleep(0.05)
+                    time.sleep(0.05)  # Sleep to stop DMM crashes
+            else:
+                raise ParameterError("Invalid data to send to instrument")
         else:
             raise ParameterError("Missing data in instrument write")
 
     def _read_measurements(self):
         """
         Attempts to read values from the DMM up until self.retrys_on_timeout amount of times
         After each attempt DMM is checked for errors
         If errors.VisaIOError during read error_cleanup is called
         raise: VisaIOError if exception on the last attempt
                ValueError if no values are read
         return: values read from the DMM
         """
-        values = self.instrument.query_ascii_values("READ?")
+        if self._manual_trigger:
+            values = self.instrument.query_ascii_values("FETCH?")
+            # Reset for next set of measurements (clear buffer).
+            # Fluke does not allow you to manually clear the buffer, so this roundabout way is used instead
+            self.set_manual_trigger(samples=self.samples)
+        else:
+            values = self.instrument.query_ascii_values("READ?")
+
         if self.legacy_mode:
             self._is_error()
         return values
 
     def _check_errors(self):
         """
         Queries the DMM for errors and splits the resp string into the message and error code
@@ -201,98 +200,97 @@
         if errors:
             if silent:
                 return errors
             else:
                 raise InstrumentError(
                     "Error(s) Returned from DMM\n"
                     + "\n".join(
-                        [
-                            "Code: {}\nMessage:{}".format(code, msg)
-                            for code, msg in errors
-                        ]
+                        [f"Code: {code}\nMessage:{msg}" for code, msg in errors]
                     )
                 )
 
-    def error_cleanup(self):
-        """
-        When VisaIOError exception caught, DMM interrupt is sent, read buffer is cleared and DMM returned to power up
-        state.  VI read buffer is then flushed.
-        DMM is then returned to previous configuration
-        """
-        self._CLEAN_UP_FLAG = True
-        # Disaster Recovery
-        self.instrument.write("\x03;*RST;*CLS")  # CTRL-C
-        time.sleep(1.1)  # time needed to clear the dmm read buffer
-        self.instrument.flush(constants.VI_READ_BUF_DISCARD)
-        self.instrument.close()
-        self.instrument.open()
-
     def _set_measurement_mode(self, mode, _range=None, suffix=None):
         """
         Helper function used to set the measurement mode for voltage_ac, voltage_dc, current_ac, current_dc,
         resistance, fresistance. Reduces previous duplicate code.
         :param mode:
         :param _range:
         :param _resolution:
         :return:
         """
         self.mode = mode
-        mode_str = "{}".format(self._modes[self._mode])
+        self._manual_trigger = False  # Default mode is auto trigger
+        mode_str = f"{self._modes[self._mode]}"
         if _range is not None:
-            mode_str += " {}".format(_range)
+            mode_str += f" {_range}"
         if suffix is not None:
-            mode_str += " {}".format(suffix)
+            mode_str += f" {suffix}"
         self._write(mode_str)
         self._write(
             [
                 "SYST:REM",
                 "TRIG:DEL:AUTO ON",
                 "TRIG:SOUR IMM",
                 "TRIG:COUN 1",
-                "SAMP:COUN {}".format(self.samples),
+                f"SAMP:COUN {self.samples}",
             ]
         )
         self._is_error()
 
     def voltage_ac(self, _range=None):
         self._set_measurement_mode("voltage_ac", _range)
 
-    def voltage_dc(self, _range=None):
-        self._set_measurement_mode("voltage_dc", _range)
+    def voltage_dc(self, _range=None, auto_impedance=False):
+        # Auto impedance OFF is the default mode.
+        if auto_impedance == True:
+            command = "; :SENS:VOLT:DC:IMP:AUTO ON"
+        else:
+            command = "; :SENS:VOLT:DC:IMP:AUTO OFF"
+        self._set_measurement_mode("voltage_dc", _range, suffix=command)
 
     def current_ac(self, _range=None):
         self._set_measurement_mode("current_ac", _range)
 
     def current_dc(self, _range=None):
         self._set_measurement_mode("current_dc", _range)
 
     def resistance(self, _range=None):
         self._set_measurement_mode("resistance", _range)
 
     def fresistance(self, _range=None):
         self._set_measurement_mode("fresistance", _range)
 
-    def frequency(self, _range=None):
-        self._set_measurement_mode("frequency", _range)
+    def frequency(self, _range=None, _volt_range=None):
+        if _volt_range:
+            self._set_measurement_mode(
+                "frequency", _range, suffix=f" ; :SENS:FREQ:VOLT:RANG {_volt_range}"
+            )
+        else:
+            self._set_measurement_mode("frequency", _range)
 
-    def period(self, _range=None):
-        self._set_measurement_mode("period", _range)
+    def period(self, _range=None, _volt_range=None):
+        if _volt_range:
+            self._set_measurement_mode(
+                "period", _range, suffix=f" ; :SENS:PER:VOLT:RANG {_volt_range}"
+            )
+        else:
+            self._set_measurement_mode("period", _range)
 
     def capacitance(self, _range=None):
         self._set_measurement_mode("capacitance", _range)
 
     def diode(self, low_current=True, high_voltage=False):
         """
         Writes configuration string for diode to the DMM
         param _range: value set for the range
         param _resolution: value set for the resolution
         """
         self._set_measurement_mode(
             "diode",
-            suffix="{}, {}".format(int(bool(low_current)), int(bool(high_voltage))),
+            suffix=f"{int(bool(low_current))}, {int(bool(high_voltage))}",
         )
 
     def continuity(self):
         """
         Writes configuration string for continuity to the DMM
         param _range: value set for the range
         param _resolution: value set for the resolution
@@ -307,45 +305,19 @@
     def mode(self, value):
         """
         Creates the variable to set the mode configuration of the DMM
         param value: The string associated with the mode being set up
         raise: ParameterError if mode trying to be set is not valid
         """
         self._write("*rst")
-        time.sleep(0.05)
         # do we need to set the default filter here?
         if value not in self._modes:
-            raise ParameterError("Unknown mode {} for DMM".format(value))
+            raise ParameterError(f"Unknown mode {value} for DMM")
         self._mode = value
 
-    def digital_filter(self):
-        """
-        Sets up DMM digital filtering
-        raise: TypeError if trying to set digital filter in an AC mode
-        """
-        if "ac" in self._mode:
-            raise TypeError
-        self._write(self._filters[self.mode] + ":FILT:DIG:STAT ON")
-
-    def analog_filter(self, bandwidth=None):
-        """
-        Sets up DMM analog filtering.  Writes the different filter strings depending on the configuration mode.  Hence,
-        configuration must be set before calling filter.
-        raise: ValueError if invalid filtering bandwidth is requested
-        """
-        if "ac" in self._mode:
-            self._bandwidth = bandwidth or 20
-            if self._bandwidth not in [3, 20, 200]:
-                raise ValueError("Bandwidth must be 3, 20 or 200")
-            self._write(self._filters[self.mode] + ":BAND {}".format(self._bandwidth))
-
-        elif any(x in self._mode for x in ["dc", "res"]):
-            self._write(self._filters[self.mode] + ":FILT:STAT ON")
-        pass
-
     def get_identity(self) -> str:
         """
         Meter returns the identification code of the meter as four fields separated by commas.
         These fields are:
             manufacturer ("FLUKE"); model (“45"); seven-digit serial number;
             version of main software and version of display software.
         :return:
```

### Comparing `fixate-0.6.0/src/fixate/drivers/dmm/helper.py` & `fixate-0.6.1.dev0/src/fixate/drivers/dmm/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,52 @@
 class DMM:
     REGEX_ID = "DMM"
     is_connected = False
 
+    def remote(self):
+        """
+        Sets instrument to remote mode
+        """
+        raise NotImplementedError
+
+    def local(self):
+        """
+        Sets instrument to local mode
+        Use remote() to restore remote operation.
+        """
+        raise NotImplementedError
+
+    def set_manual_trigger(self, samples=1):
+        """
+        Setup instrument for manual triggering.
+        :param samples: Number of samples to take per trigger event
+        """
+        raise NotImplementedError
+
+    def trigger(self):
+        """
+        Manually trigger measurement and store in instrument buffer.
+        """
+        raise NotImplementedError
+
     def measurement(self):
         raise NotImplementedError
 
     def voltage_ac(self, _range=None):
         raise NotImplementedError
 
-    def voltage_dc(self, _range=None):
+    def voltage_dc(self, _range=None, auto_impedance=False):
         raise NotImplementedError
 
     def current_ac(self, _range):
         raise NotImplementedError
 
     def current_dc(self, _range):
         raise NotImplementedError
 
-    def analog_filter(self, bandwidth=None):
-        raise NotImplementedError
-
-    def digital_filter(self):
-        raise NotImplementedError
-
     def resistance(self, _range=None):
         raise NotImplementedError
 
     def frequency(self, _range=None):
         raise NotImplementedError
 
     def fresistance(self, _range=None):
@@ -34,20 +54,14 @@
 
     def period(self, _range=None):
         raise NotImplementedError
 
     def capacitance(self, _range=None):
         raise NotImplementedError
 
-    def temperature(self):
-        raise NotImplementedError
-
-    def ftemperature(self):
-        raise NotImplementedError
-
     def continuity(self):
         raise NotImplementedError
 
     def diode(self, low_current=True, high_voltage=False):
         raise NotImplementedError
 
     def reset(self):
```

### Comparing `fixate-0.6.0/src/fixate/drivers/dso/__init__.py` & `fixate-0.6.1.dev0/src/fixate/drivers/dso/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import pyvisa
+
 import fixate.drivers
-from fixate.drivers.dso.helper import DSO
-from fixate.drivers.dso.agilent_mso_x import MSO_X_3000
 from fixate.config import find_instrument_by_id
+from fixate.drivers import InstrumentNotFoundError, InstrumentOpenError
+from fixate.drivers.dso.agilent_mso_x import MSO_X_3000
+from fixate.drivers.dso.helper import DSO
 
 
 def open() -> DSO:
     instrument = find_instrument_by_id(MSO_X_3000.REGEX_ID)
     if instrument is not None:
-        # we've found a connected instrument so open and return it
+        # We've found a configured instrument so try to open it
         rm = pyvisa.ResourceManager()
-        # open_resource could raise visa.VisaIOError?
-        driver = MSO_X_3000(rm.open_resource(instrument.address))
+        try:
+            resource = rm.open_resource(instrument.address)
+        except pyvisa.VisaIOError as e:
+            raise InstrumentOpenError(
+                f"Unable to open DSO: {instrument.address}"
+            ) from e
+        # Instantiate driver with connected instrument
+        driver = MSO_X_3000(resource)
         fixate.drivers.log_instrument_open(driver)
         return driver
-    raise fixate.drivers.InstrumentNotFoundError
+    raise InstrumentNotFoundError
```

### Comparing `fixate-0.6.0/src/fixate/drivers/dso/agilent_mso_x.py` & `fixate-0.6.1.dev0/src/fixate/drivers/dso/agilent_mso_x.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/drivers/dso/helper.py` & `fixate-0.6.1.dev0/src/fixate/drivers/dso/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/drivers/ftdi.py` & `fixate-0.6.1.dev0/src/fixate/drivers/ftdi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 import ctypes
 import struct
 import time
 import os
+import re
+
+import fixate.drivers
 from fixate.core.common import bits
 from fixate.core.exceptions import InstrumentNotConnected
 
 
-def open(ftdi_description=""):
-    create_device_info_list()
-
-    for dev in get_device_info_list():
-        if ftdi_description.encode() == dev.Description or ftdi_description == "":
-            return FTDI2xx(dev.Description)
-    raise InstrumentNotConnected(
-        "No valid ftdi found by description '{}'".format(ftdi_description)
-    )
-
-
 # Definitions
 UCHAR = ctypes.c_ubyte
 PCHAR = ctypes.POINTER(ctypes.c_char)
 PUCHAR = ctypes.POINTER(ctypes.c_ubyte)
 DWORD = ctypes.c_ulong
 LPDWORD = ctypes.POINTER(ctypes.c_ulong)
 if struct.calcsize("P") == 8:  # 64 bit
@@ -121,15 +113,15 @@
 
 
 if os.name == "nt":
     try:
         ftdI2xx = ctypes.WinDLL("FTD2XX.dll")
     except Exception as e:
         raise ImportError(
-            "Unable to find FTD2XX.dll.\nPlugging in FDTI device will install DLL."
+            "Unable to find FTD2XX.dll.\nPlugging in an FTDI device will install the DLL."
         ) from e
 else:
     try:
         ftdI2xx = ctypes.cdll.LoadLibrary("/usr/local/lib/libftd2xx.so")
     except Exception as e:
         raise ImportError(
             "Unable to find libftd2xx.so.\nInstall as per https://www.ftdichip.com/Drivers/D2XX/Linux/ReadMe-linux.txt"
@@ -446,7 +438,28 @@
                 # Clock Up
                 data_out.append(bb_mask + self.bb_clk ^ self.bb_inv_mask)
         # Latch to output
         data_out.append(bb_mask + self.bb_inv_mask)
         data_out.append(bb_mask + self.bb_latch ^ self.bb_inv_mask)
         data_out.append(bb_mask + self.bb_inv_mask)
         return data_out
+
+    def get_identity(self) -> str:
+        """Return identity string representing connected ftdi object"""
+        return self.ftdi_description.decode()
+
+
+def open(ftdi_description="") -> FTDI2xx:
+    """Open FTDI Driver"""
+    create_device_info_list()
+
+    for dev in get_device_info_list():
+        if (
+            re.fullmatch(ftdi_description, dev.Description.decode())
+            or ftdi_description == ""
+        ):
+            driver = FTDI2xx(dev.Description)
+            fixate.drivers.log_instrument_open(driver)
+            return driver
+    raise InstrumentNotConnected(
+        f"No valid ftdi found by description '{ftdi_description}'"
+    )
```

### Comparing `fixate-0.6.0/src/fixate/drivers/funcgen/__init__.py` & `fixate-0.6.1.dev0/src/fixate/drivers/funcgen/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,33 +19,38 @@
 properties:
 output_ch1
 output_ch2
 output_ch3
 output_ch4
 """
 import pyvisa
+
 import fixate.drivers
 from fixate.config import find_instrument_by_id
-
+from fixate.drivers import InstrumentNotFoundError, InstrumentOpenError
 from fixate.drivers.funcgen.helper import FuncGen
-
-from fixate.drivers.funcgen.rigol_dg1022 import RigolDG1022
 from fixate.drivers.funcgen.keysight_33500b import Keysight33500B
+from fixate.drivers.funcgen.rigol_dg1022 import RigolDG1022
 
 
 def open() -> FuncGen:
     """Open is the public api for the dmm driver for discovering and opening a connection
     to a valid Digital Multimeter
     :return:
     A instantiated class connected to a valid funcgen
     """
     for driver_class in (Keysight33500B, RigolDG1022):
         instrument = find_instrument_by_id(driver_class.REGEX_ID)
         if instrument is not None:
-            # we've found a connected instrument so open and return it
+            # We've found a configured instrument so try to open it
             rm = pyvisa.ResourceManager()
-            # open_resource could raise visa.VisaIOError?
-            driver = driver_class(rm.open_resource(instrument.address))
+            try:
+                resource = rm.open_resource(instrument.address)
+            except pyvisa.VisaIOError as e:
+                raise InstrumentOpenError(
+                    f"Unable to open FuncGen: {instrument.address}"
+                ) from e
+            # Instantiate driver with connected instrument
+            driver = driver_class(resource)
             fixate.drivers.log_instrument_open(driver)
             return driver
-
-    raise fixate.drivers.InstrumentNotFoundError
+    raise InstrumentNotFoundError
```

### Comparing `fixate-0.6.0/src/fixate/drivers/funcgen/helper.py` & `fixate-0.6.1.dev0/src/fixate/drivers/funcgen/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/drivers/funcgen/keysight_33500b.py` & `fixate-0.6.1.dev0/src/fixate/drivers/funcgen/keysight_33500b.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/drivers/funcgen/rigol_dg1022.py` & `fixate-0.6.1.dev0/src/fixate/drivers/funcgen/rigol_dg1022.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/drivers/lcr/__init__.py` & `fixate-0.6.1.dev0/src/fixate/drivers/pps/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-"""
-lcr is the lcr meter driver.
-
-Use lcr.open to connect to a connected digital multi meter
-Functions are dictacted by the metaclass in helper.py
-
-"""
-from fixate.drivers.lcr.helper import LCR, TestResult
 import pyvisa
+
 import fixate.drivers
-from fixate.drivers.lcr.agilent_u1732c import AgilentU1732C
 from fixate.config import find_instrument_by_id
+from fixate.drivers import InstrumentNotFoundError, InstrumentOpenError
+from fixate.drivers.pps.bk_178x import BK178X
+from fixate.drivers.pps.helper import PPS
+from fixate.drivers.pps.siglent_spd_3303X import SPD3303X
 
 
-def open() -> LCR:
-    instrument = find_instrument_by_id(AgilentU1732C.REGEX_ID)
-    if instrument is not None:
-        # we've found a connected instrument so open and return it
+def open() -> PPS:
+    siglent = find_instrument_by_id(SPD3303X.REGEX_ID)
+    if siglent is not None:
+        # We've found a configured instrument so try to open it
         rm = pyvisa.ResourceManager()
-        # open_resource could raise visa.VisaIOError?
-        driver = AgilentU1732C(rm.open_resource(instrument.address))
+        try:
+            resource = rm.open_resource(siglent.address)
+        except pyvisa.VisaIOError as e:
+            raise InstrumentOpenError(f"Unable to open PPS: {siglent.address}") from e
+        # Instantiate driver with connected instrument
+        driver = SPD3303X(resource)
         fixate.drivers.log_instrument_open(driver)
         return driver
-    raise fixate.drivers.InstrumentNotFoundError
+
+    bk_precision = find_instrument_by_id(BK178X.REGEX_ID)
+    if bk_precision is not None:
+        driver = BK178X(bk_precision.address)
+        driver.baud_rate = bk_precision.parameters["baud_rate"]
+        fixate.drivers.log_instrument_open(driver)
+        return driver
+
+    raise InstrumentNotFoundError
```

### Comparing `fixate-0.6.0/src/fixate/drivers/lcr/agilent_u1732c.py` & `fixate-0.6.1.dev0/src/fixate/drivers/lcr/agilent_u1732c.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/drivers/lcr/helper.py` & `fixate-0.6.1.dev0/src/fixate/drivers/lcr/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/drivers/pps/bk_178x.py` & `fixate-0.6.1.dev0/src/fixate/drivers/pps/bk_178x.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import struct
 import serial
 
-from fixate.drivers.pps import PPS
+from fixate.drivers.pps.helper import PPS
 from fixate.core.exceptions import ParameterError
 
 """
 Communication Protocol
 Byte0   Byte1    Byte2    Byte 3-24     Byte 25
 0xAA    Address  Command  Command Data  Checksum
         !=0xFF
```

### Comparing `fixate-0.6.0/src/fixate/drivers/pps/helper.py` & `fixate-0.6.1.dev0/src/fixate/drivers/pps/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/drivers/pps/siglent_spd_3303X.py` & `fixate-0.6.1.dev0/src/fixate/drivers/pps/siglent_spd_3303X.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/examples/function_generator.py` & `fixate-0.6.1.dev0/src/fixate/examples/function_generator.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/examples/multi_level_design.py` & `fixate-0.6.1.dev0/src/fixate/examples/multi_level_design.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from fixate.core.ui import user_info
 from fixate.core.common import TestClass, TestList
 from fixate.config import RESOURCES
-import fixate
-
-__version__ = "2"
 
 # Standard expected output
 """
 1: list enter
 1: setup 1
 1: test 1
 1: teardown 1
@@ -59,16 +56,14 @@
 3: list exit
 4: setup 10
 i'm a subclass
 4: teardown 10
 : list exit
 """
 
-seq = fixate.config.RESOURCES["SEQUENCER"]
-
 
 class Test(TestClass):
     """
     Dummy Test Class
     """
 
     def set_up(self):
```

### Comparing `fixate-0.6.0/src/fixate/examples/programmable_power_supply.py` & `fixate-0.6.1.dev0/src/fixate/examples/programmable_power_supply.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/examples/test_script.py` & `fixate-0.6.1.dev0/src/fixate/examples/test_script.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/examples/tiny.py` & `fixate-0.6.1.dev0/src/fixate/examples/tiny.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/examples/tiny_images.py` & `fixate-0.6.1.dev0/src/fixate/examples/tiny_images.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/examples/tiny_variants.py` & `fixate-0.6.1.dev0/src/fixate/examples/tiny_variants.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/reporting/csv.py` & `fixate-0.6.1.dev0/src/fixate/reporting/csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 import re
 
 from pubsub import pub
 
 from queue import Queue
 from fixate.core.common import TestClass
 from fixate.core.common import ExcThread
+from fixate.core.checks import CheckResult
 import fixate
 import fixate.config
 
 
 class TestClassImp(TestClass):
     """
     Minimum implementation of the Test class so that it can be used for parameter extraction from the
@@ -110,18 +111,14 @@
         pass
 
 
 class CSVWriter:
     def __init__(self):
         self.csv_queue = Queue()
         self.csv_writer = None
-        # data = fixate.config.get_config_dict()
-        # data.update(fixate.config.get_plugin_data('plg_csv'))
-        # self.csv_dir = os.path.join(*fixate.config.render_template(data["tpl_csv_path"], **data,
-        #                                                            **fixate.config.RESOURCES["SEQUENCER"].context_data))
         self.reporting = CsvReporting()
 
     def install(self):
         self.csv_writer = ExcThread(
             target=self._csv_write, args=(self.csv_queue,), name="csv-writer"
         )
         self.csv_writer.start()
@@ -192,25 +189,23 @@
             )
 
     def sequence_complete(
         self, status, passed, failed, error, skipped, sequence_status
     ):
         self._write_line_to_csv(
             [
-                "{:.2f}".format(time.perf_counter() - self.start_time),
+                f"{(time.perf_counter() - self.start_time):.2f}",
                 "Sequence",
-                "ended={}".format(
-                    self.data["tpl_time_stamp"].format(datetime.datetime.now())
-                ),
+                f"ended={self.data['tpl_time_stamp'].format(datetime.datetime.now())}",
                 sequence_status,
-                "tests-passed={}".format(passed),
-                "tests-failed={}".format(failed),
-                "tests-error={}".format(error),
-                "tests-skipped={}".format(skipped),
-                "sequence={}".format(status.upper()),
+                f"tests-passed={passed}",
+                f"tests-failed={failed}",
+                f"tests-error={error}",
+                f"tests-skipped={skipped}",
+                f"sequence={status.upper()}",
             ]
         )
         # Close out the reporting
         self.test_module = None
 
     def test_start(self, data, test_index):
         """
@@ -220,111 +215,112 @@
          the test index in the sequencer
         """
         # Add a test record for this result that is overridden if the test is repeated
         # [0, 0, 0] -> Passed, Failed, Exception
         # Test <test_index>, start, <test name>
         self._write_line_to_csv(
             [
-                "{:.2f}".format(time.perf_counter() - self.start_time),
-                "Test {}".format(test_index),
+                f"{(time.perf_counter() - self.start_time):.2f}",
+                f"Test {test_index}",
                 "start",
                 data.test_desc,
                 data.test_desc_long,
             ]
         )
 
         test_params = self.extract_test_parameters(data)
         self.current_test = test_index
         if len(test_params):
             # Test <test_index>, test-parameters, <param_name>=<param_value>, ...
             param_line = [
-                "{:.2f}".format(time.perf_counter() - self.start_time),
-                "Test {}".format(test_index),
+                f"{(time.perf_counter() - self.start_time):.2f}",
+                f"Test {test_index}",
                 "test-parameters",
             ]
             for param_name, param_value in test_params:
-                param_line.append("{}={}".format(param_name, param_value))
+                param_line.append(f"{param_name}={param_value}")
             self._write_line_to_csv(param_line)
 
     def test_exception(self, exception, test_index):
         self.current_test = test_index
         exc_line = [
-            "{:.2f}".format(time.perf_counter() - self.start_time),
-            "Test {}".format(test_index),
+            f"{(time.perf_counter() - self.start_time):.2f}",
+            f"Test {test_index}",
             "exception",
             re.sub(r",\)", ")", repr(exception)),
         ]  # Remove trailing comma for exception for python < 3.7
         self._write_line_to_csv(exc_line)
 
-    def test_comparison(self, passes, chk, chk_cnt, context):
+    def test_comparison(
+        self, passes: bool, chk: CheckResult, chk_cnt: int, context: str
+    ):
         # pub.sendMessage("Check", passes=result, chk=chk, context=self.get_context())
-        if passes:
-            status = "PASS"
-        else:
-            status = "FAIL"
+
         # Test <test_index>, check<number>, <check type>, <status>, <test_val>, <expected>
         # If exception <test_index>, check<number>, <exception details>
         chk_line = [
-            "{:.2f}".format(time.perf_counter() - self.start_time),
-            "Test {}".format(context),
-            "check{}".format(chk_cnt),
-            chk.target.__name__[1:].replace("check_", "").replace("_", " "),
+            f"{(time.perf_counter() - self.start_time):.2f}",
+            f"Test {context}",
+            f"check{chk_cnt}",
+            chk.target_name,
             chk.description,
-            status,
+            chk.status,
             chk.test_val,
         ]
-        chk_line.extend(
-            [x for x in [chk.nominal, chk._min, chk._max, chk.tol] if x is not None]
-        )
+        chk_line.extend(chk.check_params)
+        # TODO: might be clearer to make check_params a dict and then each
+        # parameter entry as "key = value" (e.g "nominal = 55")
+        # Easier to debug without referring to scripts or checks.py?
+        # e.g. chk_line.extend([f"{k} = {v}" for k,v in chk.check_params.items()])
 
         self._write_line_to_csv(chk_line)
         self.chk_cnt += 1
 
     def test_complete(self, data, test_index, status):
         self.current_test = test_index
         try:
             sequencer = fixate.config.RESOURCES["SEQUENCER"]
             passed = sequencer.chk_pass
             failed = sequencer.chk_fail
 
             self._write_line_to_csv(
                 [
-                    "{:.2f}".format(time.perf_counter() - self.start_time),
-                    "Test {}".format(test_index),
+                    f"{(time.perf_counter() - self.start_time):.2f}",
+                    f"Test {test_index}",
                     "end",
                     status,
-                    "checks-passed={}".format(passed),
-                    "checks-failed={}".format(failed),
+                    f"checks-passed={passed}",
+                    f"checks-failed={failed}",
                 ]
             )
         finally:
             self.chk_cnt = 0
 
     def user_wait_start(self, *args, **kwargs):
         self._write_line_to_csv(
             [
-                "{:.2f}".format(time.perf_counter() - self.start_time),
-                "Test {}".format(self.current_test),
+                f"{(time.perf_counter() - self.start_time):.2f}",
+                f"Test {self.current_test}",
                 "user_wait_start",
             ]
         )
 
     def user_wait_end(self, *args, **kwargs):
         self._write_line_to_csv(
             [
-                "{:.2f}".format(time.perf_counter() - self.start_time),
-                "Test {}".format(self.current_test),
+                f"{time.perf_counter() - self.start_time:.2f}",
+                f"Test {self.current_test}",
                 "user_wait_end",
             ]
         )
 
     def driver_open(self, instr_type, identity):
         self._write_line_to_csv(
             [
-                "{:.2f}".format(time.perf_counter() - self.start_time),
+                f"{(time.perf_counter() - self.start_time):.2f}",
                 "DRIVER",
                 instr_type,
                 identity,
             ]
         )
 
     @staticmethod
@@ -382,16 +378,17 @@
 
 def unregister_csv():
     """
     Note, will disable the final result eg. Unit Passed
     :return:
     """
     global writer
-    pub.unsubscribe(writer.reporting.test_start, "Test_Start")
-    pub.unsubscribe(writer.reporting.test_comparison, "Check")
-    pub.unsubscribe(writer.reporting.test_exception, "Test_Exception")
-    pub.unsubscribe(writer.reporting.test_complete, "Test_Complete")
-    pub.unsubscribe(writer.reporting.sequence_update, "Sequence_Update")
-    pub.unsubscribe(writer.reporting.sequence_complete, "Sequence_Complete")
-    pub.unsubscribe(writer.reporting.user_wait_start, "UI_block_start")
-    pub.unsubscribe(writer.reporting.user_wait_end, "UI_block_end")
-    writer.uninstall()
+    if writer is not None:
+        pub.unsubscribe(writer.reporting.test_start, "Test_Start")
+        pub.unsubscribe(writer.reporting.test_comparison, "Check")
+        pub.unsubscribe(writer.reporting.test_exception, "Test_Exception")
+        pub.unsubscribe(writer.reporting.test_complete, "Test_Complete")
+        pub.unsubscribe(writer.reporting.sequence_update, "Sequence_Update")
+        pub.unsubscribe(writer.reporting.sequence_complete, "Sequence_Complete")
+        pub.unsubscribe(writer.reporting.user_wait_start, "UI_block_start")
+        pub.unsubscribe(writer.reporting.user_wait_end, "UI_block_end")
+        writer.uninstall()
```

### Comparing `fixate-0.6.0/src/fixate/sequencer.py` & `fixate-0.6.1.dev0/src/fixate/sequencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 import time
 import re
 from pubsub import pub
 from fixate.core.common import TestList, TestClass
 from fixate.core.exceptions import SequenceAbort, CheckFail
 from fixate.core.ui import user_retry_abort_fail
+from fixate.core.checks import CheckResult
 
 STATUS_STATES = ["Idle", "Running", "Paused", "Finished", "Restart", "Aborted"]
 
 
 class ContextStackNode:
     def __init__(self, seq):
         self.index = 0
@@ -381,24 +382,24 @@
             raise SequenceAbort("Sequence Aborted By User")
         else:
             return resp == "RETRY"
 
     def _handle_sequence_abort(self):
         self.status = "Aborted"
         self.ABORT = True
-        self.test_running = False
 
-    def check(self, chk, result):
-        if result:
+    def check(self, chk: CheckResult):
+        """Update current pass/fail counts and send check criteria to subscribers"""
+        if chk.result:
             self.chk_pass += 1
         else:
             self.chk_fail += 1
         pub.sendMessage(
             "Check",
-            passes=result,
+            passes=chk.result,
             chk=chk,
             chk_cnt=self.chk_pass + self.chk_fail,
             context=self.levels(),
         )
-        if not result:
+        if not chk.result:
             raise CheckFail("Check function returned failure, aborting test")
-        return result
+        return chk.result
```

### Comparing `fixate-0.6.0/src/fixate/ui_cmdline/cmd_line.py` & `fixate-0.6.1.dev0/src/fixate/ui_cmdline/cmd_line.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 import textwrap
 from pubsub import pub
 from fixate.ui_cmdline.kbhit import KBHit
 from queue import Queue
 from fixate.core.exceptions import UserInputError
 from fixate.core.common import ExcThread
+from fixate.core.checks import CheckResult
 from fixate.config import RESOURCES
 import fixate.config
 
 wrapper = textwrap.TextWrapper(width=75)
 wrapper.break_long_words = False
 
 wrapper.drop_whitespace = True
@@ -225,18 +226,18 @@
         if target is None:
             q.put(ret_val)
             return
         ret_val = target(ret_val, **kwargs)
         if ret_val:
             q.put(("Result", ret_val))
             return
-    q.put(
-        "Exception",
-        UserInputError("Maximum number of attempts {} reached".format(attempts)),
-    )
+    # Display failure of target and send exception
+    error_str = f"Maximum number of attempts {attempts} reached. {target.__doc__}"
+    _user_display(error_str)
+    q.put(("Exception", UserInputError(error_str)))
 
 
 def _user_display(msg):
     """
     :param msg:
     :param important: creates a line of "!" either side of the message
     :return:
@@ -327,95 +328,10 @@
     # print("Test {}: Exception Occurred, {} {}".format(test_index, type(exception), exception))
     print("!" * wrapper.width)
     # TODO print traceback into a debug log file
     if fixate.config.DEBUG:
         traceback.print_tb(exception.__traceback__, file=sys.stderr)
 
 
-def round_to_3_sig_figures(chk):
-    """
-    Tries to round elements to 3 significant figures for formatting
-    :param chk:
-    :return:
-    """
-    ret_dict = {}
-    for element in ["_min", "_max", "test_val", "nominal", "tol"]:
-        ret_dict[element] = getattr(chk, element, None)
-        try:
-            ret_dict[element] = "{:.3g}".format(ret_dict[element])
-        except:
-            pass
-    return ret_dict
-
-
-def _print_comparisons(passes, chk, chk_cnt, context):
-    if passes:
-        status = "PASS"
-    else:
-        status = "FAIL"
-    format_dict = round_to_3_sig_figures(chk)
-    if chk._min is not None and chk._max is not None:
-        print(
-            reformat_text(
-                "\nCheck {chk_cnt}: {status} when comparing {test_val} {comparison} {_min} - {_max} : "
-                "{description}".format(
-                    status=status,
-                    comparison=chk.target.__name__[1:].replace("_", " "),
-                    chk_cnt=chk_cnt,
-                    description=chk.description,
-                    **format_dict
-                )
-            )
-        )
-    elif chk.nominal is not None and chk.tol is not None:
-        print(
-            reformat_text(
-                "\nCheck {chk_cnt}: {status} when comparing {test_val} {comparison} {nominal} +- {tol}% : "
-                "{description}".format(
-                    status=status,
-                    comparison=chk.target.__name__[1:].replace("_", " "),
-                    chk_cnt=chk_cnt,
-                    description=chk.description,
-                    **format_dict
-                )
-            )
-        )
-    elif chk._min is not None or chk._max is not None or chk.nominal is not None:
-        # Grabs the first value that isn't none. Nominal takes priority
-        comp_val = next(
-            format_dict[item]
-            for item in ["nominal", "_min", "_max"]
-            if format_dict[item] is not None
-        )
-        print(
-            reformat_text(
-                "\nCheck {chk_cnt}: {status} when comparing {test_val} {comparison} {comp_val} : "
-                "{description}".format(
-                    status=status,
-                    comparison=chk.target.__name__[1:].replace("_", " "),
-                    comp_val=comp_val,
-                    chk_cnt=chk_cnt,
-                    description=chk.description,
-                    **format_dict
-                )
-            )
-        )
-    else:
-        if chk.test_val is not None:
-            print(
-                reformat_text(
-                    "\nCheck {chk_cnt}: {status}: {test_val} : {description}".format(
-                        chk_cnt=chk_cnt,
-                        description=chk.description,
-                        status=status,
-                        **format_dict
-                    )
-                )
-            )
-        else:
-            print(
-                reformat_text(
-                    "\nCheck {chk_cnt} : {status}: {description}".format(
-                        description=chk.description, chk_cnt=chk_cnt, status=status
-                    )
-                )
-            )
+def _print_comparisons(passes: bool, chk: CheckResult, chk_cnt: int, context: str):
+    msg = f"\nCheck {chk_cnt}: " + chk.check_string
+    print(reformat_text(msg))
```

### Comparing `fixate-0.6.0/src/fixate/ui_cmdline/kbhit.py` & `fixate-0.6.1.dev0/src/fixate/ui_cmdline/kbhit.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/ui_gui_qt/layout.py` & `fixate-0.6.1.dev0/src/fixate/ui_gui_qt/layout.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/ui_gui_qt/subclassed_widgets.py` & `fixate-0.6.1.dev0/src/fixate/ui_gui_qt/subclassed_widgets.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.0/src/fixate/ui_gui_qt/ui_gui_qt.py` & `fixate-0.6.1.dev0/src/fixate/ui_gui_qt/ui_gui_qt.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os.path
 from queue import Queue
 from PyQt5 import QtCore, QtGui, QtWidgets
 from PyQt5.QtCore import QObject, QThread, pyqtSignal, Qt, QRectF
 from pubsub import pub
 import fixate.config
 from fixate.config import RESOURCES
+from fixate.core.checks import CheckResult
 from fixate.core.exceptions import UserInputError, SequenceAbort
 from . import layout
 
 logger = logging.getLogger(__name__)
 
 wrapper = textwrap.TextWrapper(width=75)
 wrapper.break_long_words = False
@@ -819,18 +820,18 @@
             if target is None or ret_val == "ABORT_FORCE":
                 q.put(ret_val)
                 return
             ret_val = target(ret_val, **kwargs)
             if ret_val:
                 q.put(("Result", ret_val))
                 return
-        q.put(
-            "Exception",
-            UserInputError("Maximum number of attempts {} reached".format(attempts)),
-        )
+        # Display failure of target and send exception
+        error_str = f"Maximum number of attempts {attempts} reached. {target.__doc__}"
+        self._topic_UI_display(error_str)
+        q.put(("Exception", UserInputError(error_str)))
 
     def _topic_UI_display(self, msg):
         """
         :param msg:
         :return:
         """
         if self.closing:
@@ -975,99 +976,12 @@
         )
         self.sig_history_update.emit("!" * wrapper.width)
         self.sig_active_update.emit("!" * wrapper.width)
         # TODO self.history_update traceback into a debug log file
         if fixate.config.DEBUG:
             traceback.print_tb(exception.__traceback__, file=sys.stderr)
 
-    def round_to_3_sig_figures(self, chk):
-        """
-        Tries to round elements to 3 significant figures for formatting
-        :param chk:
-        :return:
-        """
-        ret_dict = {}
-        for element in ["_min", "_max", "test_val", "nominal", "tol"]:
-            ret_dict[element] = getattr(chk, element, None)
-            try:
-                ret_dict[element] = "{:.3g}".format(ret_dict[element])
-            except:
-                pass
-        return ret_dict
-
-    def _topic_Check(self, passes, chk, chk_cnt, context):
-        if passes:
-            status = "PASS"
-        else:
-            status = "FAIL"
-        format_dict = self.round_to_3_sig_figures(chk)
-        if chk._min is not None and chk._max is not None:
-            msg = self.reformat_text(
-                "\nCheck {chk_cnt}: {status} when comparing {test_val} {comparison} {_min} - {_max} : "
-                "{description}".format(
-                    status=status,
-                    comparison=chk.target.__name__[1:].replace("_", " "),
-                    chk_cnt=chk_cnt,
-                    description=chk.description,
-                    **format_dict
-                )
-            )
-            self.sig_history_update.emit(msg)
-            if status == "FAIL":
-                self.sig_active_update.emit(msg)
-        elif chk.nominal is not None and chk.tol is not None:
-            msg = self.reformat_text(
-                "\nCheck {chk_cnt}: {status} when comparing {test_val} {comparison} {nominal} +- {tol}% : "
-                "{description}".format(
-                    status=status,
-                    comparison=chk.target.__name__[1:].replace("_", " "),
-                    chk_cnt=chk_cnt,
-                    description=chk.description,
-                    **format_dict
-                )
-            )
-            self.sig_history_update.emit(msg)
-            if status == "FAIL":
-                self.sig_active_update.emit(msg)
-        elif chk._min is not None or chk._max is not None or chk.nominal is not None:
-            # Grabs the first value that isn't none. Nominal takes priority
-            comp_val = next(
-                format_dict[item]
-                for item in ["nominal", "_min", "_max"]
-                if format_dict[item] is not None
-            )
-            msg = self.reformat_text(
-                "\nCheck {chk_cnt}: {status} when comparing {test_val} {comparison} {comp_val} : "
-                "{description}".format(
-                    status=status,
-                    comparison=chk.target.__name__[1:].replace("_", " "),
-                    comp_val=comp_val,
-                    chk_cnt=chk_cnt,
-                    description=chk.description,
-                    **format_dict
-                )
-            )
-            self.sig_history_update.emit(msg)
-            if status == "FAIL":
-                self.sig_active_update.emit(msg)
-        else:
-            if chk.test_val is not None:
-                msg = self.reformat_text(
-                    "\nCheck {chk_cnt}: {status}: {test_val} : {description}".format(
-                        chk_cnt=chk_cnt,
-                        description=chk.description,
-                        status=status,
-                        **format_dict
-                    )
-                )
-                self.sig_history_update.emit(msg)
-                if status == "FAIL":
-                    self.sig_active_update.emit(msg)
-            else:
-                msg = self.reformat_text(
-                    "\nCheck {chk_cnt} : {status}: {description}".format(
-                        description=chk.description, chk_cnt=chk_cnt, status=status
-                    )
-                )
-                self.sig_history_update.emit(msg)
-                if status == "FAIL":
-                    self.sig_active_update.emit(msg)
+    def _topic_Check(self, passes: bool, chk: CheckResult, chk_cnt: int, context: str):
+        msg = self.reformat_text(f"\nCheck {chk_cnt}: " + chk.check_string)
+        self.sig_history_update.emit(msg)
+        if not chk.result:
+            self.sig_active_update.emit(msg)
```

### Comparing `fixate-0.6.0/src/fixate.egg-info/PKG-INFO` & `fixate-0.6.1.dev0/src/fixate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixate
-Version: 0.6.0
+Version: 0.6.1.dev0
 Summary: Framework for hardware test fixtures and automated test environments
 Home-page: http://pyfixate.com/
 Author: Ryan Parry-Jones
 Author-email: ryanspj+github@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fixate-0.6.0/src/fixate.egg-info/SOURCES.txt` & `fixate-0.6.1.dev0/src/fixate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/fixate/drivers/__init__.py
 src/fixate/drivers/ftdi.py
 src/fixate/drivers/daq/__init__.py
 src/fixate/drivers/daq/daqmx.py
 src/fixate/drivers/dmm/__init__.py
 src/fixate/drivers/dmm/fluke_8846a.py
 src/fixate/drivers/dmm/helper.py
+src/fixate/drivers/dmm/keithley_6500.py
 src/fixate/drivers/dso/__init__.py
 src/fixate/drivers/dso/agilent_mso_x.py
 src/fixate/drivers/dso/helper.py
 src/fixate/drivers/funcgen/__init__.py
 src/fixate/drivers/funcgen/helper.py
 src/fixate/drivers/funcgen/keysight_33500b.py
 src/fixate/drivers/funcgen/rigol_dg1022.py
```

### Comparing `fixate-0.6.0/test/test_config.py` & `fixate-0.6.1.dev0/test/test_config.py`

 * *Files identical despite different names*

