# Comparing `tmp/paramsurvey-0.4.8.tar.gz` & `tmp/paramsurvey-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paramsurvey-0.4.8.tar", last modified: Sun Nov 22 16:28:01 2020, max compression
+gzip compressed data, was "dist/paramsurvey-0.4.9.tar", last modified: Mon Dec  7 21:16:42 2020, max compression
```

## Comparing `paramsurvey-0.4.8.tar` & `paramsurvey-0.4.9.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-11-22 16:28:01.111251 paramsurvey-0.4.8/
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      185 2020-07-19 02:11:21.000000 paramsurvey-0.4.8/.editorconfig
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       29 2020-07-19 02:11:52.000000 paramsurvey-0.4.8/.flake8
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       57 2020-07-22 05:52:33.000000 paramsurvey-0.4.8/.gitignore
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     2077 2020-11-10 20:14:28.000000 paramsurvey-0.4.8/.travis.yml
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      409 2020-11-22 05:06:33.000000 paramsurvey-0.4.8/CHANGELOG.md
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)    11355 2020-07-19 20:01:03.000000 paramsurvey-0.4.8/LICENSE
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1566 2020-09-10 18:39:24.000000 paramsurvey-0.4.8/Makefile
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     7542 2020-11-22 16:28:01.111251 paramsurvey-0.4.8/PKG-INFO
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     5499 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/README.md
-drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-11-22 16:28:01.108251 paramsurvey-0.4.8/paramsurvey/
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     6429 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/paramsurvey/__init__.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      414 2020-09-07 22:21:59.000000 paramsurvey-0.4.8/paramsurvey/examples.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     2814 2020-08-16 01:01:06.000000 paramsurvey-0.4.8/paramsurvey/params.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     2503 2020-09-07 22:21:59.000000 paramsurvey-0.4.8/paramsurvey/pslogger.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      301 2020-07-19 20:00:58.000000 paramsurvey-0.4.8/paramsurvey/psmpi.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     7602 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/paramsurvey/psmultiprocessing.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     9921 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/paramsurvey/psray.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     4716 2020-09-08 02:27:33.000000 paramsurvey-0.4.8/paramsurvey/stats.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)    14404 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/paramsurvey/utils.py
-drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-11-22 16:28:01.108251 paramsurvey-0.4.8/paramsurvey.egg-info/
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     7542 2020-11-22 16:28:00.000000 paramsurvey-0.4.8/paramsurvey.egg-info/PKG-INFO
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1118 2020-11-22 16:28:01.000000 paramsurvey-0.4.8/paramsurvey.egg-info/SOURCES.txt
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)        1 2020-11-22 16:28:01.000000 paramsurvey-0.4.8/paramsurvey.egg-info/dependency_links.txt
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      157 2020-11-22 16:28:01.000000 paramsurvey-0.4.8/paramsurvey.egg-info/requires.txt
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       12 2020-11-22 16:28:01.000000 paramsurvey-0.4.8/paramsurvey.egg-info/top_level.txt
-drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-11-22 16:28:01.109252 paramsurvey-0.4.8/scripts/
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1609 2020-09-07 22:21:59.000000 paramsurvey-0.4.8/scripts/paramsurvey-greedy-example.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      991 2020-09-07 22:21:59.000000 paramsurvey-0.4.8/scripts/paramsurvey-multistage-example.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      823 2020-09-07 22:21:59.000000 paramsurvey-0.4.8/scripts/paramsurvey-readme-example.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       38 2020-11-22 16:28:01.111251 paramsurvey-0.4.8/setup.cfg
--rwxrwxr-x   0 lindahl   (2020) lindahl   (2020)     2118 2020-11-10 20:37:12.000000 paramsurvey-0.4.8/setup.py
-drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-11-22 16:28:01.105251 paramsurvey-0.4.8/test/
-drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-11-22 16:28:01.109252 paramsurvey-0.4.8/test/__pycache__/
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     8347 2020-07-18 21:34:50.000000 paramsurvey-0.4.8/test/__pycache__/test_psmultiprocessing.cpython-36-pytest-5.3.2.pyc
-drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-11-22 16:28:01.110252 paramsurvey-0.4.8/test/integration/
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1113 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/test/integration/test-env-overrides.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      741 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/test/integration/test-generic_init_max_tasks_per_child.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      855 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/test/integration/test-multiprocessing-failure.py
--rwxrwxr-x   0 lindahl   (2020) lindahl   (2020)      535 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/test/integration/test-multiprocessing.sh
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       91 2020-08-16 01:51:19.000000 paramsurvey-0.4.8/test/integration/test-only-builtins.py
--rwxrwxr-x   0 lindahl   (2020) lindahl   (2020)     1112 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/test/integration/test-ray.sh
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)    10534 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/test/integration/test_generic.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1200 2020-09-08 02:19:28.000000 paramsurvey-0.4.8/test/integration/test_stress.py
-drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-11-22 16:28:01.111251 paramsurvey-0.4.8/test/unit/
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1149 2020-11-22 05:05:42.000000 paramsurvey-0.4.8/test/unit/test_multiprocessing.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     5482 2020-11-03 04:43:22.000000 paramsurvey-0.4.8/test/unit/test_params.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      457 2020-08-22 01:31:33.000000 paramsurvey-0.4.8/test/unit/test_pslogger.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     2576 2020-08-22 04:20:53.000000 paramsurvey-0.4.8/test/unit/test_stats.py
--rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     4868 2020-11-21 17:51:47.000000 paramsurvey-0.4.8/test/unit/test_utils.py
+drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-12-07 21:16:42.504603 paramsurvey-0.4.9/
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      185 2020-07-19 02:11:21.000000 paramsurvey-0.4.9/.editorconfig
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       29 2020-07-19 02:11:52.000000 paramsurvey-0.4.9/.flake8
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       57 2020-07-22 05:52:33.000000 paramsurvey-0.4.9/.gitignore
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     2077 2020-11-10 20:14:28.000000 paramsurvey-0.4.9/.travis.yml
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      543 2020-12-07 20:35:57.000000 paramsurvey-0.4.9/CHANGELOG.md
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)    11355 2020-07-19 20:01:03.000000 paramsurvey-0.4.9/LICENSE
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1569 2020-11-26 01:06:28.000000 paramsurvey-0.4.9/Makefile
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     7972 2020-12-07 21:16:42.504603 paramsurvey-0.4.9/PKG-INFO
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     5857 2020-12-07 16:15:40.000000 paramsurvey-0.4.9/README.md
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     2448 2020-12-06 03:56:55.000000 paramsurvey-0.4.9/azure-pipelines.yml
+drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-12-07 21:16:42.500603 paramsurvey-0.4.9/paramsurvey/
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     6508 2020-12-07 14:58:35.000000 paramsurvey-0.4.9/paramsurvey/__init__.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      414 2020-09-07 22:21:59.000000 paramsurvey-0.4.9/paramsurvey/examples.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     2814 2020-08-16 01:01:06.000000 paramsurvey-0.4.9/paramsurvey/params.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     2664 2020-12-06 07:09:14.000000 paramsurvey-0.4.9/paramsurvey/pslogger.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      301 2020-07-19 20:00:58.000000 paramsurvey-0.4.9/paramsurvey/psmpi.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     7739 2020-12-07 20:10:10.000000 paramsurvey-0.4.9/paramsurvey/psmultiprocessing.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     9962 2020-12-07 20:10:10.000000 paramsurvey-0.4.9/paramsurvey/psray.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     4716 2020-09-08 02:27:33.000000 paramsurvey-0.4.9/paramsurvey/stats.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)    14321 2020-12-07 16:32:16.000000 paramsurvey-0.4.9/paramsurvey/utils.py
+drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-12-07 21:16:42.501603 paramsurvey-0.4.9/paramsurvey.egg-info/
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     7972 2020-12-07 21:16:42.000000 paramsurvey-0.4.9/paramsurvey.egg-info/PKG-INFO
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1138 2020-12-07 21:16:42.000000 paramsurvey-0.4.9/paramsurvey.egg-info/SOURCES.txt
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)        1 2020-12-07 21:16:42.000000 paramsurvey-0.4.9/paramsurvey.egg-info/dependency_links.txt
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      157 2020-12-07 21:16:42.000000 paramsurvey-0.4.9/paramsurvey.egg-info/requires.txt
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       12 2020-12-07 21:16:42.000000 paramsurvey-0.4.9/paramsurvey.egg-info/top_level.txt
+drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-12-07 21:16:42.501603 paramsurvey-0.4.9/scripts/
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1609 2020-09-07 22:21:59.000000 paramsurvey-0.4.9/scripts/paramsurvey-greedy-example.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      991 2020-09-07 22:21:59.000000 paramsurvey-0.4.9/scripts/paramsurvey-multistage-example.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      823 2020-12-07 19:47:34.000000 paramsurvey-0.4.9/scripts/paramsurvey-readme-example.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       38 2020-12-07 21:16:42.504603 paramsurvey-0.4.9/setup.cfg
+-rwxrwxr-x   0 lindahl   (2020) lindahl   (2020)     2118 2020-11-28 01:19:45.000000 paramsurvey-0.4.9/setup.py
+drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-12-07 21:16:42.498603 paramsurvey-0.4.9/test/
+drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-12-07 21:16:42.501603 paramsurvey-0.4.9/test/__pycache__/
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     8347 2020-07-18 21:34:50.000000 paramsurvey-0.4.9/test/__pycache__/test_psmultiprocessing.cpython-36-pytest-5.3.2.pyc
+drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-12-07 21:16:42.503603 paramsurvey-0.4.9/test/integration/
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1113 2020-11-21 17:51:47.000000 paramsurvey-0.4.9/test/integration/test-env-overrides.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      831 2020-12-06 17:03:40.000000 paramsurvey-0.4.9/test/integration/test-generic_init_max_tasks_per_child.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      855 2020-11-21 17:51:47.000000 paramsurvey-0.4.9/test/integration/test-multiprocessing-failure.py
+-rwxrwxr-x   0 lindahl   (2020) lindahl   (2020)      538 2020-11-26 01:06:28.000000 paramsurvey-0.4.9/test/integration/test-multiprocessing.sh
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)       91 2020-08-16 01:51:19.000000 paramsurvey-0.4.9/test/integration/test-only-builtins.py
+-rwxrwxr-x   0 lindahl   (2020) lindahl   (2020)     1115 2020-11-26 01:06:28.000000 paramsurvey-0.4.9/test/integration/test-ray.sh
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)    10912 2020-12-07 20:12:57.000000 paramsurvey-0.4.9/test/integration/test_generic.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1200 2020-09-08 02:19:28.000000 paramsurvey-0.4.9/test/integration/test_stress.py
+drwxrwxr-x   0 lindahl   (2020) lindahl   (2020)        0 2020-12-07 21:16:42.503603 paramsurvey-0.4.9/test/unit/
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     1149 2020-11-22 05:05:42.000000 paramsurvey-0.4.9/test/unit/test_multiprocessing.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     5482 2020-11-03 04:43:22.000000 paramsurvey-0.4.9/test/unit/test_params.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)      457 2020-08-22 01:31:33.000000 paramsurvey-0.4.9/test/unit/test_pslogger.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     2576 2020-08-22 04:20:53.000000 paramsurvey-0.4.9/test/unit/test_stats.py
+-rw-rw-r--   0 lindahl   (2020) lindahl   (2020)     5238 2020-12-07 15:53:58.000000 paramsurvey-0.4.9/test/unit/test_utils.py
```

### Comparing `paramsurvey-0.4.8/.travis.yml` & `paramsurvey-0.4.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/LICENSE` & `paramsurvey-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/Makefile` & `paramsurvey-0.4.9/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 test: unit scripts generic
 
 clean_coverage:
 	rm -f .coverage
 
 test_coverage: clean_coverage
