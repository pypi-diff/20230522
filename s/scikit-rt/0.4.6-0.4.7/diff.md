# Comparing `tmp/scikit-rt-0.4.6.tar.gz` & `tmp/scikit-rt-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-rt-0.4.6.tar", last modified: Wed May 17 12:13:46 2023, max compression
+gzip compressed data, was "scikit-rt-0.4.7.tar", last modified: Mon May 22 09:23:11 2023, max compression
```

## Comparing `scikit-rt-0.4.6.tar` & `scikit-rt-0.4.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.439063 scikit-rt-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-17 12:13:46.439063 scikit-rt-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/pypi.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-17 12:13:46.439063 scikit-rt-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.403063 scikit-rt-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.407063 scikit-rt-0.4.6/src/scikit_rt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-17 12:13:46.000000 scikit-rt-0.4.6/src/scikit_rt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-17 12:13:46.000000 scikit-rt-0.4.6/src/scikit_rt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:13:46.000000 scikit-rt-0.4.6/src/scikit_rt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-17 12:13:46.000000 scikit-rt-0.4.6/src/scikit_rt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 12:13:46.000000 scikit-rt-0.4.6/src/scikit_rt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.419063 scikit-rt-0.4.6/src/skrt/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.419063 scikit-rt-0.4.6/src/skrt/better_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   132021 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/better_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/better_viewer/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    73387 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.403063 scikit-rt-0.4.6/src/skrt/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.423063 scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_Affine.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_Translation.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.423063 scikit-rt-0.4.6/src/skrt/data/niftyreg_parameter_files/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/niftyreg_parameter_files/Affine.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/data/niftyreg_parameter_files/Rigid.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/dicom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39911 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/dose.py
--rw-r--r--   0 runner    (1001) docker     (123)   255896 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)   118731 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/patient.py
--rw-r--r--   0 runner    (1001) docker     (123)   134874 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    60958 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)   352303 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.427063 scikit-rt-0.4.6/src/skrt/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/viewer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/src/skrt/viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:13:46.439063 scikit-rt-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_01_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_dose.py
--rw-r--r--   0 runner    (1001) docker     (123)    61362 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_patient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_qv_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_qv_quickviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_qv_struct_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_qv_struct_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_qv_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34152 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_roi_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_synthetic_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-17 12:09:40.000000 scikit-rt-0.4.6/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.882695 scikit-rt-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-22 09:23:11.882695 scikit-rt-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-22 09:23:11.882695 scikit-rt-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.850695 scikit-rt-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.854694 scikit-rt-0.4.7/src/scikit_rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.862695 scikit-rt-0.4.7/src/skrt/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.866695 scikit-rt-0.4.7/src/skrt/better_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   132455 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/better_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/better_viewer/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73387 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.854694 scikit-rt-0.4.7/src/skrt/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.870695 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Affine.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Translation.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.870695 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/Affine.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/Rigid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/dicom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39911 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)   255921 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118731 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134908 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60958 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   352303 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.870695 scikit-rt-0.4.7/src/skrt/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/viewer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.882695 scikit-rt-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_01_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61981 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_quickviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_struct_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_struct_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34152 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_roi_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_synthetic_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_viewer.py
```

### Comparing `scikit-rt-0.4.6/LICENSE` & `scikit-rt-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/PKG-INFO` & `scikit-rt-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.6
+Version: 0.4.7
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.6/README.md` & `scikit-rt-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/pypi.md` & `scikit-rt-0.4.7/pypi.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/setup.cfg` & `scikit-rt-0.4.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-rt
-version = 0.4.6
+version = 0.4.7
 author = H. Pullen, K. Harrison
 author_email = scikit-rt@hep.phy.cam.ac.uk
 description = Toolkit for analysis of radiotherapy data
 long_description = file: pypi.md
 long_description_content_type = text/markdown
 url = https://github.com/scikit-rt/scikit-rt
 project_urls =
```

### Comparing `scikit-rt-0.4.6/src/scikit_rt.egg-info/PKG-INFO` & `scikit-rt-0.4.7/src/scikit_rt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.6
+Version: 0.4.7
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.6/src/scikit_rt.egg-info/SOURCES.txt` & `scikit-rt-0.4.7/src/scikit_rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/scikit_rt.egg-info/requires.txt` & `scikit-rt-0.4.7/src/scikit_rt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/__init__.py` & `scikit-rt-0.4.7/src/skrt/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/application.py` & `scikit-rt-0.4.7/src/skrt/application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/better_viewer/__init__.py` & `scikit-rt-0.4.7/src/skrt/better_viewer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,16 @@
         show=True,
         include_image=False,
         no_ui=None,
         ylabel_first_only=True,
         yticks_first_only=False,
         ytick_labels_first_only=True,
         colorbar_last_only=True,
