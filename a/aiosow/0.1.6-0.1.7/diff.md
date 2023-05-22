# Comparing `tmp/aiosow-0.1.6.tar.gz` & `tmp/aiosow-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosow-0.1.6.tar", last modified: Tue May 16 12:04:04 2023, max compression
+gzip compressed data, was "aiosow-0.1.7.tar", last modified: Mon May 22 14:55:29 2023, max compression
```

## Comparing `aiosow-0.1.6.tar` & `aiosow-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:03.998016 aiosow-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 12:04:03.998016 aiosow-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-16 12:03:52.000000 aiosow-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:03.994016 aiosow-0.1.6/aiosow/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:03.998016 aiosow-0.1.6/aiosow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:04:03.998016 aiosow-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 12:03:52.000000 aiosow-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:03.998016 aiosow-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:29.705353 aiosow-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 14:55:29.705353 aiosow-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-22 14:55:15.000000 aiosow-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:29.701353 aiosow-0.1.7/aiosow/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:29.701353 aiosow-0.1.7/aiosow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:55:29.705353 aiosow-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-22 14:55:15.000000 aiosow-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:29.705353 aiosow-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_setup.py
```

### Comparing `aiosow-0.1.6/PKG-INFO` & `aiosow-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.6
+Version: 0.1.7
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.6/README.md` & `aiosow-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/aiosow/autofill.py` & `aiosow-0.1.7/aiosow/autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/aiosow/bindings.py` & `aiosow-0.1.7/aiosow/bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/aiosow/command.py` & `aiosow-0.1.7/aiosow/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from aiosow.routines import spawn_routine_consumer
 
 
 def load_composition(composition=None, **kwargs):
     debug = (
         "-d" in sys.argv
         or "--debug" in sys.argv
-        or any(arg.find("-d") != -1 or arg.find("--debug") != -1 for arg in sys.argv)
+        or any(
+            arg.find("-d") != -1 or arg.find("--debug") != -1
+            for arg in sys.argv
+        )
     )
     if "--log" in sys.argv or kwargs.get("log", False):
         logging.basicConfig(
             level=logging.DEBUG if debug else logging.INFO,
             format="[%(asctime)s][%(levelname)s] \t%(message)s",
             datefmt="%H:%M:%S",
         )
@@ -44,15 +47,17 @@
     parser.add_argument(
         "--log", help="Displays logs", action="store_true", default=False
     )
     try:
         if not composition:
             composition = sys.argv[1]
         composition = (
-            f"{composition}.bindings" if not ".bindings" in composition else composition
+            f"{composition}.bindings"
+            if not ".bindings" in composition
+            else composition
         )
         importlib.import_module(composition)
     except Exception as e:
         logging.error("An error occured opening the composition")
         raise (e)
     for module_name in sys.modules.keys():
         if "bindings" in module_name and "aiosow" not in module_name:
```

### Comparing `aiosow-0.1.6/aiosow/options.py` & `aiosow-0.1.7/aiosow/options.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/aiosow/perpetuate.py` & `aiosow-0.1.7/aiosow/perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/aiosow/routines.py` & `aiosow-0.1.7/aiosow/routines.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from typing import Callable, Union
 from functools import wraps
 
 import asyncio, logging
 
 from aiosow.perpetuate import perpetuate, autofill
 from aiosow.bindings import return_true
 from aiosow.setup import trigger_routines
@@ -43,15 +43,15 @@
 
 def get_routines():
     global ROUTINES
     return ROUTINES
 
 
 def routine(
-    frequency: int | float,
+    frequency: Union[int, float],
     condition: Callable = return_true,
     timeout: int = -1,
     perpetuate=True,
 ) -> Callable:
     """
     Specifies a function to be executed as a routine.
     **args**:
@@ -84,15 +84,17 @@
 
     # Wait until the smallest timeout has elapsed
     await asyncio.sleep(smallest_timeout)
 
     # Execute any routines that have timed out
     for routine in routines:
         routine["timeout"] -= smallest_timeout
-        routine["timeout"] = 0 if routine["timeout"] < 0 else routine["timeout"]
+        routine["timeout"] = (
+            0 if routine["timeout"] < 0 else routine["timeout"]
+        )
         if routine["timeout"] <= 0:
             condition = routine["condition"]
             function = routine["function"]
             # Check the condition before running the routine
             try:
                 if await autofill(condition, args=[], memory=memory):
                     if routine["perpetuate"]:
```

### Comparing `aiosow-0.1.6/aiosow/setup.py` & `aiosow-0.1.7/aiosow/setup.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/aiosow.egg-info/PKG-INFO` & `aiosow-0.1.7/aiosow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.6
+Version: 0.1.7
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.6/setup.py` & `aiosow-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="aiosow",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(include=["aiosow"]),
     description="An event-based framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     entry_points={
         "console_scripts": [
```

### Comparing `aiosow-0.1.6/tests/test_autofill.py` & `aiosow-0.1.7/tests/test_autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/tests/test_bindings.py` & `aiosow-0.1.7/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/tests/test_perpetuate.py` & `aiosow-0.1.7/tests/test_perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/tests/test_routines.py` & `aiosow-0.1.7/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.6/tests/test_setup.py` & `aiosow-0.1.7/tests/test_setup.py`

 * *Files identical despite different names*