-	PYTHONPATH=. pytest --cov-report= --cov-append --cov-branch --cov paramsurvey -v -v test/unit
+	PYTHONPATH=. pytest --cov-report=xml --cov-append --cov-branch --cov paramsurvey -v -v test/unit
 	COVERAGE=1 PYTHONPATH=. test/integration/test-multiprocessing.sh test/integration
 	COVERAGE=1 PYTHONPATH=.:test/integration test/integration/test-ray.sh test/integration
 
 test_coverage_verbose:
 	PARAMSURVEY_VERBOSE=3 PARAMSURVEY_VSTATS=3 COVERAGE=1 PYTHONPATH=. test/integration/test-multiprocessing.sh test/integration
 	PARAMSURVEY_VERBOSE=3 PARAMSURVEY_VSTATS=3 COVERAGE=1 PYTHONPATH=.:test/integration test/integration/test-ray.sh test/integration
```

### Comparing `paramsurvey-0.4.8/PKG-INFO` & `paramsurvey-0.4.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: paramsurvey
-Version: 0.4.8
+Version: 0.4.9
 Summary: A toolkit for doing parameter surveys
 Home-page: https://github.com/wumpus/paramsurvey
 Author: Greg Lindahl and others
 Author-email: lindahl@pbm.com
 License: Apache 2.0
 Description: # paramsurvey
         