+        zoom=None,
+        zoom_ui=None,
         **kwargs,
     ):
         '''
         Display one or more interactive images.
 
         **Parameters:**
 
@@ -905,14 +907,18 @@
         # Make individual viewers
         self.scale_in_mm = scale_in_mm
         self.viewers = []
         viewer_type = SingleViewer if not orthog_view else OrthogViewer
         kwargs = {key.replace('colour', 'color'): val for key, val in kwargs.items()}
         mask_threshold = kwargs.get("mask_threshold", 0.5)
 
+        if zoom_ui is None:
+            zoom_ui = (zoom is not None
+                       or any([bool(self.rois[i]) for i in range(self.n)]))
+
         for i in range(self.n):
             
             no_ylabel = (no_ylabel_default if
                     (i == 0 or not ylabel_first_only) else True)
             no_yticks = (no_yticks_default if
                     (i == 0 or not yticks_first_only) else True)
             no_ytick_labels = (no_ytick_labels_default if
@@ -935,14 +941,16 @@
                 legend_bbox_to_anchor=legend_bbox_to_anchor,
                 legend_loc=legend_loc,
                 include_image=include_image,
                 colorbar=colorbar,
                 no_ylabel=no_ylabel,
                 no_yticks=no_yticks,
                 no_ytick_labels=no_ytick_labels,
+                zoom=zoom,
+                zoom_ui=zoom_ui,
                 **kwargs,
             )
             self.viewers.append(viewer)
         self.n = len(self.viewers)
         if not self.n:
             print('No valid images found.')
             return
@@ -1557,20 +1565,25 @@
 
         # Deal with hiding/showing all ROIs
         for v in self.viewers:
             # Hide all ROIs
             if v.ui_roi_deselect_all.value:
                 for roi in v.rois:
                     roi.checkbox.value = False
-                v.ui_roi_deselect_all.value = False
 
             # Show all ROIs
             if v.ui_roi_select_all.value:
                 for roi in v.rois:
                     roi.checkbox.value = True
+
+        # Toggle values for deselection/selection.
+        for v in self.viewers:
+            if v.ui_roi_deselect_all.value:
+                v.ui_roi_deselect_all.value = False
+            if v.ui_roi_select_all.value:
                 v.ui_roi_select_all.value = False
 
         # Deal with view change
         view_changed = self.ui_view.value != self.view
         if view_changed:
             self.view = self.ui_view.value
             for v in self.viewers:
@@ -1695,15 +1708,15 @@
         intensity_step=None,
         figsize=_default_figsize,
         xlim=None,
         ylim=None,
         zlim=None,
         zoom=None,
         zoom_centre=None,
-        zoom_ui=False,
+        zoom_ui=None,
         cmap=None,
         colorbar=False,
         colorbar_label=None,
         clb_kwargs=None,
         clb_label_kwargs=None,
         no_xlabel=False,
         no_ylabel=False,
@@ -1891,15 +1904,15 @@
             'y-z': [zlim, ylim],
             'x-z': [zlim, xlim]
         }
         self.zoom = zoom
         self.zoom_centre = zoom_centre
         self.zoom_ui = zoom_ui
         if zoom_ui is None:
-            self.zoom_ui = bool(self.has_rois)
+            self.zoom_ui = bool(self.has_rois or zoom is not None)
         self.major_ticks = major_ticks
         self.minor_ticks = minor_ticks
         self.ticks_all_sides = ticks_all_sides
         self.no_axis_labels = no_axis_labels
         self.legend_bbox_to_anchor = legend_bbox_to_anchor
         self.legend_loc = legend_loc
         self.shift = [None, None, None]
```

### Comparing `scikit-rt-0.4.6/src/skrt/better_viewer/options.py` & `scikit-rt-0.4.7/src/skrt/better_viewer/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 
     # For axes, set spacing (pad) and size of label and title
     plt.rc("axes", labelpad=0, labelsize=25, titlepad=17, titlesize=25)
 
     # Set default text charactieristics.
     # Possible weight values are:
     # 100, 200, 300, 400 / "normal", 500, 600, 700 / "bold", 800, 900.
-    plt.rc("font", family="serif", serif=["Times"], size=20, weight=400)
+    if usetex:
+        plt.rc("font", family="serif", serif=["Times"])
+    plt.rc("font", size=20, weight=400)
 
     # Set default font size for legends.
     plt.rc("legend", fontsize=16)
 
     # Set mathematics typeface when using matplotlib's built-in fonts.
     plt.rc("mathtext", fontset="dejavuserif")
```

### Comparing `scikit-rt-0.4.6/src/skrt/core.py` & `scikit-rt-0.4.7/src/skrt/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt` & `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_Affine.txt` & `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Affine.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt` & `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt` & `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt` & `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_Rigid.txt` & `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Rigid.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/data/elastix_parameter_files/MI_Translation.txt` & `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Translation.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/dicom_writer.py` & `scikit-rt-0.4.7/src/skrt/dicom_writer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/dose.py` & `scikit-rt-0.4.7/src/skrt/dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/image.py` & `scikit-rt-0.4.7/src/skrt/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1438,25 +1438,26 @@
             print('WARNING: Unable to execute function '\
                     + 'skrt.image.Image.get_slice_foreground()')
 
         # Extract slice data.
         image_slice = self.get_data()[:, :, idx]
 
         # Obtain intensity values relative to the minimum.
-        test_slice = np.uint32(image_slice - image_slice.min())
+        test_slice = image_slice - image_slice.min()
         # Make this a 2D array.
         test_slice = np.squeeze(test_slice)
 
         # Fallback to default threshold.
         if threshold is None:
             threshold = skrt.core.Defaults().foreground_threshold
 
         # Calculate Otsu threshold, or rescale threshold value provided.
         if threshold is None:
-            rescaled_threshold = mahotas.thresholding.otsu(test_slice)
+            rescaled_threshold = mahotas.thresholding.otsu(
+                    test_slice.astype(np.uint32))
         else:
             rescaled_threshold = threshold - image_slice.min()
 
         # Handle case where slice contains intensity values above threshold,
         # and intensities are not the same.
         if ((test_slice.max() > rescaled_threshold) and
                 (test_slice.max() - test_slice.min() > 0)):
@@ -1568,15 +1569,15 @@
 
         dxy : int, default=0
             Margin, in pixel units, to be added to each slice foreground mask.
         '''
         self.load()
 
         if vmin is None and vmax is None:
-            return Image(np.ones(self.data.shape, dtype=np.int8),
+            return Image(np.ones(self.data.shape, dtype=bool),
                          affine = self.get_affine())
 
         masks = [self.get_foreground_mask(
             threshold=val, convex_hull=convex_hull,
             fill_holes=fill_holes, dxy=dxy) if val is not None
                  else None for val in [vmin, vmax]]
```

### Comparing `scikit-rt-0.4.6/src/skrt/multi.py` & `scikit-rt-0.4.7/src/skrt/multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/patient.py` & `scikit-rt-0.4.7/src/skrt/patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/registration.py` & `scikit-rt-0.4.7/src/skrt/registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
                 f"Unable to determine RegistrationClass for engine: '{engine}',"
                 f"engine_dir: '{engine_dir}';"
                 "\nknown engines are: {sorted(engines)}")
 
         self.engine = engine_cls(path=engine_dir)
 
         # Set up directory
-        path = fullpath(path).replace(" ", "_")
+        #path = fullpath(path).replace(" ", "_")
         self.path = path
         if not os.path.exists(path):
             os.makedirs(path)
         elif overwrite:
             shutil.rmtree(path)
             os.mkdir(path)
 
@@ -1219,15 +1219,16 @@
             self.register_step(step)
             return False
         return True
 
     def make_tmp_dir(self):
         """Create temporary directory."""
 
-        self._tmp_dir = os.path.join(self.path, ".tmp").replace(" ", "_")
+        #self._tmp_dir = os.path.join(self.path, ".tmp").replace(" ", "_")
+        self._tmp_dir = os.path.join(self.path, ".tmp")
         if not os.path.exists(self._tmp_dir):
             os.mkdir(self._tmp_dir)
 
     def rm_tmp_dir(self):
         """Delete temporary directory and its contents."""
 
         if not hasattr(self, "_tmp_dir"):
