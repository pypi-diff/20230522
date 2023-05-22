# Comparing `tmp/m23-0.1.130.tar.gz` & `tmp/m23-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m23-0.1.130.tar", last modified: Mon Mar 20 23:22:43 2023, max compression
+gzip compressed data, was "m23-0.2.0.tar", last modified: Mon May 22 12:56:49 2023, max compression
```

## Comparing `m23-0.1.130.tar` & `m23-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.799722 m23-0.1.130/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-20 23:22:43.799722 m23-0.1.130/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-20 23:22:20.000000 m23-0.1.130/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.787722 m23-0.1.130/m23/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-20 23:22:20.000000 m23-0.1.130/m23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-03-20 23:22:20.000000 m23-0.1.130/m23/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.791722 m23-0.1.130/m23/align/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-20 23:22:20.000000 m23-0.1.130/m23/align/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.791722 m23-0.1.130/m23/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-20 23:22:20.000000 m23-0.1.130/m23/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-03-20 23:22:20.000000 m23-0.1.130/m23/calibrate/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-03-20 23:22:20.000000 m23-0.1.130/m23/calibrate/master_calibrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.791722 m23-0.1.130/m23/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-03-20 23:22:20.000000 m23-0.1.130/m23/charts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.791722 m23-0.1.130/m23/combine/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-20 23:22:20.000000 m23-0.1.130/m23/combine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-20 23:22:20.000000 m23-0.1.130/m23/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.791722 m23-0.1.130/m23/extract/
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-03-20 23:22:20.000000 m23-0.1.130/m23/extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.795722 m23-0.1.130/m23/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/aligned_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/color_normalized_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/flux_log_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/log_file_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/masterflat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/normfactor_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/raw_image_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/reference_log_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-20 23:22:20.000000 m23-0.1.130/m23/file/ri_color_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.795722 m23-0.1.130/m23/internight_normalize/
--rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-03-20 23:22:20.000000 m23-0.1.130/m23/internight_normalize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.795722 m23-0.1.130/m23/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-20 23:22:20.000000 m23-0.1.130/m23/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-20 23:22:20.000000 m23-0.1.130/m23/matrix/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-20 23:22:20.000000 m23-0.1.130/m23/matrix/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-20 23:22:20.000000 m23-0.1.130/m23/matrix/region.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-20 23:22:20.000000 m23-0.1.130/m23/matrix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.795722 m23-0.1.130/m23/norm/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-03-20 23:22:20.000000 m23-0.1.130/m23/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-20 23:22:20.000000 m23-0.1.130/m23/norm/get_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.799722 m23-0.1.130/m23/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-20 23:22:20.000000 m23-0.1.130/m23/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-03-20 23:22:20.000000 m23-0.1.130/m23/processor/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-20 23:22:20.000000 m23-0.1.130/m23/processor/generate_masterflat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-20 23:22:20.000000 m23-0.1.130/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-20 23:22:20.000000 m23-0.1.130/m23/processor/nights_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-20 23:22:20.000000 m23-0.1.130/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-03-20 23:22:20.000000 m23-0.1.130/m23/processor/process_nights.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-20 23:22:20.000000 m23-0.1.130/m23/processor/renormalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-03-20 23:22:20.000000 m23-0.1.130/m23/processor/renormalize_config_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.799722 m23-0.1.130/m23/trans/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-20 23:22:20.000000 m23-0.1.130/m23/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-20 23:22:20.000000 m23-0.1.130/m23/trans/fits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.799722 m23-0.1.130/m23/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-03-20 23:22:20.000000 m23-0.1.130/m23/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-20 23:22:20.000000 m23-0.1.130/m23/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-20 23:22:20.000000 m23-0.1.130/m23/utils/flux_to_magnitude.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-20 23:22:20.000000 m23-0.1.130/m23/utils/rename.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:22:43.791722 m23-0.1.130/m23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-20 23:22:43.000000 m23-0.1.130/m23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-20 23:22:43.000000 m23-0.1.130/m23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 23:22:43.000000 m23-0.1.130/m23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-20 23:22:43.000000 m23-0.1.130/m23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-20 23:22:43.000000 m23-0.1.130/m23.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-20 23:22:20.000000 m23-0.1.130/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 23:22:43.799722 m23-0.1.130/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.752283 m23-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-22 12:56:49.752283 m23-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 12:56:30.000000 m23-0.2.0/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.744283 m23-0.2.0/m23/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 12:56:30.000000 m23-0.2.0/m23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-22 12:56:30.000000 m23-0.2.0/m23/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/align/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-22 12:56:30.000000 m23-0.2.0/m23/align/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 12:56:30.000000 m23-0.2.0/m23/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-22 12:56:30.000000 m23-0.2.0/m23/calibrate/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-22 12:56:30.000000 m23-0.2.0/m23/calibrate/master_calibrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-22 12:56:30.000000 m23-0.2.0/m23/charts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/combine/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-22 12:56:30.000000 m23-0.2.0/m23/combine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-22 12:56:30.000000 m23-0.2.0/m23/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-22 12:56:30.000000 m23-0.2.0/m23/extract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/aligned_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/color_normalized_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/flux_log_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/log_file_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/masterflat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/normfactor_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/raw_image_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/reference_log_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 12:56:30.000000 m23-0.2.0/m23/file/ri_color_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/internight_normalize/
+-rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-05-22 12:56:30.000000 m23-0.2.0/m23/internight_normalize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-22 12:56:30.000000 m23-0.2.0/m23/matrix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-22 12:56:30.000000 m23-0.2.0/m23/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-22 12:56:30.000000 m23-0.2.0/m23/norm/get_line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.752283 m23-0.2.0/m23/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/generate_masterflat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/nights_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/process_nights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/renormalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-22 12:56:30.000000 m23-0.2.0/m23/processor/renormalize_config_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.752283 m23-0.2.0/m23/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-22 12:56:30.000000 m23-0.2.0/m23/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 12:56:30.000000 m23-0.2.0/m23/trans/fits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.752283 m23-0.2.0/m23/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-22 12:56:30.000000 m23-0.2.0/m23/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-22 12:56:30.000000 m23-0.2.0/m23/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-22 12:56:30.000000 m23-0.2.0/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-22 12:56:30.000000 m23-0.2.0/m23/utils/rename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:49.748283 m23-0.2.0/m23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 12:56:49.000000 m23-0.2.0/m23.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 12:56:30.000000 m23-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:56:49.752283 m23-0.2.0/setup.cfg
```

### Comparing `m23-0.1.130/m23/__main__.py` & `m23-0.2.0/m23/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,65 +9,67 @@
 def process(args):
     """
     This is a subcommand that handles data processing for one or more nights
     based on the configuration file path provided
     """
     config_file: Path = args.config_file
     if not config_file.exists():
