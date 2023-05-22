# Comparing `tmp/fixate-0.6.1.dev0.tar.gz` & `tmp/fixate-0.6.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixate-0.6.1.dev0.tar", last modified: Mon May 22 01:16:37 2023, max compression
+gzip compressed data, was "fixate-0.6.1.post1.tar", last modified: Mon May 22 04:02:36 2023, max compression
```

## Comparing `fixate-0.6.1.dev0.tar` & `fixate-0.6.1.post1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.344973 fixate-0.6.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-22 01:16:37.344973 fixate-0.6.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-22 01:16:37.344973 fixate-0.6.1.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.312971 fixate-0.6.1.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.320972 fixate-0.6.1.dev0/src/fixate/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14402 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.324972 fixate-0.6.1.dev0/src/fixate/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/config/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.328972 fixate-0.6.1.dev0/src/fixate/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/config_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26866 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/jig_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/core/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.328972 fixate-0.6.1.dev0/src/fixate/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.328972 fixate-0.6.1.dev0/src/fixate/drivers/daq/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/daq/daqmx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.328972 fixate-0.6.1.dev0/src/fixate/drivers/dmm/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dmm/fluke_8846a.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dmm/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dmm/keithley_6500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.332973 fixate-0.6.1.dev0/src/fixate/drivers/dso/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37958 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dso/agilent_mso_x.py
--rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/dso/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/ftdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.332973 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25449 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/keysight_33500b.py
--rw-r--r--   0 runner    (1001) docker     (123)    26615 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/funcgen/rigol_dg1022.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.332973 fixate-0.6.1.dev0/src/fixate/drivers/lcr/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/lcr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/lcr/agilent_u1732c.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/lcr/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.336973 fixate-0.6.1.dev0/src/fixate/drivers/pps/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/pps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/pps/bk_178x.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/pps/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/drivers/pps/siglent_spd_3303X.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/src/fixate/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/function_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/multi_level_design.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/programmable_power_supply.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/tiny_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/examples/tiny_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/src/fixate/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/reporting/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/sequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/src/fixate/ui_cmdline/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_cmdline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_cmdline/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_cmdline/kbhit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25114 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/subclassed_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    38562 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/src/fixate/ui_gui_qt/ui_gui_qt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.324972 fixate-0.6.1.dev0/src/fixate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 01:16:37.000000 fixate-0.6.1.dev0/src/fixate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:16:37.340973 fixate-0.6.1.dev0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-22 01:16:24.000000 fixate-0.6.1.dev0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.103922 fixate-0.6.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-22 04:02:36.103922 fixate-0.6.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-22 04:02:36.107922 fixate-0.6.1.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.079921 fixate-0.6.1.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.083922 fixate-0.6.1.post1/src/fixate/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14402 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.087922 fixate-0.6.1.post1/src/fixate/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/config/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.091922 fixate-0.6.1.post1/src/fixate/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/core/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/core/config_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/core/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26866 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/core/jig_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/core/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.091922 fixate-0.6.1.post1/src/fixate/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.091922 fixate-0.6.1.post1/src/fixate/drivers/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/daq/daqmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.091922 fixate-0.6.1.post1/src/fixate/drivers/dmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/dmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/dmm/fluke_8846a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/dmm/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/dmm/keithley_6500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.095922 fixate-0.6.1.post1/src/fixate/drivers/dso/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/dso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37958 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/dso/agilent_mso_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/dso/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/ftdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.095922 fixate-0.6.1.post1/src/fixate/drivers/funcgen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/funcgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25449 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/funcgen/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/funcgen/keysight_33500b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26615 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/funcgen/rigol_dg1022.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.095922 fixate-0.6.1.post1/src/fixate/drivers/lcr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/lcr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/lcr/agilent_u1732c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/lcr/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.099922 fixate-0.6.1.post1/src/fixate/drivers/pps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/pps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/pps/bk_178x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/pps/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/drivers/pps/siglent_spd_3303X.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.099922 fixate-0.6.1.post1/src/fixate/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/examples/function_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/examples/multi_level_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/examples/programmable_power_supply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/examples/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/examples/tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/examples/tiny_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/examples/tiny_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.099922 fixate-0.6.1.post1/src/fixate/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/reporting/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.103922 fixate-0.6.1.post1/src/fixate/ui_cmdline/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/ui_cmdline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/ui_cmdline/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/ui_cmdline/kbhit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.103922 fixate-0.6.1.post1/src/fixate/ui_gui_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/ui_gui_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25114 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/ui_gui_qt/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/ui_gui_qt/subclassed_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38562 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/src/fixate/ui_gui_qt/ui_gui_qt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.087922 fixate-0.6.1.post1/src/fixate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-22 04:02:36.000000 fixate-0.6.1.post1/src/fixate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-22 04:02:36.000000 fixate-0.6.1.post1/src/fixate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:02:36.000000 fixate-0.6.1.post1/src/fixate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 04:02:36.000000 fixate-0.6.1.post1/src/fixate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:02:35.000000 fixate-0.6.1.post1/src/fixate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 04:02:36.000000 fixate-0.6.1.post1/src/fixate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 04:02:36.000000 fixate-0.6.1.post1/src/fixate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:02:36.103922 fixate-0.6.1.post1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-22 04:02:24.000000 fixate-0.6.1.post1/test/test_config.py
```

### Comparing `fixate-0.6.1.dev0/LICENSE.txt` & `fixate-0.6.1.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/PKG-INFO` & `fixate-0.6.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixate
-Version: 0.6.1.dev0
+Version: 0.6.1.post1
 Summary: Framework for hardware test fixtures and automated test environments
 Home-page: http://pyfixate.com/
 Author: Ryan Parry-Jones
 Author-email: ryanspj+github@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fixate-0.6.1.dev0/README.md` & `fixate-0.6.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/setup.cfg` & `fixate-0.6.1.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/__main__.py` & `fixate-0.6.1.post1/src/fixate/__main__.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/config/__init__.py` & `fixate-0.6.1.post1/src/fixate/config/__init__.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/config/helper.py` & `fixate-0.6.1.post1/src/fixate/config/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/core/checks.py` & `fixate-0.6.1.post1/src/fixate/core/checks.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/core/common.py` & `fixate-0.6.1.post1/src/fixate/core/common.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/core/config_util.py` & `fixate-0.6.1.post1/src/fixate/core/config_util.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/core/control.py` & `fixate-0.6.1.post1/src/fixate/core/control.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/core/exceptions.py` & `fixate-0.6.1.post1/src/fixate/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/core/jig_mapping.py` & `fixate-0.6.1.post1/src/fixate/core/jig_mapping.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/core/ui.py` & `fixate-0.6.1.post1/src/fixate/core/ui.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/__init__.py` & `fixate-0.6.1.post1/src/fixate/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/daq/daqmx.py` & `fixate-0.6.1.post1/src/fixate/drivers/daq/daqmx.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/dmm/__init__.py` & `fixate-0.6.1.post1/src/fixate/drivers/dmm/__init__.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/dmm/fluke_8846a.py` & `fixate-0.6.1.post1/src/fixate/drivers/dmm/fluke_8846a.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/dmm/helper.py` & `fixate-0.6.1.post1/src/fixate/drivers/dmm/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/dmm/keithley_6500.py` & `fixate-0.6.1.post1/src/fixate/drivers/dmm/keithley_6500.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/dso/__init__.py` & `fixate-0.6.1.post1/src/fixate/drivers/dso/__init__.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/dso/agilent_mso_x.py` & `fixate-0.6.1.post1/src/fixate/drivers/dso/agilent_mso_x.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/dso/helper.py` & `fixate-0.6.1.post1/src/fixate/drivers/dso/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/ftdi.py` & `fixate-0.6.1.post1/src/fixate/drivers/ftdi.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/funcgen/__init__.py` & `fixate-0.6.1.post1/src/fixate/drivers/funcgen/__init__.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/funcgen/helper.py` & `fixate-0.6.1.post1/src/fixate/drivers/funcgen/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/funcgen/keysight_33500b.py` & `fixate-0.6.1.post1/src/fixate/drivers/funcgen/keysight_33500b.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/funcgen/rigol_dg1022.py` & `fixate-0.6.1.post1/src/fixate/drivers/funcgen/rigol_dg1022.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/lcr/__init__.py` & `fixate-0.6.1.post1/src/fixate/drivers/lcr/__init__.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/lcr/agilent_u1732c.py` & `fixate-0.6.1.post1/src/fixate/drivers/lcr/agilent_u1732c.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/lcr/helper.py` & `fixate-0.6.1.post1/src/fixate/drivers/lcr/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/pps/__init__.py` & `fixate-0.6.1.post1/src/fixate/drivers/pps/__init__.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/pps/bk_178x.py` & `fixate-0.6.1.post1/src/fixate/drivers/pps/bk_178x.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/pps/helper.py` & `fixate-0.6.1.post1/src/fixate/drivers/pps/helper.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/drivers/pps/siglent_spd_3303X.py` & `fixate-0.6.1.post1/src/fixate/drivers/pps/siglent_spd_3303X.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/examples/function_generator.py` & `fixate-0.6.1.post1/src/fixate/examples/function_generator.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/examples/multi_level_design.py` & `fixate-0.6.1.post1/src/fixate/examples/multi_level_design.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/examples/programmable_power_supply.py` & `fixate-0.6.1.post1/src/fixate/examples/programmable_power_supply.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/examples/test_script.py` & `fixate-0.6.1.post1/src/fixate/examples/test_script.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/examples/tiny.py` & `fixate-0.6.1.post1/src/fixate/examples/tiny.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/examples/tiny_images.py` & `fixate-0.6.1.post1/src/fixate/examples/tiny_images.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/examples/tiny_variants.py` & `fixate-0.6.1.post1/src/fixate/examples/tiny_variants.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/reporting/csv.py` & `fixate-0.6.1.post1/src/fixate/reporting/csv.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/sequencer.py` & `fixate-0.6.1.post1/src/fixate/sequencer.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/ui_cmdline/cmd_line.py` & `fixate-0.6.1.post1/src/fixate/ui_cmdline/cmd_line.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/ui_cmdline/kbhit.py` & `fixate-0.6.1.post1/src/fixate/ui_cmdline/kbhit.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/ui_gui_qt/layout.py` & `fixate-0.6.1.post1/src/fixate/ui_gui_qt/layout.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/ui_gui_qt/subclassed_widgets.py` & `fixate-0.6.1.post1/src/fixate/ui_gui_qt/subclassed_widgets.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate/ui_gui_qt/ui_gui_qt.py` & `fixate-0.6.1.post1/src/fixate/ui_gui_qt/ui_gui_qt.py`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/src/fixate.egg-info/PKG-INFO` & `fixate-0.6.1.post1/src/fixate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixate
-Version: 0.6.1.dev0
+Version: 0.6.1.post1
 Summary: Framework for hardware test fixtures and automated test environments
 Home-page: http://pyfixate.com/
 Author: Ryan Parry-Jones
 Author-email: ryanspj+github@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fixate-0.6.1.dev0/src/fixate.egg-info/SOURCES.txt` & `fixate-0.6.1.post1/src/fixate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixate-0.6.1.dev0/test/test_config.py` & `fixate-0.6.1.post1/test/test_config.py`

 * *Files identical despite different names*

