# Comparing `tmp/g2o-python-0.0.8.tar.gz` & `tmp/g2o-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2o-python-0.0.8.tar", last modified: Mon Jan 30 10:03:12 2023, max compression
+gzip compressed data, was "g2o-python-0.0.9.tar", last modified: Tue Jan 31 06:43:39 2023, max compression
```

## Comparing `g2o-python-0.0.8.tar` & `g2o-python-0.0.9.tar`

### file list

```diff
@@ -1,899 +1,1158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.847976 g2o-python-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-30 10:02:56.000000 g2o-python-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-30 10:02:56.000000 g2o-python-0.0.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-30 10:02:56.000000 g2o-python-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-01-30 10:03:12.847976 g2o-python-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-01-30 10:02:56.000000 g2o-python-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.755976 g2o-python-0.0.8/g2o/
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/.codacy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.747976 g2o-python-0.0.8/g2o/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.755976 g2o-python-0.0.8/g2o/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/.github/workflows/clang-format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    19121 2023-01-30 10:03:12.000000 g2o-python-0.0.8/g2o/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/appveyor.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.755976 g2o-python-0.0.8/g2o/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/benchmarks/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/benchmarks/jacobian_timing_tests.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.755976 g2o-python-0.0.8/g2o/cmake_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/cmake_modules/CheckIfUnderscorePrefixedBesselFunctionsExist.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/cmake_modules/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/cmake_modules/FindCSparse.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/cmake_modules/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/cmake_modules/FindG2O.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/cmake_modules/FindMETIS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/cmake_modules/FindQGLViewer.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    21756 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/cmake_modules/FindSuiteSparse.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.759976 g2o-python-0.0.8/g2o/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.759976 g2o-python-0.0.8/g2o/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (123)    75536 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/doxygen/doxy.config
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/doxygen/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)   485883 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/g2o.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    67650 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/g2o.tex
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/license-bsd.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/license-gpl.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/license-lgpl.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.759976 g2o-python-0.0.8/g2o/doc/pics/
--rw-r--r--   0 runner    (1001) docker     (123)   108786 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/pics/classes.eps
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/pics/classes.fig
--rw-r--r--   0 runner    (1001) docker     (123)    22733 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/pics/classes.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/pics/hgraph.eps
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/pics/hgraph.fig
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/pics/slam.eps
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/pics/slam.fig
--rw-r--r--   0 runner    (1001) docker     (123)   536942 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/pics/viewer.eps
--rw-r--r--   0 runner    (1001) docker     (123)   309182 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/pics/viewer.png
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/doc/robots.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.759976 g2o-python-0.0.8/g2o/g2o/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.759976 g2o-python-0.0.8/g2o/g2o/EXTERNAL/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/EXTERNAL/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.763976 g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/freeglut_font.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/freeglut_minimal.h
--rw-r--r--   0 runner    (1001) docker     (123)    58082 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/freeglut_stroke_mono_roman.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/freeglut_stroke_roman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.763976 g2o-python-0.0.8/g2o/g2o/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.763976 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/dl_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/dl_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)    26200 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/g2o.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/g2o_cli_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/g2o_common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/g2o_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/output_helper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/output_helper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.763976 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/backbone_tree_action.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/backbone_tree_action.h
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_creator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_creator.h
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_labeler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_labeler.h
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_types_cost_function.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_types_cost_function.h
--rw-r--r--   0 runner    (1001) docker     (123)    20323 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical_test_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/simple_star_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/simple_star_ops.h
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/star.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/star.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.771976 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/convertSegmentLine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/g2o_anonymize_observations.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/g2o_simulator_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/pointsensorparameters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/pointsensorparameters.h
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_line3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_line3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry.h
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy_bearing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy_bearing.h
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy_offset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz.h
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_depth.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_depth.h
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_disparity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_disparity.h
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose3d_offset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose3d_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_se3_prior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_se3_prior.h
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d_line.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d_line.h
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d_pointline.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d_pointline.h
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator2d_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator2d_segment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator3d_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simutils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simutils.h
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/test_simulator2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/test_simulator3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.771976 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/base_main_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/base_properties_widget.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/g2o_qglviewer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/g2o_qglviewer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/g2o_viewer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/g2o_viewer_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/gui_hyper_graph_action.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/gui_hyper_graph_action.h
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/main_window.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/main_window.h
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/properties_widget.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/properties_widget.h
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/run_g2o_viewer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/run_g2o_viewer.h
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/stream_redirect.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/stream_redirect.h
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/viewer_properties_widget.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/viewer_properties_widget.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.771976 g2o-python-0.0.8/g2o/g2o/apps/linked_binaries/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/apps/linked_binaries/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.775976 g2o-python-0.0.8/g2o/g2o/autodiff/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/array_selector.h
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/autodiff.h
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/disable_warnings.h
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/fixed_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/integer_sequence_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (123)    34207 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/jet.h
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/parameter_dims.h
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/reenable_warnings.h
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/autodiff/variadic_evaluate.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.783976 g2o-python-0.0.8/g2o/g2o/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/auto_differentiation.h
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_binary_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_dynamic_vertex.h
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_fixed_sized_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_fixed_sized_edge.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_multi_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_unary_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_variable_sized_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_variable_sized_edge.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_vertex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/base_vertex.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/batch_stats.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/batch_stats.h
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/block_solver.h
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/block_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/cache.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/cache.h
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/creators.h
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/dynamic_aligned_buffer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/eigen_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     9578 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/estimate_propagator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/estimate_propagator.h
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/factory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/factory.h
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/g2o_core_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/hyper_dijkstra.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/hyper_dijkstra.h
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/hyper_graph.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/hyper_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/hyper_graph_action.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/hyper_graph_action.h
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/io_helper.h
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/jacobian_workspace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/jacobian_workspace.h
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/linear_solver.h
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/marginal_covariance_cholesky.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/marginal_covariance_cholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/matrix_operations.h
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/matrix_structure.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/matrix_structure.h
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/openmp_mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)    27099 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimizable_graph.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28390 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimizable_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_dogleg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_dogleg.h
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_gauss_newton.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_gauss_newton.h
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_levenberg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_levenberg.h
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_property.h
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_with_hessian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_with_hessian.h
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/parameter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/parameter.h
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/parameter_container.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/parameter_container.h
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/robust_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/robust_kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/robust_kernel_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/robust_kernel_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/robust_kernel_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/robust_kernel_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/solver.h
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/sparse_block_matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/sparse_block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/sparse_block_matrix_ccs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/sparse_block_matrix_diagonal.h
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/sparse_optimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/sparse_optimizer.h
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/sparse_optimizer_terminate_action.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/core/sparse_optimizer_terminate_action.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.783976 g2o-python-0.0.8/g2o/g2o/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.783976 g2o-python-0.0.8/g2o/g2o/examples/ba/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/ba/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/ba/ba_demo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.783976 g2o-python-0.0.8/g2o/g2o/examples/ba_anchored_inverse_depth/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/ba_anchored_inverse_depth/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/ba_anchored_inverse_depth/ba_anchored_inverse_depth_demo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.783976 g2o-python-0.0.8/g2o/g2o/examples/bal/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/bal/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/bal/bal_example.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.787976 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/closed_form_calibration.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/closed_form_calibration.h
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/edge_se2_pure_calib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/edge_se2_pure_calib.h
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/g2o_calibration_odom_laser_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/gm2dl_io.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/gm2dl_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/motion_information.h
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_laser_calib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_odom_laser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_pure_calibration.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.787976 g2o-python-0.0.8/g2o/g2o/examples/data_convert/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/data_convert/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/data_convert/convert_sba_slam3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.787976 g2o-python-0.0.8/g2o/g2o/examples/data_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/data_fitting/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/data_fitting/circle_fit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/data_fitting/curve_fit.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.787976 g2o-python-0.0.8/g2o/g2o/examples/dynamic_vertex/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/dynamic_vertex/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/dynamic_vertex/polynomial_fit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/dynamic_vertex/static_dynamic_function_fit.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.787976 g2o-python-0.0.8/g2o/g2o/examples/g2o_unfold/
--rw-r--r--   0 runner    (1001) docker     (123)    35161 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/g2o_unfold/g2o-unfold.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/g2o_unfold/tools.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/g2o_unfold/tools.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.787976 g2o-python-0.0.8/g2o/g2o/examples/icp/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/icp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/icp/gicp-test1.dat
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/icp/gicp_demo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/icp/gicp_sba_demo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.787976 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.787976 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/g2o_incremental.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/g2o_incremental_api.h
--rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/graph_optimizer_sparse_incremental.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/graph_optimizer_sparse_incremental.h
--rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/linear_solver_cholmod_online.h
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/protocol.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.791976 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/fast_output.h
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_interactive_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_online.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_slam_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_slam_interface.h
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/generate_commands.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/graph_optimizer_sparse_online.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/graph_optimizer_sparse_online.h
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/protocol.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/types_online.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/types_slam2d_online.h
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/types_slam3d_online.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.791976 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.791976 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/example/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/example/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/example/example_slam_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/example/example_slam_interface.h
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/example/test_slam_interface.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.791976 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/abstract_slam_interface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/parser_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/parser_interface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/slam_context_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/slam_context_interface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.795976 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/FlexLexer.h
--rw-r--r--   0 runner    (1001) docker     (123)    41636 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/bison_parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22144 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/bison_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/commands.h
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/driver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/driver.h
--rw-r--r--   0 runner    (1001) docker     (123)    49599 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/flex_scanner.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/grammar.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/location.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/parser.yy
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/position.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/scanner.h
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/scanner.l
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/slam_context.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/slam_context.h
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/stack.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/test_slam_parser.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.795976 g2o-python-0.0.8/g2o/g2o/examples/line_slam/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/line_slam/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/line_slam/line_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/line_slam/simulator_3d_line.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.795976 g2o-python-0.0.8/g2o/g2o/examples/plane_slam/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/plane_slam/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/plane_slam/plane_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/plane_slam/simulator_3d_plane.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.795976 g2o-python-0.0.8/g2o/g2o/examples/sba/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/sba/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/sba/sba_demo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.795976 g2o-python-0.0.8/g2o/g2o/examples/sim3/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/sim3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/sim3/optimize_sphere_by_sim3.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.795976 g2o-python-0.0.8/g2o/g2o/examples/simple_optimize/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/simple_optimize/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/simple_optimize/simple_optimize.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.795976 g2o-python-0.0.8/g2o/g2o/examples/slam2d/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/slam2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/slam2d/base_main_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/slam2d/main_window.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/slam2d/main_window.h
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/slam2d/slam2d_g2o.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/slam2d/slam2d_viewer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/slam2d/slam2d_viewer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.795976 g2o-python-0.0.8/g2o/g2o/examples/sphere/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/sphere/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/sphere/create_sphere.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.795976 g2o-python-0.0.8/g2o/g2o/examples/target/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/target/constant_velocity_target.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/target/continuous_to_discrete.h
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/target/static_target.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/target/targetTypes3D.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/target/targetTypes6D.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.799976 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/edge_se2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/edge_se2.h
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/edge_se2_pointxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/edge_se2_pointxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/g2o_tutorial_slam2d_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/parameter_se2_offset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/parameter_se2_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/se2.h
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/simulator.h
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/tutorial_slam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/types_tutorial_slam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/types_tutorial_slam2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/vertex_point_xy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/vertex_point_xy.h
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/vertex_se2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/vertex_se2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.799976 g2o-python-0.0.8/g2o/g2o/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.799976 g2o-python-0.0.8/g2o/g2o/solvers/cholmod/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/cholmod/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/cholmod/cholmod_ext.h
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/cholmod/cholmod_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/cholmod/cholmod_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/cholmod/linear_solver_cholmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/cholmod/solver_cholmod.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.799976 g2o-python-0.0.8/g2o/g2o/solvers/csparse/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_extension.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_extension.h
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_helper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_helper.h
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/g2o_csparse_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/g2o_csparse_extension_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/linear_solver_csparse.h
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/csparse/solver_csparse.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.803976 g2o-python-0.0.8/g2o/g2o/solvers/dense/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/dense/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/dense/linear_solver_dense.h
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/dense/solver_dense.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.803976 g2o-python-0.0.8/g2o/g2o/solvers/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/eigen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/eigen/linear_solver_eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/eigen/solver_eigen.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.803976 g2o-python-0.0.8/g2o/g2o/solvers/pcg/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/pcg/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/pcg/linear_solver_pcg.h
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/pcg/linear_solver_pcg.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/pcg/solver_pcg.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.803976 g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/g2o_slam2d_linear_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/slam2d_linear.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/solver_slam2d_linear.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/solver_slam2d_linear.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.803976 g2o-python-0.0.8/g2o/g2o/solvers/structure_only/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/structure_only/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/structure_only/structure_only.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/solvers/structure_only/structure_only_solver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.807976 g2o-python-0.0.8/g2o/g2o/stuff/
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/color_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/command_args.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/command_args.h
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/filesys_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/filesys_tools.h
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/g2o_stuff_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/misc.h
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/opengl_primitives.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/opengl_primitives.h
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/opengl_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/os_specific.c
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/os_specific.h
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/property.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/property.h
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/sampler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/sampler.h
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/sparse_helper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/sparse_helper.h
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/string_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/string_tools.h
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/tictoc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/tictoc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/timeutil.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/timeutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/tuple_tools.h
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/stuff/unscented.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.807976 g2o-python-0.0.8/g2o/g2o/types/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.807976 g2o-python-0.0.8/g2o/g2o/types/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/data_queue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/data_queue.h
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/g2o_types_data_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/laser_parameters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/laser_parameters.h
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/raw_laser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/raw_laser.h
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/robot_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/robot_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/robot_laser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/robot_laser.h
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/types_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/types_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/vertex_ellipse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/vertex_ellipse.h
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/vertex_tag.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/data/vertex_tag.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.807976 g2o-python-0.0.8/g2o/g2o/types/icp/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/icp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/icp/g2o_types_icp_api.h
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/icp/types_icp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/icp/types_icp.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.815976 g2o-python-0.0.8/g2o/g2o/types/sba/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_p2mc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_p2mc.h
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_p2sc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_p2sc.h
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_psi2uv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_psi2uv.h
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_stereo_xyz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_stereo_xyz.h
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_stereo_xyz_onlypose.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_stereo_xyz_onlypose.h
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz.h
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz2uv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz2uv.h
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz2uvu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz2uvu.h
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz_onlypose.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz_onlypose.h
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_sba_cam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_sba_cam.h
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_sba_scale.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_sba_scale.h
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_se3_expmap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/edge_se3_expmap.h
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/g2o_types_sba_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/parameter_cameraparameters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/parameter_cameraparameters.h
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/sba_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/sbacam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/sbacam.h
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/types_sba.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/types_sba.h
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/types_six_dof_expmap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/types_six_dof_expmap.h
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/vertex_cam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/vertex_cam.h
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/vertex_intrinsics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/vertex_intrinsics.h
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/vertex_se3_expmap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sba/vertex_se3_expmap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.815976 g2o-python-0.0.8/g2o/g2o/types/sclam2d/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/edge_se2_odom_differential_calib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/edge_se2_odom_differential_calib.h
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/edge_se2_sensor_calib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/edge_se2_sensor_calib.h
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/g2o_types_sclam2d_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/odometry_measurement.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/odometry_measurement.h
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/types_sclam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/types_sclam2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/vertex_odom_differential_params.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sclam2d/vertex_odom_differential_params.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.815976 g2o-python-0.0.8/g2o/g2o/types/sim3/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sim3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sim3/sim3.h
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sim3/types_seven_dof_expmap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/sim3/types_seven_dof_expmap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.819976 g2o-python-0.0.8/g2o/g2o/types/slam2d/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_pointxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_pointxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2.h
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_lotsofxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_lotsofxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_offset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_bearing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_bearing.h
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_calib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_calib.h
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_offset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_prior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_prior.h
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_twopointsxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_twopointsxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_xyprior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_xyprior.h
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_xy_prior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_xy_prior.h
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/g2o_types_slam2d_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/parameter_se2_offset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/parameter_se2_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/se2.h
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/types_slam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/types_slam2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/vertex_point_xy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/vertex_point_xy.h
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/vertex_se2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d/vertex_se2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.823976 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_line2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_line2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_line2d_pointxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_line2d_pointxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_line2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_line2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_line.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_line.h
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_pointLine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_pointLine.h
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/g2o_types_slam2d_addons_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/line_2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/types_slam2d_addons.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/types_slam2d_addons.h
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/vertex_line2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/vertex_line2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/vertex_segment2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/vertex_segment2d.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.827976 g2o-python-0.0.8/g2o/g2o/types/slam3d/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/dquat2mat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/dquat2mat.h
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/dquat2mat.wxm
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/dquat2mat_maxima_generated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_pointxyz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_pointxyz.h
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3.h
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_lotsofxyz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_lotsofxyz.h
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_offset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz.h
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz_depth.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz_depth.h
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz_disparity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz_disparity.h
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_prior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_prior.h
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_xyzprior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_xyzprior.h
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_xyz_prior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_xyz_prior.h
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/g2o_types_slam3d_api.h
--rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/isometry3d_gradients.h
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/isometry3d_mappings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/isometry3d_mappings.h
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_camera.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_camera.h
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_se3_offset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_se3_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_stereo_camera.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_stereo_camera.h
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/se3_ops.h
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/se3_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/se3quat.h
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/types_slam3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/types_slam3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/vertex_pointxyz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/vertex_pointxyz.h
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/vertex_se3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d/vertex_se3.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.831976 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_plane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_plane.h
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_calib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_calib.h
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_euler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_euler.h
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_line.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_line.h
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_plane_calib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_plane_calib.h
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/g2o_types_slam3d_addons_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/line3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/line3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/plane3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/types_slam3d_addons.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/types_slam3d_addons.h
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_line3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_line3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_plane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_plane.h
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_se3_euler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_se3_euler.h
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/g2o/what_is_in_these_directories.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.831976 g2o-python-0.0.8/g2o/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.835976 g2o-python-0.0.8/g2o/python/core/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_base_binary_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_base_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_base_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_base_fixed_sized_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_base_unary_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_base_variable_sized_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_base_variable_sized_edge.h
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_base_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_base_vertex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_batch_stats.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_batch_stats.h
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_block_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_block_solver.h
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_core.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_core.h
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_eigen_types.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_eigen_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_estimate_propagator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_estimate_propagator.h
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_hyper_dijkstra.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_hyper_dijkstra.h
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_hyper_graph.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_hyper_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_hyper_graph_action.h
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_jacobian_workspace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_jacobian_workspace.h
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_linear_solver.h
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_optimizable_graph.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_optimizable_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_optimization_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_optimization_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_parameter.h
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_robust_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_robust_kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_solver.h
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_sparse_block_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_sparse_block_matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_sparse_optimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_sparse_optimizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/core/py_sparse_optimizer_terminate_action.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.835976 g2o-python-0.0.8/g2o/python/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/examples/ba_anchored_inverse_depth_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/examples/ba_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/examples/gicp_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/examples/gicp_sba_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/examples/notebook_slam2d.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/examples/sba_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/examples/sba_demo2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/examples/simple_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/examples/type_in_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/g2opy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/g2opy.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.835976 g2o-python-0.0.8/g2o/python/types/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.835976 g2o-python-0.0.8/g2o/python/types/icp/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/icp/py_types_icp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/icp/py_types_icp.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.835976 g2o-python-0.0.8/g2o/python/types/pure/
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/pure/py_types_pure.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/pure/py_types_pure.h
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/py_types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.835976 g2o-python-0.0.8/g2o/python/types/sba/
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sba/py_sbacam.h
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sba/py_types_sba.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sba/py_types_sba.h
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sba/py_types_six_dof_expmap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sba/py_types_six_dof_expmap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.839976 g2o-python-0.0.8/g2o/python/types/sclam2d/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sclam2d/py_edge_se2_odom_differential_calib.h
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sclam2d/py_edge_se2_sensor_calib.h
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sclam2d/py_odometry_measurement.h
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sclam2d/py_types_sclam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sclam2d/py_types_sclam2d.h
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sclam2d/py_vertex_odom_differential_params.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.839976 g2o-python-0.0.8/g2o/python/types/sim3/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sim3/py_sim3.h
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sim3/py_types_seven_dof_expmap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/sim3/py_types_seven_dof_expmap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.839976 g2o-python-0.0.8/g2o/python/types/slam2d/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam2d/py_edge_pointxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam2d/py_edge_se2.h
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam2d/py_edge_se2_pointxy.h
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam2d/py_parameter_se2_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam2d/py_se2.h
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam2d/py_types_slam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam2d/py_types_slam2d.h
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam2d/py_vertex_point_xy.h
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam2d/py_vertex_se2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.839976 g2o-python-0.0.8/g2o/python/types/slam3d/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam3d/py_edge_pointxyz.h
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam3d/py_edge_se3.h
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam3d/py_edge_se3_pointxyz.h
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam3d/py_parameter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam3d/py_se3quat.h
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam3d/py_types_slam3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam3d/py_types_slam3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam3d/py_vertex_pointxyz.h
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/python/types/slam3d/py_vertex_se3.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.839976 g2o-python-0.0.8/g2o/script/
--rw-r--r--   0 runner    (1001) docker     (123)    82300 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/script/android.toolchain.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/script/codecov.sh.in
--rwxr-xr-x   0 runner    (1001) docker     (123)    21520 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/script/git-clang-format.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/script/install-deps-linux.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      191 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/script/install-deps-osx.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/script/install-deps-windows.bat
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/script/run-style-check-diff.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.839976 g2o-python-0.0.8/g2o/unit_test/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.843976 g2o-python-0.0.8/g2o/unit_test/data/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/data/data_queue_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/data/io_data.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.843976 g2o-python-0.0.8/g2o/unit_test/general/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/general/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/general/auto_diff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/general/base_fixed_sized_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/general/clear_and_redo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/general/graph_operations.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/general/robust_kernel_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/general/sparse_block_matrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.843976 g2o-python-0.0.8/g2o/unit_test/sba/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sba/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sba/io_sba.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sba/io_six_dof_expmap.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.843976 g2o-python-0.0.8/g2o/unit_test/sclam2d/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sclam2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sclam2d/io_sclam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sclam2d/odom_convert_sclam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sclam2d/sensor_offset.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.843976 g2o-python-0.0.8/g2o/unit_test/sim3/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sim3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sim3/allocate_sim3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sim3/io_sim3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/sim3/jacobians_sim3.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.843976 g2o-python-0.0.8/g2o/unit_test/slam2d/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam2d/io_slam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam2d/jacobians_slam2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam2d/mappings_se2.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.843976 g2o-python-0.0.8/g2o/unit_test/slam2d_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam2d_addons/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam2d_addons/io_slam2d_addons.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.843976 g2o-python-0.0.8/g2o/unit_test/slam3d/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam3d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam3d/io_slam3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam3d/jacobians_slam3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam3d/mappings_slam3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam3d/optimization_slam3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam3d/orthogonal_matrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.843976 g2o-python-0.0.8/g2o/unit_test/slam3d_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam3d_addons/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/slam3d_addons/io_slam3d_addons.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.847976 g2o-python-0.0.8/g2o/unit_test/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/solver/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/solver/allocate_algorithm_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/solver/linear_solver_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    40579 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/solver/sparse_system_helper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/solver/sparse_system_helper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.847976 g2o-python-0.0.8/g2o/unit_test/stuff/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/stuff/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/stuff/command_args_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/stuff/filesys_tools_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/stuff/misc_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/stuff/property_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/stuff/string_tools_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/stuff/tuple_tools_tests.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.847976 g2o-python-0.0.8/g2o/unit_test/test_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/test_helper/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/test_helper/allocate_optimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/test_helper/allocate_optimizer.h
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/test_helper/evaluate_jacobian.h
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/test_helper/g2o_test_helper_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/test_helper/io.h
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/test_helper/random_state.h
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-30 10:02:58.000000 g2o-python-0.0.8/g2o/unit_test/test_helper/test_main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.847976 g2o-python-0.0.8/g2o_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-01-30 10:03:12.000000 g2o-python-0.0.8/g2o_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33615 2023-01-30 10:03:12.000000 g2o-python-0.0.8/g2o_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 10:03:12.000000 g2o-python-0.0.8/g2o_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-30 10:03:12.000000 g2o-python-0.0.8/g2o_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 10:03:12.000000 g2o-python-0.0.8/g2o_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 10:03:12.847976 g2o-python-0.0.8/g2opy/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-30 10:02:56.000000 g2o-python-0.0.8/g2opy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-30 10:02:56.000000 g2o-python-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 10:03:12.847976 g2o-python-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-01-30 10:02:56.000000 g2o-python-0.0.8/setup.py
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.716244 g2o-python-0.0.9/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      864 2023-01-16 15:13:37.000000 g2o-python-0.0.9/.gitignore
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       76 2023-01-16 14:48:13.000000 g2o-python-0.0.9/.gitmodules
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1070 2023-01-18 15:13:04.000000 g2o-python-0.0.9/LICENSE
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2779 2023-01-31 06:43:39.712244 g2o-python-0.0.9/PKG-INFO
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1379 2023-01-31 06:42:39.000000 g2o-python-0.0.9/README.md
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.600243 g2o-python-0.0.9/_skbuild/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.600243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.604243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.608243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/g2o/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       34 2023-01-31 06:37:54.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/g2o/__init__.py
+-rw-r--r--   0 miquel    (1000) miquel    (1000)  4145088 2023-01-31 06:13:00.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/g2o/g2opy.cpython-310-x86_64-linux-gnu.so
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.616243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/g2opy/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)  4145088 2023-01-31 06:07:59.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/g2opy/g2opy.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0 miquel    (1000) miquel    (1000)  4145088 2023-01-31 06:37:54.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/g2opy.cpython-310-x86_64-linux-gnu.so
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.600243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.620243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.620243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1554 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/LICENSE
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3611 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/array_selector.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    14450 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/autodiff.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2220 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/disable_warnings.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3239 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/eigen.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    17116 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/fixed_array.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     6505 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/integer_sequence_algorithm.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    34207 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/jet.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3069 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/memory.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5174 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/parameter_dims.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1854 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/reenable_warnings.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2760 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/types.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5032 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/variadic_evaluate.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)      771 2023-01-31 06:00:18.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/config.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.624243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    13198 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/auto_differentiation.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2348 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_binary_edge.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3215 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_dynamic_vertex.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     6973 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_edge.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    12019 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_fixed_sized_edge.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     9500 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_fixed_sized_edge.hpp
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1667 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_multi_edge.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2073 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_unary_edge.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4103 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_variable_sized_edge.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     6846 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_variable_sized_edge.hpp
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4423 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_vertex.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2285 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_vertex.hpp
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3786 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/batch_stats.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     7730 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/block_solver.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    21317 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/block_solver.hpp
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3723 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/cache.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2678 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/creators.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1466 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/dynamic_aligned_buffer.hpp
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3783 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/eigen_types.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     6544 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/estimate_propagator.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5438 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/factory.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)      862 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/g2o_core_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5448 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/hyper_dijkstra.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    10802 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/hyper_graph.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     8068 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/hyper_graph_action.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1984 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/io_helper.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3493 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/jacobian_workspace.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     6768 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/linear_solver.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4128 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/marginal_covariance_cholesky.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3391 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/matrix_operations.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2769 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/matrix_structure.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2834 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/openmp_mutex.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    28390 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimizable_graph.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4230 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3552 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_dogleg.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     7653 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_factory.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2211 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_gauss_newton.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4005 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_levenberg.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2660 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_property.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2696 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_with_hessian.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2161 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/parameter.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2646 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/parameter_container.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2744 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/robust_kernel.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4946 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/robust_kernel_factory.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5279 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/robust_kernel_impl.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5151 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/solver.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    10152 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_block_matrix.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    24718 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_block_matrix.hpp
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    10276 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_block_matrix_ccs.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4106 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_block_matrix_diagonal.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    12655 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_optimizer.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2717 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_optimizer_terminate_action.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.600243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.624243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/cholmod/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2887 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/cholmod/cholmod_wrapper.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     8062 2023-01-30 09:49:37.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/cholmod/linear_solver_cholmod.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.624243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1816 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/csparse_extension.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1888 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/csparse_helper.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2968 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/csparse_wrapper.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2372 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/g2o_csparse_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1242 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/g2o_csparse_extension_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     6657 2023-01-30 09:49:37.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/linear_solver_csparse.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.624243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/dense/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3655 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/dense/linear_solver_dense.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.624243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/eigen/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     8432 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/eigen/linear_solver_eigen.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.624243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/pcg/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3499 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/pcg/linear_solver_pcg.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     7334 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/pcg/linear_solver_pcg.hpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.624243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/slam2d_linear/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2377 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/slam2d_linear/g2o_slam2d_linear_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2763 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/slam2d_linear/solver_slam2d_linear.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.624243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/structure_only/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     8461 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/structure_only/structure_only_solver.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.628243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2595 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/color_macros.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4557 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/command_args.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3256 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/filesys_tools.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2308 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/g2o_stuff_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4350 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/macros.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5186 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/misc.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4200 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/opengl_primitives.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1676 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/opengl_wrapper.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1887 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/os_specific.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4923 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/property.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4118 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/sampler.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3063 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/sparse_helper.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5108 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/string_tools.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2432 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/tictoc.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4087 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/timeutil.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2106 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/tuple_tools.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3699 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/unscented.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.600243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.628243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2108 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/data_queue.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2347 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/g2o_types_data_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2253 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/laser_parameters.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2870 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/raw_laser.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2499 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/robot_data.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3022 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/robot_laser.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1560 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/types_data.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3412 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/vertex_ellipse.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2814 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/vertex_tag.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.628243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/icp/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2315 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/icp/g2o_types_icp_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    11207 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/icp/types_icp.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.628243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2193 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_p2mc.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2166 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_p2sc.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2188 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_psi2uv.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2557 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_stereo_xyz.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2205 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_stereo_xyz_onlypose.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2141 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_xyz.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2147 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_xyz2uv.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2189 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_xyz2uvu.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2172 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_xyz_onlypose.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2519 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_sba_cam.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2323 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_sba_scale.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1976 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_se3_expmap.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2339 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/g2o_types_sba_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2161 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/parameter_cameraparameters.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2561 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/sba_utils.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3345 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/sbacam.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1775 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/types_sba.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2092 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/types_six_dof_expmap.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3246 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/vertex_cam.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2044 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/vertex_intrinsics.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2079 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/vertex_se3_expmap.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.628243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3217 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/edge_se2_odom_differential_calib.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3446 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/edge_se2_sensor_calib.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2371 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/g2o_types_sclam2d_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3442 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/odometry_measurement.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1566 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/types_sclam2d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2050 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/vertex_odom_differential_params.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.628243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sim3/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     8355 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sim3/sim3.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     6037 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sim3/types_seven_dof_expmap.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.632243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2945 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_pointxy.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4177 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2592 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_lotsofxy.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3089 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_offset.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3789 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_pointxy.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3844 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_pointxy_bearing.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2733 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_pointxy_calib.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3098 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_pointxy_offset.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2923 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_prior.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2339 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_twopointsxy.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2484 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_xyprior.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2730 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_xy_prior.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2363 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/g2o_types_slam2d_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3561 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/parameter_se2_offset.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3675 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/se2.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1964 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/types_slam2d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3482 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/vertex_point_xy.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3757 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/vertex_se2.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.632243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3022 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_line2d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3208 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_line2d_pointxy.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3644 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_se2_line2d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5044 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_se2_segment2d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4960 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_se2_segment2d_line.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     4081 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_se2_segment2d_pointLine.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2419 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/g2o_types_slam2d_addons_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2069 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/line_2d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1806 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/types_slam2d_addons.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3542 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/vertex_line2d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3931 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/vertex_segment2d.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.632243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2138 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/dquat2mat.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2962 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_pointxyz.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3808 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2578 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_lotsofxyz.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2454 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_offset.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3442 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_pointxyz.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3052 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_pointxyz_depth.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3613 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_pointxyz_disparity.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3216 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_prior.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2861 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_xyzprior.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2745 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_xyz_prior.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2363 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/g2o_types_slam3d_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    11153 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/isometry3d_gradients.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5443 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/isometry3d_mappings.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3312 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/parameter_camera.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3554 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/parameter_se3_offset.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2085 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/parameter_stereo_camera.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2016 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/se3_ops.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2239 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/se3_ops.hpp
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     8036 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/se3quat.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2124 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/types_slam3d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3638 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/vertex_pointxyz.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     5524 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/vertex_se3.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.636243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2768 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_plane.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2310 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_se3_calib.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1975 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_se3_euler.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3190 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_se3_line.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3192 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_se3_plane_calib.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1972 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/g2o_types_slam3d_addons_api.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     6561 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/line3d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     3886 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/plane3d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     1905 2023-01-16 14:48:13.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/types_slam3d_addons.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2926 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/vertex_line3d.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2938 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/vertex_plane.h
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2017 2023-01-16 15:07:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/vertex_se3_euler.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.644243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.600243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/cmake/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.644243 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/cmake/g2o/
+-rw-r--r--   0 miquel    (1000) miquel    (1000)      167 2023-01-31 06:00:18.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/cmake/g2o/g2oConfig.cmake
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     2878 2023-01-31 06:00:18.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/cmake/g2o/g2oConfigVersion.cmake
+-rw-r--r--   0 miquel    (1000) miquel    (1000)     9978 2023-01-31 06:00:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/cmake/g2o/g2oTargets-release.cmake
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    10118 2023-01-31 06:00:22.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/cmake/g2o/g2oTargets.cmake
+-rw-r--r--   0 miquel    (1000) miquel    (1000)  1333006 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_core.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    11338 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_csparse_extension.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   668968 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_solver_cholmod.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   666662 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_solver_csparse.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   568918 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_solver_dense.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   714930 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_solver_eigen.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   628538 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_solver_pcg.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   365290 2023-01-31 06:36:51.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_solver_slam2d_linear.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)    72610 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_solver_structure_only.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   228548 2023-01-31 06:36:49.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_stuff.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   118696 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_types_data.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   150622 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_types_icp.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)  1294160 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_types_sba.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   309306 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_types_sclam2d.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   196662 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_types_sim3.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)  1246652 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_types_slam2d.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   664908 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_types_slam2d_addons.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)  1204548 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_types_slam3d.a
+-rw-r--r--   0 miquel    (1000) miquel    (1000)   617620 2023-01-31 06:36:50.000000 g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/lib/libg2o_types_slam3d_addons.a
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.648244 g2o-python-0.0.9/g2o/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5676 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/.clang-format
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5027 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/.clang-tidy
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      258 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/.codacy.yaml
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.600243 g2o-python-0.0.9/g2o/.github/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.648244 g2o-python-0.0.9/g2o/.github/workflows/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2319 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/.github/workflows/ci.yml
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      746 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/.github/workflows/clang-format.yml
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2172 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/.github/workflows/windows.yml
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       40 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/.gitignore
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    19121 2023-01-31 06:43:39.000000 g2o-python-0.0.9/g2o/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      347 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/Makefile
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7633 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/README.md
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       34 2023-01-31 06:43:39.000000 g2o-python-0.0.9/g2o/__init__.py
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1074 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/appveyor.yml
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.648244 g2o-python-0.0.9/g2o/benchmarks/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      166 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/benchmarks/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     9825 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/benchmarks/jacobian_timing_tests.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.648244 g2o-python-0.0.9/g2o/cmake_modules/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2599 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/cmake_modules/CheckIfUnderscorePrefixedBesselFunctionsExist.cmake
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      182 2023-01-30 09:49:37.000000 g2o-python-0.0.9/g2o/cmake_modules/Config.cmake.in
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      618 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/cmake_modules/FindCSparse.cmake
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3509 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/cmake_modules/FindEigen3.cmake
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3277 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/cmake_modules/FindG2O.cmake
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4103 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/cmake_modules/FindMETIS.cmake
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1478 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/cmake_modules/FindQGLViewer.cmake
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    21756 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/cmake_modules/FindSuiteSparse.cmake
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      116 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/codecov.yml
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      788 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/config.h.in
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.652243 g2o-python-0.0.9/g2o/doc/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       55 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/.gitignore
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      113 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/Makefile
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.652243 g2o-python-0.0.9/g2o/doc/doxygen/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    75536 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/doxygen/doxy.config
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      121 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/doxygen/readme.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)   485883 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/g2o.pdf
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    67650 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/g2o.tex
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1400 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/license-bsd.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    35147 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/license-gpl.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7637 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/license-lgpl.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.656244 g2o-python-0.0.9/g2o/doc/pics/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)   108786 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/pics/classes.eps
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5188 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/pics/classes.fig
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    22733 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/pics/classes.svg
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5757 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/pics/hgraph.eps
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2944 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/pics/hgraph.fig
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6767 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/pics/slam.eps
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3069 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/pics/slam.fig
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)   536942 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/pics/viewer.eps
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)   309182 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/pics/viewer.png
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2435 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/doc/robots.bib
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.656244 g2o-python-0.0.9/g2o/g2o/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       11 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/.gitignore
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      592 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/CMakeLists.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.656244 g2o-python-0.0.9/g2o/g2o/EXTERNAL/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       58 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/EXTERNAL/CMakeLists.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.656244 g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1026 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1439 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/COPYING
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4632 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/freeglut_font.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3168 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/freeglut_minimal.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    58082 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/freeglut_stroke_mono_roman.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    56335 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/freeglut_stroke_roman.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.656244 g2o-python-0.0.9/g2o/g2o/apps/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      416 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/CMakeLists.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.656244 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2242 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4100 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/dl_wrapper.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2440 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/dl_wrapper.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    26200 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/g2o.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2312 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/g2o_cli_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5385 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/g2o_common.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2003 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/g2o_common.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6860 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/output_helper.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2201 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/output_helper.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.660244 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1409 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4189 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/backbone_tree_action.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4627 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/backbone_tree_action.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3584 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_creator.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4594 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_creator.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8857 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_labeler.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4002 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_labeler.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2322 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_types_cost_function.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2591 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_types_cost_function.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    20323 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1923 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6004 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical_test_functions.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    16047 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/simple_star_ops.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2948 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/simple_star_ops.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4479 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/star.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4512 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/star.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.664244 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3082 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10174 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/convertSegmentLine.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4096 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/g2o_anonymize_observations.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2327 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/g2o_simulator_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1937 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/pointsensorparameters.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2207 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/pointsensorparameters.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3649 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_line3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2208 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_line3d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2553 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2601 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1907 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2805 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1866 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry3d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2937 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1988 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3040 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy_bearing.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2025 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy_bearing.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3557 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy_offset.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2188 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy_offset.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3486 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2239 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3496 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_depth.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2265 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_depth.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3562 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_disparity.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2312 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_disparity.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3252 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2197 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3480 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2195 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose3d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3975 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose3d_offset.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2441 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose3d_offset.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2799 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_se3_prior.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2177 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_se3_prior.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3676 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2109 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3682 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d_line.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2131 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d_line.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3843 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d_pointline.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2207 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d_pointline.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3182 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     9102 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1775 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1862 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator2d_base.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8726 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator2d_segment.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1708 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator3d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1858 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator3d_base.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4277 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simutils.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2373 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simutils.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8949 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/test_simulator2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8367 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/test_simulator3d.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.664244 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2305 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    11847 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/base_main_window.ui
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2038 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/base_properties_widget.ui
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4406 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/g2o_qglviewer.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1981 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/g2o_qglviewer.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1715 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/g2o_viewer.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1876 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/g2o_viewer_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1698 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/gui_hyper_graph_action.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1501 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/gui_hyper_graph_action.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    14599 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/main_window.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2801 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/main_window.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4402 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/properties_widget.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1651 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/properties_widget.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3063 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/run_g2o_viewer.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1730 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/run_g2o_viewer.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2516 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/stream_redirect.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2184 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/stream_redirect.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2317 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/viewer_properties_widget.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1358 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/viewer_properties_widget.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.664244 g2o-python-0.0.9/g2o/g2o/apps/linked_binaries/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1942 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/apps/linked_binaries/CMakeLists.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.664244 g2o-python-0.0.9/g2o/g2o/autodiff/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      589 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1554 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/LICENSE
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3611 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/array_selector.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    14450 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/autodiff.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2220 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/disable_warnings.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3239 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/eigen.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    17116 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/fixed_array.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6505 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/integer_sequence_algorithm.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    34207 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/jet.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3069 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/memory.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5174 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/parameter_dims.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1854 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/reenable_warnings.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2760 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/types.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5032 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/autodiff/variadic_evaluate.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.668244 g2o-python-0.0.9/g2o/g2o/core/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2734 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    13198 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/auto_differentiation.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2348 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_binary_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3215 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_dynamic_vertex.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6973 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    12019 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_fixed_sized_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     9500 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_fixed_sized_edge.hpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1667 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/core/base_multi_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2073 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_unary_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4103 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_variable_sized_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6846 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_variable_sized_edge.hpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4423 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_vertex.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2285 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/base_vertex.hpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3253 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/batch_stats.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3786 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/batch_stats.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7730 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/block_solver.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    21317 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/block_solver.hpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3976 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/cache.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3723 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/cache.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2678 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/creators.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1466 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/dynamic_aligned_buffer.hpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3783 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/eigen_types.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     9578 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/estimate_propagator.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6544 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/estimate_propagator.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6062 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/factory.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5438 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/factory.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      862 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/core/g2o_core_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     9496 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/hyper_dijkstra.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5448 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/hyper_dijkstra.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6717 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/hyper_graph.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10802 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/hyper_graph.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8849 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/hyper_graph_action.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8068 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/hyper_graph_action.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1984 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/core/io_helper.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3459 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/jacobian_workspace.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3493 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/jacobian_workspace.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6768 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/linear_solver.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7331 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/marginal_covariance_cholesky.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4128 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/marginal_covariance_cholesky.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3391 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/matrix_operations.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3424 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/matrix_structure.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2769 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/matrix_structure.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2834 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/openmp_mutex.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    27099 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimizable_graph.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    28390 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimizable_graph.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2094 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4230 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8593 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_dogleg.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3552 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_dogleg.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4531 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_factory.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7653 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_factory.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3344 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_gauss_newton.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2211 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_gauss_newton.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6141 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_levenberg.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4005 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_levenberg.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2660 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_property.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3053 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_with_hessian.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2696 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_with_hessian.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1530 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/parameter.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2161 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/parameter.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4087 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/parameter_container.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2646 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/parameter_container.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1621 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/robust_kernel.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2744 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/robust_kernel.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3012 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/robust_kernel_factory.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4946 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/robust_kernel_factory.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5999 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/robust_kernel_impl.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5279 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/robust_kernel_impl.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2648 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/solver.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5151 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/solver.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10152 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/sparse_block_matrix.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    24718 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/sparse_block_matrix.hpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10276 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/sparse_block_matrix_ccs.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4106 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/sparse_block_matrix_diagonal.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    18371 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/sparse_optimizer.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    12655 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/sparse_optimizer.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3796 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/sparse_optimizer_terminate_action.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2717 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/core/sparse_optimizer_terminate_action.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.668244 g2o-python-0.0.9/g2o/g2o/examples/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1002 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/CMakeLists.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.668244 g2o-python-0.0.9/g2o/g2o/examples/ba/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      226 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/ba/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8894 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/ba/ba_demo.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/ba_anchored_inverse_depth/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      329 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/ba_anchored_inverse_depth/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10550 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/ba_anchored_inverse_depth/ba_anchored_inverse_depth_demo.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/bal/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      180 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/bal/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    12903 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/bal/bal_example.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1199 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7551 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/closed_form_calibration.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2406 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/closed_form_calibration.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2568 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/edge_se2_pure_calib.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2385 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/edge_se2_pure_calib.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2451 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/g2o_calibration_odom_laser_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     9357 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/gm2dl_io.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2274 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/gm2dl_io.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1904 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/motion_information.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5476 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_helpers.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1861 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_helpers.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6433 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_laser_calib.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10037 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_odom_laser.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    15381 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_pure_calibration.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/data_convert/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      229 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/data_convert/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5147 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/data_convert/convert_sba_slam3d.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/data_fitting/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      348 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/data_fitting/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7239 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/data_fitting/circle_fit.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5980 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/data_fitting/curve_fit.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/dynamic_vertex/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      458 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/dynamic_vertex/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7001 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/dynamic_vertex/polynomial_fit.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8904 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/dynamic_vertex/static_dynamic_function_fit.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/g2o_unfold/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    35161 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/g2o_unfold/g2o-unfold.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3326 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/g2o_unfold/tools.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2000 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/g2o_unfold/tools.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/icp/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      397 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/icp/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      367 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/icp/gicp-test1.dat
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5861 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/icp/gicp_demo.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8265 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/icp/gicp_sba_demo.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      142 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      545 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/README.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.672244 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1049 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      951 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/README.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6685 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/g2o_incremental.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1913 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/g2o_incremental_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    20034 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/graph_optimizer_sparse_incremental.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2081 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/graph_optimizer_sparse_incremental.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10478 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/linear_solver_cholmod_online.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2456 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/protocol.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.676244 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1320 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5373 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/fast_output.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1913 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_interactive_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2884 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_online.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    14024 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_slam_interface.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3157 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_slam_interface.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     9920 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/generate_commands.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8737 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/graph_optimizer_sparse_online.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2364 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/graph_optimizer_sparse_online.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2456 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/protocol.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1925 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/types_online.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3410 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/types_slam2d_online.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3297 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/types_slam3d_online.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.676244 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       80 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/CMakeLists.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.676244 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/example/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      776 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/example/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4303 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/example/example_slam_interface.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2800 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/example/example_slam_interface.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1776 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/example/test_slam_interface.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.676244 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      872 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3665 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/abstract_slam_interface.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2237 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/parser_interface.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2302 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/parser_interface.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2723 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/slam_context_interface.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2031 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/slam_context_interface.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.676244 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1043 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6746 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/FlexLexer.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    41636 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/bison_parser.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    22144 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/bison_parser.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4130 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/commands.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2556 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/driver.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3606 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/driver.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    49599 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/flex_scanner.cpp
+-rwxrwxr-x   0 miquel    (1000) miquel    (1000)      271 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/grammar.sh
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7333 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/location.hh
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6922 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/parser.yy
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      401 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/position.hh
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1341 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/scanner.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3743 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/scanner.l
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2085 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/slam_context.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1691 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/slam_context.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      320 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/stack.hh
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1758 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/test_slam_parser.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.676244 g2o-python-0.0.9/g2o/g2o/examples/line_slam/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      419 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/line_slam/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4369 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/line_slam/line_test.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10529 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/line_slam/simulator_3d_line.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.676244 g2o-python-0.0.9/g2o/g2o/examples/plane_slam/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      234 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/plane_slam/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3902 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/plane_slam/plane_test.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    13228 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/plane_slam/simulator_3d_plane.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.676244 g2o-python-0.0.9/g2o/g2o/examples/sba/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      350 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/sba/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10170 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/sba/sba_demo.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.676244 g2o-python-0.0.9/g2o/g2o/examples/sim3/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      256 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/sim3/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6019 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/sim3/optimize_sphere_by_sim3.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/examples/simple_optimize/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      310 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/simple_optimize/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3299 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/simple_optimize/simple_optimize.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/examples/slam2d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1304 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/slam2d/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5391 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/slam2d/base_main_window.ui
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5123 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/slam2d/main_window.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1494 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/slam2d/main_window.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1205 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/slam2d/slam2d_g2o.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5787 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/slam2d/slam2d_viewer.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1241 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/slam2d/slam2d_viewer.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/examples/sphere/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      195 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/sphere/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8517 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/sphere/create_sphere.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/examples/target/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      459 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/target/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6494 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/target/constant_velocity_target.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1270 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/target/continuous_to_discrete.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4417 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/target/static_target.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1691 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/target/targetTypes3D.hpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4703 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/target/targetTypes6D.hpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      761 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2125 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/edge_se2.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2407 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/edge_se2.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2379 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/edge_se2_pointxy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2210 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/edge_se2_pointxy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2365 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/g2o_tutorial_slam2d_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2396 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/parameter_se2_offset.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2439 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/parameter_se2_offset.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3302 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/se2.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    11769 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/simulator.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4019 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/simulator.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5884 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/tutorial_slam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2021 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/types_tutorial_slam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1613 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/types_tutorial_slam2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1820 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/vertex_point_xy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2130 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/vertex_point_xy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1870 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/vertex_se2.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2175 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/vertex_se2.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/solvers/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      351 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/CMakeLists.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/solvers/cholmod/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1051 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/cholmod/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2177 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/cholmod/cholmod_ext.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6010 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/cholmod/cholmod_wrapper.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2887 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/cholmod/cholmod_wrapper.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8062 2023-01-30 09:49:37.000000 g2o-python-0.0.9/g2o/g2o/solvers/cholmod/linear_solver_cholmod.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8169 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/cholmod/solver_cholmod.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/solvers/csparse/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1816 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4870 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/csparse_extension.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1816 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/csparse_extension.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2138 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/csparse_helper.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1888 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/csparse_helper.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6939 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/csparse_wrapper.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2968 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/csparse_wrapper.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2372 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/g2o_csparse_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1242 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/g2o_csparse_extension_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6657 2023-01-30 09:49:37.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/linear_solver_csparse.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5462 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/csparse/solver_csparse.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/solvers/dense/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      764 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/dense/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3655 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/dense/linear_solver_dense.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5230 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/dense/solver_dense.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/solvers/eigen/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      912 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/eigen/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8432 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/eigen/linear_solver_eigen.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6077 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/eigen/solver_eigen.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.680244 g2o-python-0.0.9/g2o/g2o/solvers/pcg/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      917 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/pcg/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3499 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/pcg/linear_solver_pcg.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7334 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/pcg/linear_solver_pcg.hpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5765 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/pcg/solver_pcg.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.684244 g2o-python-0.0.9/g2o/g2o/solvers/slam2d_linear/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      896 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/slam2d_linear/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2377 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/slam2d_linear/g2o_slam2d_linear_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3205 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/slam2d_linear/slam2d_linear.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8218 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/slam2d_linear/solver_slam2d_linear.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2763 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/slam2d_linear/solver_slam2d_linear.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.684244 g2o-python-0.0.9/g2o/g2o/solvers/structure_only/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      833 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/solvers/structure_only/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2946 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/structure_only/structure_only.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8461 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/solvers/structure_only/structure_only_solver.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.684244 g2o-python-0.0.9/g2o/g2o/stuff/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2296 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/stuff/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2595 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/color_macros.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    12380 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/command_args.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4557 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/command_args.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4637 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/filesys_tools.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3256 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/stuff/filesys_tools.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2308 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/stuff/g2o_stuff_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4350 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/macros.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5186 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/misc.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8625 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/opengl_primitives.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4200 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/stuff/opengl_primitives.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1676 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/stuff/opengl_wrapper.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2042 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/stuff/os_specific.c
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1887 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/stuff/os_specific.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3148 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/property.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4923 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/property.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2002 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/stuff/sampler.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4118 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/sampler.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3886 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/sparse_helper.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3063 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/sparse_helper.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5306 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/string_tools.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5108 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/string_tools.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5685 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/tictoc.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2432 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/tictoc.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1850 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/timeutil.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4087 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/timeutil.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2106 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/tuple_tools.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3699 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/stuff/unscented.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.684244 g2o-python-0.0.9/g2o/g2o/types/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      664 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/CMakeLists.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.684244 g2o-python-0.0.9/g2o/g2o/types/data/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1228 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/data/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2540 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/data_queue.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2108 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/data_queue.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2347 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/data/g2o_types_data_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2505 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/data/laser_parameters.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2253 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/data/laser_parameters.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3135 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/raw_laser.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2870 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/raw_laser.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1776 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/robot_data.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2499 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/robot_data.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6137 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/robot_laser.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3022 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/robot_laser.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1985 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/data/types_data.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1560 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/data/types_data.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5015 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/vertex_ellipse.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3412 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/vertex_ellipse.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3744 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/vertex_tag.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2814 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/data/vertex_tag.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.684244 g2o-python-0.0.9/g2o/g2o/types/icp/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      911 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/icp/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2315 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/icp/g2o_types_icp_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10500 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/icp/types_icp.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    11207 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/icp/types_icp.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.688244 g2o-python-0.0.9/g2o/g2o/types/sba/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1933 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sba/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5397 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_p2mc.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2193 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_p2mc.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6589 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_p2sc.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2166 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_p2sc.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3469 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_psi2uv.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2188 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_psi2uv.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3957 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_stereo_xyz.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2557 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_stereo_xyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3536 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_stereo_xyz_onlypose.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2205 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_stereo_xyz_onlypose.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3441 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2141 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3545 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz2uv.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2147 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz2uv.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2202 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz2uvu.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2189 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz2uvu.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3092 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz_onlypose.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2172 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz_onlypose.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3297 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_sba_cam.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2519 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_sba_cam.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2837 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_sba_scale.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2323 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_sba_scale.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2479 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_se3_expmap.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1976 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/edge_se3_expmap.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2339 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sba/g2o_types_sba_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2779 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/parameter_cameraparameters.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2161 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/parameter_cameraparameters.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2561 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sba/sba_utils.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4405 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/sbacam.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3345 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/sbacam.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1870 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/types_sba.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1775 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sba/types_sba.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2202 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sba/types_six_dof_expmap.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2092 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sba/types_six_dof_expmap.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2646 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/vertex_cam.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3246 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/vertex_cam.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2034 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/vertex_intrinsics.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2044 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/vertex_intrinsics.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1980 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/vertex_se3_expmap.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2079 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sba/vertex_se3_expmap.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.688244 g2o-python-0.0.9/g2o/g2o/types/sclam2d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1232 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3044 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/edge_se2_odom_differential_calib.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3217 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/edge_se2_odom_differential_calib.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3449 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/edge_se2_sensor_calib.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3446 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/edge_se2_sensor_calib.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2371 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/g2o_types_sclam2d_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3387 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/odometry_measurement.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3442 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/odometry_measurement.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2108 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/types_sclam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1566 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/types_sclam2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1734 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/vertex_odom_differential_params.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2050 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sclam2d/vertex_odom_differential_params.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.688244 g2o-python-0.0.9/g2o/g2o/types/sim3/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      918 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/sim3/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8355 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sim3/sim3.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7090 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sim3/types_seven_dof_expmap.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6037 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/sim3/types_seven_dof_expmap.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.692244 g2o-python-0.0.9/g2o/g2o/types/slam2d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1729 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2139 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_pointxy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2945 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_pointxy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6956 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4177 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6249 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_lotsofxy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2592 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_lotsofxy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3324 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_offset.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3089 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_offset.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5760 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3789 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4992 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy_bearing.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3844 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy_bearing.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2303 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy_calib.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2733 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy_calib.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4173 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy_offset.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3098 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy_offset.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2385 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_prior.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2923 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_prior.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5029 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_twopointsxy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2339 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_twopointsxy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1845 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_xyprior.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2484 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_xyprior.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2072 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_xy_prior.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2730 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_xy_prior.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2363 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/g2o_types_slam2d_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3151 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/parameter_se2_offset.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3561 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/parameter_se2_offset.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3675 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/se2.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2969 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/types_slam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1964 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/types_slam2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4036 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/vertex_point_xy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3482 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/vertex_point_xy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4449 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/vertex_se2.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3757 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d/vertex_se2.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.692244 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1551 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2057 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_line2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3022 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_line2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1820 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_line2d_pointxy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3208 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_line2d_pointxy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2398 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_line2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3644 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_line2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2309 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_segment2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5044 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_segment2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1775 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_line.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4960 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_line.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1848 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_pointLine.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4081 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_pointLine.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2419 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/g2o_types_slam2d_addons_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2069 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/line_2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2200 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/types_slam2d_addons.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1806 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/types_slam2d_addons.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3866 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/vertex_line2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3542 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/vertex_line2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4077 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/vertex_segment2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3931 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/vertex_segment2d.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.696244 g2o-python-0.0.9/g2o/g2o/types/slam3d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1800 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3682 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/dquat2mat.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2138 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/dquat2mat.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7742 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/dquat2mat.wxm
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8516 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/dquat2mat_maxima_generated.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2282 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_pointxyz.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2962 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_pointxyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5805 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3808 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6395 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_lotsofxyz.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2578 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_lotsofxyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4187 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_offset.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2454 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_offset.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6585 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_pointxyz.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3442 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_pointxyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4884 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_pointxyz_depth.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3052 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_pointxyz_depth.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7189 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_pointxyz_disparity.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3613 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_pointxyz_disparity.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3735 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_prior.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3216 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_prior.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3303 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_xyzprior.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2861 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_xyzprior.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2183 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_xyz_prior.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2745 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_xyz_prior.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2363 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/g2o_types_slam3d_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    11153 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/isometry3d_gradients.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4665 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/isometry3d_mappings.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5443 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/isometry3d_mappings.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4430 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/parameter_camera.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3312 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/parameter_camera.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3873 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/parameter_se3_offset.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3554 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/parameter_se3_offset.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1911 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/parameter_stereo_camera.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2085 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/parameter_stereo_camera.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2016 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/se3_ops.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2239 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/se3_ops.hpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8036 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/se3quat.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3174 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/types_slam3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2124 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/types_slam3d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4068 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/vertex_pointxyz.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3638 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/vertex_pointxyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4768 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/vertex_se3.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5524 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d/vertex_se3.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.700244 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1414 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1979 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_plane.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2768 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_plane.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2477 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_calib.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2310 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_calib.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3345 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_euler.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1975 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_euler.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5284 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_line.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3190 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_line.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4623 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_plane_calib.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3192 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_plane_calib.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1972 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/g2o_types_slam3d_addons_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2722 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/line3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6561 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/line3d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3886 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/plane3d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2983 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/types_slam3d_addons.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1905 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/types_slam3d_addons.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4315 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/vertex_line3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2926 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/vertex_line3d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4010 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/vertex_plane.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2938 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/vertex_plane.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1839 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/vertex_se3_euler.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2017 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/vertex_se3_euler.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1924 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/g2o/what_is_in_these_directories.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.700244 g2o-python-0.0.9/g2o/python/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1915 2023-01-31 06:43:39.000000 g2o-python-0.0.9/g2o/python/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4538 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/README.md
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.704244 g2o-python-0.0.9/g2o/python/core/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      933 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_base_binary_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      433 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_base_edge.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2818 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_base_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1150 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_base_fixed_sized_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      699 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_base_unary_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      546 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_base_variable_sized_edge.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2129 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_base_variable_sized_edge.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      692 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_base_vertex.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1504 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_base_vertex.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2933 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_batch_stats.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      119 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_batch_stats.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6920 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_block_solver.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      733 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_block_solver.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1357 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_core.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      125 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_core.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    13229 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_eigen_types.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      150 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_eigen_types.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4243 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_estimate_propagator.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      119 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_estimate_propagator.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5591 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_hyper_dijkstra.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      114 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_hyper_dijkstra.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6173 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_hyper_graph.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      115 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_hyper_graph.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      661 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_hyper_graph_action.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1075 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_jacobian_workspace.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      122 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_jacobian_workspace.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      886 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_linear_solver.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10685 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_optimizable_graph.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      117 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_optimizable_graph.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2210 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_optimization_algorithm.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      126 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_optimization_algorithm.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      430 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_parameter.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6144 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_robust_kernel.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      117 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_robust_kernel.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      775 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_solver.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      815 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_sparse_block_matrix.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      118 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_sparse_block_matrix.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     8595 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_sparse_optimizer.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      120 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_sparse_optimizer.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      798 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/core/py_sparse_optimizer_terminate_action.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.704244 g2o-python-0.0.9/g2o/python/examples/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4531 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/examples/ba_anchored_inverse_depth_demo.py
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3875 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/examples/ba_demo.py
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2685 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/examples/gicp_demo.py
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4614 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/examples/gicp_sba_demo.py
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5782 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/examples/notebook_slam2d.ipynb
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3981 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/examples/sba_demo.py
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3941 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/examples/sba_demo2.py
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1148 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/examples/simple_optimize.py
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3413 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/examples/type_in_python.py
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      194 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/g2opy.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      274 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/g2opy.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.704244 g2o-python-0.0.9/g2o/python/types/
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.704244 g2o-python-0.0.9/g2o/python/types/icp/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5361 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/icp/py_types_icp.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      109 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/icp/py_types_icp.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.704244 g2o-python-0.0.9/g2o/python/types/pure/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4387 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/pure/py_types_pure.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      110 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/pure/py_types_pure.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      755 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/py_types.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.704244 g2o-python-0.0.9/g2o/python/types/sba/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2248 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sba/py_sbacam.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3669 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sba/py_types_sba.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      113 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sba/py_types_sba.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5843 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sba/py_types_six_dof_expmap.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      121 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sba/py_types_six_dof_expmap.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.704244 g2o-python-0.0.9/g2o/python/types/sclam2d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      973 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sclam2d/py_edge_se2_odom_differential_calib.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      919 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sclam2d/py_edge_se2_sensor_calib.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1931 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sclam2d/py_odometry_measurement.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      435 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sclam2d/py_types_sclam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      113 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sclam2d/py_types_sclam2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      479 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sclam2d/py_vertex_odom_differential_params.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.704244 g2o-python-0.0.9/g2o/python/types/sim3/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1093 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sim3/py_sim3.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1813 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sim3/py_types_seven_dof_expmap.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      216 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/sim3/py_types_seven_dof_expmap.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.704244 g2o-python-0.0.9/g2o/python/types/slam2d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1116 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam2d/py_edge_pointxy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4466 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam2d/py_edge_se2.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3921 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam2d/py_edge_se2_pointxy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      635 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam2d/py_parameter_se2_offset.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1075 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam2d/py_se2.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      490 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam2d/py_types_slam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      112 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam2d/py_types_slam2d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1036 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam2d/py_vertex_point_xy.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      958 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam2d/py_vertex_se2.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.708244 g2o-python-0.0.9/g2o/python/types/slam3d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1134 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam3d/py_edge_pointxyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3382 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam3d/py_edge_se3.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3345 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam3d/py_edge_se3_pointxyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1570 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam3d/py_parameter.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2383 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam3d/py_se3quat.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      489 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam3d/py_types_slam3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      167 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam3d/py_types_slam3d.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1024 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam3d/py_vertex_pointxyz.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      801 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/python/types/slam3d/py_vertex_se3.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.708244 g2o-python-0.0.9/g2o/script/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    82300 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/script/android.toolchain.cmake
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      655 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/script/codecov.sh.in
+-rwxrwxr-x   0 miquel    (1000) miquel    (1000)    21520 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/script/git-clang-format.py
+-rwxrwxr-x   0 miquel    (1000) miquel    (1000)      582 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/script/install-deps-linux.sh
+-rwxrwxr-x   0 miquel    (1000) miquel    (1000)      191 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/script/install-deps-osx.sh
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      952 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/script/install-deps-windows.bat
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      938 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/script/run-style-check-diff.sh
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.708244 g2o-python-0.0.9/g2o/unit_test/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      779 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/CMakeLists.txt
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.708244 g2o-python-0.0.9/g2o/unit_test/data/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      149 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/data/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2983 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/data/data_queue_tests.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3056 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/data/io_data.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.708244 g2o-python-0.0.9/g2o/unit_test/general/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      286 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/general/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10140 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/general/auto_diff.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    14617 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/general/base_fixed_sized_edge.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4045 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/general/clear_and_redo.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    22305 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/general/graph_operations.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4749 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/general/robust_kernel_tests.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3264 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/general/sparse_block_matrix.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.708244 g2o-python-0.0.9/g2o/unit_test/sba/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      139 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/sba/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2743 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/sba/io_sba.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4020 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/sba/io_six_dof_expmap.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.708244 g2o-python-0.0.9/g2o/unit_test/sclam2d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      198 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/sclam2d/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3004 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/sclam2d/io_sclam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2994 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/sclam2d/odom_convert_sclam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    11259 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/sclam2d/sensor_offset.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.712244 g2o-python-0.0.9/g2o/unit_test/sim3/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      161 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/sim3/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1627 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/sim3/allocate_sim3.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2453 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/sim3/io_sim3.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2617 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/sim3/jacobians_sim3.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.712244 g2o-python-0.0.9/g2o/unit_test/slam2d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      172 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/slam2d/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3211 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam2d/io_slam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5203 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam2d/jacobians_slam2d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2247 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam2d/mappings_se2.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.712244 g2o-python-0.0.9/g2o/unit_test/slam2d_addons/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      165 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/slam2d_addons/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2711 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam2d_addons/io_slam2d_addons.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.712244 g2o-python-0.0.9/g2o/unit_test/slam3d/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      225 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/slam3d/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     7576 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam3d/io_slam3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    10734 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam3d/jacobians_slam3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3911 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam3d/mappings_slam3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5655 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam3d/optimization_slam3d.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3283 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam3d/orthogonal_matrix.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.712244 g2o-python-0.0.9/g2o/unit_test/slam3d_addons/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      165 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/slam3d_addons/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4196 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/slam3d_addons/io_slam3d_addons.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.712244 g2o-python-0.0.9/g2o/unit_test/solver/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      607 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/solver/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4442 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/solver/allocate_algorithm_test.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     6415 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/solver/linear_solver_test.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    40579 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/solver/sparse_system_helper.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2040 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/solver/sparse_system_helper.h
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.712244 g2o-python-0.0.9/g2o/unit_test/stuff/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      242 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/stuff/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4760 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/stuff/command_args_tests.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3819 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/stuff/filesys_tools_tests.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     5414 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/stuff/misc_tests.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3442 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/stuff/property_tests.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4404 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/stuff/string_tools_tests.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2082 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/stuff/tuple_tools_tests.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.712244 g2o-python-0.0.9/g2o/unit_test/test_helper/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      144 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/test_helper/CMakeLists.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2799 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/test_helper/allocate_optimizer.cpp
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1882 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/test_helper/allocate_optimizer.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4453 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/test_helper/evaluate_jacobian.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     1913 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/test_helper/g2o_test_helper_api.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     3972 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/test_helper/io.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2607 2023-01-16 15:07:22.000000 g2o-python-0.0.9/g2o/unit_test/test_helper/random_state.h
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      214 2023-01-16 14:48:13.000000 g2o-python-0.0.9/g2o/unit_test/test_helper/test_main.cpp
+drwxrwxr-x   0 miquel    (1000) miquel    (1000)        0 2023-01-31 06:43:39.712244 g2o-python-0.0.9/g2o_python.egg-info/
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     2779 2023-01-31 06:43:39.000000 g2o-python-0.0.9/g2o_python.egg-info/PKG-INFO
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)    52185 2023-01-31 06:43:39.000000 g2o-python-0.0.9/g2o_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)        1 2023-01-31 06:43:39.000000 g2o-python-0.0.9/g2o_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       19 2023-01-31 06:43:39.000000 g2o-python-0.0.9/g2o_python.egg-info/requires.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)        4 2023-01-31 06:43:39.000000 g2o-python-0.0.9/g2o_python.egg-info/top_level.txt
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)      347 2023-01-31 05:59:31.000000 g2o-python-0.0.9/pyproject.toml
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)       38 2023-01-31 06:43:39.716244 g2o-python-0.0.9/setup.cfg
+-rw-rw-r--   0 miquel    (1000) miquel    (1000)     4431 2023-01-31 06:38:22.000000 g2o-python-0.0.9/setup.py
```

### Comparing `g2o-python-0.0.8/.gitignore` & `g2o-python-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/LICENSE` & `g2o-python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/PKG-INFO` & `g2o-python-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: g2o-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper package for G2O python bindings.
 Home-page: https://github.com/miquelmassot/g2o-python
 Maintainer: Miquel Massot
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -45,15 +46,15 @@
 # g2o-python
 
 This is a wrapper of the python binding of [g2o](https://github.com/RainerKuemmerle/g2o) using its branch `pymem`.
 
 ## How to use it in your code
 
 ```python
-from g2opy import g2opy as g2o
+import g2o
 # Your code
 
 ```
 
 More examples [available here](https://github.com/RainerKuemmerle/g2o/tree/pymem/python/examples).
 
 
@@ -62,7 +63,9 @@
 ```bash
 pip install -U g2o-python
 ```
 
 ## Build from source
 
 Clone this repository and run `pip install -U --user -v .`
+
+
```

### Comparing `g2o-python-0.0.8/README.md` & `g2o-python-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # g2o-python
 
 This is a wrapper of the python binding of [g2o](https://github.com/RainerKuemmerle/g2o) using its branch `pymem`.
 
 ## How to use it in your code
 
 ```python
-from g2opy import g2opy as g2o
+import g2o
 # Your code
 
 ```
 
 More examples [available here](https://github.com/RainerKuemmerle/g2o/tree/pymem/python/examples).
```

### Comparing `g2o-python-0.0.8/g2o/.clang-format` & `g2o-python-0.0.9/g2o/.clang-format`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/.clang-tidy` & `g2o-python-0.0.9/g2o/.clang-tidy`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/.github/workflows/ci.yml` & `g2o-python-0.0.9/g2o/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/.github/workflows/clang-format.yml` & `g2o-python-0.0.9/g2o/.github/workflows/clang-format.yml`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/.github/workflows/windows.yml` & `g2o-python-0.0.9/g2o/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/CMakeLists.txt` & `g2o-python-0.0.9/g2o/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/README.md` & `g2o-python-0.0.9/g2o/README.md`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/appveyor.yml` & `g2o-python-0.0.9/g2o/appveyor.yml`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/benchmarks/jacobian_timing_tests.cpp` & `g2o-python-0.0.9/g2o/benchmarks/jacobian_timing_tests.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/cmake_modules/CheckIfUnderscorePrefixedBesselFunctionsExist.cmake` & `g2o-python-0.0.9/g2o/cmake_modules/CheckIfUnderscorePrefixedBesselFunctionsExist.cmake`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/cmake_modules/FindCSparse.cmake` & `g2o-python-0.0.9/g2o/cmake_modules/FindCSparse.cmake`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/cmake_modules/FindEigen3.cmake` & `g2o-python-0.0.9/g2o/cmake_modules/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/cmake_modules/FindG2O.cmake` & `g2o-python-0.0.9/g2o/cmake_modules/FindG2O.cmake`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/cmake_modules/FindMETIS.cmake` & `g2o-python-0.0.9/g2o/cmake_modules/FindMETIS.cmake`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/cmake_modules/FindQGLViewer.cmake` & `g2o-python-0.0.9/g2o/cmake_modules/FindQGLViewer.cmake`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/cmake_modules/FindSuiteSparse.cmake` & `g2o-python-0.0.9/g2o/cmake_modules/FindSuiteSparse.cmake`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/config.h.in` & `g2o-python-0.0.9/g2o/config.h.in`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/doxygen/doxy.config` & `g2o-python-0.0.9/g2o/doc/doxygen/doxy.config`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/g2o.pdf` & `g2o-python-0.0.9/g2o/doc/g2o.pdf`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/g2o.tex` & `g2o-python-0.0.9/g2o/doc/g2o.tex`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/license-bsd.txt` & `g2o-python-0.0.9/g2o/doc/license-bsd.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/license-gpl.txt` & `g2o-python-0.0.9/g2o/doc/license-gpl.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/license-lgpl.txt` & `g2o-python-0.0.9/g2o/doc/license-lgpl.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/pics/classes.eps` & `g2o-python-0.0.9/g2o/doc/pics/classes.eps`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/pics/classes.fig` & `g2o-python-0.0.9/g2o/doc/pics/classes.fig`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/pics/classes.svg` & `g2o-python-0.0.9/g2o/doc/pics/classes.svg`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/pics/hgraph.eps` & `g2o-python-0.0.9/g2o/doc/pics/hgraph.eps`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/pics/hgraph.fig` & `g2o-python-0.0.9/g2o/doc/pics/hgraph.fig`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/pics/slam.eps` & `g2o-python-0.0.9/g2o/doc/pics/slam.eps`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/pics/slam.fig` & `g2o-python-0.0.9/g2o/doc/pics/slam.fig`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/pics/viewer.eps` & `g2o-python-0.0.9/g2o/doc/pics/viewer.eps`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/pics/viewer.png` & `g2o-python-0.0.9/g2o/doc/pics/viewer.png`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/doc/robots.bib` & `g2o-python-0.0.9/g2o/doc/robots.bib`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/COPYING` & `g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/COPYING`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/freeglut_font.cpp` & `g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/freeglut_font.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/freeglut_minimal.h` & `g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/freeglut_minimal.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/freeglut_stroke_mono_roman.cpp` & `g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/freeglut_stroke_mono_roman.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/EXTERNAL/freeglut/freeglut_stroke_roman.cpp` & `g2o-python-0.0.9/g2o/g2o/EXTERNAL/freeglut/freeglut_stroke_roman.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/dl_wrapper.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/dl_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/dl_wrapper.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/dl_wrapper.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/g2o.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/g2o.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/g2o_cli_api.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/g2o_cli_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/g2o_common.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/g2o_common.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/g2o_common.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/g2o_common.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/output_helper.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/output_helper.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_cli/output_helper.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_cli/output_helper.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/backbone_tree_action.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/backbone_tree_action.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/backbone_tree_action.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/backbone_tree_action.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_creator.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_creator.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_creator.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_creator.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_labeler.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_labeler.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_labeler.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_labeler.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_types_cost_function.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_types_cost_function.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/edge_types_cost_function.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/edge_types_cost_function.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical_api.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical_test_functions.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/g2o_hierarchical_test_functions.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/simple_star_ops.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/simple_star_ops.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/simple_star_ops.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/simple_star_ops.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/star.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/star.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_hierarchical/star.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_hierarchical/star.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/convertSegmentLine.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/convertSegmentLine.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/g2o_anonymize_observations.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/g2o_anonymize_observations.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/g2o_simulator_api.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/g2o_simulator_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/pointsensorparameters.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/pointsensorparameters.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/pointsensorparameters.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/pointsensorparameters.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_line3d.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_line3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_line3d.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_line3d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry2d.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry2d.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry3d.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_odometry3d.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_odometry3d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy_bearing.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy_bearing.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy_bearing.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy_bearing.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy_offset.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy_offset.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxy_offset.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxy_offset.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_depth.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_depth.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_depth.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_depth.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_disparity.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_disparity.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_disparity.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pointxyz_disparity.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose2d.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose2d.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose3d.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose3d.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose3d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose3d_offset.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose3d_offset.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_pose3d_offset.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_pose3d_offset.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_se3_prior.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_se3_prior.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_se3_prior.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_se3_prior.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d_line.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d_line.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d_line.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d_line.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d_pointline.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d_pointline.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/sensor_segment2d_pointline.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/sensor_segment2d_pointline.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator2d.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator2d_base.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator2d_base.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator2d_segment.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator2d_segment.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator3d.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator3d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simulator3d_base.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simulator3d_base.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simutils.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simutils.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/simutils.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/simutils.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/test_simulator2d.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/test_simulator2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_simulator/test_simulator3d.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_simulator/test_simulator3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/base_main_window.ui` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/base_main_window.ui`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/base_properties_widget.ui` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/base_properties_widget.ui`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/g2o_qglviewer.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/g2o_qglviewer.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/g2o_qglviewer.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/g2o_qglviewer.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/g2o_viewer.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/g2o_viewer.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/g2o_viewer_api.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/g2o_viewer_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/gui_hyper_graph_action.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/gui_hyper_graph_action.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/gui_hyper_graph_action.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/gui_hyper_graph_action.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/main_window.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/main_window.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/main_window.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/main_window.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/properties_widget.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/properties_widget.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/properties_widget.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/properties_widget.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/run_g2o_viewer.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/run_g2o_viewer.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/run_g2o_viewer.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/run_g2o_viewer.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/stream_redirect.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/stream_redirect.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/stream_redirect.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/stream_redirect.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/viewer_properties_widget.cpp` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/viewer_properties_widget.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/g2o_viewer/viewer_properties_widget.h` & `g2o-python-0.0.9/g2o/g2o/apps/g2o_viewer/viewer_properties_widget.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/apps/linked_binaries/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/apps/linked_binaries/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/autodiff/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/LICENSE` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/LICENSE`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/array_selector.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/array_selector.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/autodiff.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/autodiff.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/disable_warnings.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/disable_warnings.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/eigen.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/eigen.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/fixed_array.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/fixed_array.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/integer_sequence_algorithm.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/integer_sequence_algorithm.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/jet.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/jet.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/memory.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/memory.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/parameter_dims.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/parameter_dims.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/reenable_warnings.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/reenable_warnings.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/types.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/types.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/autodiff/variadic_evaluate.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/autodiff/variadic_evaluate.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/auto_differentiation.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/auto_differentiation.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_binary_edge.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_binary_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_dynamic_vertex.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_dynamic_vertex.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_edge.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_fixed_sized_edge.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_fixed_sized_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_fixed_sized_edge.hpp` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_fixed_sized_edge.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_multi_edge.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_multi_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_unary_edge.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_unary_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_variable_sized_edge.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_variable_sized_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_variable_sized_edge.hpp` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_variable_sized_edge.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_vertex.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_vertex.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/base_vertex.hpp` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/base_vertex.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/batch_stats.cpp` & `g2o-python-0.0.9/g2o/g2o/core/batch_stats.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/batch_stats.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/batch_stats.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/block_solver.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/block_solver.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/block_solver.hpp` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/block_solver.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/cache.cpp` & `g2o-python-0.0.9/g2o/g2o/core/cache.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/cache.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/cache.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/creators.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/creators.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/dynamic_aligned_buffer.hpp` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/dynamic_aligned_buffer.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/eigen_types.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/eigen_types.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/estimate_propagator.cpp` & `g2o-python-0.0.9/g2o/g2o/core/estimate_propagator.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/estimate_propagator.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/estimate_propagator.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/factory.cpp` & `g2o-python-0.0.9/g2o/g2o/core/factory.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/factory.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/factory.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/g2o_core_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/g2o_core_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/hyper_dijkstra.cpp` & `g2o-python-0.0.9/g2o/g2o/core/hyper_dijkstra.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/hyper_dijkstra.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/hyper_dijkstra.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/hyper_graph.cpp` & `g2o-python-0.0.9/g2o/g2o/core/hyper_graph.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/hyper_graph.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/hyper_graph.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/hyper_graph_action.cpp` & `g2o-python-0.0.9/g2o/g2o/core/hyper_graph_action.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/hyper_graph_action.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/hyper_graph_action.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/io_helper.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/io_helper.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/jacobian_workspace.cpp` & `g2o-python-0.0.9/g2o/g2o/core/jacobian_workspace.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/jacobian_workspace.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/jacobian_workspace.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/linear_solver.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/linear_solver.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/marginal_covariance_cholesky.cpp` & `g2o-python-0.0.9/g2o/g2o/core/marginal_covariance_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/marginal_covariance_cholesky.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/marginal_covariance_cholesky.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/matrix_operations.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/matrix_operations.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/matrix_structure.cpp` & `g2o-python-0.0.9/g2o/g2o/core/matrix_structure.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/matrix_structure.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/matrix_structure.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/openmp_mutex.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/openmp_mutex.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimizable_graph.cpp` & `g2o-python-0.0.9/g2o/g2o/core/optimizable_graph.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimizable_graph.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimizable_graph.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm.cpp` & `g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_dogleg.cpp` & `g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_dogleg.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_dogleg.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_dogleg.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_factory.cpp` & `g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_factory.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_factory.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_factory.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_gauss_newton.cpp` & `g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_gauss_newton.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_gauss_newton.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_gauss_newton.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_levenberg.cpp` & `g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_levenberg.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_levenberg.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_levenberg.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_property.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_property.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_with_hessian.cpp` & `g2o-python-0.0.9/g2o/g2o/core/optimization_algorithm_with_hessian.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/optimization_algorithm_with_hessian.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/optimization_algorithm_with_hessian.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/parameter.cpp` & `g2o-python-0.0.9/g2o/g2o/core/parameter.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/parameter.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/parameter.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/parameter_container.cpp` & `g2o-python-0.0.9/g2o/g2o/core/parameter_container.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/parameter_container.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/parameter_container.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/robust_kernel.cpp` & `g2o-python-0.0.9/g2o/g2o/core/robust_kernel.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/robust_kernel.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/robust_kernel.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/robust_kernel_factory.cpp` & `g2o-python-0.0.9/g2o/g2o/core/robust_kernel_factory.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/robust_kernel_factory.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/robust_kernel_factory.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/robust_kernel_impl.cpp` & `g2o-python-0.0.9/g2o/g2o/core/robust_kernel_impl.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/robust_kernel_impl.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/robust_kernel_impl.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/solver.cpp` & `g2o-python-0.0.9/g2o/g2o/core/solver.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/solver.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/solver.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/sparse_block_matrix.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_block_matrix.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/sparse_block_matrix.hpp` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/sparse_block_matrix_ccs.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_block_matrix_ccs.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/sparse_block_matrix_diagonal.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_block_matrix_diagonal.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/sparse_optimizer.cpp` & `g2o-python-0.0.9/g2o/g2o/core/sparse_optimizer.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/sparse_optimizer.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_optimizer.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/sparse_optimizer_terminate_action.cpp` & `g2o-python-0.0.9/g2o/g2o/core/sparse_optimizer_terminate_action.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/core/sparse_optimizer_terminate_action.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/core/sparse_optimizer_terminate_action.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/ba/ba_demo.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/ba/ba_demo.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/ba_anchored_inverse_depth/ba_anchored_inverse_depth_demo.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/ba_anchored_inverse_depth/ba_anchored_inverse_depth_demo.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/bal/bal_example.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/bal/bal_example.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/closed_form_calibration.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/closed_form_calibration.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/closed_form_calibration.h` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/closed_form_calibration.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/edge_se2_pure_calib.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/edge_se2_pure_calib.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/edge_se2_pure_calib.h` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/edge_se2_pure_calib.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/g2o_calibration_odom_laser_api.h` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/g2o_calibration_odom_laser_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/gm2dl_io.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/gm2dl_io.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/gm2dl_io.h` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/gm2dl_io.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/motion_information.h` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/motion_information.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_helpers.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_helpers.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_helpers.h` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_helpers.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_laser_calib.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_laser_calib.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_odom_laser.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_odom_laser.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/calibration_odom_laser/sclam_pure_calibration.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/calibration_odom_laser/sclam_pure_calibration.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/data_convert/convert_sba_slam3d.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/data_convert/convert_sba_slam3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/data_fitting/circle_fit.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/data_fitting/circle_fit.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/data_fitting/curve_fit.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/data_fitting/curve_fit.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/dynamic_vertex/polynomial_fit.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/dynamic_vertex/polynomial_fit.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/dynamic_vertex/static_dynamic_function_fit.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/dynamic_vertex/static_dynamic_function_fit.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/g2o_unfold/g2o-unfold.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/g2o_unfold/g2o-unfold.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/g2o_unfold/tools.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/g2o_unfold/tools.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/g2o_unfold/tools.h` & `g2o-python-0.0.9/g2o/g2o/examples/g2o_unfold/tools.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/icp/gicp_demo.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/icp/gicp_demo.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/icp/gicp_sba_demo.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/icp/gicp_sba_demo.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/README.txt` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/README.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/README.txt` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/README.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/g2o_incremental.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/g2o_incremental.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/g2o_incremental_api.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/g2o_incremental_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/graph_optimizer_sparse_incremental.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/graph_optimizer_sparse_incremental.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/graph_optimizer_sparse_incremental.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/graph_optimizer_sparse_incremental.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/linear_solver_cholmod_online.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/linear_solver_cholmod_online.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_incremental/protocol.txt` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_incremental/protocol.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/fast_output.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/fast_output.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_interactive_api.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_interactive_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_online.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_online.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_slam_interface.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_slam_interface.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_slam_interface.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/g2o_slam_interface.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/generate_commands.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/generate_commands.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/graph_optimizer_sparse_online.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/graph_optimizer_sparse_online.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/graph_optimizer_sparse_online.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/graph_optimizer_sparse_online.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/protocol.txt` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/protocol.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/types_online.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/types_online.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/types_slam2d_online.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/types_slam2d_online.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/g2o_interactive/types_slam3d_online.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/g2o_interactive/types_slam3d_online.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/example/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/example/example_slam_interface.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/example/example_slam_interface.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/example/example_slam_interface.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/example/example_slam_interface.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/example/test_slam_interface.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/example/test_slam_interface.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/abstract_slam_interface.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/abstract_slam_interface.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/parser_interface.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/parser_interface.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/parser_interface.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/parser_interface.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/slam_context_interface.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/slam_context_interface.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/interface/slam_context_interface.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/interface/slam_context_interface.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/FlexLexer.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/FlexLexer.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/bison_parser.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/bison_parser.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/bison_parser.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/bison_parser.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/commands.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/commands.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/driver.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/driver.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/driver.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/driver.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/flex_scanner.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/flex_scanner.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/location.hh` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/location.hh`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/parser.yy` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/parser.yy`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/scanner.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/scanner.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/scanner.l` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/scanner.l`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/slam_context.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/slam_context.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/slam_context.h` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/slam_context.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/interactive_slam/slam_parser/parser/test_slam_parser.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/interactive_slam/slam_parser/parser/test_slam_parser.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/line_slam/line_test.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/line_slam/line_test.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/line_slam/simulator_3d_line.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/line_slam/simulator_3d_line.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/plane_slam/plane_test.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/plane_slam/plane_test.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/plane_slam/simulator_3d_plane.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/plane_slam/simulator_3d_plane.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/sba/sba_demo.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/sba/sba_demo.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/sim3/optimize_sphere_by_sim3.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/sim3/optimize_sphere_by_sim3.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/simple_optimize/simple_optimize.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/simple_optimize/simple_optimize.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/slam2d/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/examples/slam2d/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/slam2d/base_main_window.ui` & `g2o-python-0.0.9/g2o/g2o/examples/slam2d/base_main_window.ui`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/slam2d/main_window.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/slam2d/main_window.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/slam2d/main_window.h` & `g2o-python-0.0.9/g2o/g2o/examples/slam2d/main_window.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/slam2d/slam2d_g2o.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/slam2d/slam2d_g2o.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/slam2d/slam2d_viewer.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/slam2d/slam2d_viewer.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/slam2d/slam2d_viewer.h` & `g2o-python-0.0.9/g2o/g2o/examples/slam2d/slam2d_viewer.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/sphere/create_sphere.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/sphere/create_sphere.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/target/constant_velocity_target.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/target/constant_velocity_target.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/target/continuous_to_discrete.h` & `g2o-python-0.0.9/g2o/g2o/examples/target/continuous_to_discrete.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/target/static_target.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/target/static_target.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/target/targetTypes3D.hpp` & `g2o-python-0.0.9/g2o/g2o/examples/target/targetTypes3D.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/target/targetTypes6D.hpp` & `g2o-python-0.0.9/g2o/g2o/examples/target/targetTypes6D.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/edge_se2.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/edge_se2.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/edge_se2.h` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/edge_se2.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/edge_se2_pointxy.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/edge_se2_pointxy.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/edge_se2_pointxy.h` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/edge_se2_pointxy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/g2o_tutorial_slam2d_api.h` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/g2o_tutorial_slam2d_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/parameter_se2_offset.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/parameter_se2_offset.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/parameter_se2_offset.h` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/parameter_se2_offset.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/se2.h` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/se2.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/simulator.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/simulator.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/simulator.h` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/simulator.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/tutorial_slam2d.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/tutorial_slam2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/types_tutorial_slam2d.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/types_tutorial_slam2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/types_tutorial_slam2d.h` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/types_tutorial_slam2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/vertex_point_xy.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/vertex_point_xy.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/vertex_point_xy.h` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/vertex_point_xy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/vertex_se2.cpp` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/vertex_se2.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/examples/tutorial_slam2d/vertex_se2.h` & `g2o-python-0.0.9/g2o/g2o/examples/tutorial_slam2d/vertex_se2.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/cholmod/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/solvers/cholmod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/cholmod/cholmod_ext.h` & `g2o-python-0.0.9/g2o/g2o/solvers/cholmod/cholmod_ext.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/cholmod/cholmod_wrapper.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/cholmod/cholmod_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/cholmod/cholmod_wrapper.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/cholmod/cholmod_wrapper.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/cholmod/linear_solver_cholmod.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/cholmod/linear_solver_cholmod.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/cholmod/solver_cholmod.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/cholmod/solver_cholmod.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/solvers/csparse/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_extension.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/csparse/csparse_extension.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_extension.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/csparse_extension.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_helper.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/csparse/csparse_helper.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_helper.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/csparse_helper.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_wrapper.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/csparse/csparse_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/csparse_wrapper.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/csparse_wrapper.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/g2o_csparse_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/g2o_csparse_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/g2o_csparse_extension_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/g2o_csparse_extension_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/linear_solver_csparse.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/csparse/linear_solver_csparse.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/csparse/solver_csparse.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/csparse/solver_csparse.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/dense/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/solvers/dense/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/dense/linear_solver_dense.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/dense/linear_solver_dense.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/dense/solver_dense.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/dense/solver_dense.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/eigen/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/solvers/eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/eigen/linear_solver_eigen.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/eigen/linear_solver_eigen.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/eigen/solver_eigen.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/eigen/solver_eigen.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/pcg/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/solvers/pcg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/pcg/linear_solver_pcg.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/pcg/linear_solver_pcg.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/pcg/linear_solver_pcg.hpp` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/pcg/linear_solver_pcg.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/pcg/solver_pcg.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/pcg/solver_pcg.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/solvers/slam2d_linear/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/g2o_slam2d_linear_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/slam2d_linear/g2o_slam2d_linear_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/slam2d_linear.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/slam2d_linear/slam2d_linear.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/solver_slam2d_linear.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/slam2d_linear/solver_slam2d_linear.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/slam2d_linear/solver_slam2d_linear.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/slam2d_linear/solver_slam2d_linear.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/structure_only/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/solvers/structure_only/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/structure_only/structure_only.cpp` & `g2o-python-0.0.9/g2o/g2o/solvers/structure_only/structure_only.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/solvers/structure_only/structure_only_solver.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/solvers/structure_only/structure_only_solver.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/stuff/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/color_macros.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/color_macros.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/command_args.cpp` & `g2o-python-0.0.9/g2o/g2o/stuff/command_args.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/command_args.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/command_args.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/filesys_tools.cpp` & `g2o-python-0.0.9/g2o/g2o/stuff/filesys_tools.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/filesys_tools.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/filesys_tools.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/g2o_stuff_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/g2o_stuff_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/macros.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/macros.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/misc.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/misc.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/opengl_primitives.cpp` & `g2o-python-0.0.9/g2o/g2o/stuff/opengl_primitives.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/opengl_primitives.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/opengl_primitives.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/opengl_wrapper.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/opengl_wrapper.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/os_specific.c` & `g2o-python-0.0.9/g2o/g2o/stuff/os_specific.c`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/os_specific.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/os_specific.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/property.cpp` & `g2o-python-0.0.9/g2o/g2o/stuff/property.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/property.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/property.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/sampler.cpp` & `g2o-python-0.0.9/g2o/g2o/stuff/sampler.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/sampler.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/sampler.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/sparse_helper.cpp` & `g2o-python-0.0.9/g2o/g2o/stuff/sparse_helper.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/sparse_helper.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/sparse_helper.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/string_tools.cpp` & `g2o-python-0.0.9/g2o/g2o/stuff/string_tools.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/string_tools.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/string_tools.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/tictoc.cpp` & `g2o-python-0.0.9/g2o/g2o/stuff/tictoc.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/tictoc.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/tictoc.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/timeutil.cpp` & `g2o-python-0.0.9/g2o/g2o/stuff/timeutil.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/timeutil.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/timeutil.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/tuple_tools.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/tuple_tools.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/stuff/unscented.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/stuff/unscented.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/data_queue.cpp` & `g2o-python-0.0.9/g2o/g2o/types/data/data_queue.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/data_queue.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/data_queue.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/g2o_types_data_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/g2o_types_data_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/laser_parameters.cpp` & `g2o-python-0.0.9/g2o/g2o/types/data/laser_parameters.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/laser_parameters.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/laser_parameters.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/raw_laser.cpp` & `g2o-python-0.0.9/g2o/g2o/types/data/raw_laser.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/raw_laser.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/raw_laser.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/robot_data.cpp` & `g2o-python-0.0.9/g2o/g2o/types/data/robot_data.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/robot_data.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/robot_data.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/robot_laser.cpp` & `g2o-python-0.0.9/g2o/g2o/types/data/robot_laser.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/robot_laser.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/robot_laser.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/types_data.cpp` & `g2o-python-0.0.9/g2o/g2o/types/data/types_data.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/types_data.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/types_data.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/vertex_ellipse.cpp` & `g2o-python-0.0.9/g2o/g2o/types/data/vertex_ellipse.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/vertex_ellipse.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/vertex_ellipse.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/vertex_tag.cpp` & `g2o-python-0.0.9/g2o/g2o/types/data/vertex_tag.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/data/vertex_tag.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/data/vertex_tag.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/icp/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/icp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/icp/g2o_types_icp_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/icp/g2o_types_icp_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/icp/types_icp.cpp` & `g2o-python-0.0.9/g2o/g2o/types/icp/types_icp.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/icp/types_icp.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/icp/types_icp.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/sba/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_p2mc.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_p2mc.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_p2mc.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_p2mc.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_p2sc.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_p2sc.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_p2sc.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_p2sc.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_psi2uv.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_psi2uv.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_psi2uv.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_psi2uv.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_stereo_xyz.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_stereo_xyz.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_stereo_xyz.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_stereo_xyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_stereo_xyz_onlypose.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_stereo_xyz_onlypose.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_stereo_xyz_onlypose.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_stereo_xyz_onlypose.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_xyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz2uv.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz2uv.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz2uv.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_xyz2uv.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz2uvu.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz2uvu.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz2uvu.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_xyz2uvu.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz_onlypose.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_project_xyz_onlypose.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_project_xyz_onlypose.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_project_xyz_onlypose.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_sba_cam.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_sba_cam.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_sba_cam.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_sba_cam.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_sba_scale.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_sba_scale.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_sba_scale.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_sba_scale.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_se3_expmap.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/edge_se3_expmap.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/edge_se3_expmap.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/edge_se3_expmap.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/g2o_types_sba_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/g2o_types_sba_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/parameter_cameraparameters.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/parameter_cameraparameters.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/parameter_cameraparameters.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/parameter_cameraparameters.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/sba_utils.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/sba_utils.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/sbacam.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/sbacam.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/sbacam.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/sbacam.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/types_sba.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/types_sba.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/types_sba.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/types_sba.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/types_six_dof_expmap.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/types_six_dof_expmap.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/types_six_dof_expmap.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/types_six_dof_expmap.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/vertex_cam.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/vertex_cam.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/vertex_cam.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/vertex_cam.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/vertex_intrinsics.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/vertex_intrinsics.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/vertex_intrinsics.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/vertex_intrinsics.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/vertex_se3_expmap.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sba/vertex_se3_expmap.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sba/vertex_se3_expmap.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sba/vertex_se3_expmap.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/sclam2d/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/edge_se2_odom_differential_calib.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sclam2d/edge_se2_odom_differential_calib.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/edge_se2_odom_differential_calib.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/edge_se2_odom_differential_calib.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/edge_se2_sensor_calib.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sclam2d/edge_se2_sensor_calib.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/edge_se2_sensor_calib.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/edge_se2_sensor_calib.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/g2o_types_sclam2d_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/g2o_types_sclam2d_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/odometry_measurement.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sclam2d/odometry_measurement.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/odometry_measurement.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/odometry_measurement.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/types_sclam2d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sclam2d/types_sclam2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/types_sclam2d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/types_sclam2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/vertex_odom_differential_params.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sclam2d/vertex_odom_differential_params.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sclam2d/vertex_odom_differential_params.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sclam2d/vertex_odom_differential_params.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sim3/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/sim3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sim3/sim3.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sim3/sim3.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sim3/types_seven_dof_expmap.cpp` & `g2o-python-0.0.9/g2o/g2o/types/sim3/types_seven_dof_expmap.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/sim3/types_seven_dof_expmap.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/sim3/types_seven_dof_expmap.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_pointxy.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_pointxy.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_pointxy.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_pointxy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_lotsofxy.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_lotsofxy.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_lotsofxy.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_lotsofxy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_offset.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_offset.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_offset.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_offset.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_pointxy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_bearing.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy_bearing.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_bearing.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_pointxy_bearing.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_calib.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy_calib.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_calib.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_pointxy_calib.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_offset.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_pointxy_offset.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_pointxy_offset.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_pointxy_offset.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_prior.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_prior.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_prior.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_prior.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_twopointsxy.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_twopointsxy.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_twopointsxy.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_twopointsxy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_xyprior.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_se2_xyprior.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_se2_xyprior.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_se2_xyprior.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_xy_prior.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/edge_xy_prior.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/edge_xy_prior.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/edge_xy_prior.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/g2o_types_slam2d_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/g2o_types_slam2d_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/parameter_se2_offset.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/parameter_se2_offset.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/parameter_se2_offset.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/parameter_se2_offset.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/se2.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/se2.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/types_slam2d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/types_slam2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/types_slam2d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/types_slam2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/vertex_point_xy.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/vertex_point_xy.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/vertex_point_xy.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/vertex_point_xy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/vertex_se2.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d/vertex_se2.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d/vertex_se2.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d/vertex_se2.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_line2d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_line2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_line2d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_line2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_line2d_pointxy.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_line2d_pointxy.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_line2d_pointxy.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_line2d_pointxy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_line2d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_line2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_line2d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_se2_line2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_segment2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_se2_segment2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_line.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_line.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_line.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_se2_segment2d_line.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_pointLine.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_pointLine.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/edge_se2_segment2d_pointLine.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/edge_se2_segment2d_pointLine.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/g2o_types_slam2d_addons_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/g2o_types_slam2d_addons_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/line_2d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/line_2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/types_slam2d_addons.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/types_slam2d_addons.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/types_slam2d_addons.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/types_slam2d_addons.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/vertex_line2d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/vertex_line2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/vertex_line2d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/vertex_line2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/vertex_segment2d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam2d_addons/vertex_segment2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam2d_addons/vertex_segment2d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam2d_addons/vertex_segment2d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/dquat2mat.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/dquat2mat.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/dquat2mat.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/dquat2mat.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/dquat2mat.wxm` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/dquat2mat.wxm`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/dquat2mat_maxima_generated.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/dquat2mat_maxima_generated.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_pointxyz.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_pointxyz.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_pointxyz.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_pointxyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_lotsofxyz.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_lotsofxyz.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_lotsofxyz.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_lotsofxyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_offset.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_offset.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_offset.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_offset.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_pointxyz.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_pointxyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz_depth.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_pointxyz_depth.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz_depth.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_pointxyz_depth.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz_disparity.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_pointxyz_disparity.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_pointxyz_disparity.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_pointxyz_disparity.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_prior.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_prior.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_prior.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_prior.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_xyzprior.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_se3_xyzprior.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_se3_xyzprior.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_se3_xyzprior.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_xyz_prior.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/edge_xyz_prior.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/edge_xyz_prior.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/edge_xyz_prior.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/g2o_types_slam3d_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/g2o_types_slam3d_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/isometry3d_gradients.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/isometry3d_gradients.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/isometry3d_mappings.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/isometry3d_mappings.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/isometry3d_mappings.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/isometry3d_mappings.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_camera.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/parameter_camera.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_camera.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/parameter_camera.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_se3_offset.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/parameter_se3_offset.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_se3_offset.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/parameter_se3_offset.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_stereo_camera.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/parameter_stereo_camera.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/parameter_stereo_camera.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/parameter_stereo_camera.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/se3_ops.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/se3_ops.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/se3_ops.hpp` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/se3_ops.hpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/se3quat.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/se3quat.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/types_slam3d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/types_slam3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/types_slam3d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/types_slam3d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/vertex_pointxyz.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/vertex_pointxyz.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/vertex_pointxyz.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/vertex_pointxyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/vertex_se3.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d/vertex_se3.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d/vertex_se3.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d/vertex_se3.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/CMakeLists.txt` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_plane.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_plane.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_plane.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_plane.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_calib.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_calib.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_calib.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_se3_calib.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_euler.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_euler.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_euler.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_se3_euler.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_line.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_line.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_line.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_se3_line.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_plane_calib.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/edge_se3_plane_calib.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/edge_se3_plane_calib.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/edge_se3_plane_calib.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/g2o_types_slam3d_addons_api.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/g2o_types_slam3d_addons_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/line3d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/line3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/line3d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/line3d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/plane3d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/plane3d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/types_slam3d_addons.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/types_slam3d_addons.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/types_slam3d_addons.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/types_slam3d_addons.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_line3d.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/vertex_line3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_line3d.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/vertex_line3d.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_plane.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/vertex_plane.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_plane.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/vertex_plane.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_se3_euler.cpp` & `g2o-python-0.0.9/g2o/g2o/types/slam3d_addons/vertex_se3_euler.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/types/slam3d_addons/vertex_se3_euler.h` & `g2o-python-0.0.9/_skbuild/linux-x86_64-3.10/cmake-install/include/g2o/types/slam3d_addons/vertex_se3_euler.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/g2o/what_is_in_these_directories.txt` & `g2o-python-0.0.9/g2o/g2o/what_is_in_these_directories.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/CMakeLists.txt` & `g2o-python-0.0.9/g2o/python/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,8 +59,8 @@
     types_sim3
     types_slam2d
     types_slam2d_addons
     types_slam3d
     types_slam3d_addons
 )
 target_include_directories(g2opy PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
-install(TARGETS g2opy LIBRARY DESTINATION g2opy)
+install(TARGETS g2opy LIBRARY DESTINATION .)
```

### Comparing `g2o-python-0.0.8/g2o/python/README.md` & `g2o-python-0.0.9/g2o/python/README.md`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_base_binary_edge.h` & `g2o-python-0.0.9/g2o/python/core/py_base_binary_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_base_edge.h` & `g2o-python-0.0.9/g2o/python/core/py_base_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_base_fixed_sized_edge.h` & `g2o-python-0.0.9/g2o/python/core/py_base_fixed_sized_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_base_unary_edge.h` & `g2o-python-0.0.9/g2o/python/core/py_base_unary_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_base_variable_sized_edge.cpp` & `g2o-python-0.0.9/g2o/python/core/py_base_variable_sized_edge.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_base_variable_sized_edge.h` & `g2o-python-0.0.9/g2o/python/core/py_base_variable_sized_edge.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_base_vertex.cpp` & `g2o-python-0.0.9/g2o/python/core/py_base_vertex.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_base_vertex.h` & `g2o-python-0.0.9/g2o/python/core/py_base_vertex.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_batch_stats.cpp` & `g2o-python-0.0.9/g2o/python/core/py_batch_stats.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_block_solver.cpp` & `g2o-python-0.0.9/g2o/python/core/py_block_solver.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_block_solver.h` & `g2o-python-0.0.9/g2o/python/core/py_block_solver.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_core.cpp` & `g2o-python-0.0.9/g2o/python/core/py_core.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_eigen_types.cpp` & `g2o-python-0.0.9/g2o/python/core/py_eigen_types.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_estimate_propagator.cpp` & `g2o-python-0.0.9/g2o/python/core/py_estimate_propagator.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_hyper_dijkstra.cpp` & `g2o-python-0.0.9/g2o/python/core/py_hyper_dijkstra.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_hyper_graph.cpp` & `g2o-python-0.0.9/g2o/python/core/py_hyper_graph.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_hyper_graph_action.h` & `g2o-python-0.0.9/g2o/python/core/py_hyper_graph_action.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_jacobian_workspace.cpp` & `g2o-python-0.0.9/g2o/python/core/py_jacobian_workspace.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_linear_solver.h` & `g2o-python-0.0.9/g2o/python/core/py_linear_solver.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_optimizable_graph.cpp` & `g2o-python-0.0.9/g2o/python/core/py_optimizable_graph.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_optimization_algorithm.cpp` & `g2o-python-0.0.9/g2o/python/core/py_optimization_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_robust_kernel.cpp` & `g2o-python-0.0.9/g2o/python/core/py_robust_kernel.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_solver.h` & `g2o-python-0.0.9/g2o/python/core/py_solver.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_sparse_block_matrix.cpp` & `g2o-python-0.0.9/g2o/python/core/py_sparse_block_matrix.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_sparse_optimizer.cpp` & `g2o-python-0.0.9/g2o/python/core/py_sparse_optimizer.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/core/py_sparse_optimizer_terminate_action.h` & `g2o-python-0.0.9/g2o/python/core/py_sparse_optimizer_terminate_action.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/examples/ba_anchored_inverse_depth_demo.py` & `g2o-python-0.0.9/g2o/python/examples/ba_anchored_inverse_depth_demo.py`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/examples/ba_demo.py` & `g2o-python-0.0.9/g2o/python/examples/ba_demo.py`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/examples/gicp_demo.py` & `g2o-python-0.0.9/g2o/python/examples/gicp_demo.py`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/examples/gicp_sba_demo.py` & `g2o-python-0.0.9/g2o/python/examples/gicp_sba_demo.py`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/examples/notebook_slam2d.ipynb` & `g2o-python-0.0.9/g2o/python/examples/notebook_slam2d.ipynb`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/examples/sba_demo.py` & `g2o-python-0.0.9/g2o/python/examples/sba_demo.py`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/examples/sba_demo2.py` & `g2o-python-0.0.9/g2o/python/examples/sba_demo2.py`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/examples/simple_optimize.py` & `g2o-python-0.0.9/g2o/python/examples/simple_optimize.py`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/examples/type_in_python.py` & `g2o-python-0.0.9/g2o/python/examples/type_in_python.py`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/icp/py_types_icp.cpp` & `g2o-python-0.0.9/g2o/python/types/icp/py_types_icp.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/pure/py_types_pure.cpp` & `g2o-python-0.0.9/g2o/python/types/pure/py_types_pure.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/py_types.h` & `g2o-python-0.0.9/g2o/python/types/py_types.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/sba/py_sbacam.h` & `g2o-python-0.0.9/g2o/python/types/sba/py_sbacam.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/sba/py_types_sba.cpp` & `g2o-python-0.0.9/g2o/python/types/sba/py_types_sba.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/sba/py_types_six_dof_expmap.cpp` & `g2o-python-0.0.9/g2o/python/types/sba/py_types_six_dof_expmap.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/sclam2d/py_edge_se2_odom_differential_calib.h` & `g2o-python-0.0.9/g2o/python/types/sclam2d/py_edge_se2_odom_differential_calib.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/sclam2d/py_edge_se2_sensor_calib.h` & `g2o-python-0.0.9/g2o/python/types/sclam2d/py_edge_se2_sensor_calib.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/sclam2d/py_odometry_measurement.h` & `g2o-python-0.0.9/g2o/python/types/sclam2d/py_odometry_measurement.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/sim3/py_sim3.h` & `g2o-python-0.0.9/g2o/python/types/sim3/py_sim3.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/sim3/py_types_seven_dof_expmap.cpp` & `g2o-python-0.0.9/g2o/python/types/sim3/py_types_seven_dof_expmap.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam2d/py_edge_pointxy.h` & `g2o-python-0.0.9/g2o/python/types/slam2d/py_edge_pointxy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam2d/py_edge_se2.h` & `g2o-python-0.0.9/g2o/python/types/slam2d/py_edge_se2.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam2d/py_edge_se2_pointxy.h` & `g2o-python-0.0.9/g2o/python/types/slam2d/py_edge_se2_pointxy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam2d/py_parameter_se2_offset.h` & `g2o-python-0.0.9/g2o/python/types/slam2d/py_parameter_se2_offset.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam2d/py_se2.h` & `g2o-python-0.0.9/g2o/python/types/slam2d/py_se2.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam2d/py_vertex_point_xy.h` & `g2o-python-0.0.9/g2o/python/types/slam2d/py_vertex_point_xy.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam2d/py_vertex_se2.h` & `g2o-python-0.0.9/g2o/python/types/slam2d/py_vertex_se2.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam3d/py_edge_pointxyz.h` & `g2o-python-0.0.9/g2o/python/types/slam3d/py_edge_pointxyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam3d/py_edge_se3.h` & `g2o-python-0.0.9/g2o/python/types/slam3d/py_edge_se3.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam3d/py_edge_se3_pointxyz.h` & `g2o-python-0.0.9/g2o/python/types/slam3d/py_edge_se3_pointxyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam3d/py_parameter.h` & `g2o-python-0.0.9/g2o/python/types/slam3d/py_parameter.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam3d/py_se3quat.h` & `g2o-python-0.0.9/g2o/python/types/slam3d/py_se3quat.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam3d/py_vertex_pointxyz.h` & `g2o-python-0.0.9/g2o/python/types/slam3d/py_vertex_pointxyz.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/python/types/slam3d/py_vertex_se3.h` & `g2o-python-0.0.9/g2o/python/types/slam3d/py_vertex_se3.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/script/android.toolchain.cmake` & `g2o-python-0.0.9/g2o/script/android.toolchain.cmake`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/script/codecov.sh.in` & `g2o-python-0.0.9/g2o/script/codecov.sh.in`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/script/git-clang-format.py` & `g2o-python-0.0.9/g2o/script/git-clang-format.py`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/script/install-deps-linux.sh` & `g2o-python-0.0.9/g2o/script/install-deps-linux.sh`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/script/install-deps-windows.bat` & `g2o-python-0.0.9/g2o/script/install-deps-windows.bat`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/script/run-style-check-diff.sh` & `g2o-python-0.0.9/g2o/script/run-style-check-diff.sh`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/CMakeLists.txt` & `g2o-python-0.0.9/g2o/unit_test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/data/data_queue_tests.cpp` & `g2o-python-0.0.9/g2o/unit_test/data/data_queue_tests.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/data/io_data.cpp` & `g2o-python-0.0.9/g2o/unit_test/data/io_data.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/general/auto_diff.cpp` & `g2o-python-0.0.9/g2o/unit_test/general/auto_diff.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/general/base_fixed_sized_edge.cpp` & `g2o-python-0.0.9/g2o/unit_test/general/base_fixed_sized_edge.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/general/clear_and_redo.cpp` & `g2o-python-0.0.9/g2o/unit_test/general/clear_and_redo.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/general/graph_operations.cpp` & `g2o-python-0.0.9/g2o/unit_test/general/graph_operations.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/general/robust_kernel_tests.cpp` & `g2o-python-0.0.9/g2o/unit_test/general/robust_kernel_tests.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/general/sparse_block_matrix.cpp` & `g2o-python-0.0.9/g2o/unit_test/general/sparse_block_matrix.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/sba/io_sba.cpp` & `g2o-python-0.0.9/g2o/unit_test/sba/io_sba.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/sba/io_six_dof_expmap.cpp` & `g2o-python-0.0.9/g2o/unit_test/sba/io_six_dof_expmap.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/sclam2d/io_sclam2d.cpp` & `g2o-python-0.0.9/g2o/unit_test/sclam2d/io_sclam2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/sclam2d/odom_convert_sclam2d.cpp` & `g2o-python-0.0.9/g2o/unit_test/sclam2d/odom_convert_sclam2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/sclam2d/sensor_offset.cpp` & `g2o-python-0.0.9/g2o/unit_test/sclam2d/sensor_offset.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/sim3/allocate_sim3.cpp` & `g2o-python-0.0.9/g2o/unit_test/sim3/allocate_sim3.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/sim3/io_sim3.cpp` & `g2o-python-0.0.9/g2o/unit_test/sim3/io_sim3.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/sim3/jacobians_sim3.cpp` & `g2o-python-0.0.9/g2o/unit_test/sim3/jacobians_sim3.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam2d/io_slam2d.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam2d/io_slam2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam2d/jacobians_slam2d.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam2d/jacobians_slam2d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam2d/mappings_se2.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam2d/mappings_se2.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam2d_addons/io_slam2d_addons.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam2d_addons/io_slam2d_addons.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam3d/io_slam3d.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam3d/io_slam3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam3d/jacobians_slam3d.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam3d/jacobians_slam3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam3d/mappings_slam3d.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam3d/mappings_slam3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam3d/optimization_slam3d.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam3d/optimization_slam3d.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam3d/orthogonal_matrix.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam3d/orthogonal_matrix.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/slam3d_addons/io_slam3d_addons.cpp` & `g2o-python-0.0.9/g2o/unit_test/slam3d_addons/io_slam3d_addons.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/solver/CMakeLists.txt` & `g2o-python-0.0.9/g2o/unit_test/solver/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/solver/allocate_algorithm_test.cpp` & `g2o-python-0.0.9/g2o/unit_test/solver/allocate_algorithm_test.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/solver/linear_solver_test.cpp` & `g2o-python-0.0.9/g2o/unit_test/solver/linear_solver_test.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/solver/sparse_system_helper.cpp` & `g2o-python-0.0.9/g2o/unit_test/solver/sparse_system_helper.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/solver/sparse_system_helper.h` & `g2o-python-0.0.9/g2o/unit_test/solver/sparse_system_helper.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/stuff/command_args_tests.cpp` & `g2o-python-0.0.9/g2o/unit_test/stuff/command_args_tests.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/stuff/filesys_tools_tests.cpp` & `g2o-python-0.0.9/g2o/unit_test/stuff/filesys_tools_tests.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/stuff/misc_tests.cpp` & `g2o-python-0.0.9/g2o/unit_test/stuff/misc_tests.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/stuff/property_tests.cpp` & `g2o-python-0.0.9/g2o/unit_test/stuff/property_tests.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/stuff/string_tools_tests.cpp` & `g2o-python-0.0.9/g2o/unit_test/stuff/string_tools_tests.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/stuff/tuple_tools_tests.cpp` & `g2o-python-0.0.9/g2o/unit_test/stuff/tuple_tools_tests.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/test_helper/allocate_optimizer.cpp` & `g2o-python-0.0.9/g2o/unit_test/test_helper/allocate_optimizer.cpp`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/test_helper/allocate_optimizer.h` & `g2o-python-0.0.9/g2o/unit_test/test_helper/allocate_optimizer.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/test_helper/evaluate_jacobian.h` & `g2o-python-0.0.9/g2o/unit_test/test_helper/evaluate_jacobian.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/test_helper/g2o_test_helper_api.h` & `g2o-python-0.0.9/g2o/unit_test/test_helper/g2o_test_helper_api.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/test_helper/io.h` & `g2o-python-0.0.9/g2o/unit_test/test_helper/io.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o/unit_test/test_helper/random_state.h` & `g2o-python-0.0.9/g2o/unit_test/test_helper/random_state.h`

 * *Files identical despite different names*

### Comparing `g2o-python-0.0.8/g2o_python.egg-info/PKG-INFO` & `g2o-python-0.0.9/g2o_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: g2o-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper package for G2O python bindings.
 Home-page: https://github.com/miquelmassot/g2o-python
 Maintainer: Miquel Massot
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -45,15 +46,15 @@
 # g2o-python
 
 This is a wrapper of the python binding of [g2o](https://github.com/RainerKuemmerle/g2o) using its branch `pymem`.
 
 ## How to use it in your code
 
 ```python
-from g2opy import g2opy as g2o
+import g2o
 # Your code
 
 ```
 
 More examples [available here](https://github.com/RainerKuemmerle/g2o/tree/pymem/python/examples).
 
 
@@ -62,7 +63,9 @@
 ```bash
 pip install -U g2o-python
 ```
 
 ## Build from source
 
 Clone this repository and run `pip install -U --user -v .`
+
+
```

### Comparing `g2o-python-0.0.8/setup.py` & `g2o-python-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,24 @@
     cmake_source_dir = "g2o"
 
     install_requires = [
         'numpy',
         'scikit-build',
     ]
 
+    # Fix g2o/python/CMakeLists.txt file, install pybind11 to "."
+    with open(os.path.join(cmake_source_dir, "python/CMakeLists.txt"), "r") as file:
+        filedata = file.read()
+        filedata = filedata.replace(
+            "install(TARGETS g2opy LIBRARY DESTINATION g2opy)",
+            "install(TARGETS g2opy LIBRARY DESTINATION .)"
+        )
+    with open(os.path.join(cmake_source_dir, "python/CMakeLists.txt"), "w") as file:
+        file.write(filedata)
+
     # Fix g2o/CMakeLists.txt file, remove the lines
     #   set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${g2o_LIBRARY_OUTPUT_DIRECTORY})
     #   set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${g2o_LIBRARY_OUTPUT_DIRECTORY})
     #   set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${g2o_RUNTIME_OUTPUT_DIRECTORY})
     with open(os.path.join(cmake_source_dir, "CMakeLists.txt"), "r") as file:
         filedata = file.read()
         filedata = filedata.replace(
@@ -31,14 +41,19 @@
         filedata = filedata.replace(
             "set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${g2o_RUNTIME_OUTPUT_DIRECTORY})",
             "",
         )
     with open(os.path.join(cmake_source_dir, "CMakeLists.txt"), "w") as file:
         file.write(filedata)
 
+    # Add __init__.py at g2o root folder to be able to write in python:
+    #   import g2o
+    with open(os.path.join(cmake_source_dir, "__init__.py"), "w") as file:
+        file.write("from .g2opy import *  # noqa: F401")
+
     cmake_args = [
         # See g2o/CMakeLists.txt for options and defaults
         "-DBUILD_SHARED_LIBS=OFF",
         "-DG2O_USE_OPENGL=OFF",
         "-DG2O_BUILD_EXAMPLES=OFF",
         "-DG2O_BUILD_APPS=OFF",
         "-DG2O_BUILD_PYTHON=ON",
@@ -50,22 +65,22 @@
         import shlex
 
         cmake_args.extend(shlex.split(os.environ["CMAKE_ARGS"]))
         del shlex
 
     skbuild.setup(
         name="g2o-python",
-        version="0.0.8",
+        version="0.0.9",
         url="https://github.com/miquelmassot/g2o-python",
         license="MIT",
         description="Wrapper package for G2O python bindings.",
         long_description=io.open("README.md", encoding="utf-8").read(),
         long_description_content_type="text/markdown",
-        packages=["g2opy"],
         maintainer="Miquel Massot",
+        packages=["g2o"],
         ext_modules=EmptyListWithLength(),
         install_requires=install_requires,
         python_requires=">=3.6",
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Environment :: Console",
             "Intended Audience :: Developers",
```

