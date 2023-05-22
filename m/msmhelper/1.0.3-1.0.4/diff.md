# Comparing `tmp/msmhelper-1.0.3.tar.gz` & `tmp/msmhelper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmhelper-1.0.3.tar", last modified: Mon Apr 17 15:33:59 2023, max compression
+gzip compressed data, was "msmhelper-1.0.4.tar", last modified: Mon May 22 16:12:36 2023, max compression
```

## Comparing `msmhelper-1.0.3.tar` & `msmhelper-1.0.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-17 15:33:47.000000 msmhelper-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 15:33:47.000000 msmhelper-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-17 15:33:59.035167 msmhelper-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-04-17 15:33:47.000000 msmhelper-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-17 15:33:47.000000 msmhelper-1.0.3/extra-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-17 15:33:59.035167 msmhelper-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-17 15:33:47.000000 msmhelper-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.031167 msmhelper-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.031167 msmhelper-1.0.3/src/msmhelper/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.031167 msmhelper-1.0.3/src/msmhelper/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/ck_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/compare_discretization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6398 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/contact_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/dynamical_coring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/gaussian_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4021 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/implied_timescales.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3162 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/waiting_time_dist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4457 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/waiting_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/md/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/md/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/md/corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/md/timescales.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/msm/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/msm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/timescales.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/msm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/utils/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/plot/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/plot/_ck_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3962 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/plot/_wtd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/statetraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.031167 msmhelper-1.0.3/src/msmhelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test___main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_md_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_md_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_md_timescales.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_msm_msm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_msm_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_msm_timescales.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_msm_utils_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_statetraj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_utils__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_utils_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_utils_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.132804 msmhelper-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-22 16:12:23.000000 msmhelper-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 16:12:23.000000 msmhelper-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-05-22 16:12:36.132804 msmhelper-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-05-22 16:12:23.000000 msmhelper-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-22 16:12:23.000000 msmhelper-1.0.4/extra-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-22 16:12:36.132804 msmhelper-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-22 16:12:23.000000 msmhelper-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.124804 msmhelper-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.124804 msmhelper-1.0.4/src/msmhelper/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.128804 msmhelper-1.0.4/src/msmhelper/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/_cli/ck_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/_cli/compare_discretization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6398 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/_cli/contact_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/_cli/dynamical_coring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/_cli/gaussian_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4021 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/_cli/implied_timescales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3162 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/_cli/waiting_time_dist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4457 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/_cli/waiting_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.128804 msmhelper-1.0.4/src/msmhelper/md/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/md/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/md/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/md/timescales.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.128804 msmhelper-1.0.4/src/msmhelper/msm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/msm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/msm/msm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/msm/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/msm/timescales.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.128804 msmhelper-1.0.4/src/msmhelper/msm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/msm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/msm/utils/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.128804 msmhelper-1.0.4/src/msmhelper/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/plot/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/plot/_ck_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3962 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/plot/_wtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/statetraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.128804 msmhelper-1.0.4/src/msmhelper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/utils/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-22 16:12:23.000000 msmhelper-1.0.4/src/msmhelper/utils/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.124804 msmhelper-1.0.4/src/msmhelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-05-22 16:12:36.000000 msmhelper-1.0.4/src/msmhelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-22 16:12:36.000000 msmhelper-1.0.4/src/msmhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:12:36.000000 msmhelper-1.0.4/src/msmhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-22 16:12:36.000000 msmhelper-1.0.4/src/msmhelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-22 16:12:36.000000 msmhelper-1.0.4/src/msmhelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 16:12:36.000000 msmhelper-1.0.4/src/msmhelper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:36.132804 msmhelper-1.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test___main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_md_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_md_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_md_timescales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_msm_msm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_msm_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_msm_timescales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_msm_utils_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_statetraj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_utils__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_utils_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-22 16:12:23.000000 msmhelper-1.0.4/test/test_utils_tests.py
```

### Comparing `msmhelper-1.0.3/LICENSE` & `msmhelper-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/PKG-INFO` & `msmhelper-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmhelper
-Version: 1.0.3
+Version: 1.0.4
 Summary: Helper functions for Markov State Models.
 Home-page: https://github.com/moldyn/msmhelper
 Author: braniii
 License: BSD-3-Clause License
 Project-URL: Documentation, https://moldyn.github.io/msmhelper
 Project-URL: Source Code, https://github.com/moldyn/msmhelper
 Project-URL: Changelog, https://moldyn.github.io/msmhelper/changelog
