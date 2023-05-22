# Comparing `tmp/zipreport-lib-1.0.2.tar.gz` & `tmp/zipreport-lib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipreport-lib-1.0.2.tar", last modified: Wed May 17 16:23:16 2023, max compression
+gzip compressed data, was "zipreport-lib-1.1.0.tar", last modified: Mon May 22 16:39:59 2023, max compression
```

## Comparing `zipreport-lib-1.0.2.tar` & `zipreport-lib-1.1.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.052072 zipreport-lib-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-17 16:23:16.052072 zipreport-lib-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:23:16.052072 zipreport-lib-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.036072 zipreport-lib-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.040072 zipreport-lib-1.0.2/tests/fileutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/basefs.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/basezip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/test_diskfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/test_pathcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/test_zipfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.040072 zipreport-lib-1.0.2/tests/processors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/processors/test_mime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.040072 zipreport-lib-1.0.2/tests/render/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.040072 zipreport-lib-1.0.2/tests/render/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/filters/test_jinjafilters.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/test_jinjaloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/test_jinjarender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/tests/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/report/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/report/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/report/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/cli/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/cli/debug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/cli/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/cli/debug/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/fileutils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/fileutils/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/backend/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/diskfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/pathcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/zipfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/misc/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.048072 zipreport-lib-1.0.2/zipreport/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/weasyprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/wkhtmltopdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/zipreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.048072 zipreport-lib-1.0.2/zipreport/report/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/reportfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.048072 zipreport-lib-1.0.2/zipreport/template/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.048072 zipreport-lib-1.0.2/zipreport/template/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/jinja/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/jinjaloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/jinjarender.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/zipreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.052072 zipreport-lib-1.0.2/zipreport_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-17 16:23:16.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.374814 zipreport-lib-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-22 16:39:59.374814 zipreport-lib-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:39:59.374814 zipreport-lib-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.366814 zipreport-lib-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.366814 zipreport-lib-1.1.0/tests/fileutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/fileutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/fileutils/basefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/fileutils/basezip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/fileutils/test_diskfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/fileutils/test_pathcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/fileutils/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/fileutils/test_zipfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.366814 zipreport-lib-1.1.0/tests/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/processors/test_mime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/tests/render/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/render/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/tests/render/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/render/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/render/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/render/filters/test_jinjafilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/render/test_jinjaloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/render/test_jinjarender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/tests/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/report/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/report/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/report/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/zipreport/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/zipreport/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/cli/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/zipreport/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/cli/debug/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/zipreport/fileutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/fileutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/zipreport/fileutils/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/fileutils/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/fileutils/backend/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/fileutils/diskfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/fileutils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/fileutils/pathcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/fileutils/zipfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/zipreport/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/misc/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.370814 zipreport-lib-1.1.0/zipreport/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/processors/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/processors/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/processors/weasyprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/processors/wkhtmltopdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/processors/zipreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.374814 zipreport-lib-1.1.0/zipreport/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/report/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/report/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/report/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/report/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/report/reportfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.374814 zipreport-lib-1.1.0/zipreport/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.374814 zipreport-lib-1.1.0/zipreport/template/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/template/jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/template/jinja/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/template/jinjaloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/template/jinjarender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-22 16:39:45.000000 zipreport-lib-1.1.0/zipreport/zipreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:39:59.374814 zipreport-lib-1.1.0/zipreport_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-22 16:39:59.000000 zipreport-lib-1.1.0/zipreport_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-22 16:39:59.000000 zipreport-lib-1.1.0/zipreport_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:39:59.000000 zipreport-lib-1.1.0/zipreport_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 16:39:59.000000 zipreport-lib-1.1.0/zipreport_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:39:59.000000 zipreport-lib-1.1.0/zipreport_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-22 16:39:59.000000 zipreport-lib-1.1.0/zipreport_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 16:39:59.000000 zipreport-lib-1.1.0/zipreport_lib.egg-info/top_level.txt
```

### Comparing `zipreport-lib-1.0.2/LICENSE` & `zipreport-lib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/PKG-INFO` & `zipreport-lib-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: Joao Pinheiro
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
```

### Comparing `zipreport-lib-1.0.2/README.md` & `zipreport-lib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/setup.py` & `zipreport-lib-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/fileutils/basefs.py` & `zipreport-lib-1.1.0/tests/fileutils/basefs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/fileutils/basezip.py` & `zipreport-lib-1.1.0/tests/fileutils/basezip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/fileutils/test_diskfs.py` & `zipreport-lib-1.1.0/tests/fileutils/test_diskfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/fileutils/test_pathcache.py` & `zipreport-lib-1.1.0/tests/fileutils/test_pathcache.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/fileutils/test_zip.py` & `zipreport-lib-1.1.0/tests/fileutils/test_zip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/fileutils/test_zipfs.py` & `zipreport-lib-1.1.0/tests/fileutils/test_zipfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/processors/base.py` & `zipreport-lib-1.1.0/tests/processors/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/processors/test_mime.py` & `zipreport-lib-1.1.0/tests/processors/test_mime.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/render/base.py` & `zipreport-lib-1.1.0/tests/render/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/render/filters/base.py` & `zipreport-lib-1.1.0/tests/render/filters/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/render/filters/test_jinjafilters.py` & `zipreport-lib-1.1.0/tests/render/filters/test_jinjafilters.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/render/test_jinjaloader.py` & `zipreport-lib-1.1.0/tests/render/test_jinjaloader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/render/test_jinjarender.py` & `zipreport-lib-1.1.0/tests/render/test_jinjarender.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/report/test_builder.py` & `zipreport-lib-1.1.0/tests/report/test_builder.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/report/test_job.py` & `zipreport-lib-1.1.0/tests/report/test_job.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/report/test_loader.py` & `zipreport-lib-1.1.0/tests/report/test_loader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/tests/utils.py` & `zipreport-lib-1.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/zipreport/cli/console.py` & `zipreport-lib-1.1.0/zipreport/cli/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 
 from zipreport.cli.debug.server import DebugServer
 from zipreport.report import ReportFileBuilder, ReportFileLoader, const
 from zipreport.version import get_version
 
 
 class Commands:
-    EXT = '.zpt'
+    EXT = ".zpt"
     HELP_LINE = "  %-30s %s\n"
     LIST_LINE = "%-20s %s"
     COMMANDS = {
-        'help': ['', 'Show usage information'],
-        'version': ['[-m]', 'Show version (or version number only, if -m)'],
-        'list': ['<path>', 'List reports on the given path'],
-        'info': ['<file> [<file>...]', 'Show report details'],
-        'build': ['<directory> [output_file]', 'Build zpt file bundle'],
-        'debug': ['<directory|file> [[host]:<port>]', 'Run debug server using the directory or specified file'],
+        "help": ["", "Show usage information"],
+        "version": ["[-m]", "Show version (or version number only, if -m)"],
+        "list": ["<path>", "List reports on the given path"],
+        "info": ["<file> [<file>...]", "Show report details"],
+        "build": ["<directory> [output_file]", "Build zpt file bundle"],
+        "debug": [
+            "<directory|file> [[host]:<port>]",
+            "Run debug server using the directory or specified file",
+        ],
     }
 
     def run(self, args: list):
         if len(args) == 0:
             self.help([])
             return 0
 