-        sys.stdout.write("Provided file doesn't exist\n")
+        sys.stdout.write(f"Provided file {config_file} doesn't exist\n")
         return
     if not config_file.is_file():
         sys.stdout.write("Invalid configuration file provided\n")
         return
     start_data_processing(config_file.absolute())
 
 
 def norm(args):
     """
     This is a subcommand that handles renormalization for one or more nights
     based on the configuration file path provided
     """
     config_file: Path = args.config_file
     if not config_file.exists():
-        sys.stdout.write("Provided file doesn't exist\n")
+        sys.stdout.write(f"Provided file {config_file} doesn't exist\n")
         return
     if not config_file.is_file():
         sys.stdout.write("Invalid configuration file provided\n")
         return
     renormalize(config_file.absolute())
 
 
 def mf(args):
     """
     This is a subcommand that handles generating masterflat for a night from
     the flat images taken for the night
     """
     config_file: Path = args.config_file
     if not config_file.exists():
-        sys.stdout.write("Provided file doesn't exist\n")
+        sys.stdout.write(f"Provided file {config_file} doesn't exist\n")
         return
     if not config_file.is_file():
         sys.stdout.write("Invalid configuration file provided\n")
         return
     generate_masterflat(config_file.absolute())
 
-def csv(args): 
+
+def csv(args):
     """
     This is a subcommand that generates the csv file which holds the stars' flux values
-    for a year, this will be later used to get the data onto our server 
+    for a year, this will be later used to get the data onto our server
     """
     config_file: Path = args.config_file
     if not config_file.exists():
-        sys.stdout.write("Provided file doesn't exist\n")
+        sys.stdout.write(f"Provided file {config_file} doesn't exist\n")
         return
     if not config_file.is_file():
         sys.stdout.write("Invalid configuration file provided\n")
         return
     create_nights_csv(config_file.absolute())
 