@@ -2609,33 +2610,32 @@
         software can't be located in the existing environment.  If True, modify
         environment based on <path> in all cases.
         """
         exe_dir = None
 
         # Check if environment already set for running the registration engine.
         if not (path and force):
-            stdout = subprocess.run(
-                    ["which", str(self.name)], capture_output=True).stdout
-            if stdout:
-                exe_dir = Path(stdout.decode()).parent
+            exe_path = shutil.which(self.name)
+            if exe_path is not None:
+                exe_dir = Path(exe_path).parent
 
         # Return if environment already set and not forcing new setup,
         # of if no value specified for path (no new setup possible).
         if (exe_dir and not force) or path is None:
             return
         
         # Try to define path(s) to registration-engine executables,
         # if not already defined, or forcing new setup.
         if not exe_dir or force:
             exe_dir = self.set_exe_paths(path)
 
         if exe_dir:
             # Set environment variables.
             lib_dir = exe_dir.parent / "lib"
-            # Cover Linux and MacOS
+            # Cover Linux, MacOS, Windows.
             for env_var, env_val in [
                     ("DYLD_FALLBACK_LIBRARY_PATH", lib_dir),
                     ("LD_LIBRARY_PATH", lib_dir),
                     ("PATH", exe_dir)
                     ]:
                 if not (os.environ.get(env_var, "")).startswith(str(env_val)):
                     prepend_path(env_var, env_val)
@@ -2767,19 +2767,19 @@
             # Add parameters needed to allow warping of the moving image.
             translation.update(get_image_transform_parameters(fixed_image))
 
         return translation
 
     def get_def_cmd(self, fixed_path, outdir, tfile):
         # Return command for computing deformation field.
-        return f"{self.transformix} -def all -out {outdir} -tp {tfile}".split()
+        return [self.transformix, "-def", "all", "-out", outdir, "-tp", tfile]
 
     def get_jac_cmd(self, fixed_path, outdir, tfile):
         # Return command for computing Jacobian determinant.
-        return f"{self.transformix} -jac all -out {outdir} -tp {tfile}".split()
+        return [self.transformix, "-jac", "all", "-out", outdir, "-tp", tfile]
 
     def get_registration_cmd(
             self, fixed_path, moving_path, fixed_mask_path, moving_mask_path,
             pfile, outdir, tfile=None):
 
         # Start command with execuable and paths to fixed and moving images.
         cmd = [
@@ -2963,22 +2963,22 @@
                 "0 0 0 1",
                 ]
 
         return translation
 
     def get_def_cmd(self, fixed_path, outdir, tfile):
         # Return command for computing deformation field.
-        return (f"{self.reg_transform} -ref {fixed_path} "
-                f"-disp {tfile} {outdir}/deformationField.nii").split()
+        return [self.reg_transform, "-ref", fixed_path, "-disp",
+                tfile, f"{outdir}/deformationField.nii"]
 
     def get_jac_cmd(self, fixed_path, outdir, tfile):
         # Return command for computing Jacobian determinant.
         if ".nii" == Path(tfile).suffix:
-            return (f"{self.reg_jacobian} -trans {tfile} -ref {fixed_path} "
-                    f"-jac {outdir}/spatialJacobian.nii").split()
+            return [self.reg_jacobian, "-trans", tfile, "-ref", fixed_path,
+                    "-jac", f"{outdir}/spatialJacobian.nii"]
 
     def get_registration_cmd(
             self, fixed_path, moving_path, fixed_mask_path, moving_mask_path,
             pfile, outdir, tfile=None):
 
         # Read registration parameters from file.
         params = self.read_parameters(pfile)
@@ -3419,15 +3419,16 @@
     if path_must_exist:
         if not os.path.exists(path):
             path_ok = False
 
     if path_ok:
         if variable in os.environ:
             if os.environ[variable]:
-                os.environ[variable] = f'{path}:{os.environ[variable]}'
+                os.environ[variable] = os.pathsep.join(
+                        [path, os.environ[variable]])
         else:
             os.environ[variable] = path
 
 
 def read_parameters(infile, engine=None):
     """
     Get dictionary of parameters from a registration parameter file.
@@ -3507,15 +3508,15 @@
         Path to output parameter file.  If None, overwrite input parameter file.
 
     engine: str, default=None
         String identifying registration engine, corresponding to
         a key of the dictionary skrt.registration.engines.
     """
     get_engine_cls(engine)().shift_translation_parameters(
-            infile, dx=0, dy=0, dz=0, outfile=None)
+            infile, dx=dx, dy=dy, dz=dz, outfile=outfile)
 
 
 def write_parameters(outfile, params, engine=None):
     """
     Write dictionary of parameters to a registration parameter file.
 
     **Parameters:**