@@ -34,15 +37,15 @@
 
         if method(args[1:]) is False:
             return 1
 
         return 0
 
     def version(self, args=None):
-        minimal = len(args) == 1 and args[0] == '-m'
+        minimal = len(args) == 1 and args[0] == "-m"
         if minimal:
             vstr = "{}"
         else:
             vstr = "\nVersion: {}\n"
         print(vstr.format(get_version()))
 
     def help(self, args=None):
@@ -74,15 +77,15 @@
             return False
 
         if len(args) == 2:
             dest = Path(args[1]).resolve()
         else:
             dest = Path(src.name)
 
-        if dest.suffix == '':
+        if dest.suffix == "":
             dest = dest.with_suffix(self.EXT)
 
         result = ReportFileBuilder.build_file(src, dest)
         if not result.success():
             self.error(" ".join(result.get_errors()))
         return result.success()
 
@@ -119,20 +122,23 @@
         if not path.exists():
             self.error("Error: Invalid path")
             return False
         if not path.is_dir():
             self.error("Error: Path is not a valid directory")
             return False
 
-        for (dirpath, dirnames, filenames) in os.walk(path):
+        for dirpath, dirnames, filenames in os.walk(path):
             for f in filenames:
-                if f.endswith('.zpt'):
+                if f.endswith(".zpt"):
                     try:
                         zpt = ReportFileLoader.load_file(f)
-                        print(self.LIST_LINE % (f, zpt.get_param(const.MANIFEST_TITLE, "")))
+                        print(
+                            self.LIST_LINE
+                            % (f, zpt.get_param(const.MANIFEST_TITLE, ""))
+                        )
                     except Exception:
                         # ignore file
                         pass
         return True
 
     def info(self, args) -> bool:
         if len(args) == 0:
```

### Comparing `zipreport-lib-1.0.2/zipreport/cli/debug/server.py` & `zipreport-lib-1.1.0/zipreport/cli/debug/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,23 @@
     """Simple HTTP request handler with GET and HEAD commands.
 
     This class is based on the SimpleHTTPRequestHandler in http.server
     Due to its simplified implementation, the code is not thread-safe!!!
     """
 
     server_version = "ZipReport HTTP Server"
-    root_paths = ['/', '/index.html', '/index.htm', '/report.html', '/report.htm', ]
+    root_paths = [
+        "/",
+        "/index.html",
+        "/index.htm",
+        "/report.html",
+        "/report.htm",
+    ]
     extensions_map = {
-        '': 'application/octet-stream',
+        "": "application/octet-stream",
     }
 
     def __init__(self, *args, report_path=None, extra_mime_types=None, **kwargs):
         """
         Constructor
         :param args:
         :param report_path: path of the directory or zpt file to process
@@ -128,32 +134,32 @@
 
         if path in self.root_paths:
             if response is None:
                 success, response = self.build_report()
                 if not success:
                     return response
             # rewrite path to point to report file
-            path = '/' + const.REPORT_FILE_NAME
+            path = "/" + const.REPORT_FILE_NAME
 
         if _zpt.exists(path):
             return self.handle_file(Path(path).name, _zpt.get(path))
 
         # path not found
         return self.error_404(path)
 
     def clean_path(self, path: str) -> str:
         """
         Cleans up the request path
         :param path:str
         """
         # remove ignored parameters
-        path = path.split('?', 1)[0]
-        path = path.split('#', 1)[0]
+        path = path.split("?", 1)[0]
+        path = path.split("#", 1)[0]
         try:
-            path = unquote(path, errors='surrogatepass')
+            path = unquote(path, errors="surrogatepass")
         except UnicodeDecodeError:
             path = unquote(path)
         return posixpath.normpath(path)
 
     def guess_type(self, fname: str):
         """
         Tries to determine a filename mime type
@@ -162,15 +168,15 @@
         if ext in self.extensions_map:
             return self.extensions_map[ext]
 
         ext = ext.lower()
         if ext in self.extensions_map:
             return self.extensions_map[ext]
 
-        return self.extensions_map['']
+        return self.extensions_map[""]
 
     def handle_file(self, fname: str, contents: io.BytesIO) -> io.BytesIO:
         """
         Generates response headers for a given file
         :param fname:
         :param contents:
         :return: io.BytesIO
@@ -185,50 +191,58 @@
     def error_500(self, item: str):
         """
         Generates a customized 500 response
         :param item: optional error message
         :return: io.BytesIO
         """
         if item:
-            response = "<html><body><h3>Internal Server Error: {}</h3></body></html>".format(item)
+            response = (
+                "<html><body><h3>Internal Server Error: {}</h3></body></html>".format(
+                    item
+                )
+            )
         else:
             response = "<html><body><h3>File not found</h3></body></html>"
         return self._error(HTTPStatus.INTERNAL_SERVER_ERROR, response)
 
     def error_404(self, item: str = None) -> io.BytesIO:
         """
         Generates a customized 404 response
         :param item: optional error message
         :return: io.BytesIO
         """
         if item:
-            response = "<html><body><h3>File not found: {}</h3></body></html>".format(item)
+            response = "<html><body><h3>File not found: {}</h3></body></html>".format(
+                item
+            )
         else:
             response = "<html><body><h3>File not found</h3></body></html>"
         return self._error(HTTPStatus.NOT_FOUND, response)
 
     def _error(self, code: int, contents: str) -> io.BytesIO:
         """
         Common error response logic
         :param code: HTTP status code
         :param contents: optional HTML response
         :return: io.BytesIO
         """
         size = len(contents)
-        response = io.BytesIO(bytes(contents, encoding='utf-8'))
+        response = io.BytesIO(bytes(contents, encoding="utf-8"))
         self.send_response(code)
-        self.send_header("Content-type", "text/html; charset=%s" % sys.getfilesystemencoding())
+        self.send_header(
+            "Content-type", "text/html; charset=%s" % sys.getfilesystemencoding()
+        )
         self.send_header("Content-Length", str(size))
         self.end_headers()
         response.seek(0)
         return response
 
 
 class DebugServer:
-    DEFAULT_ADDR = 'localhost'
+    DEFAULT_ADDR = "localhost"
     DEFAULT_PORT = 8001
 
     def __init__(self, addr: str = DEFAULT_ADDR, port: int = DEFAULT_PORT):
         self._addr = addr
         self._port = port
 
     def set_addr(self, addr: str):
@@ -238,14 +252,16 @@
         self._port = port
 
     def run(self, report_path: str):
         server_address = (self._addr, int(self._port))
         handler_class = partial(ReportFileHandler, report_path=report_path)
         sys.stdout.write(
             "\nStarted debug server at http://{addr}:{port}\nServing from: {path}\nUse Ctrl+C to stop...\n\n".format(
-                addr=self._addr, port=int(self._port), path=Path(report_path).absolute()))
+                addr=self._addr, port=int(self._port), path=Path(report_path).absolute()
+            )
+        )
         httpd = HTTPServer(server_address, handler_class)
         try:
             httpd.serve_forever()
         except KeyboardInterrupt:
             pass
         return
```

### Comparing `zipreport-lib-1.0.2/zipreport/fileutils/backend/zip.py` & `zipreport-lib-1.1.0/zipreport/fileutils/backend/zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,35 +29,37 @@
 
     def new(self, buffer: io.BytesIO = None):
         """
         Initialize new zip file in memory
         :param buffer: optional buffer with zip contents
         :return:
         """
-        flags = 'w'
+        flags = "w"
         if isinstance(buffer, io.BytesIO):
             self._buffer = buffer
-            flags = 'a'
+            flags = "a"
         else:
             self._buffer = io.BytesIO()
         self._zip = zipfile.ZipFile(self._buffer, flags, zipfile.ZIP_DEFLATED)
 
     def load(self, disk_file: str):
         """
         Load zip form disk
         :param disk_file: path to zip file
         :return:
         """
         if not os.path.exists(disk_file) or not os.path.isfile(disk_file):
-            raise InMemoryZipError("Zip file '{}' does not exist or is not a valid file")
+            raise InMemoryZipError(
+                "Zip file '{}' does not exist or is not a valid file"
+            )
 
         try:
-            with open(disk_file, 'rb', buffering=0) as f:
+            with open(disk_file, "rb", buffering=0) as f:
                 self._buffer = io.BytesIO(f.read())
-                self._zip = zipfile.ZipFile(self._buffer, mode='a')
+                self._zip = zipfile.ZipFile(self._buffer, mode="a")
         except Exception as e:
             raise InMemoryZipError("Error reading Zip file: {}".format(e))
 
     def get_buffer(self) -> io.BytesIO:
         """
         Get internal buffer
         Note: this will force a close on the internal zip file; no other operations can be done afterwards
