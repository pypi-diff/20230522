# Comparing `tmp/prefect_streamline-1.1.2.tar.gz` & `tmp/prefect_streamline-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_streamline-1.1.2.tar", max compression
+gzip compressed data, was "prefect_streamline-1.1.3.tar", max compression
```

## Comparing `prefect_streamline-1.1.2.tar` & `prefect_streamline-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1078 2023-03-27 08:54:31.939300 prefect_streamline-1.1.2/LICENSE
--rw-r--r--   0        0        0     3798 2023-03-27 08:54:31.939300 prefect_streamline-1.1.2/README.md
--rw-r--r--   0        0        0     1109 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/src/prefect_streamline/__init__.py
--rw-r--r--   0        0        0     1715 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/src/prefect_streamline/cli.py
--rw-r--r--   0        0        0        0 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/src/prefect_streamline/core/__init__.py
--rw-r--r--   0        0        0     3236 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/src/prefect_streamline/core/deploy.py
--rw-r--r--   0        0        0     2379 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/src/prefect_streamline/core/importutils.py
--rw-r--r--   0        0        0      956 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/src/prefect_streamline/core/waiting.py
--rw-r--r--   0        0        0     2054 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/src/prefect_streamline/deploybook.py
--rw-r--r--   0        0        0     1246 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/src/prefect_streamline/flowtest.py
--rw-r--r--   0        0        0        0 2023-03-27 08:54:31.943301 prefect_streamline-1.1.2/src/prefect_streamline/py.typed
--rw-r--r--   0        0        0     4785 1970-01-01 00:00:00.000000 prefect_streamline-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/LICENSE
+-rw-r--r--   0        0        0     3798 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/README.md
+-rw-r--r--   0        0        0     1103 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/src/prefect_streamline/__init__.py
+-rw-r--r--   0        0        0     1715 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/src/prefect_streamline/cli.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/src/prefect_streamline/core/__init__.py
+-rw-r--r--   0        0        0     3236 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/src/prefect_streamline/core/deploy.py
+-rw-r--r--   0        0        0     2379 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/src/prefect_streamline/core/importutils.py
+-rw-r--r--   0        0        0      956 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/src/prefect_streamline/core/waiting.py
+-rw-r--r--   0        0        0     2054 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/src/prefect_streamline/deploybook.py
+-rw-r--r--   0        0        0     1246 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/src/prefect_streamline/flowtest.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:00:22.384907 prefect_streamline-1.1.3/src/prefect_streamline/py.typed
+-rw-r--r--   0        0        0     4727 1970-01-01 00:00:00.000000 prefect_streamline-1.1.3/PKG-INFO
```

### Comparing `prefect_streamline-1.1.2/LICENSE` & `prefect_streamline-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_streamline-1.1.2/README.md` & `prefect_streamline-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `prefect_streamline-1.1.2/pyproject.toml` & `prefect_streamline-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prefect_streamline"
-version = "1.1.2"
+version = "1.1.3"
 description = "Prefect_Streamline is an opinionated extension that provides helpers to deploy and test Prefect flows quickly and easily."
 authors = ["Fabien Arcellier <fabien.arcellier@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "prefect_streamline", from = "src"}
 ]
@@ -16,16 +16,16 @@
     "Environment :: Console"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 prefect = "^2.8"
 click = "^8.1.3"
-requests = "^2.28.2"
-types-requests = "^2.28.11.16"
+requests = "^2.25.0"
+types-requests = "^2.25"
 
 [tool.poetry.scripts]
 prefect-streamline = 'prefect_streamline.cli:cli'
 
 [tool.poetry.group.dev.dependencies]
 alfred-cli = "^1.2.0"
 mypy = "^0.991"
```

### Comparing `prefect_streamline-1.1.2/src/prefect_streamline/cli.py` & `prefect_streamline-1.1.3/src/prefect_streamline/cli.py`

 * *Files identical despite different names*

### Comparing `prefect_streamline-1.1.2/src/prefect_streamline/core/deploy.py` & `prefect_streamline-1.1.3/src/prefect_streamline/core/deploy.py`

 * *Files identical despite different names*

### Comparing `prefect_streamline-1.1.2/src/prefect_streamline/core/importutils.py` & `prefect_streamline-1.1.3/src/prefect_streamline/core/importutils.py`

 * *Files identical despite different names*

### Comparing `prefect_streamline-1.1.2/src/prefect_streamline/core/waiting.py` & `prefect_streamline-1.1.3/src/prefect_streamline/core/waiting.py`

 * *Files identical despite different names*

### Comparing `prefect_streamline-1.1.2/src/prefect_streamline/deploybook.py` & `prefect_streamline-1.1.3/src/prefect_streamline/deploybook.py`

 * *Files identical despite different names*

### Comparing `prefect_streamline-1.1.2/src/prefect_streamline/flowtest.py` & `prefect_streamline-1.1.3/src/prefect_streamline/flowtest.py`

 * *Files identical despite different names*

### Comparing `prefect_streamline-1.1.2/PKG-INFO` & `prefect_streamline-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: prefect-streamline
-Version: 1.1.2
+Version: 1.1.3
 Summary: Prefect_Streamline is an opinionated extension that provides helpers to deploy and test Prefect flows quickly and easily.
 License: MIT
 Author: Fabien Arcellier
 Author-email: fabien.arcellier@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: prefect (>=2.8,<3.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: types-requests (>=2.28.11.16,<3.0.0.0)
+Requires-Dist: requests (>=2.25.0,<3.0.0)
+Requires-Dist: types-requests (>=2.25,<3.0)
 Description-Content-Type: text/markdown
 
 ## prefect streamline
 
 prefect_streamline is an opinionated extension that provides helpers to deploy and test Prefect flows quickly and easily.
 
 With its deployment and testing features, you can easily ensure the quality and reliability of your workflows before deploying them.
```

