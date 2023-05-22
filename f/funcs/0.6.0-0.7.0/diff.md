# Comparing `tmp/funcs-0.6.0.tar.gz` & `tmp/funcs-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.6.0.tar", max compression
+gzip compressed data, was "funcs-0.7.0.tar", max compression
```

## Comparing `funcs-0.6.0.tar` & `funcs-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1092 2023-05-21 12:34:46.585748 funcs-0.6.0/LICENSE
--rw-r--r--   0        0        0     2872 2023-05-21 12:34:46.585748 funcs-0.6.0/README.md
--rw-r--r--   0        0        0     1714 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/__init__.py
--rw-r--r--   0        0        0      883 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/application.py
--rw-r--r--   0        0        0      857 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/callers.py
--rw-r--r--   0        0        0     5470 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/composition.py
--rw-r--r--   0        0        0      832 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/debug.py
--rw-r--r--   0        0        0      166 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/decorators.py
--rw-r--r--   0        0        0     6369 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/flow.py
--rw-r--r--   0        0        0     2260 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/functions.py
--rw-r--r--   0        0        0      418 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/getters.py
--rw-r--r--   0        0        0      782 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/primitives.py
--rw-r--r--   0        0        0        0 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/py.typed
--rw-r--r--   0        0        0     1113 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/reduction.py
--rw-r--r--   0        0        0     1031 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/types.py
--rw-r--r--   0        0        0     2346 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/unpacking.py
--rw-r--r--   0        0        0     3175 2023-05-21 12:34:46.589748 funcs-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 funcs-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-22 18:25:43.599021 funcs-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2872 2023-05-22 18:25:43.599021 funcs-0.7.0/README.md
+-rw-r--r--   0        0        0     1714 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/application.py
+-rw-r--r--   0        0        0      857 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/callers.py
+-rw-r--r--   0        0        0     5470 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/composition.py
+-rw-r--r--   0        0        0      832 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/debug.py
+-rw-r--r--   0        0        0      436 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/decorators.py
+-rw-r--r--   0        0        0     6369 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/flow.py
+-rw-r--r--   0        0        0     2260 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/functions.py
+-rw-r--r--   0        0        0      418 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/getters.py
+-rw-r--r--   0        0        0      782 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/py.typed
+-rw-r--r--   0        0        0     1113 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/reduction.py
+-rw-r--r--   0        0        0     1031 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/types.py
+-rw-r--r--   0        0        0     2346 2023-05-22 18:25:43.603021 funcs-0.7.0/funcs/unpacking.py
+-rw-r--r--   0        0        0     3212 2023-05-22 18:25:43.603021 funcs-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 funcs-0.7.0/PKG-INFO
```

### Comparing `funcs-0.6.0/LICENSE` & `funcs-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/README.md` & `funcs-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.6.0"
+funcs = "^0.7.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

### Comparing `funcs-0.6.0/funcs/__init__.py` & `funcs-0.7.0/funcs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Functional programming in Python."
 __url__ = "https://github.com/nekitdev/funcs"
 
 __title__ = "funcs"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 from funcs.application import apply, partial
 from funcs.callers import caller, method_caller
 from funcs.composition import compose, compose_once, pipe, pipe_once
 from funcs.debug import inspect, tap
 from funcs.decorators import wraps
 from funcs.flow import once, post_processing, reraise, reraise_with, suppress, wrap_with
```

### Comparing `funcs-0.6.0/funcs/application.py` & `funcs-0.7.0/funcs/application.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/funcs/callers.py` & `funcs-0.7.0/funcs/callers.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/funcs/composition.py` & `funcs-0.7.0/funcs/composition.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/funcs/debug.py` & `funcs-0.7.0/funcs/debug.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/funcs/flow.py` & `funcs-0.7.0/funcs/flow.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/funcs/functions.py` & `funcs-0.7.0/funcs/functions.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/funcs/primitives.py` & `funcs-0.7.0/funcs/primitives.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/funcs/reduction.py` & `funcs-0.7.0/funcs/reduction.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/funcs/types.py` & `funcs-0.7.0/funcs/types.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/funcs/unpacking.py` & `funcs-0.7.0/funcs/unpacking.py`

 * *Files identical despite different names*

### Comparing `funcs-0.6.0/pyproject.toml` & `funcs-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcs"
-version = "0.6.0"
+version = "0.7.0"
 description = "Functional programming in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/funcs"
@@ -28,15 +28,15 @@
 
 [[tool.poetry.packages]]
 include = "funcs"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
-typing-aliases = ">= 1.1.1"
+typing-aliases = ">= 1.1.2"
 typing-extensions = ">= 4.5.0"
 
 solus = ">= 1.1.0"
 
 [tool.poetry.group.format]
 optional = true
 
@@ -79,14 +79,17 @@
 
 [tool.poetry.group.dev.dependencies]
 changelogging = "1.3.0"
 
 [tool.black]
 line_length = 100
 
+[tool.flake8]
+max_line_length = 100
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "--cov funcs"
 testpaths = ["tests"]
@@ -133,15 +136,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "funcs"
-version = "0.6.0"
+version = "0.7.0"
 url = "https://github.com/nekitdev/funcs"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `funcs-0.6.0/PKG-INFO` & `funcs-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs
-Version: 0.6.0
+Version: 0.7.0
 Summary: Functional programming in Python.
 Home-page: https://github.com/nekitdev/funcs
 License: MIT
 Keywords: python,function,functional,paradigm
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: solus (>=1.1.0)
-Requires-Dist: typing-aliases (>=1.1.1)
+Requires-Dist: typing-aliases (>=1.1.2)
 Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/funcs
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/funcs/issues
 Project-URL: Repository, https://github.com/nekitdev/funcs
 Description-Content-Type: text/markdown
@@ -71,15 +71,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.6.0"
+funcs = "^0.7.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