@@ -93,15 +95,15 @@
         :return:
         """
         if not self.is_open():
             raise InMemoryZipError("Cannot save(); Zip is already closed.")
         try:
             self._zip.close()
             self._buffer.seek(0)
-            with open(dest_file, 'wb', buffering=0) as f:
+            with open(dest_file, "wb", buffering=0) as f:
                 f.write(self._buffer.read())
             self._buffer = None
             self._zip = None
         except Exception as e:
             raise InMemoryZipError("Error saving Zip file: {}".format(e))
 
     def zip(self) -> zipfile.ZipFile:
```

### Comparing `zipreport-lib-1.0.2/zipreport/fileutils/diskfs.py` & `zipreport-lib-1.1.0/zipreport/fileutils/diskfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,35 @@
         Add a new file
         :param name: filename with full path
         :param content: file contents
         :return:
         """
         name = self._build_path(name)
         if not self._can_create(os.path.dirname(name), name):
-            raise FsError("Cannot add file '{}'; Invalid path or already existing file".format(name))
+            raise FsError(
+                "Cannot add file '{}'; Invalid path or already existing file".format(
+                    name
+                )
+            )
         with open(name, "wb", buffering=0) as f:
             f.write(content)
 
     def mkdir(self, name: str):
         """
         Creates a directory
         :param name: full directory path
         :return:
         """
         name = self._build_path(name)
         if not self._can_create(os.path.dirname(name), name):
-            raise FsError("Cannot add file '{}'; Invalid path or already existing dir".format(name))
+            raise FsError(
+                "Cannot add file '{}'; Invalid path or already existing dir".format(
+                    name
+                )
+            )
         os.mkdir(name)
 
     def exists(self, path: str) -> bool:
         """
         Check if a given path (file or dir) exists
         :param path:
         :return:
```

### Comparing `zipreport-lib-1.0.2/zipreport/fileutils/interface.py` & `zipreport-lib-1.1.0/zipreport/fileutils/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 class FsError(Exception):
     pass
 
 
 class FsInterface:
-
     def get(self, name: str) -> io.BytesIO:
         """
         Read file
         :param name:
         :return:
         """
         pass
```

### Comparing `zipreport-lib-1.0.2/zipreport/fileutils/pathcache.py` & `zipreport-lib-1.1.0/zipreport/fileutils/pathcache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 
 
 class PathCache:
     """
     ZipFs content cache
     """
-    def __init__(self, trailing='/'):
+
+    def __init__(self, trailing="/"):
         self._sep = trailing
         self._cache = {}
 
     def add(self, item: str):
         """
         Add a file to the path cache
         :param item:
@@ -115,15 +116,15 @@
             else:
                 # invalid path
                 return result
         if root is None:
             # its a file, not a dir
             return result
 
-        return self._path_transversal(root, Path(''))
+        return self._path_transversal(root, Path(""))
 
     def _path_transversal(self, root: dict, path: Path) -> list:
         """
         Internal path transversal routine
         :param root:
         :param path:
         :return:
```

### Comparing `zipreport-lib-1.0.2/zipreport/fileutils/zipfs.py` & `zipreport-lib-1.1.0/zipreport/fileutils/zipfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
 
     def __init__(self, zip: InMemoryZip):
         """
         Constructor
         :param zip: Zip Backend
         """
-        self._sep = '/'
+        self._sep = "/"
         self._zip = zip
         self._cache = PathCache(self._sep)
         self._build_cache()
 
     def get(self, name: str) -> io.BytesIO:
         """
         Read a file
@@ -31,15 +31,17 @@
         """
         zipfile = self._zip.zip()
         try:
             info = zipfile.getinfo(self._clean_path(name))
             with zipfile.open(info) as zf:
                 return io.BytesIO(zf.read())
         except ValueError:
-            raise FsError("Error reading file '{}'. Maybe it doesn't exist?".format(name))
+            raise FsError(
+                "Error reading file '{}'. Maybe it doesn't exist?".format(name)
+            )
 
     def add(self, name: str, content):
         """
         Add a file
         :param name: filename to create
         :param content: file contents
         :return:
```

### Comparing `zipreport-lib-1.0.2/zipreport/misc/html.py` & `zipreport-lib-1.1.0/zipreport/misc/html.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.2/zipreport/processors/mime.py` & `zipreport-lib-1.1.0/zipreport/processors/mime.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,21 +23,21 @@
         self._src = []
         self._href = []
 
     def handle_starttag(self, tag, attrs):
         if not len(attrs):
             return
         attrs = dict(attrs)
-        if 'src' in attrs.keys():
-            src = attrs['src']
+        if "src" in attrs.keys():
+            src = attrs["src"]
             if self.is_local(src):
                 self._src.append(src)
 
-        elif 'href' in attrs.keys() and tag.lower() == 'link':
-            src = attrs['href']
+        elif "href" in attrs.keys() and tag.lower() == "link":
+            src = attrs["href"]
             if self.is_local(src):
                 self._href.append(src)
 
     def get_src_list(self) -> list:
         return list(dict.fromkeys(self._src))
 
     def get_href_list(self) -> list:
@@ -46,51 +46,50 @@
     def get_resource_list(self) -> list:
         a = self.get_src_list()
         a.extend(self.get_href_list())
         return list(dict.fromkeys(a))
 
     def is_local(self, url: str):
         url = url.lower()
-        for prefix in ['http://', 'https://', '//']:
+        for prefix in ["http://", "https://", "//"]:
             if url.startswith(prefix):
                 return False
         return True
 
 
 class MIMEProcessor(ProcessorInterface):
-
     def process(self, job: ReportJob) -> JobResult:
         """
         Executes a rendering job to a MIME message
         Local resources such as images are embedded in the message
         :param job: ReportJob
         :return: JobResult
         """
         opts = job.get_options()
         rpt = job.get_report()
