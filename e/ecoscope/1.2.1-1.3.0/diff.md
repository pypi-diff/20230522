# Comparing `tmp/ecoscope-1.2.1.tar.gz` & `tmp/ecoscope-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoscope-1.2.1.tar", last modified: Thu May 11 03:37:25 2023, max compression
+gzip compressed data, was "ecoscope-1.3.0.tar", last modified: Mon May 22 13:50:35 2023, max compression
```

## Comparing `ecoscope-1.2.1.tar` & `ecoscope-1.3.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.649143 ecoscope-1.2.1/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-05-10 19:33:30.000000 ecoscope-1.2.1/LICENSE
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-11 03:37:25.649143 ecoscope-1.2.1/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-05-10 19:33:30.000000 ecoscope-1.2.1/README.rst
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.641143 ecoscope-1.2.1/ecoscope/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3744 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/__init__.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.641143 ecoscope-1.2.1/ecoscope/analysis/
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/analysis/UD/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/UD/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/UD/etd_range.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/astronomy.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3881 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/percentile.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/proximity.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2735 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/speed.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/base/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/base/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/base/_dataclasses.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25180 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/base/base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/base/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/contrib/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/contrib/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/contrib/basemaps.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/contrib/foliumap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/contrib/legend.txt
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/io/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/io/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32515 2023-05-11 03:31:13.000000 ecoscope-1.2.1/ecoscope/io/earthranger.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/io/eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/io/raster.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/io/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/mapping/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/mapping/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/mapping/map.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/plotting/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/plotting/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/plotting/plot.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-05-10 19:34:04.000000 ecoscope-1.2.1/ecoscope/version.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.641143 ecoscope-1.2.1/ecoscope.egg-info/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1322 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/SOURCES.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/dependency_links.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/not-zip-safe
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      284 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/requires.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/top_level.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-05-10 19:33:30.000000 ecoscope-1.2.1/pyproject.toml
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-05-11 03:37:25.649143 ecoscope-1.2.1/setup.cfg
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1940 2023-05-10 19:33:30.000000 ecoscope-1.2.1/setup.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.649143 ecoscope-1.2.1/tests/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6554 2023-05-11 03:34:07.000000 ecoscope-1.2.1/tests/test_base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6922 2023-05-10 19:42:08.000000 ecoscope-1.2.1/tests/test_earthranger_io.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_ecodataframe.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_ecomap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_speed.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_ud.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.230748 ecoscope-1.3.0/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-05-22 06:13:31.000000 ecoscope-1.3.0/LICENSE
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-22 13:50:35.230748 ecoscope-1.3.0/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-05-22 06:13:31.000000 ecoscope-1.3.0/README.rst
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.222747 ecoscope-1.3.0/ecoscope/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3744 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/__init__.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/analysis/
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/analysis/UD/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/UD/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/UD/etd_range.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/astronomy.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3881 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/percentile.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/proximity.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2735 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/speed.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/base/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/base/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/base/_dataclasses.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25180 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/base/base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/base/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/contrib/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/contrib/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/contrib/basemaps.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/contrib/foliumap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/contrib/legend.txt
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/io/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/io/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    33272 2023-05-22 06:30:31.000000 ecoscope-1.3.0/ecoscope/io/earthranger.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/io/eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/io/raster.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/io/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/mapping/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/mapping/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/mapping/map.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.230748 ecoscope-1.3.0/ecoscope/plotting/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/plotting/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/plotting/plot.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/version.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.222747 ecoscope-1.3.0/ecoscope.egg-info/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1322 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-22 13:48:35.000000 ecoscope-1.3.0/ecoscope.egg-info/not-zip-safe
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      284 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/requires.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/top_level.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-05-22 06:13:31.000000 ecoscope-1.3.0/pyproject.toml
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-05-22 13:50:35.230748 ecoscope-1.3.0/setup.cfg
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1940 2023-05-22 06:13:31.000000 ecoscope-1.3.0/setup.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.230748 ecoscope-1.3.0/tests/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6554 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6955 2023-05-22 06:17:05.000000 ecoscope-1.3.0/tests/test_earthranger_io.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_ecodataframe.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_ecomap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_speed.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_ud.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_utils.py
```

### Comparing `ecoscope-1.2.1/LICENSE` & `ecoscope-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/PKG-INFO` & `ecoscope-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.2.1
+Version: 1.3.0
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.2.1/README.rst` & `ecoscope-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/__init__.py` & `ecoscope-1.3.0/ecoscope/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/analysis/UD/etd_range.py` & `ecoscope-1.3.0/ecoscope/analysis/UD/etd_range.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/analysis/astronomy.py` & `ecoscope-1.3.0/ecoscope/analysis/astronomy.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/analysis/ecograph.py` & `ecoscope-1.3.0/ecoscope/analysis/ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/analysis/geofence.py` & `ecoscope-1.3.0/ecoscope/analysis/geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/analysis/immobility.py` & `ecoscope-1.3.0/ecoscope/analysis/immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/analysis/percentile.py` & `ecoscope-1.3.0/ecoscope/analysis/percentile.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/analysis/proximity.py` & `ecoscope-1.3.0/ecoscope/analysis/proximity.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/analysis/seasons.py` & `ecoscope-1.3.0/ecoscope/analysis/seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/analysis/speed.py` & `ecoscope-1.3.0/ecoscope/analysis/speed.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/base/__init__.py` & `ecoscope-1.3.0/ecoscope/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/base/_dataclasses.py` & `ecoscope-1.3.0/ecoscope/base/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/base/base.py` & `ecoscope-1.3.0/ecoscope/base/base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/base/utils.py` & `ecoscope-1.3.0/ecoscope/base/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/contrib/basemaps.py` & `ecoscope-1.3.0/ecoscope/contrib/basemaps.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/contrib/foliumap.py` & `ecoscope-1.3.0/ecoscope/contrib/foliumap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/contrib/legend.txt` & `ecoscope-1.3.0/ecoscope/contrib/legend.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/io/earthranger.py` & `ecoscope-1.3.0/ecoscope/io/earthranger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import datetime
+import pytz
 import json
 import typing
 
 import geopandas as gpd
 import pandas as pd
 import requests