@@ -86,15 +86,15 @@
 ## Implemented Key Functionalities
 - Hummer-Szabo projection of optimal dimensionality reduction by [Hummer and Szabo 2014](https://doi.org/10.1021/jp508375q)
 - Dynamical coring by [Nagel et al. 2019](https://doi.org/10.1063/1.5081767)
 - Fast extraction of pathways and MSM-based prediction of pathways based on the definition of [Nagel et al. 2020](https://pubs.acs.org/doi/10.1021/acs.jctc.0c00774)
 - Fast calculation of waiting times based on both, state trajectories and MSMs
 - Blazing fast [Chapman-Kolmogorov](https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test implementation
 - Entropy-based similarity measure to compare different state discretizations, this method will be published soon in Nagel 2023
-- Contact representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact structural representation of the states
+- Contact representation by [Nagel et al. 2023](https://arxiv.org/abs/2303.03814) for a compact structural representation of the states
 - Command-line interface providing both, visualization and analysis methods
 - Provide (non-reversible) transition matrix of all states (corresponds in pyemma to `connectivity='none', 'all'` which will (probably) [never be implemented](https://github.com/markovmodel/PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/_msm_estimator_base.py#L110))
 
 ## Getting started
 ### Installation
 The package is called `msmhelper` and is available via [PyPI](https://pypi.org/project/msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install it, simply call:
 ```bash
@@ -110,40 +110,54 @@
 # via ssh key
 python3 -m pip install git+ssh://git@github.com/moldyn/msmhelper.git
 
 # or via password-based login
 python3 -m pip install git+https://github.com/moldyn/msmhelper.git
 ```
 
+### Documentation and Tutorials
+
+The [documentation](https://moldyn.github.io/msmhelper) serves as a comprehensive resource, offering a broad range of information such as general guidelines, API code references, and command line tool details. It also includes a Frequently Asked Questions (FAQ) section and outlines the procedures for contributing to the project. 
+Moreover, a suite of [tutorials](https://moldyn.github.io/msmhelper/tutorials/) is available, covering all the primary functionalities of the package. These tutorials are provided in the form of Jupyter notebooks. You can easily obtain these notebooks either directly from the [docs/tutorials](https://github.com/moldyn/msmhelper/tree/main/docs/tutorials) directory on our GitHub repository or by clicking the download buttons available on each tutorial page within the documentation.
+
+If you prefer, you can compile the documentation on your local machine by executing the following commands:
+
+```bash
+# install all additional dependencies
+python -m pip install msmhelper[docs]
+# build the docs inside the site directory
+python -m mkdocs build
+```
+
 ### Shell Completion
 Using the `bash`, `zsh` or `fish` shell click provides an easy way to
 provide shell completion, checkout the
 [docs](https://click.palletsprojects.com/en/8.1.x/shell-completion).
 In the case of bash you need to add following line to your `~/.bashrc`
 ```bash
 eval "$(_MSMHELPER_COMPLETE=bash_source msmhelper)"
 ```
 In general one can call the module directly by its entry point `$ msmhelper`
 or by calling the module `$ python -m msmhelper`. The latter method is
 preferred to ensure using the desired python environment. For enabling
 the shell completion, the entry point needs to be used.
 
-## Usage
+### Usage
 This package offers either a [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone analysis and to create commonly-used figures, or its much more powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be used to embedded it into an existing Python workflow. Check out the documentation for an overview over all modules and some example workflows, and for some examples see the [following section](#hummer-szabo-projection).
 ```python
 import msmhelper as mh
 
 # open text files
 traj = mh.openmicrostates(filename, limitsfile)
 # create markov state model
 tmat, states = mh.estimate_markov_model(traj, lagtime=1)
 ...
 ```
 
-## Hummer-Szabo Projection
+### Hummer-Szabo Projection
 In the following we show some sample figures produced directly with the command line tools. For more information on that, there is a [tutorial](https://moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more in depth. In general we can see, that applying the HS-projection removes most projection artifacts based on coarse-graining many microstates into a few macrostates.
 
 | Method | MSM | Hummer-Szabo MSM |
 | :---: | :---: | :---: |
 | Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) |
 | Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) |
 | Waiting Time Distributions | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msmhelper Version: 1.0.3 Summary: Helper functions
+Metadata-Version: 2.1 Name: msmhelper Version: 1.0.4 Summary: Helper functions
 for Markov State Models. Home-page: https://github.com/moldyn/msmhelper Author:
 braniii License: BSD-3-Clause License Project-URL: Documentation, https://
 moldyn.github.io/msmhelper Project-URL: Source Code, https://github.com/moldyn/
 msmhelper Project-URL: Changelog, https://moldyn.github.io/msmhelper/changelog
 Project-URL: Bug Tracker, https://github.com/moldyn/msmhelper/issues Keywords:
 MSM,Markov model,Markov state model,MD analysis Classifier: License :: OSI
 Approved :: BSD License Classifier: Intended Audience :: Science/Research
@@ -49,54 +49,69 @@
 (https://doi.org/10.1063/1.5081767) - Fast extraction of pathways and MSM-based
 prediction of pathways based on the definition of [Nagel et al. 2020](https://
 pubs.acs.org/doi/10.1021/acs.jctc.0c00774) - Fast calculation of waiting times
 based on both, state trajectories and MSMs - Blazing fast [Chapman-Kolmogorov]
 (https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test
 implementation - Entropy-based similarity measure to compare different state
 discretizations, this method will be published soon in Nagel 2023 - Contact
-representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact
-structural representation of the states - Command-line interface providing
-both, visualization and analysis methods - Provide (non-reversible) transition
-matrix of all states (corresponds in pyemma to `connectivity='none', 'all'`
-which will (probably) [never be implemented](https://github.com/markovmodel/
-PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/
-_msm_estimator_base.py#L110)) ## Getting started ### Installation The package
-is called `msmhelper` and is available via [PyPI](https://pypi.org/project/
-msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install
-it, simply call: ```bash python3 -m pip install --upgrade msmhelper ``` or ```
-conda install -c conda-forge msmhelper ``` or for the latest dev version
+representation by [Nagel et al. 2023](https://arxiv.org/abs/2303.03814) for a
+compact structural representation of the states - Command-line interface
+providing both, visualization and analysis methods - Provide (non-reversible)
+transition matrix of all states (corresponds in pyemma to `connectivity='none',
+'all'` which will (probably) [never be implemented](https://github.com/
+markovmodel/PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/
+estimators/_msm_estimator_base.py#L110)) ## Getting started ### Installation
+The package is called `msmhelper` and is available via [PyPI](https://pypi.org/
+project/msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To
+install it, simply call: ```bash python3 -m pip install --upgrade msmhelper ```
+or ``` conda install -c conda-forge msmhelper ``` or for the latest dev version
 ```bash # via ssh key python3 -m pip install git+ssh://git@github.com/moldyn/
 msmhelper.git # or via password-based login python3 -m pip install git+https://
-github.com/moldyn/msmhelper.git ``` ### Shell Completion Using the `bash`,
-`zsh` or `fish` shell click provides an easy way to provide shell completion,
-checkout the [docs](https://click.palletsprojects.com/en/8.1.x/shell-
-completion). In the case of bash you need to add following line to your
-`~/.bashrc` ```bash eval "$(_MSMHELPER_COMPLETE=bash_source msmhelper)" ``` In
-general one can call the module directly by its entry point `$ msmhelper` or by
-calling the module `$ python -m msmhelper`. The latter method is preferred to
-ensure using the desired python environment. For enabling the shell completion,
-the entry point needs to be used. ## Usage This package offers either a
-[command line interface](https://moldyn.github.io/msmhelper/reference/cli) to
-run standalone analysis and to create commonly-used figures, or its much more
-powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be
-used to embedded it into an existing Python workflow. Check out the
-documentation for an overview over all modules and some example workflows, and
-for some examples see the [following section](#hummer-szabo-projection).
-```python import msmhelper as mh # open text files traj = mh.openmicrostates
-(filename, limitsfile) # create markov state model tmat, states =
-mh.estimate_markov_model(traj, lagtime=1) ... ``` ## Hummer-Szabo Projection In
-the following we show some sample figures produced directly with the command
-line tools. For more information on that, there is a [tutorial](https://
-moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more
-in depth. In general we can see, that applying the HS-projection removes most
-projection artifacts based on coarse-graining many microstates into a few
-macrostates. | Method | MSM | Hummer-Szabo MSM | | :---: | :---: | :---: | |
-Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/
-assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales)
-| [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/
+github.com/moldyn/msmhelper.git ``` ### Documentation and Tutorials The
+[documentation](https://moldyn.github.io/msmhelper) serves as a comprehensive
+resource, offering a broad range of information such as general guidelines, API
+code references, and command line tool details. It also includes a Frequently
+Asked Questions (FAQ) section and outlines the procedures for contributing to
+the project. Moreover, a suite of [tutorials](https://moldyn.github.io/
+msmhelper/tutorials/) is available, covering all the primary functionalities of
+the package. These tutorials are provided in the form of Jupyter notebooks. You
+can easily obtain these notebooks either directly from the [docs/tutorials]
+(https://github.com/moldyn/msmhelper/tree/main/docs/tutorials) directory on our
+GitHub repository or by clicking the download buttons available on each
+tutorial page within the documentation. If you prefer, you can compile the
+documentation on your local machine by executing the following commands:
+```bash # install all additional dependencies python -m pip install msmhelper
+[docs] # build the docs inside the site directory python -m mkdocs build ```
+### Shell Completion Using the `bash`, `zsh` or `fish` shell click provides an
+easy way to provide shell completion, checkout the [docs](https://
+click.palletsprojects.com/en/8.1.x/shell-completion). In the case of bash you
+need to add following line to your `~/.bashrc` ```bash eval "$
+(_MSMHELPER_COMPLETE=bash_source msmhelper)" ``` In general one can call the
+module directly by its entry point `$ msmhelper` or by calling the module `$
+python -m msmhelper`. The latter method is preferred to ensure using the
+desired python environment. For enabling the shell completion, the entry point
+needs to be used. ### Usage This package offers either a [command line
+interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone
+analysis and to create commonly-used figures, or its much more powerful [API]
+(https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be used to
+embedded it into an existing Python workflow. Check out the documentation for
+an overview over all modules and some example workflows, and for some examples
+see the [following section](#hummer-szabo-projection). ```python import
+msmhelper as mh # open text files traj = mh.openmicrostates(filename,
+limitsfile) # create markov state model tmat, states = mh.estimate_markov_model
+(traj, lagtime=1) ... ``` ### Hummer-Szabo Projection In the following we show
+some sample figures produced directly with the command line tools. For more
+information on that, there is a [tutorial](https://moldyn.github.io/msmhelper/
+tutorials/hummerszabo) explaining the methods more in depth. In general we can
+see, that applying the HS-projection removes most projection artifacts based on
+coarse-graining many microstates into a few macrostates. | Method | MSM |
+Hummer-Szabo MSM | | :---: | :---: | :---: | | Implied Timescales | [![Implied
+Timescales](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | [!
+[Implied Timescales](https://moldyn.github.io/msmhelper/assets/
 8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | |
 Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
 msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/
 #msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
 msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/
 #msmhelper-ck-test) | | Waiting Time Distributions | [![waiting time
 distribution](https://moldyn.github.io/msmhelper/assets/
```

### Comparing `msmhelper-1.0.3/README.md` & `msmhelper-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ## Implemented Key Functionalities
 - Hummer-Szabo projection of optimal dimensionality reduction by [Hummer and Szabo 2014](https://doi.org/10.1021/jp508375q)
 - Dynamical coring by [Nagel et al. 2019](https://doi.org/10.1063/1.5081767)
 - Fast extraction of pathways and MSM-based prediction of pathways based on the definition of [Nagel et al. 2020](https://pubs.acs.org/doi/10.1021/acs.jctc.0c00774)
 - Fast calculation of waiting times based on both, state trajectories and MSMs
 - Blazing fast [Chapman-Kolmogorov](https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test implementation
 - Entropy-based similarity measure to compare different state discretizations, this method will be published soon in Nagel 2023
-- Contact representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact structural representation of the states
+- Contact representation by [Nagel et al. 2023](https://arxiv.org/abs/2303.03814) for a compact structural representation of the states
 - Command-line interface providing both, visualization and analysis methods
 - Provide (non-reversible) transition matrix of all states (corresponds in pyemma to `connectivity='none', 'all'` which will (probably) [never be implemented](https://github.com/markovmodel/PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/_msm_estimator_base.py#L110))
 
 ## Getting started
 ### Installation
 The package is called `msmhelper` and is available via [PyPI](https://pypi.org/project/msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install it, simply call:
 ```bash
@@ -80,40 +80,54 @@
 # via ssh key
 python3 -m pip install git+ssh://git@github.com/moldyn/msmhelper.git
 
 # or via password-based login
 python3 -m pip install git+https://github.com/moldyn/msmhelper.git
 ```
 
+### Documentation and Tutorials
+
+The [documentation](https://moldyn.github.io/msmhelper) serves as a comprehensive resource, offering a broad range of information such as general guidelines, API code references, and command line tool details. It also includes a Frequently Asked Questions (FAQ) section and outlines the procedures for contributing to the project. 
+Moreover, a suite of [tutorials](https://moldyn.github.io/msmhelper/tutorials/) is available, covering all the primary functionalities of the package. These tutorials are provided in the form of Jupyter notebooks. You can easily obtain these notebooks either directly from the [docs/tutorials](https://github.com/moldyn/msmhelper/tree/main/docs/tutorials) directory on our GitHub repository or by clicking the download buttons available on each tutorial page within the documentation.
+
+If you prefer, you can compile the documentation on your local machine by executing the following commands:
+
+```bash
+# install all additional dependencies
+python -m pip install msmhelper[docs]
+# build the docs inside the site directory
+python -m mkdocs build
+```
+
 ### Shell Completion
 Using the `bash`, `zsh` or `fish` shell click provides an easy way to
 provide shell completion, checkout the
 [docs](https://click.palletsprojects.com/en/8.1.x/shell-completion).
 In the case of bash you need to add following line to your `~/.bashrc`
 ```bash
 eval "$(_MSMHELPER_COMPLETE=bash_source msmhelper)"
 ```
 In general one can call the module directly by its entry point `$ msmhelper`
 or by calling the module `$ python -m msmhelper`. The latter method is
 preferred to ensure using the desired python environment. For enabling
 the shell completion, the entry point needs to be used.
 
-## Usage
+### Usage
 This package offers either a [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone analysis and to create commonly-used figures, or its much more powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be used to embedded it into an existing Python workflow. Check out the documentation for an overview over all modules and some example workflows, and for some examples see the [following section](#hummer-szabo-projection).
 ```python
 import msmhelper as mh
 
 # open text files
 traj = mh.openmicrostates(filename, limitsfile)
 # create markov state model
 tmat, states = mh.estimate_markov_model(traj, lagtime=1)
 ...
 ```
 
-## Hummer-Szabo Projection
+### Hummer-Szabo Projection
 In the following we show some sample figures produced directly with the command line tools. For more information on that, there is a [tutorial](https://moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more in depth. In general we can see, that applying the HS-projection removes most projection artifacts based on coarse-graining many microstates into a few macrostates.
 
 | Method | MSM | Hummer-Szabo MSM |
 | :---: | :---: | :---: |
 | Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) |
 | Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) |
 | Waiting Time Distributions | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) |
```

#### html2text {}

```diff
@@ -33,54 +33,69 @@
 (https://doi.org/10.1063/1.5081767) - Fast extraction of pathways and MSM-based
 prediction of pathways based on the definition of [Nagel et al. 2020](https://
 pubs.acs.org/doi/10.1021/acs.jctc.0c00774) - Fast calculation of waiting times
 based on both, state trajectories and MSMs - Blazing fast [Chapman-Kolmogorov]
 (https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test
 implementation - Entropy-based similarity measure to compare different state
 discretizations, this method will be published soon in Nagel 2023 - Contact
-representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact
-structural representation of the states - Command-line interface providing
-both, visualization and analysis methods - Provide (non-reversible) transition
-matrix of all states (corresponds in pyemma to `connectivity='none', 'all'`
-which will (probably) [never be implemented](https://github.com/markovmodel/
-PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/
-_msm_estimator_base.py#L110)) ## Getting started ### Installation The package
-is called `msmhelper` and is available via [PyPI](https://pypi.org/project/
-msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install
-it, simply call: ```bash python3 -m pip install --upgrade msmhelper ``` or ```
-conda install -c conda-forge msmhelper ``` or for the latest dev version
+representation by [Nagel et al. 2023](https://arxiv.org/abs/2303.03814) for a
+compact structural representation of the states - Command-line interface
+providing both, visualization and analysis methods - Provide (non-reversible)
+transition matrix of all states (corresponds in pyemma to `connectivity='none',
+'all'` which will (probably) [never be implemented](https://github.com/
+markovmodel/PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/
+estimators/_msm_estimator_base.py#L110)) ## Getting started ### Installation
+The package is called `msmhelper` and is available via [PyPI](https://pypi.org/
+project/msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To
+install it, simply call: ```bash python3 -m pip install --upgrade msmhelper ```
+or ``` conda install -c conda-forge msmhelper ``` or for the latest dev version
 ```bash # via ssh key python3 -m pip install git+ssh://git@github.com/moldyn/
 msmhelper.git # or via password-based login python3 -m pip install git+https://
-github.com/moldyn/msmhelper.git ``` ### Shell Completion Using the `bash`,
-`zsh` or `fish` shell click provides an easy way to provide shell completion,
-checkout the [docs](https://click.palletsprojects.com/en/8.1.x/shell-
-completion). In the case of bash you need to add following line to your
-`~/.bashrc` ```bash eval "$(_MSMHELPER_COMPLETE=bash_source msmhelper)" ``` In
-general one can call the module directly by its entry point `$ msmhelper` or by
-calling the module `$ python -m msmhelper`. The latter method is preferred to
-ensure using the desired python environment. For enabling the shell completion,
-the entry point needs to be used. ## Usage This package offers either a
-[command line interface](https://moldyn.github.io/msmhelper/reference/cli) to
-run standalone analysis and to create commonly-used figures, or its much more
-powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be
-used to embedded it into an existing Python workflow. Check out the
-documentation for an overview over all modules and some example workflows, and
-for some examples see the [following section](#hummer-szabo-projection).
-```python import msmhelper as mh # open text files traj = mh.openmicrostates
-(filename, limitsfile) # create markov state model tmat, states =
-mh.estimate_markov_model(traj, lagtime=1) ... ``` ## Hummer-Szabo Projection In
-the following we show some sample figures produced directly with the command
-line tools. For more information on that, there is a [tutorial](https://
-moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more
-in depth. In general we can see, that applying the HS-projection removes most
-projection artifacts based on coarse-graining many microstates into a few
-macrostates. | Method | MSM | Hummer-Szabo MSM | | :---: | :---: | :---: | |
-Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/
-assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales)
-| [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/
+github.com/moldyn/msmhelper.git ``` ### Documentation and Tutorials The
+[documentation](https://moldyn.github.io/msmhelper) serves as a comprehensive
+resource, offering a broad range of information such as general guidelines, API
+code references, and command line tool details. It also includes a Frequently
+Asked Questions (FAQ) section and outlines the procedures for contributing to
+the project. Moreover, a suite of [tutorials](https://moldyn.github.io/
+msmhelper/tutorials/) is available, covering all the primary functionalities of
+the package. These tutorials are provided in the form of Jupyter notebooks. You
+can easily obtain these notebooks either directly from the [docs/tutorials]
+(https://github.com/moldyn/msmhelper/tree/main/docs/tutorials) directory on our
+GitHub repository or by clicking the download buttons available on each
+tutorial page within the documentation. If you prefer, you can compile the
+documentation on your local machine by executing the following commands:
+```bash # install all additional dependencies python -m pip install msmhelper
+[docs] # build the docs inside the site directory python -m mkdocs build ```
+### Shell Completion Using the `bash`, `zsh` or `fish` shell click provides an
+easy way to provide shell completion, checkout the [docs](https://
+click.palletsprojects.com/en/8.1.x/shell-completion). In the case of bash you
+need to add following line to your `~/.bashrc` ```bash eval "$
+(_MSMHELPER_COMPLETE=bash_source msmhelper)" ``` In general one can call the
+module directly by its entry point `$ msmhelper` or by calling the module `$
+python -m msmhelper`. The latter method is preferred to ensure using the
+desired python environment. For enabling the shell completion, the entry point
+needs to be used. ### Usage This package offers either a [command line
+interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone
+analysis and to create commonly-used figures, or its much more powerful [API]
+(https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be used to
+embedded it into an existing Python workflow. Check out the documentation for
+an overview over all modules and some example workflows, and for some examples
+see the [following section](#hummer-szabo-projection). ```python import
+msmhelper as mh # open text files traj = mh.openmicrostates(filename,
+limitsfile) # create markov state model tmat, states = mh.estimate_markov_model
+(traj, lagtime=1) ... ``` ### Hummer-Szabo Projection In the following we show
+some sample figures produced directly with the command line tools. For more
+information on that, there is a [tutorial](https://moldyn.github.io/msmhelper/
+tutorials/hummerszabo) explaining the methods more in depth. In general we can
+see, that applying the HS-projection removes most projection artifacts based on
+coarse-graining many microstates into a few macrostates. | Method | MSM |
+Hummer-Szabo MSM | | :---: | :---: | :---: | | Implied Timescales | [![Implied
+Timescales](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | [!
+[Implied Timescales](https://moldyn.github.io/msmhelper/assets/
 8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | |
 Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
 msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/
 #msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
 msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/
 #msmhelper-ck-test) | | Waiting Time Distributions | [![waiting time
 distribution](https://moldyn.github.io/msmhelper/assets/
```

### Comparing `msmhelper-1.0.3/extra-requirements.txt` & `msmhelper-1.0.4/extra-requirements.txt`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/setup.cfg` & `msmhelper-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/setup.py` & `msmhelper-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 README = remove_gh_dark_mode_only_tags(
     (HERE / 'README.md').read_text(),
 )
 
 # This call to setup() does all the work
 setuptools.setup(
     name='msmhelper',
-    version='1.0.3',
+    version='1.0.4',
     description='Helper functions for Markov State Models.',
     long_description=README,
     long_description_content_type='text/markdown',
     keywords=[
         'MSM',
         'Markov model',
         'Markov state model',
```

### Comparing `msmhelper-1.0.3/src/msmhelper/__init__.py` & `msmhelper-1.0.4/src/msmhelper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 from .utils import (
     rename_by_population,
     rename_by_index,
     shift_data,
     unique,
 )
 
-__version__ = '1.0.3'
+__version__ = '1.0.4'
```

### Comparing `msmhelper-1.0.3/src/msmhelper/__main__.py` & `msmhelper-1.0.4/src/msmhelper/__main__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/_cli/ck_test.py` & `msmhelper-1.0.4/src/msmhelper/_cli/ck_test.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/_cli/compare_discretization.py` & `msmhelper-1.0.4/src/msmhelper/_cli/compare_discretization.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/_cli/contact_rep.py` & `msmhelper-1.0.4/src/msmhelper/_cli/contact_rep.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/_cli/dynamical_coring.py` & `msmhelper-1.0.4/src/msmhelper/_cli/dynamical_coring.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/_cli/gaussian_filter.py` & `msmhelper-1.0.4/src/msmhelper/_cli/gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/_cli/implied_timescales.py` & `msmhelper-1.0.4/src/msmhelper/_cli/implied_timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/_cli/waiting_time_dist.py` & `msmhelper-1.0.4/src/msmhelper/_cli/waiting_time_dist.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/_cli/waiting_times.py` & `msmhelper-1.0.4/src/msmhelper/_cli/waiting_times.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/io.py` & `msmhelper-1.0.4/src/msmhelper/io.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/md/__init__.py` & `msmhelper-1.0.4/src/msmhelper/md/__init__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/md/comparison.py` & `msmhelper-1.0.4/src/msmhelper/md/comparison.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/md/corrections.py` & `msmhelper-1.0.4/src/msmhelper/md/corrections.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/md/timescales.py` & `msmhelper-1.0.4/src/msmhelper/md/timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/msm/__init__.py` & `msmhelper-1.0.4/src/msmhelper/msm/__init__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/msm/msm.py` & `msmhelper-1.0.4/src/msmhelper/msm/msm.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 def estimate_markov_model(trajs, lagtime):
     """Estimates Markov State Model.
 
     This method estimates the MSM based on the transition count matrix.
 
     Parameters
     ----------
-    trajs : statetraj or list or ndarray or list of ndarray
-        State trajectory/trajectories. The states should start from zero and
-        need to be integers.
+    trajs : StateTraj or list or ndarray or list of ndarray
+        State trajectory/trajectories used to estimate the MSM.
     lagtime : int
         Lag time for estimating the markov model given in [frames].
 
     Returns
     -------
     T : ndarray
-        Transition rate matrix.
-    permutation : ndarray
-        Array with corresponding states.
+        Transition probability matrix $T_{ij}$, containing the transition
+        probability transition from state $i\to j$.
+    states : ndarray
+        Array holding states corresponding to the columns of $T_{ij}$.
 
     """
     trajs = StateTraj(trajs)
     return trajs.estimate_markov_model(lagtime)
 
 
 def _estimate_markov_model(trajs, lagtime, nstates, perm=None):
```

### Comparing `msmhelper-1.0.3/src/msmhelper/msm/tests.py` & `msmhelper-1.0.4/src/msmhelper/msm/tests.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,22 +12,32 @@
 
 from msmhelper import utils
 from msmhelper.statetraj import LumpedStateTraj, StateTraj
 
 
 @decorit.alias('ck_test')
 def chapman_kolmogorov_test(trajs, lagtimes, tmax):
-    r"""Calculate the Chapman Kolmogorov equation.
+    r"""Calculate the Chapman-Kolmogorov equation.
 
-    This method estimates the Chapman Kolmogorov equation
+    This method evaluates both sides of the Chapman-Kolmogorov equation
 
     $$T(\tau n) = T^n(\tau)\;.$$
 
-    Projected onto the diagonal this is known as the Chapman Kolmogorov test.
-    For more details see, e.g., the review Prinz et al.[^1].
+    So to compare the transition probability estimated based on the lag time
+    $n\tau$ (referred as "MD") with the transition probability estimated based
+    on the lag time $\tau$ and propagated $n$ times (referred as "MSM"), we can
+    use the Chapman-Kolmogorov test. If the model is Markovian, both sides are
+    identical, and the deviation indicates how Markovian the model is. The
+    Chapman-Kolmogorov test is commonly projected onto the diagonal (so
+    limiting to $T_{ii}$). For more details, see the review by Prinz et al.
+    [^1].
+
+    The returned dictionary can be visualized using
+    [msmhelper.plot.plot_ck_test][]. An example can be found in the
+    [tutorial](/msmhelper/tutorials/msm/#chapman-kolmogorov-test).
 
     [^1]: Prinz et al., **Markov models of molecular kinetics: Generation and
         validation**, *J. Chem. Phys.*, 134, 174105 (2011),
         doi:[10.1063/1.3565032](https://doi.org/10.1063/1.3565032)
 
     Parameters
     ----------
@@ -38,15 +48,15 @@
         Lagtimes for estimating the markov model given in [frames].
     tmax : int
         Longest time to evaluate the CK equation given in [frames].
 
     Returns
     -------
     cktest : dict
-        Dictionary holding for each lagtime the ckequation and with 'md' the
+        Dictionary holding for each lagtime the CK equation and with 'md' the
         reference.
 
     """
     # format input
     trajs = StateTraj(trajs)
     lagtimes = np.atleast_1d(lagtimes)
     lagtimes = np.sort(lagtimes)
```

### Comparing `msmhelper-1.0.3/src/msmhelper/msm/timescales.py` & `msmhelper-1.0.4/src/msmhelper/msm/timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/msm/utils/linalg.py` & `msmhelper-1.0.4/src/msmhelper/msm/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/plot/_ck_test.py` & `msmhelper-1.0.4/src/msmhelper/plot/_ck_test.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/plot/_wtd.py` & `msmhelper-1.0.4/src/msmhelper/plot/_wtd.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/statetraj.py` & `msmhelper-1.0.4/src/msmhelper/statetraj.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,18 +219,18 @@
         ----------
         lagtime : int
             Lag time for estimating the markov model given in [frames].
 
         Returns
         -------
         T : ndarray
-            Transition rate matrix.
-
-        permutation : ndarray
-            Array with corresponding states.
+            Transition probability matrix $T_{ij}$, containing the transition
+            probability transition from state $i\to j$.
+        states : ndarray
+            Array holding states corresponding to the columns of $T_{ij}$.
 
         """
         return mh.msm.msm._estimate_markov_model(
             self.index_trajs,
             lagtime,
             self.nstates,
             self.states,
@@ -529,18 +529,18 @@
         ----------
         lagtime : int
             Lag time for estimating the markov model given in [frames].
 
         Returns
         -------
         T : ndarray
-            Transition rate matrix.
-
-        permutation : ndarray
-            Array with corresponding states.
+            Transition probability matrix $T_{ij}$, containing the transition
+            probability transition from state $i\to j$.
+        states : ndarray
+            Array holding states corresponding to the columns of $T_{ij}$.
 
         """
         # in the following corresponds 'i' to micro and 'a' to macro
         msm_i, _ = mh.msm.msm._estimate_markov_model(
             self.microstate_index_trajs,
             lagtime,
             self.nmicrostates,
```

### Comparing `msmhelper-1.0.3/src/msmhelper/utils/__init__.py` & `msmhelper-1.0.4/src/msmhelper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/utils/_utils.py` & `msmhelper-1.0.4/src/msmhelper/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/utils/datasets.py` & `msmhelper-1.0.4/src/msmhelper/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/utils/filtering.py` & `msmhelper-1.0.4/src/msmhelper/utils/filtering.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper/utils/tests.py` & `msmhelper-1.0.4/src/msmhelper/utils/tests.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper.egg-info/PKG-INFO` & `msmhelper-1.0.4/src/msmhelper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmhelper
-Version: 1.0.3
+Version: 1.0.4
 Summary: Helper functions for Markov State Models.
 Home-page: https://github.com/moldyn/msmhelper
 Author: braniii
 License: BSD-3-Clause License
 Project-URL: Documentation, https://moldyn.github.io/msmhelper
 Project-URL: Source Code, https://github.com/moldyn/msmhelper
 Project-URL: Changelog, https://moldyn.github.io/msmhelper/changelog
@@ -86,15 +86,15 @@
 ## Implemented Key Functionalities
 - Hummer-Szabo projection of optimal dimensionality reduction by [Hummer and Szabo 2014](https://doi.org/10.1021/jp508375q)
 - Dynamical coring by [Nagel et al. 2019](https://doi.org/10.1063/1.5081767)
 - Fast extraction of pathways and MSM-based prediction of pathways based on the definition of [Nagel et al. 2020](https://pubs.acs.org/doi/10.1021/acs.jctc.0c00774)
 - Fast calculation of waiting times based on both, state trajectories and MSMs
 - Blazing fast [Chapman-Kolmogorov](https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test implementation
 - Entropy-based similarity measure to compare different state discretizations, this method will be published soon in Nagel 2023
-- Contact representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact structural representation of the states
+- Contact representation by [Nagel et al. 2023](https://arxiv.org/abs/2303.03814) for a compact structural representation of the states
 - Command-line interface providing both, visualization and analysis methods
 - Provide (non-reversible) transition matrix of all states (corresponds in pyemma to `connectivity='none', 'all'` which will (probably) [never be implemented](https://github.com/markovmodel/PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/_msm_estimator_base.py#L110))
 
 ## Getting started
 ### Installation
 The package is called `msmhelper` and is available via [PyPI](https://pypi.org/project/msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install it, simply call:
 ```bash
@@ -110,40 +110,54 @@
 # via ssh key
 python3 -m pip install git+ssh://git@github.com/moldyn/msmhelper.git
 
 # or via password-based login
 python3 -m pip install git+https://github.com/moldyn/msmhelper.git
 ```
 
+### Documentation and Tutorials
+
+The [documentation](https://moldyn.github.io/msmhelper) serves as a comprehensive resource, offering a broad range of information such as general guidelines, API code references, and command line tool details. It also includes a Frequently Asked Questions (FAQ) section and outlines the procedures for contributing to the project. 
+Moreover, a suite of [tutorials](https://moldyn.github.io/msmhelper/tutorials/) is available, covering all the primary functionalities of the package. These tutorials are provided in the form of Jupyter notebooks. You can easily obtain these notebooks either directly from the [docs/tutorials](https://github.com/moldyn/msmhelper/tree/main/docs/tutorials) directory on our GitHub repository or by clicking the download buttons available on each tutorial page within the documentation.
+
+If you prefer, you can compile the documentation on your local machine by executing the following commands:
+
+```bash
+# install all additional dependencies
+python -m pip install msmhelper[docs]
+# build the docs inside the site directory
+python -m mkdocs build
+```
+
 ### Shell Completion
 Using the `bash`, `zsh` or `fish` shell click provides an easy way to
 provide shell completion, checkout the
 [docs](https://click.palletsprojects.com/en/8.1.x/shell-completion).
 In the case of bash you need to add following line to your `~/.bashrc`
 ```bash
 eval "$(_MSMHELPER_COMPLETE=bash_source msmhelper)"
 ```
 In general one can call the module directly by its entry point `$ msmhelper`
 or by calling the module `$ python -m msmhelper`. The latter method is
 preferred to ensure using the desired python environment. For enabling
 the shell completion, the entry point needs to be used.
 
-## Usage
+### Usage
 This package offers either a [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone analysis and to create commonly-used figures, or its much more powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be used to embedded it into an existing Python workflow. Check out the documentation for an overview over all modules and some example workflows, and for some examples see the [following section](#hummer-szabo-projection).
 ```python
 import msmhelper as mh
 
 # open text files
 traj = mh.openmicrostates(filename, limitsfile)
 # create markov state model
 tmat, states = mh.estimate_markov_model(traj, lagtime=1)
 ...
 ```
 
-## Hummer-Szabo Projection
+### Hummer-Szabo Projection
 In the following we show some sample figures produced directly with the command line tools. For more information on that, there is a [tutorial](https://moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more in depth. In general we can see, that applying the HS-projection removes most projection artifacts based on coarse-graining many microstates into a few macrostates.
 
 | Method | MSM | Hummer-Szabo MSM |
 | :---: | :---: | :---: |
 | Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) |
 | Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) |
 | Waiting Time Distributions | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msmhelper Version: 1.0.3 Summary: Helper functions
+Metadata-Version: 2.1 Name: msmhelper Version: 1.0.4 Summary: Helper functions
 for Markov State Models. Home-page: https://github.com/moldyn/msmhelper Author:
 braniii License: BSD-3-Clause License Project-URL: Documentation, https://
 moldyn.github.io/msmhelper Project-URL: Source Code, https://github.com/moldyn/
 msmhelper Project-URL: Changelog, https://moldyn.github.io/msmhelper/changelog
 Project-URL: Bug Tracker, https://github.com/moldyn/msmhelper/issues Keywords:
 MSM,Markov model,Markov state model,MD analysis Classifier: License :: OSI
 Approved :: BSD License Classifier: Intended Audience :: Science/Research
@@ -49,54 +49,69 @@
 (https://doi.org/10.1063/1.5081767) - Fast extraction of pathways and MSM-based
 prediction of pathways based on the definition of [Nagel et al. 2020](https://
 pubs.acs.org/doi/10.1021/acs.jctc.0c00774) - Fast calculation of waiting times
 based on both, state trajectories and MSMs - Blazing fast [Chapman-Kolmogorov]
 (https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test
 implementation - Entropy-based similarity measure to compare different state
 discretizations, this method will be published soon in Nagel 2023 - Contact
-representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact
-structural representation of the states - Command-line interface providing
-both, visualization and analysis methods - Provide (non-reversible) transition
-matrix of all states (corresponds in pyemma to `connectivity='none', 'all'`
-which will (probably) [never be implemented](https://github.com/markovmodel/
-PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/
-_msm_estimator_base.py#L110)) ## Getting started ### Installation The package
-is called `msmhelper` and is available via [PyPI](https://pypi.org/project/
-msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install
-it, simply call: ```bash python3 -m pip install --upgrade msmhelper ``` or ```
-conda install -c conda-forge msmhelper ``` or for the latest dev version
+representation by [Nagel et al. 2023](https://arxiv.org/abs/2303.03814) for a
+compact structural representation of the states - Command-line interface
+providing both, visualization and analysis methods - Provide (non-reversible)
+transition matrix of all states (corresponds in pyemma to `connectivity='none',
+'all'` which will (probably) [never be implemented](https://github.com/
+markovmodel/PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/
+estimators/_msm_estimator_base.py#L110)) ## Getting started ### Installation
+The package is called `msmhelper` and is available via [PyPI](https://pypi.org/
+project/msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To
+install it, simply call: ```bash python3 -m pip install --upgrade msmhelper ```
+or ``` conda install -c conda-forge msmhelper ``` or for the latest dev version
 ```bash # via ssh key python3 -m pip install git+ssh://git@github.com/moldyn/
 msmhelper.git # or via password-based login python3 -m pip install git+https://
-github.com/moldyn/msmhelper.git ``` ### Shell Completion Using the `bash`,
-`zsh` or `fish` shell click provides an easy way to provide shell completion,
-checkout the [docs](https://click.palletsprojects.com/en/8.1.x/shell-
-completion). In the case of bash you need to add following line to your
-`~/.bashrc` ```bash eval "$(_MSMHELPER_COMPLETE=bash_source msmhelper)" ``` In
-general one can call the module directly by its entry point `$ msmhelper` or by
-calling the module `$ python -m msmhelper`. The latter method is preferred to
-ensure using the desired python environment. For enabling the shell completion,
-the entry point needs to be used. ## Usage This package offers either a
-[command line interface](https://moldyn.github.io/msmhelper/reference/cli) to
-run standalone analysis and to create commonly-used figures, or its much more
-powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be
-used to embedded it into an existing Python workflow. Check out the
-documentation for an overview over all modules and some example workflows, and
-for some examples see the [following section](#hummer-szabo-projection).
-```python import msmhelper as mh # open text files traj = mh.openmicrostates
-(filename, limitsfile) # create markov state model tmat, states =
-mh.estimate_markov_model(traj, lagtime=1) ... ``` ## Hummer-Szabo Projection In
-the following we show some sample figures produced directly with the command
-line tools. For more information on that, there is a [tutorial](https://
-moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more
-in depth. In general we can see, that applying the HS-projection removes most
-projection artifacts based on coarse-graining many microstates into a few
-macrostates. | Method | MSM | Hummer-Szabo MSM | | :---: | :---: | :---: | |
-Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/
-assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales)
-| [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/
+github.com/moldyn/msmhelper.git ``` ### Documentation and Tutorials The
+[documentation](https://moldyn.github.io/msmhelper) serves as a comprehensive
+resource, offering a broad range of information such as general guidelines, API
+code references, and command line tool details. It also includes a Frequently
+Asked Questions (FAQ) section and outlines the procedures for contributing to
+the project. Moreover, a suite of [tutorials](https://moldyn.github.io/
+msmhelper/tutorials/) is available, covering all the primary functionalities of
+the package. These tutorials are provided in the form of Jupyter notebooks. You
+can easily obtain these notebooks either directly from the [docs/tutorials]
+(https://github.com/moldyn/msmhelper/tree/main/docs/tutorials) directory on our
+GitHub repository or by clicking the download buttons available on each
+tutorial page within the documentation. If you prefer, you can compile the
+documentation on your local machine by executing the following commands:
+```bash # install all additional dependencies python -m pip install msmhelper
+[docs] # build the docs inside the site directory python -m mkdocs build ```
+### Shell Completion Using the `bash`, `zsh` or `fish` shell click provides an
+easy way to provide shell completion, checkout the [docs](https://
+click.palletsprojects.com/en/8.1.x/shell-completion). In the case of bash you
+need to add following line to your `~/.bashrc` ```bash eval "$
+(_MSMHELPER_COMPLETE=bash_source msmhelper)" ``` In general one can call the
+module directly by its entry point `$ msmhelper` or by calling the module `$
+python -m msmhelper`. The latter method is preferred to ensure using the
+desired python environment. For enabling the shell completion, the entry point
+needs to be used. ### Usage This package offers either a [command line
+interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone
+analysis and to create commonly-used figures, or its much more powerful [API]
+(https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be used to
+embedded it into an existing Python workflow. Check out the documentation for
+an overview over all modules and some example workflows, and for some examples
+see the [following section](#hummer-szabo-projection). ```python import
+msmhelper as mh # open text files traj = mh.openmicrostates(filename,
+limitsfile) # create markov state model tmat, states = mh.estimate_markov_model
+(traj, lagtime=1) ... ``` ### Hummer-Szabo Projection In the following we show
+some sample figures produced directly with the command line tools. For more
+information on that, there is a [tutorial](https://moldyn.github.io/msmhelper/
+tutorials/hummerszabo) explaining the methods more in depth. In general we can
+see, that applying the HS-projection removes most projection artifacts based on
+coarse-graining many microstates into a few macrostates. | Method | MSM |
+Hummer-Szabo MSM | | :---: | :---: | :---: | | Implied Timescales | [![Implied
+Timescales](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | [!
+[Implied Timescales](https://moldyn.github.io/msmhelper/assets/
 8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | |
 Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
 msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/
 #msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
 msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/
 #msmhelper-ck-test) | | Waiting Time Distributions | [![waiting time
 distribution](https://moldyn.github.io/msmhelper/assets/
```

### Comparing `msmhelper-1.0.3/src/msmhelper.egg-info/SOURCES.txt` & `msmhelper-1.0.4/src/msmhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/src/msmhelper.egg-info/requires.txt` & `msmhelper-1.0.4/src/msmhelper.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 pandas
 decorit
 scipy
 click
 prettypyplot
 
 [all]
-pytest-rerunfailures
-mkdocs-literate-nav
 mkdocs-material
+pytest-cov
+pytest
+pytest-mpl
 mkdocs-jupyter
 pyemma
-jupyter_contrib_nbextensions
-pytest-mpl
+mkdocs-literate-nav
+mkdocs-gen-files
 mkdocstrings-python
 mkdocstrings
-pytest
 mkdocs-click
-mkdocs-gen-files
-flake8
-pytest-cov
+pytest-rerunfailures
 mkdocs-section-index
+jupyter_contrib_nbextensions
+flake8
 
 [docs]
-mkdocs-literate-nav
 mkdocs-material
 mkdocs-jupyter
 pyemma
-jupyter_contrib_nbextensions
+mkdocs-literate-nav
+mkdocs-gen-files
 mkdocstrings-python
 mkdocstrings
 mkdocs-click
-mkdocs-gen-files
 mkdocs-section-index
+jupyter_contrib_nbextensions
 
 [testing]
-pytest-rerunfailures
-pytest-mpl
+pytest-cov
 pytest
+pytest-mpl
+pytest-rerunfailures
 flake8
-pytest-cov
```

### Comparing `msmhelper-1.0.3/test/test___main__.py` & `msmhelper-1.0.4/test/test___main__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_io.py` & `msmhelper-1.0.4/test/test_io.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_md_comparison.py` & `msmhelper-1.0.4/test/test_md_comparison.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_md_corrections.py` & `msmhelper-1.0.4/test/test_md_corrections.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_md_timescales.py` & `msmhelper-1.0.4/test/test_md_timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_msm_msm.py` & `msmhelper-1.0.4/test/test_msm_msm.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_msm_tests.py` & `msmhelper-1.0.4/test/test_msm_tests.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_msm_timescales.py` & `msmhelper-1.0.4/test/test_msm_timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_msm_utils_linalg.py` & `msmhelper-1.0.4/test/test_msm_utils_linalg.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_plot.py` & `msmhelper-1.0.4/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_statetraj.py` & `msmhelper-1.0.4/test/test_statetraj.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_utils__utils.py` & `msmhelper-1.0.4/test/test_utils__utils.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_utils_filtering.py` & `msmhelper-1.0.4/test/test_utils_filtering.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.3/test/test_utils_tests.py` & `msmhelper-1.0.4/test/test_utils_tests.py`

 * *Files identical despite different names*