-        html = str(rpt.get(opts[job.OPT_MAIN_SCRIPT]).read(), encoding='utf-8')
+        html = str(rpt.get(opts[job.OPT_MAIN_SCRIPT]).read(), encoding="utf-8")
 
         mime_msg = EmailMessage()
         parser = ResourceParser()
         parser.feed(html)
 
         resources = {}
         # replace html references with cid
         for src in parser.get_resource_list():
             cid = make_msgid()
             resources[cid] = src
             html = html.replace('="{}"'.format(src), '="cid:{}"'.format(cid[1:-1]))
             html = html.replace("='{}'".format(src), "='cid:{}'".format(cid[1:-1]))
 
-        mime_msg.add_alternative(html, subtype='html')
+        mime_msg.add_alternative(html, subtype="html")
 
         # add related resources
         payload = mime_msg.get_payload()[0]
         for cid, fname in resources.items():
             res = rpt.get(fname)
             ctype, encoding = mimetypes.guess_type(fname)
             if ctype is None or encoding is not None:
-                ctype = 'application/octet-stream'
-            maintype, subtype = ctype.split('/', 1)
+                ctype = "application/octet-stream"
+            maintype, subtype = ctype.split("/", 1)
             payload.add_related(res.read(), maintype, subtype, cid=cid)
 
         return JobResult(mime_msg, True, "")
```

### Comparing `zipreport-lib-1.0.2/zipreport/processors/weasyprint.py` & `zipreport-lib-1.1.0/zipreport/processors/weasyprint.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
         # custom weasyprint fetcher
         def f(url):
             return self.fetcher(zpt, url)
 
         rpt = HTML(
             base_url="/",
-            string=io.TextIOWrapper(zpt.get(REPORT_FILE_NAME), encoding='utf-8').read(),
-            url_fetcher=f
+            string=io.TextIOWrapper(zpt.get(REPORT_FILE_NAME), encoding="utf-8").read(),
+            url_fetcher=f,
         ).write_pdf(None, stylesheets=self._css, font_config=self._fconfig)
         return JobResult(io.BytesIO(rpt), True, "")
 
     def fetcher(self, zpt, url):
         """
         Internal fetcher for WeasyPrint to access in-report resources such as images, css and js
         :param zpt: ReportFile
@@ -69,14 +69,14 @@
         :return:
         """
         if url.startswith("http"):
             return default_url_fetcher(url)
 
         fallback = url
         # support for both file:// and relative urls
-        if url.startswith('file://'):
+        if url.startswith("file://"):
             url = url[7:]
 
         if zpt.exists(url):
-            return {'string': zpt.get(url).read()}
+            return {"string": zpt.get(url).read()}
 
         return default_url_fetcher(fallback)
```

### Comparing `zipreport-lib-1.0.2/zipreport/processors/wkhtmltopdf.py` & `zipreport-lib-1.1.0/zipreport/processors/wkhtmltopdf.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from zipreport.report.job import ReportJob, JobResult
 
 
 class WkHtml2PdfProcessor(ProcessorInterface):
     """
     wkhtmltopdf report processor
     """
-    MARGIN_MINIMUM_MM = '5'
+
+    MARGIN_MINIMUM_MM = "5"
 
     def __init__(self, cli_path: str):
         """
         Constructor
         :param cli_path: full path to wkhtmltopdf binary
         """
         self._cli = cli_path
@@ -36,61 +37,83 @@
             path = Path(tempfile.mkdtemp())
             cmd = self.build_cmd(job, path)
             job.get_report().get_fs().get_backend().zip().extractall(path)
 
             subprocess.run(cmd, cwd=path, check=True)
             report_file = path / const.PDF_FILE_NAME
             if report_file.exists():
-                with open(report_file, 'rb') as f:
+                with open(report_file, "rb") as f:
                     report = io.BytesIO(f.read())
                     success = True
 
-        except (subprocess.CalledProcessError, FileNotFoundError, PermissionError, FileExistsError) as e:
+        except (
+            subprocess.CalledProcessError,
+            FileNotFoundError,
+            PermissionError,
+            FileExistsError,
+        ) as e:
             error = str(e)
 
         if path:
             rmtree(path)
 
         return JobResult(report, success, error)
 
-    def build_cmd(self, job: ReportJob, path: Path, dest_file: str = const.PDF_FILE_NAME):
+    def build_cmd(
+        self, job: ReportJob, path: Path, dest_file: str = const.PDF_FILE_NAME
+    ):
         """
         Parse ReportJob options and generate command-line arguments for wkhtmltopdf
         :param job: ReportJob
         :param path: full path for the report root
         :param dest_file: full path for PDF file to be generated
         :return: list
         """
         opts = job.get_options()
         args = [
             str(Path(self._cli)),
-            '--enable-local-file-access',
-            '--allow', str(path),
-            '--no-stop-slow-scripts',
-            '--page-size', opts[ReportJob.OPT_PAGE_SIZE],
-            '--javascript-delay', str(opts[ReportJob.OPT_SETTLING_TIME]),
+            "--enable-local-file-access",
+            "--allow",
+            str(path),
+            "--no-stop-slow-scripts",
+            "--page-size",
+            opts[ReportJob.OPT_PAGE_SIZE],
+            "--javascript-delay",
+            str(opts[ReportJob.OPT_SETTLING_TIME]),
         ]
 
         # non-default margins
         if opts[ReportJob.OPT_MARGINS] == const.PDF_MARGIN_NONE:
-            args.extend([
-                '--margin-bottom', "0",
-                '--margin-left', "0",
-                '--margin-right', "0",
-                '--margin-top', "0"
-            ])
+            args.extend(
+                [
+                    "--margin-bottom",
+                    "0",
+                    "--margin-left",
+                    "0",
+                    "--margin-right",
+                    "0",
+                    "--margin-top",
+                    "0",
+                ]
+            )
 
         if opts[ReportJob.OPT_MARGINS] == const.PDF_MARGIN_MINIMUM:
-            args.extend([
-                '--margin-bottom', self.MARGIN_MINIMUM_MM,
-                '--margin-left', self.MARGIN_MINIMUM_MM,
-                '--margin-right', self.MARGIN_MINIMUM_MM,
-                '--margin-top', self.MARGIN_MINIMUM_MM,
-            ])
+            args.extend(
+                [
+                    "--margin-bottom",
+                    self.MARGIN_MINIMUM_MM,
+                    "--margin-left",
+                    self.MARGIN_MINIMUM_MM,
+                    "--margin-right",
+                    self.MARGIN_MINIMUM_MM,
+                    "--margin-top",
+                    self.MARGIN_MINIMUM_MM,
+                ]
+            )
 
         # page orientation
         if opts[ReportJob.OPT_LANDSCAPE]:
-            args.append('--orientation')
-            args.append('Landscape')
+            args.append("--orientation")
+            args.append("Landscape")
 
         args.extend([opts[ReportJob.OPT_MAIN_SCRIPT], dest_file])
         return args
```

### Comparing `zipreport-lib-1.0.2/zipreport/processors/zipreport.py` & `zipreport-lib-1.1.0/zipreport/processors/zipreport.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 
 class ZipReportClient:
     """
     zipreport-server API Client
     """
 