-        [![Build Status](https://travis-ci.com/wumpus/paramsurvey.svg?branch=master)](https://travis-ci.com/wumpus/paramsurvey) [![Coverage Status](https://coveralls.io/repos/github/wumpus/paramsurvey/badge.svg?branch=master)](https://coveralls.io/github/wumpus/paramsurvey?branch=master) [![Apache License 2.0](https://img.shields.io/github/license/wumpus/paramsurvey.svg)](LICENSE)
+        [![Build Status](https://dev.azure.com/lindahl0577/paramsurvey/_apis/build/status/wumpus.paramsurvey?branchName=master)](https://dev.azure.com/lindahl0577/paramsurvey/_build/latest?definitionId=1&branchName=master) [![Coverage](https://coveralls.io/repos/github/wumpus/paramsurvey/badge.svg?branch=master)](https://coveralls.io/github/wumpus/paramsurvey?branch=master) [![Apache License 2.0](https://img.shields.io/github/license/wumpus/paramsurvey.svg)](LICENSE)
         
         paramsurvey is a set of tools for creating and executing parameter surveys.
         
         paramsurvey has a pluggable parallel backend. The supported backends at present
         are python's multiprocessing module, and computing cluster software `ray`. An `mpi` backend is planned.
         
         ## Example
@@ -103,14 +103,23 @@
         ```
         
         For retrospective debugging, i.e. your run crashes and you are sad
         that you specified a lower verbosity than you desire post-crash,
         `paramsurvey` creates a hidden logfile in the current directory for
         every run, named `.paramusurvey-DATE-TIME.log`.
         
+        ### Backend-specific arguments
+        
+        Both `init()` and `map()` take a backend-specific keyword argument named for the backend, and
+        ignored by other backends. For example, to pass an argument only used by the `ray` backend,
+        
+        ```
+        paramsurvey.map(..., ray={'num_gpus': 1})
+        ```
+        
         ## The MapResults object
         
         The MapResults object has several properties:
         
         * `results` is a Pandas DataFrame containing the values of the pset and the keys returned by the worker function. If you prefer to deal with dictionaries
         and are not worried about memory usage, `results.to_dict` returns a list of dictionaries.
         * `failed` is a list of failed psets dictionaries, plus an extra '_exception' key if an exception was raised in the worker function.
```

### Comparing `paramsurvey-0.4.8/README.md` & `paramsurvey-0.4.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # paramsurvey
 
-[![Build Status](https://travis-ci.com/wumpus/paramsurvey.svg?branch=master)](https://travis-ci.com/wumpus/paramsurvey) [![Coverage Status](https://coveralls.io/repos/github/wumpus/paramsurvey/badge.svg?branch=master)](https://coveralls.io/github/wumpus/paramsurvey?branch=master) [![Apache License 2.0](https://img.shields.io/github/license/wumpus/paramsurvey.svg)](LICENSE)
+[![Build Status](https://dev.azure.com/lindahl0577/paramsurvey/_apis/build/status/wumpus.paramsurvey?branchName=master)](https://dev.azure.com/lindahl0577/paramsurvey/_build/latest?definitionId=1&branchName=master) [![Coverage](https://coveralls.io/repos/github/wumpus/paramsurvey/badge.svg?branch=master)](https://coveralls.io/github/wumpus/paramsurvey?branch=master) [![Apache License 2.0](https://img.shields.io/github/license/wumpus/paramsurvey.svg)](LICENSE)
 
 paramsurvey is a set of tools for creating and executing parameter surveys.
 
 paramsurvey has a pluggable parallel backend. The supported backends at present
 are python's multiprocessing module, and computing cluster software `ray`. An `mpi` backend is planned.
 
 ## Example
@@ -95,14 +95,23 @@
 ```
 
 For retrospective debugging, i.e. your run crashes and you are sad
 that you specified a lower verbosity than you desire post-crash,
 `paramsurvey` creates a hidden logfile in the current directory for
 every run, named `.paramusurvey-DATE-TIME.log`.
 
+### Backend-specific arguments
+
+Both `init()` and `map()` take a backend-specific keyword argument named for the backend, and
+ignored by other backends. For example, to pass an argument only used by the `ray` backend,
+
+```
+paramsurvey.map(..., ray={'num_gpus': 1})
+```
+
 ## The MapResults object
 
 The MapResults object has several properties:
 
 * `results` is a Pandas DataFrame containing the values of the pset and the keys returned by the worker function. If you prefer to deal with dictionaries
 and are not worried about memory usage, `results.to_dict` returns a list of dictionaries.
 * `failed` is a list of failed psets dictionaries, plus an extra '_exception' key if an exception was raised in the worker function.
```

### Comparing `paramsurvey-0.4.8/paramsurvey/__init__.py` & `paramsurvey-0.4.9/paramsurvey/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
     global our_backend
     if backend in backends:
         pslogger.log('initializing paramsurvey {} backend'.format(backend), stderr=verbose)
         our_backend = backends[backend]
         our_backend['name'] = backend
         if 'lazy' in our_backend:
             our_backend.update(our_backend['lazy']())
-        system_kwargs, other_kwargs = resolve_kwargs(global_kwargs, kwargs, backend, backends)
-        our_backend['init'](system_kwargs, **other_kwargs)
+        system_kwargs, backend_kwargs, other_kwargs = resolve_kwargs(global_kwargs, kwargs, backend, backends)
+        our_backend['init'](system_kwargs, backend_kwargs, **other_kwargs)
     else:  # pragma: no cover
         raise ValueError('unknown backend '+backend+', valid backends: '+', '.join(backends.keys()))
 
 
 def backend():
     '''Returns the paramsurvey backend in use.
 
@@ -184,10 +184,10 @@
     sys.stderr.flush()
     sys.stdout.flush()
 
     for kw in ('backend', 'ncores', 'max_tasks_per_child'):
         if kw in kwargs:
             raise ValueError('{} can only be passed to init, not map'.format(kw))
 
-    system_kwargs, other_kwargs = resolve_kwargs(global_kwargs, kwargs, our_backend['name'], backends)
+    system_kwargs, backend_kwargs, other_kwargs = resolve_kwargs(global_kwargs, kwargs, our_backend['name'], backends)
 
-    return our_backend['map'](*args, system_kwargs=system_kwargs, **other_kwargs)
+    return our_backend['map'](*args, system_kwargs=system_kwargs, backend_kwargs=backend_kwargs, **other_kwargs)
```

### Comparing `paramsurvey-0.4.8/paramsurvey/params.py` & `paramsurvey-0.4.9/paramsurvey/params.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/paramsurvey/pslogger.py` & `paramsurvey-0.4.9/paramsurvey/pslogger.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 
 '''
 import datetime
 import os
 import sys
 import socket
 
+logger_filename = None
+
 
 def atomic_create_ish(filenames):
     '''
     Figure out which on this list of filenames does not already exist.
     Not safe on NFS filesystems.
     '''
     for f in filenames:
         try:
             fd = open(f, 'xt')
+            global logger_filename
+            logger_filename = f
         except FileExistsError:
             continue
         break
     else:
         raise ValueError('unable to open a unique logfile, rerun')
 
     return fd
@@ -43,14 +47,16 @@
     middle = datetime.datetime.utcnow().strftime('%Y%m%d-%H%M%S')
     middleplus = datetime.datetime.utcnow().strftime('%Y%m%d-%H%M%S.%f')
     middles = (middle, middleplus, middleplus+'a')
 
     global logfd
     if pslogger_fd:
         logfd = pslogger_fd
+        global logger_filename
+        logger_filename = '(internal)'
     else:
         logfd = atomic_create_ish([pslogger_prefix+m+'.log' for m in middles])
 
     print('paramsurvey starttime', middleplus, file=logfd)
     print('hostname', socket.gethostname(), file=logfd)
     print('command line', repr(sys.argv), file=logfd)
     for e in sorted(['PYTHONPATH', 'VIRTUAL_ENV', 'CONDA_DEFAULT_ENV', 'CONDA_PREFIX']):
```

### Comparing `paramsurvey-0.4.8/paramsurvey/psmultiprocessing.py` & `paramsurvey-0.4.9/paramsurvey/psmultiprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,40 +9,38 @@
 from . import stats
 from . import pslogger
 
 pool = None
 our_ncores = None
 
 
-def init(system_kwargs, **kwargs):
+def init(system_kwargs, backend_kwargs):
     global pool
     global our_ncores
     if pool:  # yes we can be called multiple times  # pragma: no cover
         return
 
-    pool_kwargs = {}
-
     ncores = system_kwargs.pop('ncores', None)
     if ncores is None or ncores == 0:
         ncores = _core_count()
     elif ncores < 0:
         # negative ncores means subtract
         ncores = max(_core_count() + ncores, 1)
-    pool_kwargs['processes'] = ncores
+    backend_kwargs['processes'] = ncores
     our_ncores = ncores
 
     max_tasks_per_child = system_kwargs.pop('max_tasks_per_child', None)
     if max_tasks_per_child:
-        pool_kwargs['maxtasksperchild'] = max_tasks_per_child
+        backend_kwargs['maxtasksperchild'] = max_tasks_per_child
 
     verbose = system_kwargs['verbose']
     pslogger.log('initializing multiprocessing pool with {} processes'.format(ncores), stderr=verbose)
-    pslogger.log('Pool() kwargs are', pool_kwargs, stderr=verbose > 1)
+    pslogger.log('Pool() kwargs are', backend_kwargs, stderr=verbose > 1)
 
-    pool = multiprocessing.Pool(**pool_kwargs)
+    pool = multiprocessing.Pool(**backend_kwargs)
 
 
 def finalize():
     # needed to make things like pytest coverage reporting work
     pslogger.finalize()
     pool.close()
     pool.join()
@@ -141,22 +139,26 @@
         progress.report()
         system_stats.report()
 
     return group_size
 
 
 def map(func, psets, out_func=None, system_kwargs=None, user_kwargs=None, chdir=None, out_subdirs=None,
-        progress_dt=None, group_size=None, name='default', max_tasks_per_child=None, **kwargs):
+        progress_dt=None, group_size=None, name='default', max_tasks_per_child=None, backend_kwargs={},
+        **kwargs):
 
     verbose = system_kwargs['verbose']
     vstats = system_kwargs['vstats']
 
     if utils.psets_empty(psets):
         return
 
+    if backend_kwargs:
+        raise TypeError('multiprocessing.map does not currently take any backend kwargs')
+
     psets, system_stats, system_kwargs = utils.map_prep(psets, name, system_kwargs, chdir,
                                                         out_subdirs, progress_dt=progress_dt, **kwargs)
 
     if max_tasks_per_child is not None:
         pslogger.log('max_tasks_per_child={} is ignored by the multiprocessing map() call, do it in init()'.format(max_tasks_per_child), stderr=verbose)
 
     progress = system_kwargs['progress']
```

### Comparing `paramsurvey-0.4.8/paramsurvey/psray.py` & `paramsurvey-0.4.9/paramsurvey/psray.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,55 +16,49 @@
     if rayfile is None:  # pragma: no cover
         rayfile = os.path.expanduser('~/.ray-head-details')
     with open(rayfile) as f:
         address, password = f.read().split()
     return address, password
 
 
-def init(system_kwargs, **kwargs):
+def init(system_kwargs, backend_kwargs):
     if ray.is_initialized():
         # this happens with our test scripts
         # also a user might call init() repeatedly, perhaps with inconsistant args
         pslogger.log('init.ray called repeatedly')
         return
 
     verbose = system_kwargs['verbose']
 
-    ray_kwargs = {}
-
     ncores = system_kwargs.pop('ncores', None)
     if ncores is not None:
-        if ncores >= 0:
-            # what does ncores=0 mean to ray?
-            ray_kwargs['num_cpus'] = ncores
-            pslogger.log('init.ray ncores=', ncores, 'probably has no effect', stderr=verbose > 1)
-        else:
-            pslogger.log('init.ray negative ncores=', ncores, 'ignored', stderr=verbose)
+        pslogger.log('init.ray ncores={} ignored'.format(ncores), stderr=verbose)
+        # when we actually are willing to start ray here, pay attention to ncores
 
     max_tasks_per_child = system_kwargs.pop('max_tasks_per_child', None)
     if max_tasks_per_child:
         if verbose:
             pslogger.log('init.ray max_tasks_per_child=', max_tasks_per_child, stderr=verbose > 1)
 
         # the docs say this should work, but it gets: TypeError: options() got an unexpected keyword argument 'max_calls'
         # paramsurvey.psray.do_work_wrapper = paramsurvey.psray.do_work_wrapper.options(max_calls=max_tasks_per_child)
 
         # this is a hack that works, if it is used before the workers are instantiated
         do_work_wrapper._max_calls = max_tasks_per_child
 
-    # should allow these to be kwargs
-    address, password = read_ray_config()
-    kwargs['address'] = address
-    kwargs['_redis_password'] = password  # added the leading _ in ray 1.0.0
+    if 'address' not in backend_kwargs and '_redis_password' not in backend_kwargs:
+        address, password = read_ray_config()
+        backend_kwargs['address'] = address
+        backend_kwargs['_redis_password'] = password  # added the leading _ in ray 1.0.0
 
     if os.environ.get('RAY_LOCAL_MODE', False):
-        kwargs['local_mode'] = True
+        backend_kwargs['local_mode'] = True
 
     # should we create a ray head if there is no cluster?
-    ray.init(**kwargs)
+    ray.init(**backend_kwargs)
 
 
 def finalize():
     pslogger.finalize()
     ray.shutdown()
 
 
@@ -196,15 +190,15 @@
 
         # dynamic group_size adjustment
 
     return futures, cores, group_size
 
 
 def map(func, psets, out_func=None, system_kwargs=None, user_kwargs=None, chdir=None, out_subdirs=None,
-        progress_dt=None, group_size=None, name='default', **kwargs):
+        progress_dt=None, group_size=None, name='default', backend_kwargs={}, **kwargs):
 
     verbose = system_kwargs['verbose']
     vstats = system_kwargs['vstats']
 
     if utils.psets_empty(psets):
         return
 
@@ -237,27 +231,32 @@
         # make this dynamic someday
         group_size = 1
 
     pslogger.log('paramsurvey.psray map: psets {}, cores {}, group_size {}, verbose {}'.format(
         len(psets), cores, group_size, system_kwargs['verbose']
     ), stderr=verbose > 1)
 
+    wrapper = do_work_wrapper
+
+    if backend_kwargs:
+        wrapper = wrapper.options(**backend_kwargs)
+
     futures = []
     pset_index = 0
 
     while True:
         while len(futures) <= cores * factor:
             pset_group, pset_index = utils.get_pset_group(psets, pset_index, group_size)
             if len(pset_group) == 0:
                 break
 
             pset_group, pset_ids = utils.make_pset_ids(pset_group)
             system_kwargs['pset_ids'].update(pset_ids)
 
-            futures.append(do_work_wrapper.remote(func, worker_system_kwargs, user_kwargs, pset_group))
+            futures.append(wrapper.remote(func, worker_system_kwargs, user_kwargs, pset_group))
             progress.active += len(pset_group)
             progress.report()
             system_stats.report()
 
         if pset_index >= len(psets):
             break
```

### Comparing `paramsurvey-0.4.8/paramsurvey/stats.py` & `paramsurvey-0.4.9/paramsurvey/stats.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/paramsurvey/utils.py` & `paramsurvey-0.4.9/paramsurvey/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         if keyword.iskeyword(c):
             raise ValueError('pset key "{}" is a Python keyword; this cases problems with pandas'.format(c))
         if c.startswith('_'):
             raise ValueError('pset key "{}" starts with an underscore; this cases problems with pandas'.format(c))
     return psets
 
 
-def map_prep(psets, name, system_kwargs, chdir, out_subdirs, keep_results=True, progress_dt=None, **kwargs):
+def map_prep(psets, name, system_kwargs, chdir, out_subdirs, keep_results=True, progress_dt=None, raise_in_wrapper=None):
     verbose = system_kwargs['verbose']
     vstats = system_kwargs['vstats']
 
     pslogger.log('paramsurvey.map start time', datetime.datetime.utcnow().strftime('%Y%m%d-%H%M%S'))
     pslogger.log('paramsurvey.map starting work on '+name, stderr=verbose)
     pslogger.log('paramsurvey.map system_kwargs '+repr(system_kwargs), stderr=verbose > 1)
 
@@ -216,16 +216,16 @@
         system_kwargs['results'] = DF_Appender(ignore_index=True)
     if chdir:
         system_kwargs['chdir'] = chdir
     if out_subdirs:
         system_kwargs['out_subdirs'] = out_subdirs
     if name:
         system_kwargs['name'] = name
-    if 'raise_in_wrapper' in kwargs:
-        system_kwargs['raise_in_wrapper'] = kwargs['raise_in_wrapper']
+    if raise_in_wrapper:
+        system_kwargs['raise_in_wrapper'] = raise_in_wrapper
 
     system_kwargs['pset_ids'] = {}
 
     system_stats = stats.PerfStats(vstats=vstats)
 
     pslogger.log('paramsurvey.map pset count {}, pset columns {}'.format(len(psets), list(psets.columns.values)))
 
@@ -317,15 +317,18 @@
             pslogger.log('saw exception in worker: ' + user_ret['exception'], stderr=verbose)
             pslogger.log('pset: '+repr(system_kwargs['pset_ids'][pset_id]), stderr=verbose > 1)
 
             system_kwargs['pset_ids'][pset_id]['_exception'] = user_ret['exception']
 
             if 'traceback' in user_ret:
                 system_kwargs['pset_ids'][pset_id]['_traceback'] = user_ret['traceback']
-                pslogger.log('traceback:\n' + user_ret['traceback'], stderr=verbose > 1)
+                verbose_t = verbose > 1
+                pslogger.log('traceback:\n' + user_ret['traceback'], stderr=verbose_t)
+                if verbose > 0 and not verbose_t:
+                    print('(traceback is in', pslogger.logger_filename+')', file=sys.stderr)
         else:
             del system_kwargs['pset_ids'][pset_id]
             user_ret['pset'].pop('_pset_id', None)
 
             new_row = user_ret['pset'].copy()
             if user_ret['result']:  # allowed to be None
                 new_row.update(user_ret['result'])
@@ -379,37 +382,32 @@
     system_kwargs = {}
     other_kwargs = {}
 
     for k in kwargs:
         if k in global_kwargs:
             gkw = global_kwargs[k]
             if gkw.get('strong'):
-                pslogger.log('environment variable overrides passed in value for', k, verbose > 0)
+                pslogger.log('environment variable overrides passed in value for '+k, verbose > 0)
                 system_kwargs[k] = gkw['value']
             else:
                 system_kwargs[k] = kwargs[k]
         else:
             other_kwargs[k] = kwargs[k]
     for k in global_kwargs:
         if k not in system_kwargs:
             system_kwargs[k] = global_kwargs[k]['value']
 
-    backend_prefixes = tuple(x+'_' for x in backends.keys())
-    kept_other_kwargs = {}
-    for k in other_kwargs:
-        if k.startswith(backend_prefixes):
-            if k.startswith(backend+'_'):
-                k2 = k.replace(backend+'_', '', 1)
-                kept_other_kwargs[k2] = other_kwargs[k]
-            else:
-                pslogger.log('discarding kwarg due to our backend choice: ', k, other_kwargs[k], stderr=verbose > 1)
-        else:
-            kept_other_kwargs[k] = other_kwargs[k]
+    backend_kwargs = other_kwargs.pop(backend, {})
+
+    for b in backends:
+        if b in other_kwargs:
+            pslogger.log('discarding kwarg {} due to our backend choice'.format(b), stderr=verbose > 1)
+            other_kwargs.pop(b)
 
-    return system_kwargs, kept_other_kwargs
+    return system_kwargs, backend_kwargs, other_kwargs
 
 
 def make_subdir_name(count, prefix='ps'):
     try:
         digits = math.ceil(math.log10(count))
     except Exception:
         print('count argument must be a number greater than 0', file=sys.stderr)
```

### Comparing `paramsurvey-0.4.8/paramsurvey.egg-info/PKG-INFO` & `paramsurvey-0.4.9/paramsurvey.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: paramsurvey
-Version: 0.4.8
+Version: 0.4.9
 Summary: A toolkit for doing parameter surveys
 Home-page: https://github.com/wumpus/paramsurvey
 Author: Greg Lindahl and others
 Author-email: lindahl@pbm.com
 License: Apache 2.0
 Description: # paramsurvey
         
-        [![Build Status](https://travis-ci.com/wumpus/paramsurvey.svg?branch=master)](https://travis-ci.com/wumpus/paramsurvey) [![Coverage Status](https://coveralls.io/repos/github/wumpus/paramsurvey/badge.svg?branch=master)](https://coveralls.io/github/wumpus/paramsurvey?branch=master) [![Apache License 2.0](https://img.shields.io/github/license/wumpus/paramsurvey.svg)](LICENSE)
+        [![Build Status](https://dev.azure.com/lindahl0577/paramsurvey/_apis/build/status/wumpus.paramsurvey?branchName=master)](https://dev.azure.com/lindahl0577/paramsurvey/_build/latest?definitionId=1&branchName=master) [![Coverage](https://coveralls.io/repos/github/wumpus/paramsurvey/badge.svg?branch=master)](https://coveralls.io/github/wumpus/paramsurvey?branch=master) [![Apache License 2.0](https://img.shields.io/github/license/wumpus/paramsurvey.svg)](LICENSE)
         
         paramsurvey is a set of tools for creating and executing parameter surveys.
         
         paramsurvey has a pluggable parallel backend. The supported backends at present
         are python's multiprocessing module, and computing cluster software `ray`. An `mpi` backend is planned.
         
         ## Example
@@ -103,14 +103,23 @@
         ```
         
         For retrospective debugging, i.e. your run crashes and you are sad
         that you specified a lower verbosity than you desire post-crash,
         `paramsurvey` creates a hidden logfile in the current directory for
         every run, named `.paramusurvey-DATE-TIME.log`.
         
+        ### Backend-specific arguments
+        
+        Both `init()` and `map()` take a backend-specific keyword argument named for the backend, and
+        ignored by other backends. For example, to pass an argument only used by the `ray` backend,
+        
+        ```
+        paramsurvey.map(..., ray={'num_gpus': 1})
+        ```
+        
         ## The MapResults object
         
         The MapResults object has several properties:
         
         * `results` is a Pandas DataFrame containing the values of the pset and the keys returned by the worker function. If you prefer to deal with dictionaries
         and are not worried about memory usage, `results.to_dict` returns a list of dictionaries.
         * `failed` is a list of failed psets dictionaries, plus an extra '_exception' key if an exception was raised in the worker function.
```

### Comparing `paramsurvey-0.4.8/paramsurvey.egg-info/SOURCES.txt` & `paramsurvey-0.4.9/paramsurvey.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .flake8
 .gitignore
 .travis.yml
 CHANGELOG.md
 LICENSE
 Makefile
 README.md
+azure-pipelines.yml
 setup.py
 paramsurvey/__init__.py
 paramsurvey/examples.py
 paramsurvey/params.py
 paramsurvey/pslogger.py
 paramsurvey/psmpi.py
 paramsurvey/psmultiprocessing.py
```

### Comparing `paramsurvey-0.4.8/scripts/paramsurvey-greedy-example.py` & `paramsurvey-0.4.9/scripts/paramsurvey-greedy-example.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/scripts/paramsurvey-multistage-example.py` & `paramsurvey-0.4.9/scripts/paramsurvey-multistage-example.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/scripts/paramsurvey-readme-example.py` & `paramsurvey-0.4.9/scripts/paramsurvey-readme-example.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/setup.py` & `paramsurvey-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/test/__pycache__/test_psmultiprocessing.cpython-36-pytest-5.3.2.pyc` & `paramsurvey-0.4.9/test/__pycache__/test_psmultiprocessing.cpython-36-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/test/integration/test-env-overrides.py` & `paramsurvey-0.4.9/test/integration/test-env-overrides.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/test/integration/test-generic_init_max_tasks_per_child.py` & `paramsurvey-0.4.9/test/integration/test-generic_init_max_tasks_per_child.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 def return_pid(pset, system_kwargs, user_kwargs):
     return {'pid': os.getpid()}
 
 
 def test_init_max_tasks_per_child():
+    # this test is in a separate file because it cannot share a session with test_generic
     paramsurvey.init(pslogger_fd=pslogger_fd, max_tasks_per_child=1)
 
     psets = [{'foo': 1}] * 10
     results = paramsurvey.map(return_pid, psets, name='init_max_tasks_per_child set')
     pids = set(r.pid for r in results.itertuples())
     assert len(pids) == len(results), 'init_max_tasks_per_child=1 has unique pids'
```

### Comparing `paramsurvey-0.4.8/test/integration/test-multiprocessing-failure.py` & `paramsurvey-0.4.9/test/integration/test-multiprocessing-failure.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/test/integration/test-multiprocessing.sh` & `paramsurvey-0.4.9/test/integration/test-multiprocessing.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/sh
 
 if [ ! -z "$COVERAGE" ]; then
-    COVERAGE="--cov-report= --cov-append --cov-branch --cov paramsurvey -v -v"
+    COVERAGE="--cov-report=xml --cov-append --cov-branch --cov paramsurvey -v -v"
 fi
 
 PARAMSURVEY_BACKEND=multiprocessing pytest $COVERAGE $PYTEST_STDERR_VISIBLE $1
 PARAMSURVEY_BACKEND=multiprocessing pytest $COVERAGE $PYTEST_STDERR_VISIBLE $1/test-multiprocessing-failure.py
 PARAMSURVEY_BACKEND=multiprocessing pytest $COVERAGE $PYTEST_STDERR_VISIBLE $1/test-env-overrides.py
 PARAMSURVEY_BACKEND=multiprocessing pytest $COVERAGE $PYTEST_STDERR_VISIBLE $1/test-generic_init_max_tasks_per_child.py
```

### Comparing `paramsurvey-0.4.8/test/integration/test-ray.sh` & `paramsurvey-0.4.9/test/integration/test-ray.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/sh
 
 if [ ! -z "$COVERAGE" ]; then
-    COVERAGE="--cov-report= --cov-append --cov-branch --cov paramsurvey -v -v"
+    COVERAGE="--cov-report=xml --cov-append --cov-branch --cov paramsurvey -v -v"
 fi
 
 if [ ! -z "$ONLY_BUILTINS" ]; then
     PARAMSURVEY_BACKEND=ray pytest $COVERAGE $1/test-only-builtins.py
     exit 0
 fi
```

### Comparing `paramsurvey-0.4.8/test/integration/test_generic.py` & `paramsurvey-0.4.9/test/integration/test_generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     df = results.missing.to_df()
     assert isinstance(df, pd.DataFrame)
     assert len(df) == len(results.missing)
 
 
 def do_test_args(pset, system_kwargs, user_kwargs):
     # this function cannot be nested inside test_args() because nested funcs can't be pickled
-    print('GREG worker getcwd is', os.getcwd())
     assert os.getcwd() == user_kwargs['expected_cwd'], 'chdir appears to work, getcwd=' + os.getcwd()
     assert 'out_subdir' in system_kwargs
 
 
 def test_args(capsys, paramsurvey_init):
     if platform.system() == 'Darwin':
         # in Darwin, the tempfile directory is process-specific
@@ -207,14 +206,16 @@
 
     # ray redirects stderr to stdout, while multiprocessing prints it in the worker
     # TODO: add stderr/out capture everywhere and use it here
     #assert 'Traceback ' in captured.out or 'Traceback ' in captured.err
 
     # the standard progress function prints this
     assert 'failures: 1' in captured.out or 'failures: 1' in captured.err
+    assert 'exceptions: 1' in captured.out or 'exceptions: 1' in captured.err
+    assert 'traceback is in' in captured.err, 'pointer to hidden logfile given at default verbose'
 
     log = pslogger_fd.getvalue()
     assert 'Traceback' in log, 'python traceback seen'
     assert 'ValueError' in log, 'python exception seen'
     assert 'pset:' in log, 'our pset logline seen'
 
 
@@ -288,18 +289,24 @@
     duration = 0.1
     psets = [{'duration': duration}] * 10
     results = paramsurvey.map(sleep_worker, psets, limit=3, name='sleep with limit')
     assert len(results) == 3
 
 
 def test_map_ncores(paramsurvey_init):
+    # valid for init() but not map()
     with pytest.raises(ValueError):
         paramsurvey.map(sleep_worker, [{'foo': 1}], ncores=3)
 
 
-def test_map_max_tasks_per_child(paramsurvey_init):
-    with pytest.raises(ValueError):
-        paramsurvey.map(sleep_worker, [{'foo': 1}], max_tasks_per_child=1)
+def test_invalid_kwarg(paramsurvey_init):
+    with pytest.raises(TypeError):
+        paramsurvey.init(doesnotexist=True)
+    with pytest.raises(TypeError):
+        paramsurvey.map(sleep_worker, [{}], doesnotexist=True)
+    with pytest.raises(TypeError):
+        paramsurvey.map(sleep_worker, [{}], ray={'doesnotexist': True}, multiprocessing={'doesnotexist': True})
+    pass
 
 
 def test_overlarge_pset():
     pass
```

### Comparing `paramsurvey-0.4.8/test/integration/test_stress.py` & `paramsurvey-0.4.9/test/integration/test_stress.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/test/unit/test_multiprocessing.py` & `paramsurvey-0.4.9/test/unit/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/test/unit/test_params.py` & `paramsurvey-0.4.9/test/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/test/unit/test_stats.py` & `paramsurvey-0.4.9/test/unit/test_stats.py`

 * *Files identical despite different names*

### Comparing `paramsurvey-0.4.8/test/unit/test_utils.py` & `paramsurvey-0.4.9/test/unit/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,55 +73,62 @@
     return ret
 
 
 def test_init_resolve_kwargs():
     gkwargs = copy2(paramsurvey.global_kwargs)
     with patch.dict(os.environ, {'PARAMSURVEY_VERBOSE': '3'}, clear=True):
         utils.initialize_kwargs(gkwargs, {'verbose': 1})
-        system_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {'verbose': 2, 'unrecognized': 'asdf'}, '', {})
+        system_kwargs, backend_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {'verbose': 2, 'unrecognized': 'asdf'}, '', {})
         assert system_kwargs['verbose'] == 3, 'env variables trump all'
+        assert backend_kwargs == {}
         assert other_kwargs['unrecognized'] == 'asdf', 'unrecognized args pass through'
 
     gkwargs = copy2(paramsurvey.global_kwargs)
     with patch.dict(os.environ, {}, clear=True):
         utils.initialize_kwargs(gkwargs, {'verbose': 1})
-        system_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {'verbose': 2}, '', {})
+        system_kwargs, backend_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {'verbose': 2}, '', {})
         assert system_kwargs['verbose'] == 2, 'closest wins'
+        assert backend_kwargs == {}
         assert other_kwargs == {}
 
     gkwargs = copy2(paramsurvey.global_kwargs)
     with patch.dict(os.environ, {}, clear=True):
         utils.initialize_kwargs(gkwargs, {'verbose': 1})
-        system_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {}, '', {})
+        system_kwargs, backend_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {}, '', {})
         assert system_kwargs['verbose'] == 1, 'init kwarg comes last'
+        assert backend_kwargs == {}
         assert other_kwargs == {}
 
     gkwargs = copy2(paramsurvey.global_kwargs)
     with patch.dict(os.environ, {}, clear=True):
         utils.initialize_kwargs(gkwargs, {})
-        system_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {}, '', {})
+        system_kwargs, backend_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {}, '', {})
         assert system_kwargs['verbose'] == 1, 'default'
+        assert backend_kwargs == {}
         assert other_kwargs == {}
 
     gkwargs = copy2(paramsurvey.global_kwargs)
     with patch.dict(os.environ, {'PARAMSURVEY_BACKEND': 'FOO'}, clear=True):
         utils.initialize_kwargs(gkwargs, {})
-        system_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {}, '', {})
+        system_kwargs, backend_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, {}, '', {})
         assert system_kwargs['backend'] == 'FOO', 'type works'
