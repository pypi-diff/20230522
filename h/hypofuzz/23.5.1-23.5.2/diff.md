# Comparing `tmp/hypofuzz-23.5.1.tar.gz` & `tmp/hypofuzz-23.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypofuzz-23.5.1.tar", last modified: Sun May 14 01:44:54 2023, max compression
+gzip compressed data, was "hypofuzz-23.5.2.tar", last modified: Mon May 22 17:33:00 2023, max compression
```

## Comparing `hypofuzz-23.5.1.tar` & `hypofuzz-23.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.540266 hypofuzz-23.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/src/hypofuzz/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/hy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/src/hypofuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/tests/test_coverage_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/tests/test_fuzz_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.877132 hypofuzz-23.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 17:33:00.877132 hypofuzz-23.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:33:00.877132 hypofuzz-23.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.869132 hypofuzz-23.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.873132 hypofuzz-23.5.2/src/hypofuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/hy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.873132 hypofuzz-23.5.2/src/hypofuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.877132 hypofuzz-23.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/tests/test_coverage_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/tests/test_fuzz_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/tests/test_version.py
```

### Comparing `hypofuzz-23.5.1/LICENSE` & `hypofuzz-23.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/PKG-INFO` & `hypofuzz-23.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.5.1
+Version: 23.5.2
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.5.1/README.md` & `hypofuzz-23.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/setup.py` & `hypofuzz-23.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/src/hypofuzz/corpus.py` & `hypofuzz-23.5.2/src/hypofuzz/corpus.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/src/hypofuzz/cov.py` & `hypofuzz-23.5.2/src/hypofuzz/cov.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/src/hypofuzz/dashboard.py` & `hypofuzz-23.5.2/src/hypofuzz/dashboard.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/src/hypofuzz/debugger.py` & `hypofuzz-23.5.2/src/hypofuzz/debugger.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/src/hypofuzz/entrypoint.py` & `hypofuzz-23.5.2/src/hypofuzz/entrypoint.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/src/hypofuzz/hy.py` & `hypofuzz-23.5.2/src/hypofuzz/hy.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import itertools
 import sys
 import time
 import traceback
 from random import Random
 from typing import Any, Callable, Dict, Generator, List, NoReturn, Optional, Union
 
-from hypothesis import settings, strategies as st
+from hypothesis import settings
 from hypothesis.core import (
     BuildContext,
+    Stuff,
     deterministic_PRNG,
     failure_exceptions_to_catch,
     get_trimmed_traceback,
     process_arguments_to_given,
 )
 from hypothesis.database import ExampleDatabase
 from hypothesis.errors import StopTest, UnsatisfiedAssumption
@@ -83,45 +84,45 @@
         cls,
         wrapped_test: Any,
         *,
         nodeid: Optional[str] = None,
         extra_kw: Optional[Dict[str, object]] = None,
     ) -> "FuzzProcess":
         """Return a FuzzProcess for an @given-decorated test function."""
-        _, _, _, search_strategy = process_arguments_to_given(
+        _, _, _, stuff = process_arguments_to_given(
             wrapped_test,
             arguments=(),
             kwargs=extra_kw or {},
             given_kwargs=wrapped_test.hypothesis._given_kwargs,
             params=get_signature(wrapped_test).parameters,
         )
         return cls(
             test_fn=wrapped_test.hypothesis.inner_test,
-            strategy=search_strategy,
+            stuff=stuff,
             nodeid=nodeid,
             database_key=function_digest(wrapped_test.hypothesis.inner_test),
             hypothesis_database=wrapped_test._hypothesis_internal_use_settings.database
             or settings.default.database,
         )
 
     def __init__(
         self,
         test_fn: Callable,
-        strategy: st.SearchStrategy,
+        stuff: Stuff,
         *,
         random_seed: int = 0,
         nodeid: Optional[str] = None,
         database_key: bytes,
         hypothesis_database: ExampleDatabase,
     ) -> None:
         """Construct a FuzzProcess from specific arguments."""
         # The actual fuzzer implementation
         self.random = Random(random_seed)
         self.__test_fn = test_fn
-        self.__strategy = strategy
+        self.__stuff = stuff
         self.nodeid = nodeid or test_fn.__qualname__
 
         # The seed pool is responsible for managing all seed state, including saving
         # novel seeds to the database.  This includes tracking how often each branch
         # has been hit, minimal covering examples, and so on.
         self.pool = Pool(hypothesis_database, database_key)
         self._mutator_blackbox = BlackBoxMutator(self.pool, self.random)
@@ -249,19 +250,28 @@
         assert collector is not None
         reports: List[str] = []
         argstrings: List[str] = []
         data = ConjectureData(max_length=BUFFER_SIZE, prefix=buffer, random=self.random)
         try:
             with deterministic_PRNG(), BuildContext(
                 data, is_final=True
-            ), constant_stack_depth(), with_reporter(reports.append):
+            ) as context, constant_stack_depth(), with_reporter(reports.append):
                 # Note that the data generation and test execution happen in the same
                 # coverage context.  We may later split this, or tag each separately.
                 with collector:
-                    args, kwargs = data.draw(self.__strategy)
+                    if self.__stuff.selfy is not None:
+                        data.hypothesis_runner = self.__stuff.selfy
+                    # Generate all arguments to the test function.
+                    args = self.__stuff.args
+                    kwargs = dict(self.__stuff.kwargs)
+                    a, kw, argslices = context.prep_args_kwargs_from_strategies(
+                        (), self.__stuff.given_kwargs
+                    )
+                    assert not a, "strategies all moved to kwargs by now"
+                    kwargs.update(kw)
 
                     # Save the repr of our arguments so they can be reported later
                     argstrings.extend(map(repr, args))
                     argstrings.extend(f"{k}={v!r}" for k, v in kwargs.items())
 
                     self.__test_fn(*args, **kwargs)
         except StopTest:
```

### Comparing `hypofuzz-23.5.1/src/hypofuzz/interface.py` & `hypofuzz-23.5.2/src/hypofuzz/interface.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/src/hypofuzz.egg-info/PKG-INFO` & `hypofuzz-23.5.2/src/hypofuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.5.1
+Version: 23.5.2
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.5.1/src/hypofuzz.egg-info/SOURCES.txt` & `hypofuzz-23.5.2/src/hypofuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/tests/test_corpus.py` & `hypofuzz-23.5.2/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.1/tests/test_version.py` & `hypofuzz-23.5.2/tests/test_version.py`

 * *Files identical despite different names*