-    def __init__(self, url: str, api_key: str, api_version: int = 1, secure_ssl: bool = False):
+    def __init__(
+        self, url: str, api_key: str, api_version: int = 1, secure_ssl: bool = False
+    ):
         """
         Constructor
         :param url: zipreport-server API url
         :param api_key: API key
         :param api_version: API version (default 1)
         :param secure_ssl: check SSL CA (default False)
         """
@@ -34,26 +36,26 @@
         """
         Execute a ReportJob using API
         :param job: ReportJob
         :return: JobResult
         """
         url = "{}/v{}/render".format(self._url, self._api_version)
         request_data = {
-            'report': ('report.zpt', job.get_report().save()),
+            "report": ("report.zpt", job.get_report().save()),
         }
         for k, v in job.get_options().items():
             request_data[k] = (None, v)
 
         try:
             session = requests.sessions.session()
-            session.headers['X-Auth-Key'] = self._api_key
+            session.headers["X-Auth-Key"] = self._api_key
             r = session.post(url, verify=self._secure_ssl, files=request_data)
 
             if r.status_code == 200:
-                if r.headers.get('Content-Type') == "application/pdf":
+                if r.headers.get("Content-Type") == "application/pdf":
                     return JobResult(io.BytesIO(r.content), True, "")
 
         except Exception as e:
             return JobResult(None, False, str(e))
 
         return JobResult(None, False, "HTTP Code {}".format(r.status_code))
 
@@ -85,20 +87,23 @@
 
 
 class ZipReportCliProcessor(ProcessorInterface):
     """
     Local zipreport-cli report processor
     """
 
-    def __init__(self, cli_path: str):
+    def __init__(self, cli_path: str, *args):
         """
         Constructor
         :param cli_path: full path to zipreport-cli binary
         """
         self._cli = cli_path
+        if not args:
+            args = []
+        self._args = args
 
     def process(self, job: ReportJob) -> JobResult:
         """
         Execute a ReportJob by calling the zipreport-cli binary
         :param job: ReportJob
         :return: JobResult
         """
@@ -110,19 +115,24 @@
         try:
             path = Path(tempfile.mkdtemp())
             job.get_report().get_fs().get_backend().zip().extractall(path)
 
             subprocess.run(cmd, cwd=path, check=True)
             report_file = path / const.PDF_FILE_NAME
             if report_file.exists():
-                with open(report_file, 'rb') as f:
+                with open(report_file, "rb") as f:
                     report = io.BytesIO(f.read())
                     success = True
 
-        except (subprocess.CalledProcessError, FileNotFoundError, PermissionError, FileExistsError) as e:
+        except (
+            subprocess.CalledProcessError,
+            FileNotFoundError,
+            PermissionError,
+            FileExistsError,
+        ) as e:
             error = str(e)
 
         if path:
             rmtree(path)
 
         return JobResult(report, success, error)
 
@@ -132,28 +142,29 @@
         :param job: ReportJob
         :param dest_file: full path for PDF file to be generated
         :return: list
         """
         opts = job.get_options()
         args = [
             Path(self._cli),
-            '--pagesize={}'.format(opts[ReportJob.OPT_PAGE_SIZE]),
-            '--margins={}'.format(opts[ReportJob.OPT_MARGINS]),
-            '--timeout={}'.format(opts[ReportJob.OPT_RENDER_TIMEOUT]),
-            '--delay={}'.format(opts[ReportJob.OPT_SETTLING_TIME]),
+            "--pagesize={}".format(opts[ReportJob.OPT_PAGE_SIZE]),
+            "--margins={}".format(opts[ReportJob.OPT_MARGINS]),
+            "--timeout={}".format(opts[ReportJob.OPT_RENDER_TIMEOUT]),
+            "--delay={}".format(opts[ReportJob.OPT_SETTLING_TIME]),
         ]
 
         if opts[ReportJob.OPT_LANDSCAPE]:
-            args.append('--no-portrait')
+            args.append("--no-portrait")
 
         if opts[ReportJob.OPT_JS_EVENT]:
-            args.append('--js-event')
-            args.append('--js-timeout={}'.format(opts[ReportJob.OPT_JS_TIMEOUT]))
+            args.append("--js-event")
+            args.append("--js-timeout={}".format(opts[ReportJob.OPT_JS_TIMEOUT]))
 
         if opts[ReportJob.OPT_IGNORE_SSL_ERRORS]:
-            args.append('--ignore-certificate-errors')
+            args.append("--ignore-certificate-errors")
 
         if opts[ReportJob.OPT_NO_INSECURE_CONTENT]:
-            args.append('--no-insecure')
+            args.append("--no-insecure")
 
+        args.extend(self._args)
         args.extend([opts[ReportJob.OPT_MAIN_SCRIPT], dest_file])
         return args
```

### Comparing `zipreport-lib-1.0.2/zipreport/report/builder.py` & `zipreport-lib-1.1.0/zipreport/report/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 import os
 import sys
 from pathlib import Path
 from typing import Tuple, Union
 
 from zipreport.fileutils import ZipFs, FsInterface, DiskFs
 from zipreport.fileutils.backend.zip import InMemoryZip
-from zipreport.report.const import MANIFEST_FILE_NAME, ZIPREPORT_FILE_EXTENSION, INDEX_FILE_NAME, \
-    MANIFEST_REQUIRED_FIELDS
+from zipreport.report.const import (
+    MANIFEST_FILE_NAME,
+    ZIPREPORT_FILE_EXTENSION,
+    INDEX_FILE_NAME,
+    MANIFEST_REQUIRED_FIELDS,
+)
 
 
 class BuildResult:
-
     def __init__(self, error=None):
         self._err = []
         self.add_error(error)
 
     def add_error(self, error):
         if type(error) is list:
             self._err.extend(error)
@@ -32,47 +35,58 @@
 
 class ReportFileBuilder:
     """
     Report building object
     """
 
     @staticmethod
-    def build_file(path: str, output_file: str, console=sys.stdout, overwrite: bool = False) -> BuildResult:
+    def build_file(
+        path: str, output_file: str, console=sys.stdout, overwrite: bool = False
+    ) -> BuildResult:
         """
         Assemble a report file from a specific path
         :param path: report dir path
         :param output_file: destination report file
         :param console: console writer
         :param overwrite: if True, overwrite destination if exists
         :return: BuildResult
         """
         status = BuildResult()
         path = Path(path)
         output_file = Path(output_file)
         if output_file.suffix != ZIPREPORT_FILE_EXTENSION:
-            output_file = output_file.parent / (output_file.name + ZIPREPORT_FILE_EXTENSION)
+            output_file = output_file.parent / (
+                output_file.name + ZIPREPORT_FILE_EXTENSION
+            )
 
         console.write("\n== Building Report {} ==\n".format(output_file))
 
         # check paths
         if not path.exists():
             return status.add_error("Path '{}' not found".format(path))
 
         if not path.is_dir():
             return status.add_error("Path '{}' is not a directory".format(path))
 
         if output_file.exists():
             if not output_file.is_file():
                 return status.add_error(
-                    "Output file '{}' already exists and doesn't seem to be a file".format(output_file))
+                    "Output file '{}' already exists and doesn't seem to be a file".format(
+                        output_file
+                    )
+                )
             if not overwrite:
-                return status.add_error("Output file '{}' already exists".format(output_file))
+                return status.add_error(
+                    "Output file '{}' already exists".format(output_file)
+                )
         else:
             if not output_file.parent.exists():
-                return status.add_error("Invalid path for output file: '{}'".format(output_file))
+                return status.add_error(
+                    "Invalid path for output file: '{}'".format(output_file)
+                )
 
         # build ZipFs
         zfs_status, zfs = ReportFileBuilder.build_zipfs(path, console)
         if not zfs_status.success():
             return zfs_status
 
         try:
@@ -86,15 +100,17 @@
         except Exception as e:
             return status.add_error("Error saving zpt file: {}".format(e))
 
         console.write("Done!\n")
         return status
 
     @staticmethod
-    def build_zipfs(path: str, console=sys.stdout) -> Tuple[BuildResult, Union[ZipFs, None]]:
+    def build_zipfs(
+        path: str, console=sys.stdout
+    ) -> Tuple[BuildResult, Union[ZipFs, None]]:
         """
         Assemble a ZipFs structure from a specific path
         :param path: report dir path
         :param console: console writer
         :return: [BuildResult, ZipFs]
         """
         status = BuildResult()
@@ -124,18 +140,21 @@
             for f in files:
                 names.append(dirname / Path(f))
 
         for name in names:
             dest_name = name.relative_to(path)
             console.write("Copying {}...\n".format(dest_name))
             try:
-                with open(name, 'rb') as f:
+                with open(name, "rb") as f:
                     zfs.add(dest_name, f.read())
             except Exception as e:
-                return status.add_error("Error copying file {}: {}".format(name, e)), None
+                return (
+                    status.add_error("Error copying file {}: {}".format(name, e)),
+                    None,
+                )
         return status, zfs
 
     @staticmethod
     def valid_zpt(fs: FsInterface) -> Tuple[BuildResult, Union[dict, None]]:
         """
         Validates if a FsInterface is a valid report
         :param fs: FsInterface