+        assert backend_kwargs == {}
         assert other_kwargs == {}
 
     gkwargs = copy2(paramsurvey.global_kwargs)
     with patch.dict(os.environ, {}, clear=True):
         utils.initialize_kwargs(gkwargs, {})
-        kwargs = {'ray_foo': 1, 'multiprocessing_bar': 2, 'other_baz': 3}
-        system_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, kwargs, 'ray', {'ray': '', 'multiprocessing': ''})
-        assert other_kwargs == {'foo': 1, 'other_baz': 3}
+        kwargs = {'ray': {'foo': 1}, 'multiprocessing': {'bar': 2}, 'other': {'baz': 3}}
+        system_kwargs, backend_kwargs, other_kwargs = utils.resolve_kwargs(gkwargs, kwargs, 'ray', {'ray': '', 'multiprocessing': ''})
+        assert backend_kwargs == {'foo': 1}
+        assert other_kwargs == {'other': {'baz': 3}}
 
     gkwargs = copy2(paramsurvey.global_kwargs)
     with patch.dict(os.environ, {'PARAMSURVEY_VERBOSE': 'None'}, clear=True):
+        # int('None') raises ValueError
         with pytest.raises(ValueError):
             utils.initialize_kwargs(gkwargs, {})
 
 
 def test_psets_empty():
     psets = []
     assert utils.psets_empty(psets)
```

