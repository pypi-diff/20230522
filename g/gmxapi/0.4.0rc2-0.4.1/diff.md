# Comparing `tmp/gmxapi-0.4.0rc2.tar.gz` & `tmp/gmxapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/eric/develop/CLionProjects/gromacs2023/python_packaging/gmxapi/dist/tmpw5xnmrln/gmxapi-0.4.0rc2.tar", last modified: Thu Jan 12 16:33:26 2023, max compression
+gzip compressed data, was "/Users/eric/develop/CLionProjects/gromacs2023/python_packaging/gmxapi/dist/.tmp-qsfur0sc/gmxapi-0.4.1.tar", last modified: Mon May 22 16:55:00 2023, max compression
```

## Comparing `gmxapi-0.4.0rc2.tar` & `gmxapi-0.4.1.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/
--rw-r--r--   0 eric       (501) staff       (20)    18861 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/CMakeLists.txt
--rw-r--r--   0 eric       (501) staff       (20)    24479 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      112 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)      745 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      498 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/README.rst
--rw-r--r--   0 eric       (501) staff       (20)      138 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/pyproject.toml
--rw-r--r--   0 eric       (501) staff       (20)      536 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)    17937 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/cpp/
--rw-r--r--   0 eric       (501) staff       (20)     9478 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/export_context.cpp
--rw-r--r--   0 eric       (501) staff       (20)     3686 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/export_system.cpp
--rw-r--r--   0 eric       (501) staff       (20)     7541 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/export_tprfile.cpp
--rw-r--r--   0 eric       (501) staff       (20)     6083 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/gmxpy_exceptions.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4745 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/gmxpy_exceptions.h
--rw-r--r--   0 eric       (501) staff       (20)     2066 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/launch_0_2_1.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4744 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/module.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4070 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/module.h
--rw-r--r--   0 eric       (501) staff       (20)     3040 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/mpi_bindings.cpp
--rw-r--r--   0 eric       (501) staff       (20)     3243 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/mpi_bindings.h
--rw-r--r--   0 eric       (501) staff       (20)     2097 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/mpi_gromacs_support.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2827 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/mpi_no_gromacs_support.cpp
--rw-r--r--   0 eric       (501) staff       (20)     5054 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/pycontext.cpp
--rw-r--r--   0 eric       (501) staff       (20)     3446 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/pycontext.h
--rw-r--r--   0 eric       (501) staff       (20)     3048 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/pycontext_create.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2999 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/pycontext_create_no_mpi.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2034 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/pysystem.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2151 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/pysystem.h
--rw-r--r--   0 eric       (501) staff       (20)     3465 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/wrapped_exceptions.h
--rw-r--r--   0 eric       (501) staff       (20)     3529 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/wrapped_exceptions_0_1_0.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4065 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/cpp/wrapped_exceptions_0_3_1.cpp
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/gmxapi/
--rw-r--r--   0 eric       (501) staff       (20)     2814 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     3532 2023-01-12 08:47:41.000000 gmxapi-0.4.0rc2/src/gmxapi/_logging.py
--rw-r--r--   0 eric       (501) staff       (20)     2300 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/_transform.py
--rw-r--r--   0 eric       (501) staff       (20)    31056 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/abc.py
--rw-r--r--   0 eric       (501) staff       (20)    21887 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/commandline.py
--rw-r--r--   0 eric       (501) staff       (20)     5362 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/datamodel.py
--rw-r--r--   0 eric       (501) staff       (20)     4315 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/exceptions.py
--rw-r--r--   0 eric       (501) staff       (20)      416 2022-12-23 13:51:08.000000 gmxapi-0.4.0rc2/src/gmxapi/gmxconfig.json
--rw-r--r--   0 eric       (501) staff       (20)      367 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/gmxconfig.json.in
--rw-r--r--   0 eric       (501) staff       (20)   244525 2023-01-12 16:32:26.000000 gmxapi-0.4.0rc2/src/gmxapi/operation.py
--rw-r--r--   0 eric       (501) staff       (20)    30569 2023-01-12 08:47:41.000000 gmxapi-0.4.0rc2/src/gmxapi/runtime.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/gmxapi/simulation/
--rw-r--r--   0 eric       (501) staff       (20)     2787 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/simulation/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     2316 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/simulation/abc.py
--rw-r--r--   0 eric       (501) staff       (20)    57397 2022-12-11 09:03:28.000000 gmxapi-0.4.0rc2/src/gmxapi/simulation/context.py
--rw-r--r--   0 eric       (501) staff       (20)     9778 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/simulation/fileio.py
--rw-r--r--   0 eric       (501) staff       (20)    50529 2022-12-11 09:03:28.000000 gmxapi-0.4.0rc2/src/gmxapi/simulation/mdrun.py
--rw-r--r--   0 eric       (501) staff       (20)    18838 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/simulation/modify_input.py
--rw-r--r--   0 eric       (501) staff       (20)    19300 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/simulation/read_tpr.py
--rw-r--r--   0 eric       (501) staff       (20)    35454 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/simulation/workflow.py
--rw-r--r--   0 eric       (501) staff       (20)     7806 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/testsupport.py
--rw-r--r--   0 eric       (501) staff       (20)     6753 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/typing.py
--rw-r--r--   0 eric       (501) staff       (20)     2808 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/src/gmxapi/utility.py
--rw-r--r--   0 eric       (501) staff       (20)     8615 2023-01-12 16:33:06.000000 gmxapi-0.4.0rc2/src/gmxapi/version.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/gmxapi.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      745 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/gmxapi.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1695 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/gmxapi.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/gmxapi.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2022-12-01 09:15:04.000000 gmxapi-0.4.0rc2/src/gmxapi.egg-info/not-zip-safe
--rw-r--r--   0 eric       (501) staff       (20)       50 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/gmxapi.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)        7 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/src/gmxapi.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-01-12 16:33:26.000000 gmxapi-0.4.0rc2/test/
--rw-r--r--   0 eric       (501) staff       (20)     5358 2022-12-11 09:03:28.000000 gmxapi-0.4.0rc2/test/CMakeLists.txt
--rw-r--r--   0 eric       (501) staff       (20)    13256 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/test/test_commandline.py
--rw-r--r--   0 eric       (501) staff       (20)     2317 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/test/test_exceptions.py
--rw-r--r--   0 eric       (501) staff       (20)     5296 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/test/test_feature_check.py
--rw-r--r--   0 eric       (501) staff       (20)     4009 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/test/test_fileio.py
--rw-r--r--   0 eric       (501) staff       (20)     4689 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/test/test_fileio_low_level.py
--rw-r--r--   0 eric       (501) staff       (20)    11778 2022-12-11 09:03:28.000000 gmxapi-0.4.0rc2/test/test_mdrun.py
--rw-r--r--   0 eric       (501) staff       (20)     6540 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/test/test_operation.py
--rw-r--r--   0 eric       (501) staff       (20)     8151 2022-12-11 09:03:28.000000 gmxapi-0.4.0rc2/test/test_runtime.py
--rw-r--r--   0 eric       (501) staff       (20)     5584 2022-12-06 12:22:43.000000 gmxapi-0.4.0rc2/test/test_subgraph.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/
+-rw-r--r--   0 eric       (501) staff       (20)    18861 2023-05-22 16:45:32.000000 gmxapi-0.4.1/CMakeLists.txt
+-rw-r--r--   0 eric       (501) staff       (20)    24479 2023-05-15 03:20:39.000000 gmxapi-0.4.1/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      188 2023-05-22 16:45:32.000000 gmxapi-0.4.1/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)      742 2023-05-22 16:55:00.000000 gmxapi-0.4.1/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      498 2023-05-15 03:20:39.000000 gmxapi-0.4.1/README.rst
+-rw-r--r--   0 eric       (501) staff       (20)      138 2023-05-22 16:45:32.000000 gmxapi-0.4.1/pyproject.toml
+-rw-r--r--   0 eric       (501) staff       (20)      536 2023-05-22 16:55:00.000000 gmxapi-0.4.1/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)    17937 2023-05-22 16:45:32.000000 gmxapi-0.4.1/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/cpp/
+-rw-r--r--   0 eric       (501) staff       (20)    10101 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/cpp/export_context.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     3686 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/export_system.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     7541 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/export_tprfile.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     6083 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/gmxpy_exceptions.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4745 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/gmxpy_exceptions.h
+-rw-r--r--   0 eric       (501) staff       (20)     2066 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/launch_0_2_1.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4744 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/module.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4070 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/module.h
+-rw-r--r--   0 eric       (501) staff       (20)     3040 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/mpi_bindings.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     3243 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/mpi_bindings.h
+-rw-r--r--   0 eric       (501) staff       (20)     2097 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/mpi_gromacs_support.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2827 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/mpi_no_gromacs_support.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     5054 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pycontext.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     3446 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pycontext.h
+-rw-r--r--   0 eric       (501) staff       (20)     3048 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pycontext_create.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2999 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pycontext_create_no_mpi.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2034 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pysystem.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2151 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pysystem.h
+-rw-r--r--   0 eric       (501) staff       (20)     3465 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/wrapped_exceptions.h
+-rw-r--r--   0 eric       (501) staff       (20)     3529 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/wrapped_exceptions_0_1_0.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4065 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/wrapped_exceptions_0_3_1.cpp
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi/
+-rw-r--r--   0 eric       (501) staff       (20)     2814 2023-05-15 03:21:49.000000 gmxapi-0.4.1/src/gmxapi/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     3532 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/_logging.py
+-rw-r--r--   0 eric       (501) staff       (20)     2300 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/_transform.py
+-rw-r--r--   0 eric       (501) staff       (20)    31056 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/abc.py
+-rw-r--r--   0 eric       (501) staff       (20)    22158 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/commandline.py
+-rw-r--r--   0 eric       (501) staff       (20)     5362 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/datamodel.py
+-rw-r--r--   0 eric       (501) staff       (20)     4315 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/exceptions.py
+-rw-r--r--   0 eric       (501) staff       (20)      367 2023-05-22 16:45:32.000000 gmxapi-0.4.1/src/gmxapi/gmxconfig.json.in
+-rw-r--r--   0 eric       (501) staff       (20)   244525 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/operation.py
+-rw-r--r--   0 eric       (501) staff       (20)    31523 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/runtime.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi/simulation/
+-rw-r--r--   0 eric       (501) staff       (20)     2787 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     2316 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/abc.py
+-rw-r--r--   0 eric       (501) staff       (20)    57397 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/context.py
+-rw-r--r--   0 eric       (501) staff       (20)     9778 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/fileio.py
+-rw-r--r--   0 eric       (501) staff       (20)    50717 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/mdrun.py
+-rw-r--r--   0 eric       (501) staff       (20)    18838 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/modify_input.py
+-rw-r--r--   0 eric       (501) staff       (20)    19300 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/read_tpr.py
+-rw-r--r--   0 eric       (501) staff       (20)    36791 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/workflow.py
+-rw-r--r--   0 eric       (501) staff       (20)     7932 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/testsupport.py
+-rw-r--r--   0 eric       (501) staff       (20)     6753 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/typing.py
+-rw-r--r--   0 eric       (501) staff       (20)     2808 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/utility.py
+-rw-r--r--   0 eric       (501) staff       (20)     8612 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/version.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      742 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1721 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-22 16:54:59.000000 gmxapi-0.4.1/src/gmxapi.egg-info/not-zip-safe
+-rw-r--r--   0 eric       (501) staff       (20)       50 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)        7 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/test/
+-rw-r--r--   0 eric       (501) staff       (20)     5358 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/CMakeLists.txt
+-rw-r--r--   0 eric       (501) staff       (20)     7010 2023-05-22 16:45:32.000000 gmxapi-0.4.1/test/conftest.py
+-rw-r--r--   0 eric       (501) staff       (20)      113 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/pytest.ini
+-rw-r--r--   0 eric       (501) staff       (20)    13256 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_commandline.py
+-rw-r--r--   0 eric       (501) staff       (20)     2317 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_exceptions.py
+-rw-r--r--   0 eric       (501) staff       (20)     5296 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_feature_check.py
+-rw-r--r--   0 eric       (501) staff       (20)     4009 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_fileio.py
+-rw-r--r--   0 eric       (501) staff       (20)     4689 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_fileio_low_level.py
+-rw-r--r--   0 eric       (501) staff       (20)    12615 2023-05-22 16:38:39.000000 gmxapi-0.4.1/test/test_mdrun.py
+-rw-r--r--   0 eric       (501) staff       (20)     6540 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_operation.py
+-rw-r--r--   0 eric       (501) staff       (20)     8151 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_runtime.py
+-rw-r--r--   0 eric       (501) staff       (20)     5584 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_subgraph.py
+-rw-r--r--   0 eric       (501) staff       (20)    49825 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/testdata.json
```

### Comparing `gmxapi-0.4.0rc2/CMakeLists.txt` & `gmxapi-0.4.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/LICENSE` & `gmxapi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/PKG-INFO` & `gmxapi-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmxapi
-Version: 0.4.0rc2
+Version: 0.4.1
 Summary: gmxapi Python interface for GROMACS.
 Home-page: http://gmxapi.org/
 Author: GROMACS gmxapi team
 Author-email: info@gmxapi.org
 License: LGPL
 Requires-Python: >=3.7
 License-File: LICENSE