@@ -148,22 +167,29 @@
         except Exception as e:
             return status.add_error("Error processing manifest: {}".format(e)), None
 
         if type(manifest) is not dict:
             return status.add_error("Invalid manifest format"), None
         for field, _type in MANIFEST_REQUIRED_FIELDS.items():
             if field not in manifest.keys():
-                status.add_error("Missing mandatory field '{}' in manifest file".format(field))
+                status.add_error(
+                    "Missing mandatory field '{}' in manifest file".format(field)
+                )
             else:
                 if type(manifest[field]) != _type:
-                    status.add_error("Invalid type in manifest field '{}'".format(field))
+                    status.add_error(
+                        "Invalid type in manifest field '{}'".format(field)
+                    )
 
         if not status.success():
             return status, None
 
         # check index.html
         try:
             fs.get(INDEX_FILE_NAME)
         except Exception as e:
-            return status.add_error("Index file '{}' not found".format(INDEX_FILE_NAME)), None
+            return (
+                status.add_error("Index file '{}' not found".format(INDEX_FILE_NAME)),
+                None,
+            )
 
         return status, manifest
```

### Comparing `zipreport-lib-1.0.2/zipreport/report/job.py` & `zipreport-lib-1.1.0/zipreport/report/job.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 import collections
 from copy import deepcopy
 
-from .const import *
+from .const import (
+    PDF_PAGE_A4,
+    REPORT_FILE_NAME,
+    PDF_MARGIN_DEFAULT,
+    DEFAULT_SETTLING_TIME_MS,
+    DEFAULT_RENDER_TIMEOUT_S,
+    DEFAULT_JS_TIMEOUT_S,
+    DEFAULT_PROCESS_TIMEOUT_S,
+    MANIFEST_REPORT_FILE,
+    VALID_PAGE_SIZES,
+    VALID_MARGINS
+)
 from .reportfile import ReportFile
 
 # Result type used by Processors
 # pdf:io.BytesIO; success:bool, error:str
-JobResult = collections.namedtuple('JobResult', ['report', 'success', 'error'])
+JobResult = collections.namedtuple("JobResult", ["report", "success", "error"])
 
 
 class ReportJob:
-
     # Available options
-    OPT_PAGE_SIZE = 'page_size'
-    OPT_MAIN_SCRIPT = 'script'
-    OPT_MARGINS = 'margins'
-    OPT_LANDSCAPE = 'landscape'
-    OPT_SETTLING_TIME = 'settling_time'
-    OPT_RENDER_TIMEOUT = 'timeout_render'
-    OPT_JS_TIMEOUT = 'timeout_js'
-    OPT_PROCESS_TIMEOUT = 'timeout_process'
-    OPT_JS_EVENT = 'js_event'
-    OPT_IGNORE_SSL_ERRORS = 'ignore_ssl_errors'
-    OPT_NO_INSECURE_CONTENT = 'secure_only'
+    OPT_PAGE_SIZE = "page_size"
+    OPT_MAIN_SCRIPT = "script"
+    OPT_MARGINS = "margins"
+    OPT_LANDSCAPE = "landscape"
+    OPT_SETTLING_TIME = "settling_time"
+    OPT_RENDER_TIMEOUT = "timeout_render"
+    OPT_JS_TIMEOUT = "timeout_js"
+    OPT_PROCESS_TIMEOUT = "timeout_process"
+    OPT_JS_EVENT = "js_event"
+    OPT_IGNORE_SSL_ERRORS = "ignore_ssl_errors"
+    OPT_NO_INSECURE_CONTENT = "secure_only"
 
     # option defaults
     DEFAULT_OPTIONS = {
-        OPT_PAGE_SIZE: PDF_PAGE_A4,
-        OPT_MAIN_SCRIPT: REPORT_FILE_NAME,
-        OPT_MARGINS: PDF_MARGIN_DEFAULT,
-        OPT_LANDSCAPE: False,
-        OPT_SETTLING_TIME: DEFAULT_SETTLING_TIME_MS,
-        OPT_RENDER_TIMEOUT: DEFAULT_RENDER_TIMEOUT_S,
-        OPT_JS_TIMEOUT: DEFAULT_JS_TIMEOUT_S,
-        OPT_PROCESS_TIMEOUT: DEFAULT_PROCESS_TIMEOUT_S,
-        OPT_JS_EVENT: False,
-        OPT_IGNORE_SSL_ERRORS: False,
-        OPT_NO_INSECURE_CONTENT: False,
+        "page_size": PDF_PAGE_A4,
+        "script": REPORT_FILE_NAME,
+        "margins": PDF_MARGIN_DEFAULT,
+        "landscape": False,
+        "settling_time": DEFAULT_SETTLING_TIME_MS,
+        "timeout_render": DEFAULT_RENDER_TIMEOUT_S,
+        "timeout_js": DEFAULT_JS_TIMEOUT_S,
+        "timeout_process": DEFAULT_PROCESS_TIMEOUT_S,
+        "js_event": False,
+        "ignore_ssl_errors": False,
+        "secure_only": False,
     }
 
     def __init__(self, report: ReportFile):
         """
         Constructor
         Create a new rendering job from a ReportFile
         :param report: ReportFile object to use
         """
         self._report = report
         self._options = deepcopy(self.DEFAULT_OPTIONS)
         # set optional report file name from manifest
         if report is not None:
-            self._options[self.OPT_MAIN_SCRIPT] = report.get_param(MANIFEST_REPORT_FILE, REPORT_FILE_NAME)
+            self._options[self.OPT_MAIN_SCRIPT] = report.get_param(
+                MANIFEST_REPORT_FILE, REPORT_FILE_NAME
+            )
 
     def get_options(self) -> dict:
         """
         Retrieve job options
         :return: dict
         """
         return self._options
