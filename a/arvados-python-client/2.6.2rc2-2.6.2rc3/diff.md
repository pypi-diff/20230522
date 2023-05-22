# Comparing `tmp/arvados-python-client-2.6.2rc2.tar.gz` & `tmp/arvados-python-client-2.6.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-python-client-2.6.2rc2.tar", last modified: Fri Apr 21 19:29:28 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-python-client-2.6.2rc3.tar", last modified: Mon May  1 21:19:59 2023, max compression
```

## Comparing `arvados-python-client-2.6.2rc2.tar` & `arvados-python-client-2.6.2rc3.tar`

### file list

```diff
@@ -1,98 +1,96 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      230 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2088 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6450 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2329 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/_normalize_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3492 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/arvados/_pycurlhelper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/_ranges.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-04-21 19:29:27.000000 arvados-python-client-2.6.2rc2/arvados/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17005 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    49239 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    76777 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/collection.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados/commands/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2125 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/_util.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    31921 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/arv_copy.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18701 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/federation_migrate.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13261 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23760 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3357 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11841 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/migrate19.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57541 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/run.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4765 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1629 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/config.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      896 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9017 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/diskcache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12489 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/arvados/http_to_keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    61059 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/arvados/keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8472 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2635 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3750 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/timer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19413 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/vocabulary.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)   370019 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/arvados-v1-discovery.json
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2077 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      278 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-copy
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-federation-migrate
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-get
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-keepdocker
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-ls
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-migrate-docker19
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-normalize
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-put
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-ws
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    12910 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/discovery2pydoc.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4676 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10182 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/arvados_testutil.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/keepstub.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/manifest_examples.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/tests/performance/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/performance/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/performance/performance_profiler.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/performance/test_a_sample.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    38152 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/run_test_server.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/slow_test.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18619 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_copy.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8686 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10021 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_normalize.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43464 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_benchmark_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77435 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18037 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/tests/test_http.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    82578 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_keep_client.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_keep_locator.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2425 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_retry_job_helpers.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_sdk.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11619 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7865 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_vocabulary.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2088 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6450 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2329 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/_normalize_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3492 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/_pycurlhelper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/_ranges.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17005 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    49239 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    76777 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/collection.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados/commands/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2125 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/_util.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    31921 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/arv_copy.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18701 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/federation_migrate.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13261 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23760 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3357 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11841 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/migrate19.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57541 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/run.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4765 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/commands/ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1629 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/config.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      896 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9017 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/diskcache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12489 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/http_to_keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    61777 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8472 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2635 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3750 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/timer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19413 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados/vocabulary.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2032 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      343 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-copy
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-federation-migrate
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-get
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-keepdocker
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-ls
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-migrate-docker19
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-normalize
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-put
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/bin/arv-ws
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2141 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10182 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/arvados_testutil.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/keepstub.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/manifest_examples.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:59.000000 arvados-python-client-2.6.2rc3/tests/performance/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/performance/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/performance/performance_profiler.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/performance/test_a_sample.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    38152 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/run_test_server.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/slow_test.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18619 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_copy.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8686 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10021 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_normalize.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2023-05-01 21:19:49.000000 arvados-python-client-2.6.2rc3/tests/test_arv_ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43464 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_benchmark_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77435 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18037 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_http.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    82578 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_keep_client.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_keep_locator.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2425 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_retry_job_helpers.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_sdk.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11619 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7865 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2023-05-01 21:19:50.000000 arvados-python-client-2.6.2rc3/tests/test_vocabulary.py
```

### Comparing `arvados-python-client-2.6.2rc2/LICENSE-2.0.txt` & `arvados-python-client-2.6.2rc3/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/PKG-INFO` & `arvados-python-client-2.6.2rc3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.6.2rc2
+Version: 2.6.2rc3
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.6.2rc2/README.rst` & `arvados-python-client-2.6.2rc3/README.rst`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/__init__.py` & `arvados-python-client-2.6.2rc3/arvados/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/_normalize_stream.py` & `arvados-python-client-2.6.2rc3/arvados/_normalize_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/_pycurlhelper.py` & `arvados-python-client-2.6.2rc3/arvados/_pycurlhelper.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/_ranges.py` & `arvados-python-client-2.6.2rc3/arvados/_ranges.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/api.py` & `arvados-python-client-2.6.2rc3/arvados/api.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/arvfile.py` & `arvados-python-client-2.6.2rc3/arvados/arvfile.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/cache.py` & `arvados-python-client-2.6.2rc3/arvados/cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/collection.py` & `arvados-python-client-2.6.2rc3/arvados/collection.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/_util.py` & `arvados-python-client-2.6.2rc3/arvados/commands/_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/arv_copy.py` & `arvados-python-client-2.6.2rc3/arvados/commands/arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/federation_migrate.py` & `arvados-python-client-2.6.2rc3/arvados/commands/federation_migrate.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/get.py` & `arvados-python-client-2.6.2rc3/arvados/commands/get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/keepdocker.py` & `arvados-python-client-2.6.2rc3/arvados/commands/keepdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/ls.py` & `arvados-python-client-2.6.2rc3/arvados/commands/ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/migrate19.py` & `arvados-python-client-2.6.2rc3/arvados/commands/migrate19.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/put.py` & `arvados-python-client-2.6.2rc3/arvados/commands/put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/run.py` & `arvados-python-client-2.6.2rc3/arvados/commands/run.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/commands/ws.py` & `arvados-python-client-2.6.2rc3/arvados/commands/ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/config.py` & `arvados-python-client-2.6.2rc3/arvados/config.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/crunch.py` & `arvados-python-client-2.6.2rc3/arvados/crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/diskcache.py` & `arvados-python-client-2.6.2rc3/arvados/diskcache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/errors.py` & `arvados-python-client-2.6.2rc3/arvados/errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/events.py` & `arvados-python-client-2.6.2rc3/arvados/events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/http_to_keep.py` & `arvados-python-client-2.6.2rc3/arvados/http_to_keep.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/keep.py` & `arvados-python-client-2.6.2rc3/arvados/keep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1170,29 +1170,45 @@
         headers['X-Request-Id'] = request_id
 
         slot = None
         blob = None
         try:
             locator = KeepLocator(loc_s)
             if method == "GET":
-                slot, first = self.block_cache.reserve_cache(locator.md5sum)
-                if not first:
+                while slot is None:
+                    slot, first = self.block_cache.reserve_cache(locator.md5sum)
+                    if first:
+                        # Fresh and empty "first time it is used" slot
+                        break
                     if prefetch:
-                        # this is request for a prefetch, if it is
-                        # already in flight, return immediately.
-                        # clear 'slot' to prevent finally block from
-                        # calling slot.set()
+                        # this is request for a prefetch to fill in
+                        # the cache, don't need to wait for the
+                        # result, so if it is already in flight return
+                        # immediately.  Clear 'slot' to prevent
+                        # finally block from calling slot.set()
                         slot = None
                         return None
-                    self.hits_counter.add(1)
+
                     blob = slot.get()
-                    if blob is None:
-                        raise arvados.errors.KeepReadError(
-                            "failed to read {}".format(loc_s))
-                    return blob
+                    if blob is not None:
+                        self.hits_counter.add(1)
+                        return blob
+
+                    # If blob is None, this means either
+                    #
+                    # (a) another thread was fetching this block and
+                    # failed with an error or
+                    #
+                    # (b) cache thrashing caused the slot to be
+                    # evicted (content set to None) by another thread
+                    # between the call to reserve_cache() and get().
+                    #
+                    # We'll handle these cases by reserving a new slot
+                    # and then doing a full GET request.
+                    slot = None
 
             self.misses_counter.add(1)
 
             # If the locator has hints specifying a prefix (indicating a
             # remote keepproxy) or the UUID of a local gateway service,
             # read data from the indicated service(s) instead of the usual
             # list of local disk services.
```