+
 parser = argparse.ArgumentParser(prog="M23 Data processor", epilog="Made in Rapti")
 subparsers = parser.add_subparsers()
 
 # We are dividing our command line function into subcommands
 # The first subcommand is `process` denoting a full fledged data processing for night(s)
 process_parser = subparsers.add_parser("process", help="Process raw data for one or more nights")
 process_parser.add_argument(
@@ -90,15 +92,15 @@
 mf_parser = subparsers.add_parser("mf", help="Generate masterflat for a night from its raw flats")
 mf_parser.add_argument(
     "config_file", type=Path, help="Path to toml configuration file for master flat generatation"
 )  # positional argument
 # Adding a default value so we later know which subcommand was invoked
 mf_parser.set_defaults(func=mf)
 
-# Csv generator parser 
+# CSV generator parser
 csv_parser = subparsers.add_parser("csv", help="Generate csv flux file for a given year")
 csv_parser.add_argument(
     "config_file", type=Path, help="Path to toml configuration file for csv generation"
 )  # positional argument
 # Adding a default value so we later know which subcommand was invoked
 csv_parser.set_defaults(func=csv)
```

### Comparing `m23-0.1.130/m23/align/__init__.py` & `m23-0.2.0/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/calibrate/calibration.py` & `m23-0.2.0/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/calibrate/master_calibrate.py` & `m23-0.2.0/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/charts/__init__.py` & `m23-0.2.0/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/combine/__init__.py` & `m23-0.2.0/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/constants.py` & `m23-0.2.0/m23/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 LOG_FILES_COMBINED_FOLDER_NAME = "Log Files Combined"
 FLUX_LOGS_COMBINED_FOLDER_NAME = "Flux Logs Combined"
 COLOR_NORMALIZED_FOLDER_NAME = "Color Normalized"
 CHARTS_FOLDER_NAME = "Charts"
 MASTER_DARK_NAME = "masterdark.fit"
 MASTER_FLAT_NAME = "masterflat.fit"
 
+# INTRA_NIGHT
+# Any star that appears more than this threshold away from the reference file
+# will be masked out during intra night normalization
+INTRA_NIGHT_IMPACT_THRESHOLD_PIXELS = 2
+
 # MISC
 CAMERA_CHANGE_2022_DATE = date(2022, 6, 16)
 TYPICAL_NEW_CAMERA_CROP_REGION = [
     [[0, 448], [0, 0], [492, 0], [210, 181]],
     [[0, 1600], [0, 2048], [480, 2048], [210, 1867]],
     [[1400, 2048], [2048, 2048], [2048, 1500], [1834, 1830]],
     [[1508, 0], [1852, 241], [2048, 521], [2048, 0]],
```

### Comparing `m23-0.1.130/m23/extract/__init__.py` & `m23-0.2.0/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/__init__.py` & `m23-0.2.0/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/aligned_combined_file.py` & `m23-0.2.0/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/color_normalized_file.py` & `m23-0.2.0/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/flux_log_combined_file.py` & `m23-0.2.0/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/log_file_combined_file.py` & `m23-0.2.0/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/masterflat_file.py` & `m23-0.2.0/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/normfactor_file.py` & `m23-0.2.0/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/raw_image_file.py` & `m23-0.2.0/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/reference_log_file.py` & `m23-0.2.0/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/file/ri_color_file.py` & `m23-0.2.0/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/internight_normalize/__init__.py` & `m23-0.2.0/m23/internight_normalize/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 import logging
-import sys
 from pathlib import Path
 from typing import Callable, Dict, List
 
 import numpy as np
 from scipy.optimize import curve_fit
 
 from m23.charts import draw_internight_brightness_chart, draw_internight_color_chart
 from m23.constants import COLOR_NORMALIZED_FOLDER_NAME, FLUX_LOGS_COMBINED_FOLDER_NAME
 from m23.file.color_normalized_file import ColorNormalizedFile
 from m23.file.flux_log_combined_file import FluxLogCombinedFile
-from m23.file.reference_log_file import ReferenceLogFile
+from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.ri_color_file import RIColorFile
-from m23.utils import (
-    get_date_from_input_night_folder_name,
-    get_log_file_name,
-    get_radius_folder_name,
-)
+from m23.utils import get_date_from_input_night_folder_name, get_radius_folder_name
 from m23.utils.flux_to_magnitude import flux_to_magnitude
 
 # Note that this code is implemented based on the internight normalization in IDL
 # https://github.com/LutherAstrophysics/idl-files/blob/39dfa1c0c6d03d64020c42583bbcaa94655d69cc/inter_night_normalization_345.pro
 
 
 def internight_normalize(
     night: Path,
-    reference_file: Path,
+    logfile_combined_reference_file: LogFileCombinedFile,
     color_file: Path,
     radii_of_extraction: List[int],
 ) -> None:
     """
     This function normalizes the Flux Logs Combined for a night with respect to
     the data in the reference night. It also saves the result of inter-night
     normalization.  We typically the image 71 on Aug 4 2003 night as the
@@ -64,20 +59,20 @@
 
     `reference_file` is a valid file path in conventional reference file format
 
     `color_file` is a valid file path in conventional R-I color file format
     """
 
     for radius in radii_of_extraction:
-        internight_normalize_auxiliary(night, reference_file, color_file, radius)
+        internight_normalize_auxiliary(night, logfile_combined_reference_file, color_file, radius)
 
 
 def internight_normalize_auxiliary(
     night: Path,
-    reference_file: Path,
+    logfile_combined_reference_file: LogFileCombinedFile,
     color_file: Path,
     radius_of_extraction: int,
 ):
     """
     This is an auxiliary function for internight_normalize that's different from
     the `internight_normalize` because this function takes
     `radius_of_extraction` unlike `internight_normalize` that takes
@@ -102,29 +97,28 @@
     flux_logs_files: List[FluxLogCombinedFile] = [
         FluxLogCombinedFile(file) for file in FLUX_LOGS_COMBINED_FOLDER.glob("*")
     ]
     # Filter out the files that don't match conventional flux log combined file format
     flux_logs_files = list(filter(lambda x: x.is_valid_file_name(), flux_logs_files))
 
     color_data_file = RIColorFile(color_file)
-    reference_file_data = ReferenceLogFile(reference_file)
 
     # This dictionary holds the data for each
     # Star's median ADU, normalization factor and normalized ADU
     data_dict: ColorNormalizedFile.Data_Dict_Type = {
         log_file.star_number(): ColorNormalizedFile.StarData(
             # Median flux value
             log_file.specialized_median_for_internight_normalization(),
             np.nan,  # Normalized median
             np.nan,  # Norm factor
             # Star color in color ref file
             color_data_file.get_star_color(log_file.star_number()),
             np.nan,  # Actual color value used
             log_file.attendance(),  # Attendance of the star for the night
-            reference_file_data.get_star_adu(log_file.star_number()) or np.nan,
+            logfile_combined_reference_file.get_star_data(log_file.star_number()).radii_adu[radius_of_extraction] or np.nan
         )
         for log_file in flux_logs_files
     }
     last_star_no = 2508  # Note not 2510 as 2509/10 don't have data in ref file
 
     # We calculate the ratio of signal in reference file data and the special
     # median signal for a star for the night. We do this for each stars with
@@ -195,22 +189,28 @@
                 stars_to_include.append(star_no)
 
         # Colors
         x_values = [data_dict[star_no].measured_mean_r_i for star_no in stars_to_include]
         # Signal ratios
         y_values = [stars_signal_ratio[star_no] for star_no in stars_to_include]
 
+        # Sort by x
+        x_sort_indices = np.argsort(x_values)
+        x_values - np.array(x_values)[x_sort_indices]
+        y_values - np.array(y_values)[x_sort_indices]
+        stars_to_include = np.array(stars_to_include)[x_sort_indices]
+
         # These lines of code check to make sure the first or last data point in
         # the signal value isn't an outlier.  First or last data points tend to
         # greatly affect the polynomial fit, so if the data points are 2
         # standard deviations away from the next closest point, they are
         # replaced with the mean of the next two closest points.
-        std_signals = np.std(y_values)
+        std_signals = np.std(y_values, ddof=1)
         beginning_diff = abs(y_values[0] - y_values[1]) / std_signals
-        ending_diff = abs(y_values[0] - y_values[1]) / std_signals
+        ending_diff = abs(y_values[-1] - y_values[-2]) / std_signals
         if beginning_diff > 2 or ending_diff > 2:
             modified_y_value = y_values.copy()  # Note making copy is important
             if beginning_diff > 2:
                 # Note python slicing excludes last element, IDL's includes
                 modified_y_value[0] = np.mean(modified_y_value[1:4])
             if ending_diff > 2:
                 # Note python slicing excludes last element, IDL's includes
@@ -240,34 +240,34 @@
         }
 
     # This holds the y_differences for three sections calculated in the loop above
     y_differences = []
     for section_number in sections:
         y_differences += section_data[section_number]["y_differences"]
 
-    y_diff_std = np.std(y_differences)
+    y_diff_std = np.std(y_differences, ddof=1)
     y_diff_mean = np.mean(y_differences)
     y_diff_min = y_diff_mean - 5 * y_diff_std
     y_diff_max = y_diff_mean + 5 * y_diff_std
-    y_no_of_bins = 11  # We want to use 11 bins, like IDL code
+    y_no_of_bins = 10  # We want to use 10 bins, like IDL code
     bin_frequencies, bins_edges = np.histogram(
         y_differences, range=[y_diff_min, y_diff_max], bins=y_no_of_bins
     )
     bins_mid_values = []
     for index, current_value in enumerate(bins_edges[:-1]):
         next_value = bins_edges[index + 1]
         bins_mid_values.append((current_value + next_value) / 2)
     fit_coefficients, _ = curve_fit(n_term_3_gauss_fit, bins_mid_values, bin_frequencies)
     mean, sigma = fit_coefficients[1], fit_coefficients[2]
     sigma = abs(sigma)  # Important since sigma given by our curve fit could be negative
 
     # Now we find stars for which y_difference is more than 2std away from mean
     stars_outside_threshold = []
-    top_threshold = mean + 2 * sigma
-    bottom_threshold = mean - 2 * sigma
+    top_threshold = mean + 2.5 * sigma
+    bottom_threshold = mean - 2.5 * sigma
     # We now create a list of stars that are outside the specified threshold
     for section_number in sections:
         section_y_differences = section_data[section_number]["y_differences"]
         section_stars = section_data[section_number]["stars_to_include"]
         for index, y_diff in enumerate(section_y_differences):
             if y_diff < bottom_threshold or y_diff > top_threshold:
                 if sigma != 0:  # Guard for when fit fails and sigma is 0
```

### Comparing `m23-0.1.130/m23/matrix/fill.py` & `m23-0.2.0/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/norm/__init__.py` & `m23-0.2.0/m23/norm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 from datetime import date
 from pathlib import Path
 from typing import List
 
 import numpy as np
 
+from m23.constants import INTRA_NIGHT_IMPACT_THRESHOLD_PIXELS
 from m23.file.flux_log_combined_file import FluxLogCombinedFile
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.normfactor_file import NormfactorFile
 from m23.file.reference_log_file import ReferenceLogFile
 
 from .get_line import get_star_to_ignore_bit_vector
 
@@ -76,15 +77,15 @@
             if not all([x > 0 for x in star_data_in_log_file.radii_adu.values()]) or star_data_in_log_file.sky_adu <= 0:
                 adu_of_current_log_file[star_index] = 0 # Ignore this star for normfactor calc of this logfile
                 continue
 
             star_x_reffile, star_y_reffile = reference_log_file.get_star_xy(star_no)
             star_x_position, star_y_position = star_data_in_log_file.x, star_data_in_log_file.y
             
-            if math.sqrt((star_x_reffile - star_x_position) ** 2 + (star_y_reffile - star_y_position) ** 2) > 1:
+            if math.sqrt((star_x_reffile - star_x_position) ** 2 + (star_y_reffile - star_y_position) ** 2) > INTRA_NIGHT_IMPACT_THRESHOLD_PIXELS:
                 adu_of_current_log_file[star_index] = 0
             
         all_log_files.append(adu_of_current_log_file)
     
     # Now for each log file we calculate its normfactor
     # For each logfile, its normfactor is the median of normfactors of the stars
     # in that image.
```

### Comparing `m23-0.1.130/m23/norm/get_line.py` & `m23-0.2.0/m23/norm/get_line.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import Iterable
 
 import numpy as np
 
 from m23.file.log_file_combined_file import LogFileCombinedFile
 
 
@@ -13,25 +14,31 @@
     bright line at the edge after alignment step in old camera images. Note that
     in the bit vector, 0 means that star is to be avoided, 1 means the star is
     to be included.
     """
     y_coordinates = log_file_combined_file.get_x_position_column()
     x_coordinates = log_file_combined_file.get_y_position_column()
 
+    night_date = log_file_combined_file.night_date()
+    logger = logging.getLogger("LOGGER_" + str(night_date))
+
     # We now alter the x and the y values of the stars that don't have 
     # any ADU value because we don't want to consider them as the stars in 
-    # the corners
+    # the corners. Note that we reset this value after calculating stars to ignore
+    stars_with_bogus_set = {} 
 
     for index in range(len(log_file_combined_file.data())):
         star_no = index + 1
         star_data = log_file_combined_file.get_star_data(star_no)
         if not (star_data.sky_adu > 0 and all([adu > 0 for adu in star_data.radii_adu.values()])): # Note that some may be nan values
             # Set a bogus value on the star's x and y coordinate 
             # so that it won't affect corner star calculation
             bogus = 512
+            stars_with_bogus_set[star_no] = [x_coordinates[index], y_coordinates[index]]
+            logger.debug(f"Intranight Linfit. Setting bogus x, y as {bogus} to star {star_no}. Found star data {star_data}. Logfile {log_file_combined_file}")
             x_coordinates[index] = bogus
             y_coordinates[index] = bogus
         
     bit_vector=[]
 
     # IDL and Python has axes reversed
     dist_from_top_left = np.sqrt(x_coordinates**2+y_coordinates**2) 
@@ -80,14 +87,24 @@
     x_and_y_coordinates = np.stack((x_coordinates, y_coordinates), axis = 1)
     for star_position in x_and_y_coordinates: 
         if should_include(star_position):
                 bit_vector.append(1)
         else:
             bit_vector.append(0)
 
+
+    # Cleanup
+    # Reverse the x, y co-ordinates of the stars with where we set bogus co-ordinates
+    for star, actual_coordinates in stars_with_bogus_set.items():
+        actual_x, actual_y = actual_coordinates
+        x_coordinates[star - 1] = actual_x
+        y_coordinates[star - 1] = actual_y
+
+
+
     return bit_vector
 
 def is_point_to_left_of_line(a, b, point):
     eqn_y = lambda x : a*x + b
     eqn_x = lambda y : (y - b)/ a
     x, y = point
     x_prime = eqn_x(y)
```

### Comparing `m23-0.1.130/m23/processor/config_loader.py` & `m23-0.2.0/m23/processor/config_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from m23.constants import (
     CAMERA_CHANGE_2022_DATE,
     INPUT_CALIBRATION_FOLDER_NAME,
     M23_RAW_IMAGES_FOLDER_NAME,
     TYPICAL_NEW_CAMERA_CROP_REGION,
 )
+from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.utils import (
     get_darks,
     get_date_from_input_night_folder_name,
     get_flats,
     get_raw_images,
 )
 
@@ -43,14 +44,15 @@
     nights: List[ConfigInputNight]
     radii_of_extraction: List[int]
 
 
 class ConfigReference(TypedDict):
     image: str | Path
     file: str | Path
+    logfile : str | Path
     color: str | Path
 
 
 class ConfigOutput(TypedDict):
     path: str | Path
 
 
@@ -308,22 +310,23 @@
     """
     Returns True if input for all nights is valid, False otherwise.
     """
     return all([validate_night(night) for night in list_of_nights])
 
 
 def validate_reference_files(
-    reference_image: str, reference_file: str, color_ref_file: str
+    reference_image: str, reference_file: str, color_ref_file: str, logfile : str, radii : List[int]
 ) -> bool:
     """
     Returns True if reference_image and reference_file paths exist
     """
     img_path = Path(reference_image)
     file_path = Path(reference_file)
     color_path = Path(color_ref_file)
+    logfile_path = Path(logfile)
     if not (
         img_path.exists() and img_path.is_file() and img_path.suffix == ".fit"
     ):
         sys.stderr.write(
             "Make sure that the reference exists and has .fit extension"
         )
         return False
@@ -341,14 +344,34 @@
         and color_path.is_file()
         and color_path.suffix == ".txt"
     ):
         sys.stderr.write(
             "Make sure that the color reference file exists and has .txt extension\n"
         )
         return False
+    if not (
+        logfile_path.exists()
+        and logfile_path.is_file()
+        and logfile_path.suffix == ".txt"
+    ):
+        sys.stderr.write(
+            "Make sure that the log file exists and has .txt extension\n"
+        )
+        return False
+    
+    # Make sure that the logfile combined reference file has 
+    # all radii of extraction data
+    available_radii = LogFileCombinedFile(logfile_path).get_star_data(1).radii_adu.keys()
+    for i in radii:
+        if i not in available_radii:
+            sys.stderr.write(
+                f"Radius {i} ADU data not present in provided logfile combined file. \n"
+            )
+            return False
+
     return True
 
 
 def validate_file(
     file_path: Path, on_success: Callable[[Config], None]
 ) -> None:
     """
@@ -368,26 +391,27 @@
             "processing": {
                 "no_of_images_to_combine": int(_),
                 "radii_of_extraction": list(radii_of_extraction),
             },
             "reference": {
                 "image": str(reference_image),
                 "file": str(reference_file),
+                "logfile": str(logfile),
                 "color": str(color_ref_file),
             },
             "input": {"nights": list(list_of_nights)},
             "output": {"path": str(_)},
         } if (
             verify_optional_image_options(optional_image_options)
             and is_valid_radii_of_extraction(radii_of_extraction)
             and validate_input_nights(list_of_nights)
             and validate_reference_files(
-                reference_image, reference_file, color_ref_file
+                reference_image, reference_file, color_ref_file, logfile, radii_of_extraction
             )
         ):
             on_success(
                 sanity_check(create_processing_config(toml.load(file_path)))
             )
         case _:
             sys.stderr.write(
-                "Stopping because the provided configuration file has issues.\n"
+                "Stopping because the provided configuration file doesn't match the required format.\n"
             )
```

### Comparing `m23-0.1.130/m23/processor/generate_masterflat.py` & `m23-0.2.0/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/processor/generate_masterflat_config_loader.py` & `m23-0.2.0/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/processor/nights_csv.py` & `m23-0.2.0/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/processor/nights_csv_config_loader.py` & `m23-0.2.0/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/processor/process_nights.py` & `m23-0.2.0/m23/processor/process_nights.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,21 +49,21 @@
     radii_of_extraction: List[int],
     reference_log_file: ReferenceLogFile,
     log_files_to_use: List[LogFileCombinedFile],
     img_duration: float,
     night_date: date,
     color_ref_file_path: Path,
     output: Path,
+    logfile_combined_reference_logfile : LogFileCombinedFile
+
 ):
     """
     This is a normalization helper function extracted so that it can be reused by the renormalization script
     """
     FLUX_LOGS_COMBINED_OUTPUT_FOLDER = output / FLUX_LOGS_COMBINED_FOLDER_NAME
-    ref_file_path = reference_log_file.path()
-
     logger = logging.getLogger("LOGGER_" + str(night_date))
 
     for radius in radii_of_extraction:
         logger.info(f"Normalizing for radius of extraction {radius} px")
         RADIUS_FOLDER = FLUX_LOGS_COMBINED_OUTPUT_FOLDER / get_radius_folder_name(radius)
         RADIUS_FOLDER.mkdir(exist_ok=True)  # Create folder if it doesn't exist
         for file in RADIUS_FOLDER.glob("*"):
@@ -75,15 +75,15 @@
             RADIUS_FOLDER,
             radius,
             img_duration,
             night_date,
         )
     draw_normfactors_chart(log_files_to_use, FLUX_LOGS_COMBINED_OUTPUT_FOLDER.parent)
     # Internight normalization
-    internight_normalize(output, ref_file_path, color_ref_file_path, radii_of_extraction)
+    internight_normalize(output, logfile_combined_reference_logfile, color_ref_file_path, radii_of_extraction)
 
 
 def process_night(night: ConfigInputNight, config: Config, output: Path, night_date: date):
     """
     Processes a given night of data based on the settings provided in `config` dict
     """
     # Save the config file used to do the current data processing
@@ -112,14 +112,15 @@
     logger.addHandler(ch2)  # Write to stdout
     logger.info(f"Starting processing for {night_date}")
 
     ref_image_path = config["reference"]["image"]
     ref_file_path = config["reference"]["file"]
     color_ref_file_path = config["reference"]["color"]
     reference_log_file = ReferenceLogFile(ref_file_path)
+    logfile_combined_reference_logfile = LogFileCombinedFile(config["reference"]["logfile"])
 
     # Define relevant input folders for the night being processed
     NIGHT_INPUT_FOLDER: Path = night["path"]
     NIGHT_INPUT_CALIBRATION_FOLDER: Path = NIGHT_INPUT_FOLDER / INPUT_CALIBRATION_FOLDER_NAME
     NIGHT_INPUT_IMAGES_FOLDER = NIGHT_INPUT_FOLDER / M23_RAW_IMAGES_FOLDER_NAME
 
     # Define and create relevant output folders for the night being processed
@@ -261,14 +262,15 @@
         radii_of_extraction,
         reference_log_file,
         log_files_to_normalize,
         image_duration,
         night_date,
         color_ref_file_path,
         output,
+        logfile_combined_reference_logfile
     )
 
 
 def start_data_processing_auxiliary(config: Config):
     """
     This function processes (one or more) nights defined in config dict by
     putting together various functionalities like calibration, alignment,
```

### Comparing `m23-0.1.130/m23/processor/renormalize.py` & `m23-0.2.0/m23/processor/renormalize.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,23 +28,28 @@
         ch.setFormatter(formatter)
         logger.addHandler(ch)
         # Write to std out in addition to writing to a logfile
         ch2 = logging.StreamHandler(sys.stdout)
         ch2.setFormatter(formatter)
         logger.addHandler(ch2)  # Write to stdout
 
-        logger.info(f"Running renormalization for radii {radii_of_extraction}")
+        first_image = night["first_logfile_number"]
+        last_image = night["last_logfile_number"]
+        logger.info(
+            f"Running renormalization for radii {radii_of_extraction}. Img: {first_image}-{last_image}"
+        )
 
         FLUX_LOGS_COMBINED_FOLDER: Path = NIGHT_FOLDER / FLUX_LOGS_COMBINED_FOLDER_NAME
         # Create log files combined folder if it doesn't yet exist
         FLUX_LOGS_COMBINED_FOLDER.mkdir(exist_ok=True)
 
         reference_log_file = ReferenceLogFile(
             renormalize_dict["reference"]["file"],
         )
+        logfile_combined_reference_logfile = LogFileCombinedFile(renormalize_dict["reference"]["logfile"])
 
         # Ensure color ref file path is str
         color_ref_file_path = str(renormalize_dict["reference"]["color"])
 
         log_files_to_use = [LogFileCombinedFile(file) for file in night["files_to_use"]]
         img_duration = log_files_to_use[0].img_duration()
 
@@ -53,14 +58,15 @@
             radii_of_extraction,
             reference_log_file,
             log_files_to_use,
             img_duration,
             night_date,
             color_ref_file_path,
             NIGHT_FOLDER,
+            logfile_combined_reference_logfile
         )
 
 
 def renormalize(file_path: str):
     """
     Starts renormalization with the configuration file `file_path` provided as the argument.
     Calls auxiliary function `renormalize_auxiliary` if the configuration is valid.
```

### Comparing `m23-0.1.130/m23/processor/renormalize_config_loader.py` & `m23-0.2.0/m23/processor/renormalize_config_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 from pathlib import Path
 from typing import Callable, List, TypedDict
 
 import toml
 from typing_extensions import NotRequired
 
 from m23.constants import LOG_FILES_COMBINED_FOLDER_NAME
+from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.processor.config_loader import (
     is_night_name_valid,
     is_valid_radii_of_extraction,
 )
 from m23.utils import get_image_number_in_log_file_combined_file
 
 
 class RenormalizeConfigProcessing(TypedDict):
     radii_of_extraction: List[int]
 
 
 class RenormalizeConfigReference(TypedDict):
     file: Path | str
+    logfile: Path | str
     color: Path | str
 
 
 class RenormalizeConfigNight(TypedDict):
     path: Path | str
     first_logfile_number: int
     last_logfile_number: int
@@ -72,14 +74,31 @@
 
     # Validate reference file
     ref_file = Path(config["reference"]["file"])
     if not (ref_file.exists() and ref_file.is_file() and ref_file.suffix == ".txt"):
         sys.stderr.write("Make sure the provided reference file exits and has txt extension\n")
         return False
 
+    # Validate logfile file
+    logfile = Path(config["reference"]["logfile"])
+    if not (logfile.exists() and logfile.is_file() and logfile.suffix == ".txt"):
+        sys.stderr.write("Make sure the provided logfile file exits and has txt extension\n")
+        return False
+
+    # Make sure that the logfile combined reference file has 
+    # all radii of extraction data
+    available_radii = LogFileCombinedFile(logfile).get_star_data(1).radii_adu.keys()
+    for i in config["processing"]["radii_of_extraction"]:
+        if i not in available_radii:
+            sys.stderr.write(
+                f"Radius {i} ADU data not present in provided logfile combined file. \n"
+            )
+            return False
+
+
     color_ref_file = Path(config["reference"]["color"])
     if not (
         color_ref_file.exists() and color_ref_file.is_file() and color_ref_file.suffix == ".txt"
     ):
         sys.stderr.write(
             "Make sure the provided color reference file exits and has txt extension\n"
         )
@@ -175,15 +194,15 @@
     """
     if not file_path.exists() or not file_path.exists():
         raise FileNotFoundError("Cannot find configuration file")
     match toml.load(file_path):
         case {
             "processing": {"radii_of_extraction": list(_)},
             "input": {"nights": list(_)},
-            "reference": {"file": str(_), "color": str(_)},
+            "reference": {"file": str(_), "color": str(_), "logfile" : str(_)},
         } as renormalize_config if is_valid(renormalize_config):
             on_success(sanity_check(create_enhanced_config(renormalize_config)))
         case _:
             sys.stderr.write("Stopping because the provided configuration file has issues.\n")
 
 
 if __name__ == "__main__":
```

### Comparing `m23-0.1.130/m23/utils/__init__.py` & `m23-0.2.0/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/utils/date.py` & `m23-0.2.0/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23/utils/rename.py` & `m23-0.2.0/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-0.1.130/m23.egg-info/SOURCES.txt` & `m23-0.2.0/m23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