```

### Comparing `scikit-rt-0.4.6/src/skrt/segmentation.py` & `scikit-rt-0.4.7/src/skrt/segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/simulation.py` & `scikit-rt-0.4.7/src/skrt/simulation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/structures.py` & `scikit-rt-0.4.7/src/skrt/structures.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/viewer/core.py` & `scikit-rt-0.4.7/src/skrt/viewer/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/src/skrt/viewer/viewer.py` & `scikit-rt-0.4.7/src/skrt/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_01_setup.py` & `scikit-rt-0.4.7/tests/test_01_setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_application.py` & `scikit-rt-0.4.7/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_core.py` & `scikit-rt-0.4.7/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_dose.py` & `scikit-rt-0.4.7/tests/test_dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_image.py` & `scikit-rt-0.4.7/tests/test_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -994,42 +994,57 @@
     # with the sphere dimensions, allowing tolreance of +/-1.
     for idx in range(3):
         assert abs(bb_centre[idx] - centre[idx]) <= 1
         assert abs(bb_widths[idx] - 2 * radius) <= 1
 
 @needs_mahotas
 def test_create_intensity_mask():
+    """
+    Test creation of intensity masks.
+    """
+    # Create synthetic image (default intensity -1024),
+    # featuring cube and sphere of higher intensities.
     sim = SyntheticImage((100, 100, 40))
-    sim.add_cube(side_length=5, name="cube", centre=(25, 60, 12), intensity=60)
-    sim.add_sphere(radius=10, name="sphere", centre=(80, 20, 12), intensity=50)
+    sim.add_cube(
+            side_length=5, name="cube", centre=(25, 60, 12), intensity=60.4)
+    sim.add_sphere(
+            radius=10, name="sphere", centre=(80, 20, 12), intensity=50.6)
 
+    # Create expected masks given different minimum and maximum intensities.
     nx, ny, nz = sim.get_n_voxels()
-    ones = np.ones((ny, nx, nz), dtype=np.uint32)
+    ones = np.ones((ny, nx, nz), dtype=bool)
     masks = [
             ((None, None), ones),
-            ((45, 55), ones * (sim.get_data() == 50)),
-            ((55, None), ones * (sim.get_data() == 60)),
-            ((None, 55),  1 - ones * (sim.get_data() == 60)),
+            ((50.59, 50.61), ones * (sim.get_data() == 50.6)),
+            ((60, None), ones * (sim.get_data() == 60.4)),
+            ((None, 55),  1 - ones * (sim.get_data() == 60.4)),
             ]
 
+    # Check intensitiy masks against expected masks.
     for intensities, mask2 in masks:
         vmin, vmax = intensities
         mask1 = sim.get_intensity_mask(vmin, vmax).get_data()
-        mask1 = mask1.astype(np.uint32)
         mask1[mask1 > 0] = 1
 
         assert mask1.shape == mask2.shape
+        # If there are no constraints on vmin and vmax,
+        # all elements of the intensity mask should be True
+        # (minimum and maximum both 1).
+        # Otherwise, the minimum should be 0 and the maximum should be 1.
         if vmin is None and vmax is None:
             assert mask1.min() == 1
         else:
             assert mask1.min() == 0
         assert mask1.max() == 1
         assert mask1.min() == mask2.min()
         assert mask1.max() == mask2.max()
         assert mask1.sum() == mask2.sum()
+
+        # Check that intensity mask is voxel for voxel identical
+        # to the created mask.
         assert np.all(mask1 == mask2)
 
 @needs_mahotas
 def test_translation_to_align():
     """Test calculation of translation to align pair of images."""
 
     # Create synthetic images featuring a sphere.
```

### Comparing `scikit-rt-0.4.6/tests/test_multi.py` & `scikit-rt-0.4.7/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_patient.py` & `scikit-rt-0.4.7/tests/test_patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_qv_image.py` & `scikit-rt-0.4.7/tests/test_qv_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_qv_quickviewer.py` & `scikit-rt-0.4.7/tests/test_qv_quickviewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_qv_struct_loader.py` & `scikit-rt-0.4.7/tests/test_qv_struct_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_qv_struct_metrics.py` & `scikit-rt-0.4.7/tests/test_qv_struct_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_qv_structs.py` & `scikit-rt-0.4.7/tests/test_qv_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_registration.py` & `scikit-rt-0.4.7/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_roi_metrics.py` & `scikit-rt-0.4.7/tests/test_roi_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_segmentation.py` & `scikit-rt-0.4.7/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_structs.py` & `scikit-rt-0.4.7/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_synthetic_image.py` & `scikit-rt-0.4.7/tests/test_synthetic_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.6/tests/test_viewer.py` & `scikit-rt-0.4.7/tests/test_viewer.py`

 * *Files identical despite different names*

