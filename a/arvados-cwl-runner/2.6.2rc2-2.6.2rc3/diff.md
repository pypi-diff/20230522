# Comparing `tmp/arvados-cwl-runner-2.6.2rc2.tar.gz` & `tmp/arvados-cwl-runner-2.6.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.2rc2.tar", last modified: Fri Apr 21 19:29:36 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.2rc3.tar", last modified: Mon May  1 21:20:06 2023, max compression
```

## Comparing `arvados-cwl-runner-2.6.2rc2.tar` & `arvados-cwl-runner-2.6.2rc3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    20122 2023-04-21 19:29:20.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.0.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.1.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.2.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35160 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvcontainer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvtool.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31804 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvworkflow.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/context.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3986 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/done.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44521 2023-04-21 19:29:20.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/executor.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17991 2023-04-21 19:29:20.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/perf.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39024 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/runner.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1353 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl/util.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      177 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/bin/arvados-cwl-runner
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/bin/cwl-runner
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2072 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:36.000000 arvados-cwl-runner-2.6.2rc2/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/hw.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/matcher.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/mock_discovery.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_container.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_copy_deps.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_make_output.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_set_output_prop.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_submit.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_tq.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_urljoin.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2058 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.2rc2/tests/test_util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    20122 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.0.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.1.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.2.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35160 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvcontainer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvtool.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31521 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvworkflow.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/context.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3986 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/done.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44529 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/executor.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17991 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/perf.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39024 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/runner.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1810 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      177 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/bin/arvados-cwl-runner
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/bin/cwl-runner
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2073 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/hw.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/matcher.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/mock_discovery.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_container.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_copy_deps.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_make_output.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_set_output_prop.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_submit.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_tq.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_urljoin.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3439 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_util.py
```

### Comparing `arvados-cwl-runner-2.6.2rc2/LICENSE-2.0.txt` & `arvados-cwl-runner-2.6.2rc3/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/PKG-INFO` & `arvados-cwl-runner-2.6.2rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.2rc2
+Version: 2.6.2rc3
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/__init__.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.0.yml` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.0.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.1.yml` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.1.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arv-cwl-schema-v1.2.yml` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.2.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvcontainer.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvcontainer.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvdocker.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvtool.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvtool.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/arvworkflow.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvworkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 from .runner import (upload_dependencies, packed_workflow, upload_workflow_collection,
                      trim_anonymous_location, remove_redundant_fields, discover_secondary_files,
                      make_builder, arvados_jobs_image, FileUpdates)
 from .pathmapper import ArvPathMapper, trim_listing
 from .arvtool import ArvadosCommandTool, set_cluster_target
 from ._version import __version__
+from .util import common_prefix
 
 from .perf import Perf
 
 logger = logging.getLogger('arvados.cwl-runner')
 metrics = logging.getLogger('arvados.cwl-runner.metrics')
 
 max_res_pars = ("coresMin", "coresMax", "ramMin", "ramMax", "tmpdirMin", "tmpdirMax")
@@ -231,14 +232,15 @@
         rel = rel_ref(r, baseuri, urlexpander, merged_map, jobmapper)
         merged_map.setdefault(path, FileUpdates({}, {}))
         rename = "keep:%s/%s" %(pdh, rel)
         for mm in merged_map:
             merged_map[mm].resolved[r] = rename
     return req
 
+
 def drop_ids(d):
     if isinstance(d, MutableSequence):
         for i, s in enumerate(d):
             drop_ids(s)
     elif isinstance(d, MutableMapping):
         if "id" in d and d["id"].startswith("file:"):
             del d["id"]
@@ -276,30 +278,15 @@
             include_files.add(urllib.parse.urldefrag(w[8:])[0])
 
     all_files = workflow_files | import_files | include_files
 
     # Find the longest common prefix among all the file names.  We'll
     # use this to recreate the directory structure in a keep
     # collection with correct relative references.
-    n = 7
-    allmatch = True
-    if firstfile:
-        while allmatch:
-            n += 1
-            for f in all_files:
-                if len(f)-1 < n:
-                    n -= 1
-                    allmatch = False
-                    break
-                if f[n] != firstfile[n]:
-                    allmatch = False
-                    break
-
-        while firstfile[n] != "/":
-            n -= 1
+    prefix = common_prefix(firstfile, all_files)
 
     col = arvados.collection.Collection(api_client=arvRunner.api)
 
     # Now go through all the files and update references to other
     # files.  We previously scanned for file dependencies, these are
     # are passed in as merged_map.
     #
@@ -328,44 +315,44 @@
         export_as_json = result.fa.flow_style()
 
         # 2. find $import, $include, $schema, run, location
         # 3. update field value
         update_refs(result, w, tool.doc_loader.expand_url, merged_map, jobmapper, runtimeContext, "", "")
 
         # Write the updated file to the collection.
-        with col.open(w[n+1:], "wt") as f:
+        with col.open(w[len(prefix):], "wt") as f:
             if export_as_json:
                 json.dump(result, f, indent=4, separators=(',',': '))
             else:
                 yamlloader.dump(result, stream=f)
 
         # Also store a verbatim copy of the original files
-        with col.open(os.path.join("original", w[n+1:]), "wt") as f:
+        with col.open(os.path.join("original", w[len(prefix):]), "wt") as f:
             f.write(text)
 
 
     # Upload files referenced by $include directives, these are used
     # unchanged and don't need to be updated.
     for w in include_files:
-        with col.open(w[n+1:], "wb") as f1:
-            with col.open(os.path.join("original", w[n+1:]), "wb") as f3:
+        with col.open(w[len(prefix):], "wb") as f1:
+            with col.open(os.path.join("original", w[len(prefix):]), "wb") as f3:
                 with open(uri_file_path(w), "rb") as f2:
                     dat = f2.read(65536)
                     while dat:
                         f1.write(dat)
                         f3.write(dat)
                         dat = f2.read(65536)
 
     # Now collect metadata: the collection name and git properties.
 
     toolname = tool.tool.get("label") or tool.metadata.get("label") or os.path.basename(tool.tool["id"])
     if git_info and git_info.get("http://arvados.org/cwl#gitDescribe"):
         toolname = "%s (%s)" % (toolname, git_info.get("http://arvados.org/cwl#gitDescribe"))
 
-    toolfile = tool.tool["id"][n+1:]
+    toolfile = tool.tool["id"][len(prefix):]
 
     properties = {
         "type": "workflow",
         "arv:workflowMain": toolfile,
     }
 
     if git_info:
```

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/context.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/context.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/done.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/done.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/executor.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,15 @@
                 pageSize = self.poll_api._rootDesc.get('maxItemsPerResponse', 1000)
 
                 while keys:
                     page = keys[:pageSize]
                     try:
                         proc_states = table.list(filters=[["uuid", "in", page]]).execute(num_retries=self.num_retries)
                     except Exception as e:
-                        logger.exception("Error checking states on API server: %s", e)
+                        logger.warning("Temporary error checking states on API server: %s", e)
                         remain_wait = self.poll_interval
                         continue
 
                     for p in proc_states["items"]:
                         self.on_message({
                             "object_uuid": p["uuid"],
                             "event_type": "update",
```

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/fsaccess.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/pathmapper.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/perf.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/perf.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl/runner.py` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl/runner.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/PKG-INFO` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.2rc2
+Version: 2.6.2rc3
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_cwl_runner.egg-info/SOURCES.txt` & `arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/arvados_version.py` & `arvados-cwl-runner-2.6.2rc3/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/setup.py` & `arvados-cwl-runner-2.6.2rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
           'cwltool==3.1.20230127121939',
           'schema-salad==8.4.20230127112827',
           'arvados-python-client{}'.format(pysdk_dep),
           'ciso8601 >= 2.0.0',
           'networkx < 2.6',
           'msgpack==1.0.3',
           'importlib-metadata<5',
-          'setuptools>=40.3.0'
+          'setuptools>=40.3.0',
       ],
       data_files=[
           ('share/doc/arvados-cwl-runner', ['LICENSE-2.0.txt', 'README.rst']),
       ],
       python_requires=">=3.5, <4",
       classifiers=[
           'Programming Language :: Python :: 3',
```

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/matcher.py` & `arvados-cwl-runner-2.6.2rc3/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/test_container.py` & `arvados-cwl-runner-2.6.2rc3/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/test_copy_deps.py` & `arvados-cwl-runner-2.6.2rc3/tests/test_copy_deps.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/test_fsaccess.py` & `arvados-cwl-runner-2.6.2rc3/tests/test_fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/test_make_output.py` & `arvados-cwl-runner-2.6.2rc3/tests/test_make_output.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/test_pathmapper.py` & `arvados-cwl-runner-2.6.2rc3/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/test_set_output_prop.py` & `arvados-cwl-runner-2.6.2rc3/tests/test_set_output_prop.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/test_submit.py` & `arvados-cwl-runner-2.6.2rc3/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/test_tq.py` & `arvados-cwl-runner-2.6.2rc3/tests/test_tq.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc2/tests/test_urljoin.py` & `arvados-cwl-runner-2.6.2rc3/tests/test_urljoin.py`

 * *Files identical despite different names*