```

### Comparing `gmxapi-0.4.0rc2/setup.cfg` & `gmxapi-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/setup.py` & `gmxapi-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/export_context.cpp` & `gmxapi-0.4.1/src/cpp/export_context.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -124,27 +124,17 @@
     {
         auto val = py::cast<std::string>(py::str(params["max_hours"]));
         mdargs.emplace_back("-maxh");
         mdargs.emplace_back(val);
     }
     if (params.contains("append_output"))
     {
-        try
+        if (!params["append_output"].cast<bool>())
         {
-            if (!params["append_output"].cast<bool>())
-            {
-                mdargs.emplace_back("-noappend");
-            }
-        }
-        catch (const py::cast_error& e)
-        {
-            // Couldn't cast to bool for some reason.
-            // Convert to gmxapi exception (not implemented)
-            // ref. https://github.com/kassonlab/gmxapi/issues/125
-            throw;
+            mdargs.emplace_back("-noappend");
         }
     }
     return mdargs;
 }
 
 static std::vector<std::string> makeMDArgs_CLI(const py::dict& params)
 {
@@ -172,24 +162,33 @@
             }
             // If value is a non-string iterator, get each value.
             try
             {
                 auto it = py::iter(value);
                 while (it != py::iterator::sentinel())
                 {
-                    mdargs.emplace_back(py::cast<std::string>(*it));
+                    mdargs.emplace_back(py::str(*it));
                     ++it;
                 }
                 continue;
             }