-from erclient.client import ERClient, ERClientException
+from erclient.client import ERClient, ERClientException, ERClientNotFound
 from tqdm.auto import tqdm
 
 import ecoscope
 from ecoscope.io.utils import pack_columns, to_hex
 
 
 def fatal_status_code(e):
@@ -23,14 +24,30 @@
             kwargs["service_root"] = f"{server}/api/v1.0"
             kwargs["token_url"] = f"{server}/oauth2/token"
 
         self.sub_page_size = sub_page_size
         self.tcp_limit = tcp_limit
         kwargs["client_id"] = kwargs.get("client_id", "das_web_client")
         super().__init__(**kwargs)
+        try:
+            self.login()
+        except ERClientNotFound:
+            raise ERClientNotFound("Failed login. Check Stack Trace for specific reason.")
+
+    def _token_request(self, payload):
+        response = requests.post(self.token_url, data=payload)
+        if response.ok:
+            self.auth = json.loads(response.text)
+            expires_in = int(self.auth["expires_in"]) - 5 * 60
+            self.auth_expires = pytz.utc.localize(datetime.datetime.utcnow()) + datetime.timedelta(seconds=expires_in)
+            return True
+
+        self.auth = None
+        self.auth_expires = pytz.utc.localize(datetime.datetime.min)
+        raise ERClientNotFound(json.loads(response.text)["error_description"])
 
     @staticmethod
     def _clean_kwargs(addl_kwargs={}, **kwargs):
         for k in addl_kwargs.keys():
             print(f"Warning: {k} is a non-standard parameter. Results may be unexpected.")
         return {k: v for k, v in {**addl_kwargs, **kwargs}.items() if v is not None}
 
@@ -372,15 +389,15 @@
             )
 
         if include_subjectsource_details:
             observations = observations.merge(
                 self.get_subjectsources(subjects=",".join(observations["subject_id"].unique())).add_prefix(
                     "subjectsource__"
                 ),
-                left_on=["id", "source"],
+                left_on=["subject_id", "source"],
                 right_on=["subjectsource__subject", "subjectsource__source"],
             )
 
         if relocations:
             return ecoscope.base.Relocations.from_gdf(
                 observations,
                 groupby_col="subject_id",
```

### Comparing `ecoscope-1.2.1/ecoscope/io/eetools.py` & `ecoscope-1.3.0/ecoscope/io/eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/io/raster.py` & `ecoscope-1.3.0/ecoscope/io/raster.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/io/utils.py` & `ecoscope-1.3.0/ecoscope/io/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/mapping/map.py` & `ecoscope-1.3.0/ecoscope/mapping/map.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope/plotting/plot.py` & `ecoscope-1.3.0/ecoscope/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/ecoscope.egg-info/PKG-INFO` & `ecoscope-1.3.0/ecoscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.2.1
+Version: 1.3.0
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.2.1/ecoscope.egg-info/SOURCES.txt` & `ecoscope-1.3.0/ecoscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/pyproject.toml` & `ecoscope-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/setup.py` & `ecoscope-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/tests/test_base.py` & `ecoscope-1.3.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/tests/test_earthranger_io.py` & `ecoscope-1.3.0/tests/test_earthranger_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 def test_get_subject_observations(er_io):
     relocations = er_io.get_subject_observations(
         subject_ids=er_io.SUBJECT_IDS,
         include_subject_details=True,
         include_source_details=True,
         include_subjectsource_details=True,
     )
+    assert not relocations.empty
     assert isinstance(relocations, ecoscope.base.Relocations)
     assert "groupby_col" in relocations
     assert "fixtime" in relocations
     assert "extra__source" in relocations
 
 
 def test_get_source_observations(er_io):
```

### Comparing `ecoscope-1.2.1/tests/test_ecodataframe.py` & `ecoscope-1.3.0/tests/test_ecodataframe.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/tests/test_ecograph.py` & `ecoscope-1.3.0/tests/test_ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/tests/test_eetools.py` & `ecoscope-1.3.0/tests/test_eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/tests/test_geofence.py` & `ecoscope-1.3.0/tests/test_geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/tests/test_immobility.py` & `ecoscope-1.3.0/tests/test_immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/tests/test_seasons.py` & `ecoscope-1.3.0/tests/test_seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.1/tests/test_ud.py` & `ecoscope-1.3.0/tests/test_ud.py`

 * *Files identical despite different names*

