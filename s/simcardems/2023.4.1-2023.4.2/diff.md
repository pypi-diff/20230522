# Comparing `tmp/simcardems-2023.4.1.tar.gz` & `tmp/simcardems-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simcardems-2023.4.1.tar", last modified: Tue May 16 08:44:01 2023, max compression
+gzip compressed data, was "simcardems-2023.4.2.tar", last modified: Mon May 22 19:01:17 2023, max compression
```

## Comparing `simcardems-2023.4.1.tar` & `simcardems-2023.4.2.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.900084 simcardems-2023.4.1/
--rw-r--r--   0 root         (0) root         (0)    26526 2023-05-16 08:34:16.000000 simcardems-2023.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3845 2023-05-16 08:44:01.900084 simcardems-2023.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3141 2023-05-16 08:34:16.000000 simcardems-2023.4.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-16 08:44:01.900084 simcardems-2023.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      296 2023-05-16 08:34:16.000000 simcardems-2023.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.888084 simcardems-2023.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems/
--rw-r--r--   0 root         (0) root         (0)     3453 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2388 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/benchmark.py
--rw-r--r--   0 root         (0) root         (0)     5423 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     9241 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/cli.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/config.py
--rw-r--r--   0 root         (0) root         (0)    18669 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/datacollector.py
--rw-r--r--   0 root         (0) root         (0)     9907 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/ep_model.py
--rw-r--r--   0 root         (0) root         (0)    17148 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/geometry.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/gui.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/lvgeometry.py
--rw-r--r--   0 root         (0) root         (0)    11482 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/mechanics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems/models/
--rw-r--r--   0 root         (0) root         (0)      660 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      819 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60660 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    14164 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6993 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    60244 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    12046 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.900084 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6989 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    70534 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    12043 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.900084 simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60536 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
--rw-r--r--   0 root         (0) root         (0)     5730 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/newton_solver.py
--rw-r--r--   0 root         (0) root         (0)    21621 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/postprocess.py
--rw-r--r--   0 root         (0) root         (0)     7156 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/runner.py
--rw-r--r--   0 root         (0) root         (0)     6485 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/save_load_functions.py
--rw-r--r--   0 root         (0) root         (0)     4515 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/slabgeometry.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/time_stepper.py
--rw-r--r--   0 root         (0) root         (0)     5462 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/utils.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/value_extractor.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3845 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2016 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 08:34:34.000000 simcardems-2023.4.1/src/simcardems.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.900084 simcardems-2023.4.1/tests/
--rw-r--r--   0 root         (0) root         (0)      523 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_datacollector.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_mechanics_model.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_postprocessing.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_runner.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_save_load_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/
+-rw-r--r--   0 root         (0) root         (0)    26526 2023-05-22 18:51:36.000000 simcardems-2023.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-05-22 19:01:17.577035 simcardems-2023.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-05-22 18:51:36.000000 simcardems-2023.4.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-22 19:01:17.581035 simcardems-2023.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      296 2023-05-22 18:51:36.000000 simcardems-2023.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.569035 simcardems-2023.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.573035 simcardems-2023.4.2/src/simcardems/
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     9241 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/config.py
+-rw-r--r--   0 root         (0) root         (0)    18669 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/datacollector.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/ep_model.py
+-rw-r--r--   0 root         (0) root         (0)    17148 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/geometry.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/gui.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/lvgeometry.py
+-rw-r--r--   0 root         (0) root         (0)    11482 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/mechanics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      819 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60760 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    14164 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6993 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    60344 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12046 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    70634 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12043 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60636 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
+-rw-r--r--   0 root         (0) root         (0)     5730 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/newton_solver.py
+-rw-r--r--   0 root         (0) root         (0)    21621 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/runner.py
+-rw-r--r--   0 root         (0) root         (0)     6485 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/save_load_functions.py
+-rw-r--r--   0 root         (0) root         (0)     4515 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/slabgeometry.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/time_stepper.py
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/value_extractor.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.573035 simcardems-2023.4.2/src/simcardems.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 18:51:58.000000 simcardems-2023.4.2/src/simcardems.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_datacollector.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_mechanics_model.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_postprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_save_load_functions.py
```

### Comparing `simcardems-2023.4.1/LICENSE` & `simcardems-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/PKG-INFO` & `simcardems-2023.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.4.1/README.md` & `simcardems-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/setup.cfg` & `simcardems-2023.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/__init__.py` & `simcardems-2023.4.2/src/simcardems/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/benchmark.py` & `simcardems-2023.4.2/src/simcardems/benchmark.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/boundary_conditions.py` & `simcardems-2023.4.2/src/simcardems/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/cli.py` & `simcardems-2023.4.2/src/simcardems/cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/config.py` & `simcardems-2023.4.2/src/simcardems/config.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/datacollector.py` & `simcardems-2023.4.2/src/simcardems/datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/ep_model.py` & `simcardems-2023.4.2/src/simcardems/ep_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from . import geometry
 from . import utils
 from .config import Config
 
 if TYPE_CHECKING:
     from .models.em_model import BaseEMCoupling