```

### Comparing `zipreport-lib-1.0.2/zipreport/report/loader.py` & `zipreport-lib-1.1.0/zipreport/report/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 
 class ReportFileLoaderError(Exception):
     pass
 
 
 class ReportFileLoader:
-
     @staticmethod
     def load(source: str) -> ReportFile:
         """
         Load ReportFile from a source (either directory or a ZPT)
         :param source:
         :return: ReportFile
         """
@@ -34,15 +33,17 @@
         Generate ReportFile from a directory with a valid report template
         :param path: template path
         :return: ReportFile
         """
         zstatus, zfs = ReportFileBuilder.build_zipfs(path, StringIO())
         if not zstatus.success():
             error_msg = "; ".join(zstatus.get_errors())
-            raise ReportFileLoaderError("Error loading report from path '{}': '{}'".format(path, error_msg))
+            raise ReportFileLoaderError(
+                "Error loading report from path '{}': '{}'".format(path, error_msg)
+            )
         try:
             manifest = json.loads(bytes(zfs.get(MANIFEST_FILE_NAME).getbuffer()))
         except Exception as e:
             raise ReportFileLoaderError("Error: {}".format(e))
         return ReportFile(zfs, manifest)
 
     @staticmethod
@@ -70,10 +71,12 @@
         Generates a ReportFile from a ZipFs
         :param zfs: ZipFs
         :return: ReportFile
         """
         # load manifest
         status, manifest = ReportFileBuilder.valid_zpt(zfs)
         if not status.success():
-            raise ReportFileLoaderError("Error: {}".format("; ".join(status.get_errors())))
+            raise ReportFileLoaderError(
+                "Error: {}".format("; ".join(status.get_errors()))
+            )
 
         return ReportFile(zfs, manifest)
```

### Comparing `zipreport-lib-1.0.2/zipreport/report/reportfile.py` & `zipreport-lib-1.1.0/zipreport/report/reportfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 
 class ReportFileError(Exception):
     pass
 
 
 class ReportFile:
-
     def __init__(self, source: ZipFs, manifest: dict):
         if not isinstance(manifest, dict):
             raise ReportFileError("Invalid manifest format")
         if not isinstance(source, ZipFs):
             raise ReportFileError("Invalid source type")
         self._manifest = manifest
         self._fs = source
```

### Comparing `zipreport-lib-1.0.2/zipreport/template/jinja/filters.py` & `zipreport-lib-1.1.0/zipreport/template/jinja/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from jinja2 import pass_environment
 from jinja2.defaults import DEFAULT_FILTERS
 
 from zipreport.template.jinjaloader import JinjaReportLoader
 from zipreport.misc import html_tag
 
 # attribute names
-ARG_DATA = 'data'
-ATTR_SRC = 'src'
-ATTR_ALT = 'alt'
-ATTR_WIDTH = 'width'
-ATTR_HEIGHT = 'height'
-ATTR_CLASS = 'class'
+ARG_DATA = "data"
+ATTR_SRC = "src"
+ATTR_ALT = "alt"
+ATTR_WIDTH = "width"
+ATTR_HEIGHT = "height"
+ATTR_CLASS = "class"
 
 # named parameters allowed in image filters
 IMAGE_NAMED_PARAMS = [ARG_DATA, ATTR_ALT, ATTR_WIDTH, ATTR_HEIGHT, ATTR_CLASS]
 
 
 def dynamic_image(args: list, kwargs: Union[dict, None], extension: str):
     """
@@ -40,15 +40,17 @@
     generator = args[1]
     callable_generator = callable(generator)
 
     if not isinstance(loader, JinjaReportLoader):
         raise RuntimeError("Invalid environment. png() filter requires ReportLoader")
 
     if not callable_generator and not isinstance(generator, str):
-        raise RuntimeError("png() must be applied to a callable function or a placeholder string")
+        raise RuntimeError(
+            "png() must be applied to a callable function or a placeholder string"
+        )
 
     # process args and kwargs
     if kwargs is None:
         kwargs = {}
 
     img_args = {}
     ai = 2  # user arguments start in 3
@@ -64,24 +66,24 @@
     if ARG_DATA not in img_args.keys():
         img_args[ARG_DATA] = None
 
     # execute callable & save image
     zpt = loader.get_report()
     if callable_generator:
         result = generator(img_args[ARG_DATA])
-        name = Path('data') / (uuid4().hex + extension)
+        name = Path("data") / (uuid4().hex + extension)
         zpt.add(name, result)
     else:
         # if generator is string, skip image generation and use specified file
         name = generator
 
     # assemble html tag
     img_args.pop(ARG_DATA)
     img_args[ATTR_SRC] = "{}".format(name)
-    return markupsafe.Markup(html_tag('img', img_args))
+    return markupsafe.Markup(html_tag("img", img_args))
 
 
 @pass_environment
 def dynamic_png(*args, **kwargs) -> markupsafe.Markup:
     """
     Dynamic PNG img tag generator
     Can be called either via positional arguments or via named arguments, or both