-            catch (py::type_error&)
+            catch (py::error_already_set& eas)
             {
+                // `py::iter` throws TypeError for bad arguments, but it comes through the C API,
+                // so pybind11 wraps it in py::error_already_set, not py::type_error. Ref:
+                // https://pybind11.readthedocs.io/en/stable/advanced/exceptions.html#handling-exceptions-from-python-in-c
+                // Only suppress TypeError.
+                if (!eas.matches(PyExc_TypeError))
+                {
+                    throw;
+                }
             }
-            // Otherwise, convert the value to string.
-            mdargs.emplace_back(py::cast<std::string>(value));
+            // Otherwise, cast the Python value to a Python string (which is implicitly convertible
+            // to std::string).
+            mdargs.emplace_back(py::str(value));
         }
     }
     return mdargs;
 }
 
 
 /*! \internal
@@ -248,14 +247,25 @@
     // Add argument type before it is used for more sensible automatic bindings behavior.
     py::class_<MDArgs, std::unique_ptr<MDArgs>> mdargs(m, "MDArgs");
     mdargs.def(py::init(), "Create an empty MDArgs object.");
     mdargs.def(
             "set",
             [](MDArgs* self, const py::dict& params) { setMDArgs(self, params); },
             "Assign parameters in MDArgs from Python dict.");
+    mdargs.def(
+            "get_args",
+            [](const MDArgs& self) {
+                auto args = py::list(self.size());
+                for (int i = 0; i < self.size(); ++i)
+                {
+                    args[i] = py::str(self[i]);
+                };
+                return args;
+            },
+            "Get an iterator of command line argument tokens, if possible and relevant.");
 
     // Export execution context class
     py::class_<PyContext, std::shared_ptr<PyContext>> context(m, "Context");
     context.def(py::init(), "Create a default execution context.");
     context.def("setMDArgs", &PyContext::setMDArgs, "Set MD runtime parameters.");
 
     context.def("add_mdmodule", &PyContext::addMDModule, "Add an MD plugin for the simulation.");
```

### Comparing `gmxapi-0.4.0rc2/src/cpp/export_system.cpp` & `gmxapi-0.4.1/src/cpp/export_system.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/export_tprfile.cpp` & `gmxapi-0.4.1/src/cpp/export_tprfile.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/gmxpy_exceptions.cpp` & `gmxapi-0.4.1/src/cpp/gmxpy_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/gmxpy_exceptions.h` & `gmxapi-0.4.1/src/cpp/gmxpy_exceptions.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/launch_0_2_1.cpp` & `gmxapi-0.4.1/src/cpp/launch_0_2_1.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/module.cpp` & `gmxapi-0.4.1/src/cpp/module.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/module.h` & `gmxapi-0.4.1/src/cpp/module.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/mpi_bindings.cpp` & `gmxapi-0.4.1/src/cpp/mpi_bindings.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/mpi_bindings.h` & `gmxapi-0.4.1/src/cpp/mpi_bindings.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/mpi_gromacs_support.cpp` & `gmxapi-0.4.1/src/cpp/mpi_gromacs_support.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/mpi_no_gromacs_support.cpp` & `gmxapi-0.4.1/src/cpp/mpi_no_gromacs_support.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/pycontext.cpp` & `gmxapi-0.4.1/src/cpp/pycontext.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/pycontext.h` & `gmxapi-0.4.1/src/cpp/pycontext.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/pycontext_create.cpp` & `gmxapi-0.4.1/src/cpp/pycontext_create.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/pycontext_create_no_mpi.cpp` & `gmxapi-0.4.1/src/cpp/pycontext_create_no_mpi.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/pysystem.cpp` & `gmxapi-0.4.1/src/cpp/pysystem.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/pysystem.h` & `gmxapi-0.4.1/src/cpp/pysystem.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/wrapped_exceptions.h` & `gmxapi-0.4.1/src/cpp/wrapped_exceptions.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/wrapped_exceptions_0_1_0.cpp` & `gmxapi-0.4.1/src/cpp/wrapped_exceptions_0_1_0.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/cpp/wrapped_exceptions_0_3_1.cpp` & `gmxapi-0.4.1/src/cpp/wrapped_exceptions_0_3_1.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/__init__.py` & `gmxapi-0.4.1/src/gmxapi/__init__.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/_logging.py` & `gmxapi-0.4.1/src/gmxapi/_logging.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/_transform.py` & `gmxapi-0.4.1/src/gmxapi/_transform.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/abc.py` & `gmxapi-0.4.1/src/gmxapi/abc.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/commandline.py` & `gmxapi-0.4.1/src/gmxapi/commandline.py`

 * *Files 3% similar despite different names*

```diff
@@ -381,24 +381,32 @@
     and resources from the Python interpreter.
     (See https://docs.python.org/3/library/subprocess.html#subprocess.run)
 
     .. versionadded:: 0.3.1
         If specified, *env* replaces the default environment variables map seen by *executable* in the
         subprocess.
 
+    .. versionchanged:: 0.4.1
+        If unspecified, *env* defaults to a **filtered** copy of the current environment
+        (with MPI-related environment variables removed).
+        See :py:func:`gmxapi.runtime.filtered_mpi_environ()`.
+
     In addition to controlling environment variables used for user-input, it may be
     necessary to adjust the environment to prevent the subprocess from inheriting variables that it
     should not. This is particularly relevant if the Python script is launched with ``mpiexec`` and
     then ``commandline_wrapper`` is used to launch an MPI-aware executable that may try to manage
     the MPI context. (Reference :issue:`4421`)
 
     When overriding the environment variables, don't forget to include basic variables
     like PATH that are necessary for the executable to run. `os.getenv` can help.
     E.g. ``commandline_operation(..., env={'PATH': os.getenv('PATH'), ...})``
 
+    See Also:
+        :py:func:`gmxapi.runtime.filtered_mpi_environ()`.
+
     Output:
         The output node of the resulting operation handle contains
 
         * ``directory``: filesystem path that was used as the working directory for the subprocess
         * ``file``: the mapping of CLI flags to filename strings resulting from the ``output_files`` kwarg
         * ``returncode``: return code of the subprocess.
         * ``stderr``: A string mapping from process STDERR; it will be the
@@ -416,14 +424,15 @@
     Note that re-executing a gmxapi script in the same directory will cause
     commands to be executed again in the same directories. If this presents a
     risk of data corruption (or just wasted compute cycles), you may include
     the key word argument ``_exist_ok=False`` to force an error. Please consider
     contacting the developers through any of the various GROMACS community
     channels to further discuss your use case.
     """
+    import gmxapi.runtime
 
     # Implementation details: When used in a script, this function returns an
     # instance of an operation. However, because of the dynamic specification of
     # inputs and outputs, each invocation may have the overhead of defining new
     # types to express the data flow topology, regardless of the executable.
     # If this overhead is problematic, consider exposing the intermediate step
     # at which the Operation is fully specified to facilitate reuse.
@@ -503,24 +512,17 @@
     output_options = filemap_to_flag_list(output_files).output.data
     command = gmx.concatenate_lists(
         [[executable], arguments, input_options, output_options]
     )
     shell = gmx.make_constant(False)
 
     if env is None:
-
-        @gmx.function_wrapper(
-            # allow_duplicate=True
-        )
-        def _env() -> dict:
-            import os
-
-            return dict(os.environ)
-
-        env = _env().output.data
+        env = gmx.function_wrapper(allow_duplicate=True)(
+            gmxapi.runtime.filtered_mpi_environ
+        )().output.data
     cli_args = {"command": command, "shell": shell, "env": env}
     cli_args.update(**kwargs)
     if stdin is not None:
         cli_args["stdin"] = stdin
 
     ##
     # 3. Merge operations
```

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/datamodel.py` & `gmxapi-0.4.1/src/gmxapi/datamodel.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/exceptions.py` & `gmxapi-0.4.1/src/gmxapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/operation.py` & `gmxapi-0.4.1/src/gmxapi/operation.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/runtime.py` & `gmxapi-0.4.1/src/gmxapi/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,28 +63,29 @@
     :py:mod:`gmxapi.simulation.mdrun`, decoupling MPI communicator handling
     from :py:mod:`gmxapi.simulation.context`.
     See also https://gitlab.com/gromacs/gromacs/-/issues/3718
 
 """
 
 __all__ = (
+    "filtered_mpi_environ",
+    "filtered_prefixes",
     "scoped_resources",
     "ResourceAllocation",
     "ResourceAssignment",
     "ResourceRequirements",
 )
 
 import dataclasses
 import functools
+import os
 import threading
 import typing
 import warnings
 import weakref
-from typing import TYPE_CHECKING
-from _weakref import ReferenceType
 from contextlib import contextmanager
 
 import gmxapi.utility
 from gmxapi import exceptions
 from gmxapi import logger as root_logger
 
 try:
@@ -96,17 +97,17 @@
     Protocol = typing.Generic
 
 # Initialize module-level logger
 logger = root_logger.getChild(__name__)
 logger.info("Importing {}".format(__name__))
 
 
-if TYPE_CHECKING:
+if typing.TYPE_CHECKING:
     try:
-        import Comm as Communicator
+        import mpi4py.MPI.Comm as Communicator
     except ImportError:
         Communicator = None
 
 
 # gmxapi requires mpi4py, but it is useful to allow module-level imports to fail
 # so that documentation builds can succeed without package dependencies. It is
 # also helpful to retain the accompanying logic in case we want to decouple from
@@ -183,15 +184,15 @@
     finalized.
 
     To transfer ownership of the communicator in *task* or *ensemble*, add
     a finalizer using either the *finalizer* key word argument or the
     `add_finalizer` method.
     """
 
-    parent: "ReferenceType[ResourceAllocation[CommunicatorT, ReceivedTokenT]]"
+    parent: "weakref.ReferenceType[ResourceAllocation[CommunicatorT, ReceivedTokenT]]"
     """Resource allocation from which the current assignment is derived.
     
     Notes that this is a weak reference to the provided ResourceAllocation.
     See :py:mod:`weakref`.
     """
 
     _resource_id: typing.Optional = None
@@ -484,14 +485,15 @@
                 Blocks may span node boundaries.
                 When allocation spans multiple nodes, we should try to align blocks at
                 node boundaries so that we can assume that a rank assigned None could
                 lend its CPU core to the closest non-None member. This is not currently
                 possible. If pursued in the future, it could be appropriate to create
                 an additional resource layer comprising a parent MPI.Group for the
                 processes "owning" each subset of cores.
+
             """
 
             assert len(set(roots) - {None}) == n_subtasks
             assert set(roots) - {None} == set(range(n_subtasks))
 
             _current_offset = 0
             subtask_ranks = [0] * base_comm_size
@@ -756,7 +758,47 @@
         allocation=allocation, requirements=requirements
     )
 
     try:
         yield resources
     finally:
         resources.close()
+
+
+filtered_prefixes = (
+    "DCMF_",  # IBM
+    "MPICH_",
+    "MPIEXEC_",
+    "MPIO_",  # IBM
+    "MV2_",  # MVAPICH2 and some forks
+    "MVAPICH_",
+    "HYDRA_",  # MPICH
+    "OMPI_",  # OpenMPI
+    "PMI_",  # Process Management Interface
+    "PMIX_",  # Newer PMI and batch systems
+    "I_MPI_",  # Intel MPI
+)
+"""MPI-related environment variable prefixes.
+
+Environment variable prefixes known to be associated with MPI implementations,
+which may affect MPI context detection, and which should not matter outside of
+MPI contexts.
+
+References:
+    * :issue:`4423`
+    * :issue:`4736`
+
+"""
+
+
+def filtered_mpi_environ() -> dict:
+    """Return a filtered environment variables map with MPI-related entries removed.
+
+    See Also:
+        :py:data:`filtered_prefixes`
+
+    """
+    return {
+        key: value
+        for key, value in os.environ.items()
+        if not any(key.startswith(prefix) for prefix in filtered_prefixes)
+    }
```

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/simulation/__init__.py` & `gmxapi-0.4.1/src/gmxapi/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/simulation/abc.py` & `gmxapi-0.4.1/src/gmxapi/simulation/abc.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/simulation/context.py` & `gmxapi-0.4.1/src/gmxapi/simulation/context.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/simulation/fileio.py` & `gmxapi-0.4.1/src/gmxapi/simulation/fileio.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/simulation/mdrun.py` & `gmxapi-0.4.1/src/gmxapi/simulation/mdrun.py`

 * *Files 2% similar despite different names*

```diff
@@ -986,21 +986,27 @@
     *input* may be a TPR file name or an object providing the SimulationInput interface.
 
     *runtime_args* allows an optional dictionary of mdrun options, using the option flag
     (including the leading hyphen ``-``) as the dictionary key.
     For mdrun command line options that do not take a value (e.g. ``-noappend``),
     use ``None`` as the dictionary value.
 
-    Note:
-        New function names will be appearing to handle tasks that are separate
+    Warning:
+        Run time argument processing does not have Python bindings at this time.
+        key-value pairs are passed as plain text to the underlying library.
+        Usage errors can be hard to discover. Refer to the MD log file in the output
+        directory for messages regarding argument processing.
+
+        Note, in particular, that the available ``mdrun`` arguments can depend on the
+        GROMACS build configuration, such as whether an MPI library or thread-MPI
+        is enabled.
+
+    See Also:
+        The :doc:`/onlinehelp/gmx-mdrun` command line tool.
 
-        "simulate" is plausibly a dispatcher or base class for various tasks
-        dispatched by mdrun. Specific work factories are likely "minimize,"
-        "test_particle_insertion," "legacy_simulation" (do_md), or "simulation"
-        composition (which may be leap-frog, vv, and other algorithms)
     """
     # The job of this function is to arrange for the creation of a workflow node
     # by transforming arguments into a DataSourceCollection and providing the
     # collection to a Director.
     # The Director is specific to the Operation (this module) but could be generated
     # with the help of simple metaprogramming in the future (e.g. just declare
     # requirements or helpers in a class definition).
```

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/simulation/modify_input.py` & `gmxapi-0.4.1/src/gmxapi/simulation/modify_input.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/simulation/read_tpr.py` & `gmxapi-0.4.1/src/gmxapi/simulation/read_tpr.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/simulation/workflow.py` & `gmxapi-0.4.1/src/gmxapi/simulation/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -683,21 +683,23 @@
         append_output (bool): Append output for continuous trajectories if True, truncate existing output data if False. (default True)
         end_time (float): Specify the final time in the simulation trajectory, overriding input read from TPR.
         grid (tuple): Domain decomposition grid divisions (nx, ny, nz). (-dd)
         max_hours (float): Terminate after 0.99 times this many hours if simulation is still running. (-maxh)
         pme_ranks (int): number of separate ranks to be used for PME electrostatics. (-npme)
         threads_per_pme_rank (int): Number of OpenMP threads per PME rank. (-ntomp_pme)
         steps (int): Override input files and run for this many steps. (-nsteps; deprecated)
-        threads (int): Total number of threads to start. (-nt)
+        threads (int): Total number of threads to start for thread-MPI GROMACS. (-nt)
         threads_per_rank (int): number of OpenMP threads to start per MPI rank. (-ntomp)
         tmpi (int): number of thread-MPI ranks to start. (-ntmpi)
 
     ..  versionchanged:: 0.1
         *pme_threads_per_rank* renamed to *threads_per_pme_rank*.
 
+    Note that run time simulator arguments can also be provided through `gmxapi.mdrun` *runtime_args*.
+
     Returns:
         simulation member of a gmx.workflow.WorkSpec object
 
     Produces a WorkSpec with the following data::
 
         version: gmxapi_workspec_0_1
         elements:
@@ -710,16 +712,18 @@
                 operation: md
                 depends: ['tpr_input']
                 params: {'kw1': arg1, 'kw2': arg2, ...}
 
     Bugs: version 0.0.6
         * There is not a way to programatically check the current step number on disk.
           See https://github.com/kassonlab/gmxapi/issues/56 and https://github.com/kassonlab/gmxapi/issues/85
+
     """
     import os
+    from gmxapi.utility import config
 
     usage = "argument to from_tpr() should be a valid filename or list of filenames, followed by optional key word arguments."
 
     # Normalize to tuple input type.
     if isinstance(input, list) or isinstance(input, tuple):
         tpr_list = tuple([to_string(element) for element in input])
     else:
@@ -730,14 +734,32 @@
 
     # Check for valid filenames
     for arg in tpr_list:
         if not (os.path.exists(arg) and os.path.isfile(arg)):
             arg_path = os.path.abspath(arg)
             raise exceptions.UsageError(usage + " Got {}".format(arg_path))
 
+    # Prepare a message about the build configuration.
+    # From gmxapi/CMakeLists.txt, this is "library", "tmpi", or None
+    mpi_type = config().get("gmx_mpi_type")
+    mpi_message = ""
+    if not mpi_type:
+        mpi_message = "Currently using GROMACS that was built with no MPI."
+    elif mpi_type == "tmpi":
+        mpi_message = "Currently using GROMACS that was built with internal thread-MPI."
+    elif mpi_type == "library":
+        mpi_message = (
+            "Currently using GROMACS that was built against an external MPI library."
+        )
+    else:
+        warnings.warn(
+            f"The gmxapi Python package does not recognize the GROMACS library MPI type: {mpi_type}. "
+            "Compatibility checks may be impaired."
+        )
+
     # Note: These are runner parameters, not MD parameters, and should be in the call to gmx.run() instead of here.
     # Reference https://github.com/kassonlab/gmxapi/issues/95
     # Also note that it is not well defined whether or which arguments should be allowed to differ within
     # an ensemble. But to allow parallel trajectory continuation, we have to accept distinct `-cpi` arguments.
     # Note that this violates the traditional gmxapi assumption that all ranks see the same
     # instructions. The "md_sim" element of the gmxapi 0.0.7 workspec ends up being unique
     # to the rank that sees it.
@@ -747,17 +769,27 @@
         del kwargs["-noappend"]
     for arg_key in kwargs:
         if arg_key == "grid" or arg_key == "dd":
             params["grid"] = tuple(kwargs[arg_key])
         elif arg_key == "pme_ranks" or arg_key == "npme":
             params["pme_ranks"] = int(kwargs[arg_key])
         elif arg_key == "threads" or arg_key == "nt":
-            params["threads"] = int(kwargs[arg_key])
+            if mpi_type == "tmpi":
+                params["threads"] = int(kwargs[arg_key])
+            else:
+                raise exceptions.ValueError(
+                    f"'{arg_key}' argument requires thread-MPI GROMACS. " + mpi_message
+                )
         elif arg_key == "tmpi" or arg_key == "ntmpi":
-            params["tmpi"] = int(kwargs[arg_key])
+            if mpi_type == "tmpi":
+                params["tmpi"] = int(kwargs[arg_key])
+            else:
+                raise exceptions.ValueError(
+                    f"'{arg_key}' argument requires thread-MPI GROMACS. " + mpi_message
+                )
         elif arg_key == "threads_per_rank" or arg_key == "ntomp":
             params["threads_per_rank"] = int(kwargs[arg_key])
         elif (
             arg_key == "pme_threads_per_rank"
             or arg_key == "threads_per_pme_rank"
             or arg_key == "ntomp_pme"
         ):
```

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/testsupport.py` & `gmxapi-0.4.1/src/gmxapi/testsupport.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,17 +164,22 @@
 def gmxconfig():
     from .commandline import _config
 
     config = _config()
     yield config
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture(scope="function")
 def mdrun_kwargs(request, gmxconfig):
-    """pytest fixture to provide a mdrun_kwargs dictionary for the mdrun ResourceManager."""
+    """pytest fixture to provide a mdrun_kwargs dictionary for the mdrun ResourceManager.
+
+    .. versionchanged:: 0.4.1
+        Use function scope to avoid unexpectedly mutating the dictionary between tests.
+
+    """
     if gmxconfig is None:
         raise RuntimeError("--threads argument requires a usable gmxconfig.json")
     arg = request.config.getoption("--threads")
     if arg is None:
         return {}
     mpi_type = gmxconfig["gmx_mpi_type"]
     if mpi_type is not None and mpi_type == "tmpi":
```

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/typing.py` & `gmxapi-0.4.1/src/gmxapi/typing.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/utility.py` & `gmxapi-0.4.1/src/gmxapi/utility.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/src/gmxapi/version.py` & `gmxapi-0.4.1/src/gmxapi/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 import warnings
 
 from .exceptions import FeatureNotAvailableError
 
 # TODO(#3851): Version management policy and procedures.
 _major = 0
 _minor = 4
-_micro = 0
-_suffix = "rc2"
+_micro = 1
+_suffix = ""
 
 # Reference https://www.python.org/dev/peps/pep-0440/ and
 # https://packaging.pypa.io/en/latest/version/ for
 # versioning semantics and rules.
 __version__ = "{major}.{minor}.{micro}{suffix}".format(
     major=_major, minor=_minor, micro=_micro, suffix=_suffix
 )
```

### Comparing `gmxapi-0.4.0rc2/src/gmxapi.egg-info/PKG-INFO` & `gmxapi-0.4.1/src/gmxapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmxapi
-Version: 0.4.0rc2
+Version: 0.4.1
 Summary: gmxapi Python interface for GROMACS.
 Home-page: http://gmxapi.org/
 Author: GROMACS gmxapi team
 Author-email: info@gmxapi.org
 License: LGPL
 Requires-Python: >=3.7
 License-File: LICENSE
```

### Comparing `gmxapi-0.4.0rc2/src/gmxapi.egg-info/SOURCES.txt` & `gmxapi-0.4.1/src/gmxapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 src/gmxapi/__init__.py
 src/gmxapi/_logging.py
 src/gmxapi/_transform.py
 src/gmxapi/abc.py
 src/gmxapi/commandline.py
 src/gmxapi/datamodel.py
 src/gmxapi/exceptions.py
-src/gmxapi/gmxconfig.json
 src/gmxapi/gmxconfig.json.in
 src/gmxapi/operation.py
 src/gmxapi/runtime.py
 src/gmxapi/testsupport.py
 src/gmxapi/typing.py
 src/gmxapi/utility.py
 src/gmxapi/version.py
@@ -52,16 +51,19 @@
 src/gmxapi/simulation/context.py
 src/gmxapi/simulation/fileio.py
 src/gmxapi/simulation/mdrun.py
 src/gmxapi/simulation/modify_input.py
 src/gmxapi/simulation/read_tpr.py
 src/gmxapi/simulation/workflow.py
 test/CMakeLists.txt
+test/conftest.py
+test/pytest.ini
 test/test_commandline.py
 test/test_exceptions.py
 test/test_feature_check.py
 test/test_fileio.py
 test/test_fileio_low_level.py
 test/test_mdrun.py
 test/test_operation.py
 test/test_runtime.py
-test/test_subgraph.py
+test/test_subgraph.py
+test/testdata.json
```

### Comparing `gmxapi-0.4.0rc2/test/CMakeLists.txt` & `gmxapi-0.4.1/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/test/test_commandline.py` & `gmxapi-0.4.1/test/test_commandline.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/test/test_exceptions.py` & `gmxapi-0.4.1/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/test/test_feature_check.py` & `gmxapi-0.4.1/test/test_feature_check.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/test/test_fileio.py` & `gmxapi-0.4.1/test/test_fileio.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/test/test_fileio_low_level.py` & `gmxapi-0.4.1/test/test_fileio_low_level.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/test/test_mdrun.py` & `gmxapi-0.4.1/test/test_mdrun.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,43 @@
     # status messages from libgromacs as intended. Ref #4541
     stderr = md.output.stderr.result()
     assert os.path.exists(stderr)
     with open(stderr, "r") as fh:
         assert "starting mdrun" in fh.read()
 
 
+@pytest.mark.skipif(
+    not api_is_at_least(0, 4, 1), reason="runtime_args was refined for gmxapi 0.4.1."
+)
+def test_runtime_args(mdrun_kwargs):
+    import gmxapi._gmxapi as core
+
+    # Check the C++ bindings for our basic set of options.
+    mdargs = core.MDArgs()
+    mdargs.set(mdrun_kwargs)
+
+    # Before gmxapi 0.4.1, a non-string value was not handled properly.
+    mdrun_kwargs["-rdd"] = 2.5
+    mdargs = core.MDArgs()
+    mdargs.set(mdrun_kwargs)
+
+    # Test non-scalar argument value.
+    mdrun_kwargs["-dd"] = (1, 1, 1)
+    mdargs = core.MDArgs()
+    mdargs.set(mdrun_kwargs)
+
+    # Test flag-like argument with no value.
+    mdrun_kwargs["-noappend"] = None
+    mdargs.set(mdrun_kwargs)
+    assert all(arg != "" for arg in mdargs.get_args())
+
+    argstring = " ".join(mdargs.get_args())
+    assert "-dd 1 1 1" in argstring
+
+
 @pytest.mark.usefixtures("cleandir")
 def test_mdrun_runtime_args(spc_water_box, caplog, mdrun_kwargs):
     """Test that *runtime_args* is respected.
 
     When an ensemble is possible, confirm that an array of inputs
     causes each rank to produce a unique simulation with unique output.
     """
```

### Comparing `gmxapi-0.4.0rc2/test/test_operation.py` & `gmxapi-0.4.1/test/test_operation.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/test/test_runtime.py` & `gmxapi-0.4.1/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.0rc2/test/test_subgraph.py` & `gmxapi-0.4.1/test/test_subgraph.py`

 * *Files identical despite different names*

