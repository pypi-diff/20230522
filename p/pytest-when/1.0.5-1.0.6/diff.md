# Comparing `tmp/pytest_when-1.0.5.tar.gz` & `tmp/pytest_when-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_when-1.0.5.tar", last modified: Fri May 19 18:46:58 2023, max compression
+gzip compressed data, was "pytest_when-1.0.6.tar", last modified: Mon May 22 12:49:34 2023, max compression
```

## Comparing `pytest_when-1.0.5.tar` & `pytest_when-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11342 2023-05-19 18:46:22.374647 pytest_when-1.0.5/LICENSE
--rw-r--r--   0        0        0     2709 2023-05-19 18:46:22.374647 pytest_when-1.0.5/README.md
--rw-r--r--   0        0        0     2776 2023-05-19 18:46:58.727794 pytest_when-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 18:46:22.374647 pytest_when-1.0.5/pytest_when/__init__.py
--rw-r--r--   0        0        0       45 2023-05-19 18:46:22.374647 pytest_when-1.0.5/pytest_when/plugin.py
--rw-r--r--   0        0        0        0 2023-05-19 18:46:22.374647 pytest_when-1.0.5/pytest_when/py.typed
--rw-r--r--   0        0        0    10667 2023-05-19 18:46:22.374647 pytest_when-1.0.5/pytest_when/when.py
--rw-r--r--   0        0        0        0 2023-05-19 18:46:22.374647 pytest_when-1.0.5/tests/resources/__init__.py
--rw-r--r--   0        0        0      131 2023-05-19 18:46:22.374647 pytest_when-1.0.5/tests/resources/example_module.py
--rw-r--r--   0        0        0     2492 2023-05-19 18:46:22.374647 pytest_when-1.0.5/tests/test_create_call_key.py
--rw-r--r--   0        0        0     5848 2023-05-19 18:46:22.374647 pytest_when-1.0.5/tests/test_integration.py
--rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 pytest_when-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-22 12:48:58.509722 pytest_when-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2709 2023-05-22 12:48:58.509722 pytest_when-1.0.6/README.md
+-rw-r--r--   0        0        0     2766 2023-05-22 12:49:34.722300 pytest_when-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 12:48:58.509722 pytest_when-1.0.6/pytest_when/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-22 12:48:58.509722 pytest_when-1.0.6/pytest_when/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-22 12:48:58.509722 pytest_when-1.0.6/pytest_when/py.typed
+-rw-r--r--   0        0        0    10667 2023-05-22 12:48:58.509722 pytest_when-1.0.6/pytest_when/when.py
+-rw-r--r--   0        0        0        0 2023-05-22 12:48:58.509722 pytest_when-1.0.6/tests/resources/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-22 12:48:58.509722 pytest_when-1.0.6/tests/resources/example_module.py
+-rw-r--r--   0        0        0     2492 2023-05-22 12:48:58.509722 pytest_when-1.0.6/tests/test_create_call_key.py
+-rw-r--r--   0        0        0     5848 2023-05-22 12:48:58.509722 pytest_when-1.0.6/tests/test_integration.py
+-rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 pytest_when-1.0.6/PKG-INFO
```

### Comparing `pytest_when-1.0.5/LICENSE` & `pytest_when-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.5/README.md` & `pytest_when-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.5/pyproject.toml` & `pytest_when-1.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -133,36 +133,35 @@
     "pre-commit>=2.21.0",
     "black>=23.3.0",
     "isort>=5.11.5",
     "mypy>=1.2.0",
     "ruff>=0.0.263",
 ]
 test = [
-    "pytest>=7.3.1",
     "pytest-cov>=4.0.0",
-    "pytest-mock>=3.10.0",
 ]
 
 [tool.pdm.version]
 source = "scm"
 
 [project]
 name = "pytest_when"
 dynamic = []
 description = "Utility which makes mocking more readable and controllable"
 authors = [
     { name = "zhukovgreen", email = "iam+pytest-when@zhukovgreen.pro" },
 ]
 dependencies = [
-    "environs>=9.5.0",
-    "pip>=23.1.2",
+    "pytest>=7.3.1",
+    "pytest-mock>=3.10.0",
+    "typing-extensions>=4.5.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "1.0.5"
+version = "1.0.6"
 
 [project.entry-points.pytest11]
 pytest-when = "pytest_when.plugin"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/pytest-when"
```

### Comparing `pytest_when-1.0.5/pytest_when/when.py` & `pytest_when-1.0.6/pytest_when/when.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.5/tests/test_create_call_key.py` & `pytest_when-1.0.6/tests/test_create_call_key.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.5/tests/test_integration.py` & `pytest_when-1.0.6/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.5/PKG-INFO` & `pytest_when-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pytest-when
-Version: 1.0.5
+Version: 1.0.6
 Summary: Utility which makes mocking more readable and controllable
 Author-Email: zhukovgreen <iam+pytest-when@zhukovgreen.pro>
 Project-URL: Repository, https://github.com/zhukovgreen/pytest-when
 Requires-Python: >=3.8
-Requires-Dist: environs>=9.5.0
-Requires-Dist: pip>=23.1.2
+Requires-Dist: pytest>=7.3.1
+Requires-Dist: pytest-mock>=3.10.0
+Requires-Dist: typing-extensions>=4.5.0
 Description-Content-Type: text/markdown
 
 # pytest-when
 
 Plugin provides a `when` fixture, which enables the following way of mocking
 the python objects:
```