### Comparing `arvados-python-client-2.6.2rc2/arvados/retry.py` & `arvados-python-client-2.6.2rc3/arvados/retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/safeapi.py` & `arvados-python-client-2.6.2rc3/arvados/safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/stream.py` & `arvados-python-client-2.6.2rc3/arvados/stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/timer.py` & `arvados-python-client-2.6.2rc3/arvados/timer.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/util.py` & `arvados-python-client-2.6.2rc3/arvados/util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados/vocabulary.py` & `arvados-python-client-2.6.2rc3/arvados/vocabulary.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/PKG-INFO` & `arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.6.2rc2
+Version: 2.6.2rc3
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/SOURCES.txt` & `arvados-python-client-2.6.2rc3/arvados_python_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE-2.0.txt
 MANIFEST.in
 README.rst
-arvados-v1-discovery.json
 arvados_version.py
-discovery2pydoc.py
 setup.py
 arvados/__init__.py
 arvados/_normalize_stream.py
 arvados/_pycurlhelper.py
 arvados/_ranges.py
 arvados/_version.py
 arvados/api.py
```

### Comparing `arvados-python-client-2.6.2rc2/arvados_version.py` & `arvados-python-client-2.6.2rc3/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/bin/arv-normalize` & `arvados-python-client-2.6.2rc3/bin/arv-normalize`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/arvados_testutil.py` & `arvados-python-client-2.6.2rc3/tests/arvados_testutil.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/keepstub.py` & `arvados-python-client-2.6.2rc3/tests/keepstub.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/manifest_examples.py` & `arvados-python-client-2.6.2rc3/tests/manifest_examples.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/performance/performance_profiler.py` & `arvados-python-client-2.6.2rc3/tests/performance/performance_profiler.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/run_test_server.py` & `arvados-python-client-2.6.2rc3/tests/run_test_server.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_api.py` & `arvados-python-client-2.6.2rc3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_arv_copy.py` & `arvados-python-client-2.6.2rc3/tests/test_arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_arv_get.py` & `arvados-python-client-2.6.2rc3/tests/test_arv_get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_arv_keepdocker.py` & `arvados-python-client-2.6.2rc3/tests/test_arv_keepdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_arv_ls.py` & `arvados-python-client-2.6.2rc3/tests/test_arv_ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_arv_normalize.py` & `arvados-python-client-2.6.2rc3/tests/test_arv_normalize.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_arv_put.py` & `arvados-python-client-2.6.2rc3/tests/test_arv_put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_arv_ws.py` & `arvados-python-client-2.6.2rc3/tests/test_arv_ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_arvfile.py` & `arvados-python-client-2.6.2rc3/tests/test_arvfile.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_benchmark_collections.py` & `arvados-python-client-2.6.2rc3/tests/test_benchmark_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_cache.py` & `arvados-python-client-2.6.2rc3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_collections.py` & `arvados-python-client-2.6.2rc3/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_crunch.py` & `arvados-python-client-2.6.2rc3/tests/test_crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_errors.py` & `arvados-python-client-2.6.2rc3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_events.py` & `arvados-python-client-2.6.2rc3/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_http.py` & `arvados-python-client-2.6.2rc3/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_keep_client.py` & `arvados-python-client-2.6.2rc3/tests/test_keep_client.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_keep_locator.py` & `arvados-python-client-2.6.2rc3/tests/test_keep_locator.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_retry.py` & `arvados-python-client-2.6.2rc3/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_retry_job_helpers.py` & `arvados-python-client-2.6.2rc3/tests/test_retry_job_helpers.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_safeapi.py` & `arvados-python-client-2.6.2rc3/tests/test_safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_sdk.py` & `arvados-python-client-2.6.2rc3/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_stream.py` & `arvados-python-client-2.6.2rc3/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_util.py` & `arvados-python-client-2.6.2rc3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.2rc2/tests/test_vocabulary.py` & `arvados-python-client-2.6.2rc3/tests/test_vocabulary.py`

 * *Files identical despite different names*