+    from .models.cell_model import BaseCellModel
 
 logger = utils.getLogger(__name__)
 
 
 def setup_cell_model(
     cls,
     coupling: BaseEMCoupling,
@@ -269,26 +270,28 @@
 def load_json(filename: str):
     with open(filename, "r") as fid:
         d = json.load(fid)
     return d
 
 
 def handle_cell_params(
-    CellModel: Type[cbcbeat.CardiacCellModel],
+    CellModel: Type[BaseCellModel],
     cell_params: Optional[Dict[str, float]] = None,
     disease_state: str = "healthy",
     drug_factors_file: str = "",
     popu_factors_file: str = "",
 ):
-    cell_params_tmp = CellModel.default_parameters(disease_state)
+    cell_params_tmp = CellModel.default_parameters()
     # FIXME: In this case we update the parameters first, while in the
     # initial condition case we do that last. We need to be consistent
     # about this.
     if cell_params is not None:
         cell_params_tmp.update(cell_params)
+
+    CellModel.update_disease_parameters(cell_params_tmp, disease_state=disease_state)
     # Adding optional drug factors to parameters (if drug_factors_file exists)
     if file_exist(drug_factors_file, ".json"):
         logger.info(f"Drug scaling factors loaded from {drug_factors_file}")
         cell_params_tmp.update(load_json(drug_factors_file))
     else:
         if drug_factors_file != "":
             logger.warning(f"Unable to load drug factors file {drug_factors_file}")
```

### Comparing `simcardems-2023.4.1/src/simcardems/geometry.py` & `simcardems-2023.4.2/src/simcardems/geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/gui.py` & `simcardems-2023.4.2/src/simcardems/gui.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/lvgeometry.py` & `simcardems-2023.4.2/src/simcardems/lvgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/mechanics_model.py` & `simcardems-2023.4.2/src/simcardems/mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/__init__.py` & `simcardems-2023.4.2/src/simcardems/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from . import cell_model
 from . import em_model
 from . import explicit_ORdmm_Land
 from . import fully_coupled_ORdmm_Land
 from . import fully_coupled_Tor_Land
 from . import pureEP_ORdmm_Land
 
 
@@ -23,10 +24,11 @@
 
 
 __all__ = [
     "explicit_ORdmm_Land",
     "fully_coupled_ORdmm_Land",
     "fully_coupled_Tor_Land",
     "em_model",
+    "cell_model",
     "pureEP_ORdmm_Land",
     "loggers",
 ]
```

### Comparing `simcardems-2023.4.1/src/simcardems/models/em_model.py` & `simcardems-2023.4.2/src/simcardems/models/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/__init__.py` & `simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/cell_model.py` & `simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/cell_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 The module was autogenerated from a gotran ode file
 """
 from collections import OrderedDict
 from typing import Dict
 
 import dolfin
 import ufl
-from cbcbeat.cellmodels import CardiacCellModel
 from dolfin import as_vector
 from dolfin import Constant
 
 from ... import utils
+from ..cell_model import BaseCellModel
 from .em_model import EMCoupling
 
 logger = utils.getLogger(__name__)
 
 
 def Max(a, b):
     return (a + b + abs(a - b)) / Constant(2.0)
 
 
 def Min(a, b):
     return (a + b - abs(a - b)) / Constant(2.0)
 
 
-class ORdmmLandExplicit(CardiacCellModel):
+class ORdmmLandExplicit(BaseCellModel):
     def __init__(
         self,
         coupling: EMCoupling,
         params=None,
         init_conditions=None,
     ):
         """
@@ -44,15 +44,34 @@
         logger.debug("Initialize ORdmm Land model")
 
         super().__init__(params, init_conditions)
         self.lmbda = coupling.lmbda_ep
         self.dLambda = coupling.dLambda_ep
 
     @staticmethod
-    def default_parameters(disease_state: str = "healthy") -> Dict[str, float]:
+    def update_disease_parameters(
+        params: Dict[str, float],
+        disease_state: str = "healthy",
+    ) -> None:
+        if disease_state.lower() == "hf":
+            logger.info("Update scaling parameters for heart failure model")
+            params["HF_scaling_CaMKa"] = 1.50
+            params["HF_scaling_Jrel_inf"] = pow(0.8, 8.0)
+            params["HF_scaling_Jleak"] = 1.3
+            params["HF_scaling_Jup"] = 0.45
+            params["HF_scaling_GNaL"] = 1.3
+            params["HF_scaling_GK1"] = 0.68
+            params["HF_scaling_thL"] = 1.8
+            params["HF_scaling_Gto"] = 0.4
+            params["HF_scaling_Gncx"] = 1.6
+            params["HF_scaling_Pnak"] = 0.7
+            params["HF_scaling_cat50_ref"] = 0.6
+
+    @staticmethod
+    def default_parameters() -> Dict[str, float]:
         """Set-up and return default parameters.
 
         Parameters
         ----------
         disease_state : str, optional
             String with "hf" or "healthy", by default "healthy".
             If "hf", then parameters representing heart failure
@@ -231,28 +250,14 @@
                 ("HF_scaling_Gto", 1.0),
                 ("HF_scaling_Gncx", 1.0),
                 ("HF_scaling_Pnak", 1.0),
                 ("HF_scaling_cat50_ref", 1.0),
             ],
         )
 
-        if disease_state.lower() == "hf":
-            logger.info("Update scaling parameters for heart failure model")
-            params["HF_scaling_CaMKa"] = 1.50
-            params["HF_scaling_Jrel_inf"] = pow(0.8, 8.0)
-            params["HF_scaling_Jleak"] = 1.3
-            params["HF_scaling_Jup"] = 0.45
-            params["HF_scaling_GNaL"] = 1.3
-            params["HF_scaling_GK1"] = 0.68
-            params["HF_scaling_thL"] = 1.8
-            params["HF_scaling_Gto"] = 0.4
-            params["HF_scaling_Gncx"] = 1.6
-            params["HF_scaling_Pnak"] = 0.7
-            params["HF_scaling_cat50_ref"] = 0.6
-
         return params
 
     @staticmethod
     def default_initial_conditions():
         "Set-up and return default initial conditions."
         ic = OrderedDict(
             [
```

### Comparing `simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/em_model.py` & `simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py` & `simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py` & `simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py` & `simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 from __future__ import division
 
 from collections import OrderedDict
 from typing import Dict
 
 import dolfin
 import ufl
-from cbcbeat.cellmodels import CardiacCellModel
 from dolfin import as_vector
 from dolfin import Constant
 
 from ... import utils
+from ..cell_model import BaseCellModel
 from .em_model import EMCoupling
 
 logger = utils.getLogger(__name__)
 
 
 def Max(a, b):
     return (a + b + abs(a - b)) / Constant(2.0)
 
 
 def Min(a, b):
     return (a + b - abs(a - b)) / Constant(2.0)
 
 
-class ORdmmLandFull(CardiacCellModel):
+class ORdmmLandFull(BaseCellModel):
     def __init__(
         self,
         coupling: EMCoupling,
         params=None,
         init_conditions=None,
     ):
         """
@@ -45,15 +45,34 @@
 
         super().__init__(params, init_conditions)
         self.lmbda = coupling.lmbda_ep
         self.Zetas = coupling.Zetas_ep
         self.Zetaw = coupling.Zetaw_ep
 
     @staticmethod
-    def default_parameters(disease_state: str = "healthy") -> Dict[str, float]:
+    def update_disease_parameters(
+        params: Dict[str, float],
+        disease_state: str = "healthy",
+    ) -> None:
+        if disease_state.lower() == "hf":
+            logger.info("Update scaling parameters for heart failure model")
+            params["HF_scaling_CaMKa"] = 1.50
+            params["HF_scaling_Jrel_inf"] = pow(0.8, 8.0)
+            params["HF_scaling_Jleak"] = 1.3
+            params["HF_scaling_Jup"] = 0.45
+            params["HF_scaling_GNaL"] = 1.3
+            params["HF_scaling_GK1"] = 0.68
+            params["HF_scaling_thL"] = 1.8
+            params["HF_scaling_Gto"] = 0.4
+            params["HF_scaling_Gncx"] = 1.6
+            params["HF_scaling_Pnak"] = 0.7
+            params["HF_scaling_cat50_ref"] = 0.6
+
+    @staticmethod
+    def default_parameters() -> Dict[str, float]:
         """Set-up and return default parameters.
         Parameters
         ----------
         disease_state : str, optional
             String with "hf" or "healthy", by default "healthy".
             If "hf", then parameters representing heart failure
             will be used.
@@ -230,28 +249,14 @@
                 ("HF_scaling_Gto", 1.0),
                 ("HF_scaling_Gncx", 1.0),
                 ("HF_scaling_Pnak", 1.0),
                 ("HF_scaling_cat50_ref", 1.0),
             ],
         )
 
-        if disease_state.lower() == "hf":
-            logger.info("Update scaling parameters for heart failure model")
-            params["HF_scaling_CaMKa"] = 1.50
-            params["HF_scaling_Jrel_inf"] = pow(0.8, 8.0)
-            params["HF_scaling_Jleak"] = 1.3
-            params["HF_scaling_Jup"] = 0.45
-            params["HF_scaling_GNaL"] = 1.3
-            params["HF_scaling_GK1"] = 0.68
-            params["HF_scaling_thL"] = 1.8
-            params["HF_scaling_Gto"] = 0.4
-            params["HF_scaling_Gncx"] = 1.6
-            params["HF_scaling_Pnak"] = 0.7
-            params["HF_scaling_cat50_ref"] = 0.6
-
         return params
 
     @staticmethod
     def default_initial_conditions():
         "Set-up and return default initial conditions."
         ic = OrderedDict(
             [
```

### Comparing `simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py` & `simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/__init__.py` & `simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/active_model.py` & `simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py` & `simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from __future__ import division
 
 from collections import OrderedDict
 from typing import Dict
 
 import dolfin
 import ufl
-from cbcbeat.cellmodels import CardiacCellModel
 from dolfin import as_vector
 from dolfin import Constant
 
 from ... import utils
+from ..cell_model import BaseCellModel
 from .em_model import EMCoupling
 
 logger = utils.getLogger(__name__)
 
 
 def Max(a, b):
     return (a + b + abs(a - b)) / Constant(2.0)
@@ -30,15 +30,15 @@
 def vs_functions_to_dict(vs):
     state_names = TorLandFull.default_initial_conditions().keys()
     return {
         name: utils.sub_function(vs, index) for index, name in enumerate(state_names)
     }
 
 
-class TorLandFull(CardiacCellModel):
+class TorLandFull(BaseCellModel):
     def __init__(
         self,
         coupling: EMCoupling,
         params=None,
         init_conditions=None,
     ):
         """
@@ -54,15 +54,34 @@
 
         super().__init__(params, init_conditions)
         self.lmbda = coupling.lmbda_ep
         self.Zetas = coupling.Zetas_ep
         self.Zetaw = coupling.Zetaw_ep
 
     @staticmethod
-    def default_parameters(disease_state: str = "healthy") -> Dict[str, float]:
+    def update_disease_parameters(
+        params: Dict[str, float],
+        disease_state: str = "healthy",
+    ) -> None:
+        if disease_state.lower() == "hf":
+            logger.info("Update scaling parameters for heart failure model")
+            params["HF_scaling_CaMKa"] = 1.50
+            params["HF_scaling_Jrel_inf"] = pow(0.8, 8.0)
+            params["HF_scaling_Jleak"] = 1.3
+            params["HF_scaling_Jup"] = 0.45
+            params["HF_scaling_GNaL"] = 1.3
+            params["HF_scaling_GK1"] = 0.68
+            params["HF_scaling_thL"] = 1.8
+            params["HF_scaling_Gto"] = 0.4
+            params["HF_scaling_Gncx"] = 1.6
+            params["HF_scaling_Pnak"] = 0.7
+            params["HF_scaling_cat50_ref"] = 0.7
+
+    @staticmethod
+    def default_parameters() -> Dict[str, float]:
         """Set-up and return default parameters.
 
         Parameters
         ----------
         disease_state : str, optional
             String with "hf" or "healthy", by default "healthy".
             If "hf", then parameters representing heart failure
@@ -246,28 +265,14 @@
                 ("HF_scaling_Gto", 1.0),
                 ("HF_scaling_Gncx", 1.0),
                 ("HF_scaling_Pnak", 1.0),
                 ("HF_scaling_cat50_ref", 1.0),
             ],
         )
 
-        if disease_state.lower() == "hf":
-            logger.info("Update scaling parameters for heart failure model")
-            params["HF_scaling_CaMKa"] = 1.50
-            params["HF_scaling_Jrel_inf"] = pow(0.8, 8.0)
-            params["HF_scaling_Jleak"] = 1.3
-            params["HF_scaling_Jup"] = 0.45
-            params["HF_scaling_GNaL"] = 1.3
-            params["HF_scaling_GK1"] = 0.68
-            params["HF_scaling_thL"] = 1.8
-            params["HF_scaling_Gto"] = 0.4
-            params["HF_scaling_Gncx"] = 1.6
-            params["HF_scaling_Pnak"] = 0.7
-            params["HF_scaling_cat50_ref"] = 0.7
-
         return params
 
     @staticmethod
     def default_initial_conditions():
         "Set-up and return default initial conditions."
         ic = OrderedDict(
             [
```

### Comparing `simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/em_model.py` & `simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py` & `simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 The module was autogenerated from a gotran ode file
 """
 from collections import OrderedDict
 from typing import Dict
 
 import dolfin
 import ufl
-from cbcbeat.cellmodels import CardiacCellModel
 from dolfin import as_vector
 from dolfin import Constant
 
 from ... import utils
+from ..cell_model import BaseCellModel
 
 logger = utils.getLogger(__name__)
 
 
 def Max(a, b):
     return (a + b + abs(a - b)) / Constant(2.0)
 
 
 def Min(a, b):
     return (a + b - abs(a - b)) / Constant(2.0)
 
 
-class ORdmmLandPureEp(CardiacCellModel):
+class ORdmmLandPureEp(BaseCellModel):
     def __init__(self, params=None, init_conditions=None, **kwargs):
         """
         Create cardiac cell model
 
         *Arguments*
          params (dict, :py:class:`dolfin.Mesh`, optional)
            optional model parameters
@@ -36,15 +36,34 @@
            optional initial conditions
         """
         logger.debug("Initialize ORdmm Land model")
 
         super().__init__(params, init_conditions)
 
     @staticmethod
-    def default_parameters(disease_state: str = "healthy") -> Dict[str, float]:
+    def update_disease_parameters(
+        params: Dict[str, float],
+        disease_state: str = "healthy",
+    ) -> None:
+        if disease_state.lower() == "hf":
+            logger.info("Update scaling parameters for heart failure model")
+            params["HF_scaling_CaMKa"] = 1.50
+            params["HF_scaling_Jrel_inf"] = pow(0.8, 8.0)
+            params["HF_scaling_Jleak"] = 1.3
+            params["HF_scaling_Jup"] = 0.45
+            params["HF_scaling_GNaL"] = 1.3
+            params["HF_scaling_GK1"] = 0.68
+            params["HF_scaling_thL"] = 1.8
+            params["HF_scaling_Gto"] = 0.4
+            params["HF_scaling_Gncx"] = 1.6
+            params["HF_scaling_Pnak"] = 0.7
+            params["HF_scaling_cat50_ref"] = 0.6
+
+    @staticmethod
+    def default_parameters() -> Dict[str, float]:
         """Set-up and return default parameters.
 
         Parameters
         ----------
         disease_state : str, optional
             String with "hf" or "healthy", by default "healthy".
             If "hf", then parameters representing heart failure
@@ -225,28 +244,14 @@
                 ("HF_scaling_Gto", 1.0),
                 ("HF_scaling_Gncx", 1.0),
                 ("HF_scaling_Pnak", 1.0),
                 ("HF_scaling_cat50_ref", 1.0),
             ],
         )
 
-        if disease_state.lower() == "hf":
-            logger.info("Update scaling parameters for heart failure model")
-            params["HF_scaling_CaMKa"] = 1.50
-            params["HF_scaling_Jrel_inf"] = pow(0.8, 8.0)
-            params["HF_scaling_Jleak"] = 1.3
-            params["HF_scaling_Jup"] = 0.45
-            params["HF_scaling_GNaL"] = 1.3
-            params["HF_scaling_GK1"] = 0.68
-            params["HF_scaling_thL"] = 1.8
-            params["HF_scaling_Gto"] = 0.4
-            params["HF_scaling_Gncx"] = 1.6
-            params["HF_scaling_Pnak"] = 0.7
-            params["HF_scaling_cat50_ref"] = 0.6
-
         return params
 
     @staticmethod
     def default_initial_conditions():
         "Set-up and return default initial conditions."
         ic = OrderedDict(
             [
```

### Comparing `simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/em_model.py` & `simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/newton_solver.py` & `simcardems-2023.4.2/src/simcardems/newton_solver.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/postprocess.py` & `simcardems-2023.4.2/src/simcardems/postprocess.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/runner.py` & `simcardems-2023.4.2/src/simcardems/runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/save_load_functions.py` & `simcardems-2023.4.2/src/simcardems/save_load_functions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/slabgeometry.py` & `simcardems-2023.4.2/src/simcardems/slabgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/time_stepper.py` & `simcardems-2023.4.2/src/simcardems/time_stepper.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/utils.py` & `simcardems-2023.4.2/src/simcardems/utils.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems/value_extractor.py` & `simcardems-2023.4.2/src/simcardems/value_extractor.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/src/simcardems.egg-info/PKG-INFO` & `simcardems-2023.4.2/src/simcardems.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.4.1/src/simcardems.egg-info/SOURCES.txt` & `simcardems-2023.4.2/src/simcardems.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/simcardems.egg-info/SOURCES.txt
 src/simcardems.egg-info/dependency_links.txt
 src/simcardems.egg-info/entry_points.txt
 src/simcardems.egg-info/not-zip-safe
 src/simcardems.egg-info/requires.txt
 src/simcardems.egg-info/top_level.txt
 src/simcardems/models/__init__.py
+src/simcardems/models/cell_model.py
 src/simcardems/models/em_model.py
 src/simcardems/models/explicit_ORdmm_Land/__init__.py
 src/simcardems/models/explicit_ORdmm_Land/cell_model.py
 src/simcardems/models/explicit_ORdmm_Land/em_model.py
 src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
 src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
 src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
```

### Comparing `simcardems-2023.4.1/tests/test_boundary_conditions.py` & `simcardems-2023.4.2/tests/test_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/tests/test_cli.py` & `simcardems-2023.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/tests/test_datacollector.py` & `simcardems-2023.4.2/tests/test_datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/tests/test_geometry.py` & `simcardems-2023.4.2/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/tests/test_mechanics_model.py` & `simcardems-2023.4.2/tests/test_mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/tests/test_models.py` & `simcardems-2023.4.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/tests/test_postprocessing.py` & `simcardems-2023.4.2/tests/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/tests/test_runner.py` & `simcardems-2023.4.2/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.1/tests/test_save_load_functions.py` & `simcardems-2023.4.2/tests/test_save_load_functions.py`

 * *Files identical despite different names*

