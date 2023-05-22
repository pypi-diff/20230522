# Comparing `tmp/hypofuzz-23.5.2.tar.gz` & `tmp/hypofuzz-23.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypofuzz-23.5.2.tar", last modified: Mon May 22 17:33:00 2023, max compression
+gzip compressed data, was "hypofuzz-23.5.3.tar", last modified: Mon May 22 21:36:05 2023, max compression
```

## Comparing `hypofuzz-23.5.2.tar` & `hypofuzz-23.5.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.877132 hypofuzz-23.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 17:33:00.877132 hypofuzz-23.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:33:00.877132 hypofuzz-23.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.869132 hypofuzz-23.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.873132 hypofuzz-23.5.2/src/hypofuzz/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/hy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/src/hypofuzz/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.873132 hypofuzz-23.5.2/src/hypofuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 17:33:00.000000 hypofuzz-23.5.2/src/hypofuzz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:00.877132 hypofuzz-23.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/tests/test_coverage_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/tests/test_fuzz_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-22 17:32:48.000000 hypofuzz-23.5.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.910917 hypofuzz-23.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/src/hypofuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/hy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/src/hypofuzz/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/src/hypofuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 21:36:05.000000 hypofuzz-23.5.3/src/hypofuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:36:05.914917 hypofuzz-23.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/tests/test_coverage_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/tests/test_fuzz_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-22 21:35:56.000000 hypofuzz-23.5.3/tests/test_version.py
```

### Comparing `hypofuzz-23.5.2/LICENSE` & `hypofuzz-23.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/PKG-INFO` & `hypofuzz-23.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.5.2
+Version: 23.5.3
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.5.2/README.md` & `hypofuzz-23.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/setup.py` & `hypofuzz-23.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/src/hypofuzz/corpus.py` & `hypofuzz-23.5.3/src/hypofuzz/corpus.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import abc
 import enum
 from random import Random
 from typing import (
     Callable,
     Counter,
     Dict,
+    FrozenSet,
     Iterable,
     List,
     Optional,
     Set,
     Tuple,
     Type,
     Union,
@@ -54,30 +55,41 @@
     return f"@reproduce_failure({hypothesis_version!r}, {encode_failure(buffer)!r})"
 
 
 class EngineStub:
     """A knock-off ConjectureEngine, just large enough to run a shrinker."""
 
     def __init__(
-        self, test_fn: Callable[[bytes], ConjectureData], random: Random
+        self,
+        test_fn: Callable[[bytes], ConjectureData],
+        random: Random,
+        passing_buffers: FrozenSet[bytes],
     ) -> None:
         self.cached_test_function = test_fn
         self.random = random
         self.call_count = 0
         self.report_debug_info = False
+        self.__passing_buffers = passing_buffers
 
     def debug(self, msg: str) -> None:
         """Unimplemented stub."""
 
     def explain_next_call_as(self, msg: str) -> None:
         """Unimplemented stub."""
 
     def clear_call_explanation(self) -> None:
         """Unimplemented stub."""
 
+    def passing_buffers(self, prefix: bytes = b"") -> FrozenSet[bytes]:
+        """Return a collection of bytestrings which cause the test to pass.
+
+        Optionally restrict this by a certain prefix, which is useful for explain mode.
+        """
+        return frozenset(b for b in self.__passing_buffers if b.startswith(prefix))
+
 
 class Pool:
     """Manage the seed pool for a fuzz target.
 
     The class tracks the minimal valid example which covers each known arc.
     """
 
@@ -157,16 +169,16 @@
         branches = result.extra_information.branches
         buf = result.buffer
 
         # If the example is "interesting", i.e. the test failed, add the buffer to
         # the database under Hypothesis' default key so it will be reproduced.
         if result.status == Status.INTERESTING:
             origin = result.interesting_origin
-            if origin not in self.interesting_examples or sort_key(result) < sort_key(
-                self.interesting_examples[origin]
+            if origin not in self.interesting_examples or (
+                sort_key(result) < sort_key(self.interesting_examples[origin][0])
             ):
                 self._database.save(self._key, result.buffer)
                 self.interesting_examples[origin] = (
                     result,
                     [
                         result.extra_information.call_repr,
                         result.extra_information.reports,
@@ -296,18 +308,19 @@
             # of incidental progress, where shrinking hard problems stumbles over
             # smaller starting points for the easy ones.
             arc_to_shrink = max(
                 set(self.covering_buffers) - minimal_branches,
                 key=lambda a: sort_key(self.covering_buffers[a]),
             )
             shrinker = Shrinker(
-                EngineStub(fn, random),
+                EngineStub(fn, random, passing_buffers=frozenset()),
                 self.results[self.covering_buffers[arc_to_shrink]],
                 predicate=lambda d, a=arc_to_shrink: a in d.extra_information.branches,
                 allow_transition=None,
+                explain=False,
             )
             shrinker.shrink()
             self.__shrunk_to_buffers.add(shrinker.shrink_target.buffer)
             minimal_branches |= {
                 arc
                 for arc, buf in self.covering_buffers.items()
                 if buf == shrinker.shrink_target.buffer
```

### Comparing `hypofuzz-23.5.2/src/hypofuzz/cov.py` & `hypofuzz-23.5.3/src/hypofuzz/cov.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/src/hypofuzz/dashboard.py` & `hypofuzz-23.5.3/src/hypofuzz/dashboard.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/src/hypofuzz/debugger.py` & `hypofuzz-23.5.3/src/hypofuzz/debugger.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/src/hypofuzz/entrypoint.py` & `hypofuzz-23.5.3/src/hypofuzz/entrypoint.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/src/hypofuzz/hy.py` & `hypofuzz-23.5.3/src/hypofuzz/hy.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from hypothesis.errors import StopTest, UnsatisfiedAssumption
 from hypothesis.internal.conjecture.data import ConjectureData, Status
 from hypothesis.internal.conjecture.engine import BUFFER_SIZE
 from hypothesis.internal.conjecture.junkdrawer import stack_depth_of_caller
 from hypothesis.internal.conjecture.shrinker import Shrinker
 from hypothesis.internal.reflection import function_digest, get_signature
 from hypothesis.reporting import with_reporter
+from hypothesis.vendor.pretty import RepresentationPrinter
 from sortedcontainers import SortedKeyList
 
 from .corpus import BlackBoxMutator, CrossOverMutator, EngineStub, HowGenerated, Pool
 from .cov import CustomCollectionContext
 
 record_pytrace: Optional[Callable[..., Any]]
 try:
@@ -193,25 +194,28 @@
         # database.  We do make it infrequent to manage the overhead though.
         if self.ninputs % 1000 == 0 and self.since_new_cov > 1000:
             self._replay_buffer.extend(self.pool.fetch())
 
         # seen_count = len(self.pool.arc_counts)
 
         # Run the input
-        result = self._run_test_on(self.generate_prefix())
+        result = self._run_test_on(self.generate_prefix(), extend=BUFFER_SIZE)
 
         if result.status is Status.INTERESTING:
             # Shrink to our minimal failing example, since we'll stop after this.
             self.shrinking = True
+            passing_buffers = frozenset(
+                b for b, r in self.pool.results.items() if r.status == Status.VALID
+            )
             shrinker = Shrinker(
-                EngineStub(self._run_test_on, self.random),
+                EngineStub(self._run_test_on, self.random, passing_buffers),
                 result,
                 predicate=lambda d: d.status is Status.INTERESTING,
                 allow_transition=None,
-                explain=True,
+                explain=False,  # TODO: enable explain mode
             )
             self.stop_shrinking_at = self.elapsed_time + 300
             with contextlib.suppress(HitShrinkTimeoutError):
                 shrinker.shrink()
             self.shrinking = False
             if record_pytrace:
                 # Replay minimal example under our time-travelling debug tracer
@@ -232,29 +236,34 @@
         # if len(self.pool.arc_counts) > seen_count and not self._early_blackbox_mode:
         #     self.pool.distill(self._run_test_on, self.random)
 
     def _run_test_on(
         self,
         buffer: bytes,
         *,
+        error_on_discard: bool = False,
+        extend: int = 0,
         source: HowGenerated = HowGenerated.shrinking,
         collector: Optional[contextlib.AbstractContextManager] = None,
     ) -> ConjectureData:
         """Run the test_fn on a given buffer of bytes, in a way a Shrinker can handle.
 
         In normal operation, it's called via run_one (above), but we might also
         delegate to the shrinker to find minimal covering examples.
         """
         start = time.perf_counter()
         self.ninputs += 1
         collector = collector or CustomCollectionContext()  # type: ignore
         assert collector is not None
         reports: List[str] = []
-        argstrings: List[str] = []
-        data = ConjectureData(max_length=BUFFER_SIZE, prefix=buffer, random=self.random)
+        data = ConjectureData(
+            max_length=min(BUFFER_SIZE, len(buffer) + extend),
+            prefix=buffer,
+            random=self.random,
+        )
         try:
             with deterministic_PRNG(), BuildContext(
                 data, is_final=True
             ) as context, constant_stack_depth(), with_reporter(reports.append):
                 # Note that the data generation and test execution happen in the same
                 # coverage context.  We may later split this, or tag each separately.
                 with collector:
@@ -265,17 +274,28 @@
                     kwargs = dict(self.__stuff.kwargs)
                     a, kw, argslices = context.prep_args_kwargs_from_strategies(
                         (), self.__stuff.given_kwargs
                     )
                     assert not a, "strategies all moved to kwargs by now"
                     kwargs.update(kw)
 
-                    # Save the repr of our arguments so they can be reported later
-                    argstrings.extend(map(repr, args))
-                    argstrings.extend(f"{k}={v!r}" for k, v in kwargs.items())
+                    printer = RepresentationPrinter(context=context)
+                    printer.repr_call(
+                        self.__test_fn.__name__,
+                        args,
+                        kwargs,
+                        force_split=True,
+                        arg_slices=argslices,
+                        leading_comment=(
+                            "# " + context.data.slice_comments[(0, 0)]
+                            if (0, 0) in context.data.slice_comments
+                            else None
+                        ),
+                    )
+                    data.extra_information.call_repr = printer.getvalue()
 
                     self.__test_fn(*args, **kwargs)
         except StopTest:
             data.status = Status.OVERRUN
         except UnsatisfiedAssumption:
             data.status = Status.INVALID
         except failure_exceptions_to_catch() as e:
@@ -283,17 +303,14 @@
             tb = get_trimmed_traceback()
             filename, lineno, *_ = traceback.extract_tb(tb)[-1]
             data.interesting_origin = (type(e), filename, lineno)
             data.extra_information.traceback = "".join(
                 traceback.format_exception(type(e), value=e, tb=tb)
             )
         finally:
-            data.extra_information.call_repr = (
-                self.__test_fn.__name__ + "(" + ", ".join(argstrings) + ")"
-            )
             data.extra_information.reports = "\n".join(map(str, reports))
 
         # In addition to coverage branches, use psudeo-coverage information provided via
         # the `hypothesis.event()` function - exploiting user-defined partitions
         # designed for diagnostic output to guide generation.  See
         # https://hypothesis.readthedocs.io/en/latest/details.html#hypothesis.event
         data.extra_information.branches = frozenset(
```

### Comparing `hypofuzz-23.5.2/src/hypofuzz/interface.py` & `hypofuzz-23.5.3/src/hypofuzz/interface.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/src/hypofuzz.egg-info/PKG-INFO` & `hypofuzz-23.5.3/src/hypofuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.5.2
+Version: 23.5.3
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.5.2/src/hypofuzz.egg-info/SOURCES.txt` & `hypofuzz-23.5.3/src/hypofuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/tests/test_corpus.py` & `hypofuzz-23.5.3/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.5.2/tests/test_version.py` & `hypofuzz-23.5.3/tests/test_version.py`

 * *Files identical despite different names*