@@ -91,15 +93,15 @@
 
     Named args:
         {{ callable | png(data=data_source, alt=alt_text, width=width, height=height, class=css_class= }}
 
     Mixed args:
         {{ callable | png(with=128, height=128 }}
     """
-    return dynamic_image(args, kwargs, '.png')
+    return dynamic_image(args, kwargs, ".png")
 
 
 @pass_environment
 def dynamic_gif(*args, **kwargs) -> markupsafe.Markup:
     """
     Dynamic GIF img tag generator
     Can be called either via positional arguments or via named arguments, or both
@@ -109,15 +111,15 @@
 
     Named args:
         {{ callable | gif(data=data_source, alt=alt_text, width=width, height=height, class=css_class= }}
 
     Mixed args:
         {{ callable | gif(with=128, height=128 }}
     """
-    return dynamic_image(args, kwargs, '.gif')
+    return dynamic_image(args, kwargs, ".gif")
 
 
 @pass_environment
 def dynamic_jpg(*args, **kwargs) -> markupsafe.Markup:
     """
     Dynamic JPG img tag generator
     Can be called either via positional arguments or via named arguments, or both
@@ -127,15 +129,15 @@
 
     Named args:
         {{ callable | jpg(data=data_source, alt=alt_text, width=width, height=height, class=css_class= }}
 
     Mixed args:
         {{ callable | jpg(with=128, height=128 }}
     """
-    return dynamic_image(args, kwargs, '.jpg')
+    return dynamic_image(args, kwargs, ".jpg")
 
 
 @pass_environment
 def dynamic_svg(*args, **kwargs) -> markupsafe.Markup:
     """
     Dynamic SVG img tag generator
     Can be called either via positional arguments or via named arguments, or both
@@ -145,25 +147,27 @@
 
     Named args:
         {{ callable | svg(data=data_source, alt=alt_text, width=width, height=height, class=css_class= }}
 
     Mixed args:
         {{ callable | svg(with=128, height=128 }}
     """
-    return dynamic_image(args, kwargs, '.svg')
+    return dynamic_image(args, kwargs, ".svg")
 
 
 def do_json(*args) -> markupsafe.Markup:
     if len(*args) != 1:
-        raise RuntimeError("Invalid number of arguments. json filter requires a variable")
+        raise RuntimeError(
+            "Invalid number of arguments. json filter requires a variable"
+        )
     try:
         return markupsafe.Markup(json.dumps(args[0]))
     except ValueError:
         raise
 
 
 # Register filters
-DEFAULT_FILTERS['png'] = dynamic_png
-DEFAULT_FILTERS['gif'] = dynamic_gif
-DEFAULT_FILTERS['jpg'] = dynamic_jpg
-DEFAULT_FILTERS['svg'] = dynamic_svg
-DEFAULT_FILTERS['json'] = do_json
+DEFAULT_FILTERS["png"] = dynamic_png
+DEFAULT_FILTERS["gif"] = dynamic_gif
+DEFAULT_FILTERS["jpg"] = dynamic_jpg
+DEFAULT_FILTERS["svg"] = dynamic_svg
+DEFAULT_FILTERS["json"] = do_json
```

### Comparing `zipreport-lib-1.0.2/zipreport/template/jinjaloader.py` & `zipreport-lib-1.1.0/zipreport/template/jinjaloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import io
 
 from jinja2 import BaseLoader, TemplateNotFound
 from zipreport.report import ReportFile
 
 
 class JinjaReportLoader(BaseLoader):
-
     def __init__(self, zpt: ReportFile):
         self.zpt = zpt
 
     def get_source(self, environment, template):
         def updated():
             return True
 
         if not self.zpt.exists(template):
             raise TemplateNotFound(template)
-        source = io.TextIOWrapper(self.zpt.get(template), encoding='utf-8').read()
+        source = io.TextIOWrapper(self.zpt.get(template), encoding="utf-8").read()
         return source, template, updated
 
     def get_report(self):
         """
         Retrieve Report Object
         :return: ReportFile
         """
```

### Comparing `zipreport-lib-1.0.2/zipreport/template/jinjarender.py` & `zipreport-lib-1.1.0/zipreport/template/jinjarender.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import json
 from copy import deepcopy
 
 from jinja2 import select_autoescape, Environment
 
 from zipreport.template.jinjaloader import JinjaReportLoader
 from zipreport.report import ReportFile
-from zipreport.report.const import INDEX_FILE_NAME, MANIFEST_PARAMETERS, REPORT_FILE_NAME, DATA_FILE_NAME
+from zipreport.report.const import (
+    INDEX_FILE_NAME,
+    MANIFEST_PARAMETERS,
+    REPORT_FILE_NAME,
+    DATA_FILE_NAME,
+)
+
 # register filters
 from zipreport.template.jinja import filters
 
 
 class JinjaRender:
-    OPT_EXTENSIONS = 'extensions'
-    OPT_STRICT_PARAMS = 'strict_params'
+    OPT_EXTENSIONS = "extensions"
+    OPT_STRICT_PARAMS = "strict_params"
 
     DEFAULT_OPTIONS = {
         OPT_EXTENSIONS: [],
         OPT_STRICT_PARAMS: True,
     }
 
     def __init__(self, zpt: ReportFile, options: dict = None):
@@ -36,16 +42,16 @@
         """
         Build jinja environment
 
         :return:  Environment
         """
         return Environment(
             loader=JinjaReportLoader(self.zpt),
-            autoescape=select_autoescape(['html', 'xml']),
-            extensions=self.options[self.OPT_EXTENSIONS]
+            autoescape=select_autoescape(["html", "xml"]),
+            extensions=self.options[self.OPT_EXTENSIONS],
         )
 
     def check_params(self, data: dict):
         """
         Check that all parameters specified on the manifest file exist, if strict params enabled
 
         :param data: data to validate
@@ -53,18 +59,24 @@
         """
         if not self.options[self.OPT_STRICT_PARAMS]:
             return
 
         expected = self.zpt.get_param(MANIFEST_PARAMETERS)
         for param in expected:
             if param not in data.keys():
-                raise RuntimeError("Parameter '{}' missing on render() call".format(param))
-
-    def render(self, data: dict = None, template: str = INDEX_FILE_NAME,
-               default_data_file: str = DATA_FILE_NAME) -> str:
+                raise RuntimeError(
+                    "Parameter '{}' missing on render() call".format(param)
+                )
+
+    def render(
+        self,
+        data: dict = None,
+        template: str = INDEX_FILE_NAME,
+        default_data_file: str = DATA_FILE_NAME,
+    ) -> str:
         """
         Render the template into REPORT_FILE_NAME, inside the ReportFile
 
         if data is None, render() will try to load a default json data file to use as data to be passed to the view
         Keep in mind, zipreport dynamic filters can't be used as default data
 
         :param data: data to be passed to the template
```

### Comparing `zipreport-lib-1.0.2/zipreport/zipreport.py` & `zipreport-lib-1.1.0/zipreport/zipreport.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from zipreport.processors.interface import ProcessorInterface
-from zipreport.processors import ZipReportProcessor, ZipReportClient, ZipReportCliProcessor, MIMEProcessor, \
-    WkHtml2PdfProcessor
+from zipreport.processors import (
+    ZipReportProcessor,
+    ZipReportClient,
+    ZipReportCliProcessor,
+    MIMEProcessor,
+    WkHtml2PdfProcessor,
+)
 from zipreport.report import ReportFile
 from zipreport.report.job import ReportJob, JobResult
 from zipreport.template import JinjaRender
 
 
 class BaseReport:
     """
@@ -51,36 +56,41 @@
 
 
 class ZipReport(BaseReport):
     """
     zipreport-server API based report generation
     """
 
-    def __init__(self, url: str, api_key: str, api_version: int = 1, secure_ssl: bool = False):
+    def __init__(
+        self, url: str, api_key: str, api_version: int = 1, secure_ssl: bool = False
+    ):
         """
         Constructor
         :param url: zipreport-server url
         :param api_key: zipreport-server api key
         :param api_version: api version (default 1)
         :param secure_ssl: if true, verifies CA validity for SSL certificates (default false)
         """
-        super(ZipReport, self).__init__(ZipReportProcessor(ZipReportClient(url, api_key, api_version, secure_ssl)))
+        super(ZipReport, self).__init__(
+            ZipReportProcessor(ZipReportClient(url, api_key, api_version, secure_ssl))
+        )
 
 
 class ZipReportCli(BaseReport):
     """
     zipreport-cli local report generation
     """
 
-    def __init__(self, cli_path: str):
+    def __init__(self, cli_path: str, *args):
         """
         Constructor
         :param cli_path: full path to zipreport-cli binary
+        :param *args: optional arguments to pass to the cli processor
         """
-        super(ZipReportCli, self).__init__(ZipReportCliProcessor(cli_path))
+        super(ZipReportCli, self).__init__(ZipReportCliProcessor(cli_path, *args))
 
 
 class WkHtml2PdfReport(BaseReport):
     """
     wkhtmltopdf report generation
     """
```

### Comparing `zipreport-lib-1.0.2/zipreport_lib.egg-info/PKG-INFO` & `zipreport-lib-1.1.0/zipreport_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: Joao Pinheiro
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
```

### Comparing `zipreport-lib-1.0.2/zipreport_lib.egg-info/SOURCES.txt` & `zipreport-lib-1.1.0/zipreport_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

