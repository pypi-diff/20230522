# Comparing `tmp/checkmk_dev_tools-0.1.3.tar.gz` & `tmp/checkmk_dev_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkmk_dev_tools-0.1.3.tar", max compression
+gzip compressed data, was "checkmk_dev_tools-0.1.4.tar", max compression
```

## Comparing `checkmk_dev_tools-0.1.3.tar` & `checkmk_dev_tools-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1056 2023-05-17 11:57:16.555506 checkmk_dev_tools-0.1.3/README.rst
--rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.3/cmk_dev/__init__.py
--rwxr-xr-x   0        0        0    11148 2023-05-22 12:22:21.988260 checkmk_dev_tools-0.1.3/cmk_dev/ci_artifacts.py
--rwxr-xr-x   0        0        0     2184 2023-05-10 11:28:30.476996 checkmk_dev_tools-0.1.3/cmk_dev/cli.py
--rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.3/cmk_dev/listen_std.py
--rw-r--r--   0        0        0     1919 2023-05-22 12:23:43.480644 checkmk_dev_tools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-17 11:57:16.555506 checkmk_dev_tools-0.1.4/README.rst
+-rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.4/cmk_dev/__init__.py
+-rwxr-xr-x   0        0        0    11148 2023-05-22 12:22:21.988260 checkmk_dev_tools-0.1.4/cmk_dev/ci_artifacts.py
+-rwxr-xr-x   0        0        0     2184 2023-05-10 11:28:30.476996 checkmk_dev_tools-0.1.4/cmk_dev/cli.py
+-rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.4/cmk_dev/listen_std.py
+-rw-r--r--   0        0        0     1919 2023-05-22 12:55:27.493637 checkmk_dev_tools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.4/PKG-INFO
```

### Comparing `checkmk_dev_tools-0.1.3/README.rst` & `checkmk_dev_tools-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.3/cmk_dev/ci_artifacts.py` & `checkmk_dev_tools-0.1.4/cmk_dev/ci_artifacts.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.3/cmk_dev/cli.py` & `checkmk_dev_tools-0.1.4/cmk_dev/cli.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.3/cmk_dev/listen_std.py` & `checkmk_dev_tools-0.1.4/cmk_dev/listen_std.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.3/pyproject.toml` & `checkmk_dev_tools-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "checkmk_dev_tools"
-version = "0.1.3"
+name = "checkmk-dev-tools"
+version = "0.1.4"
 description = "Checkmk DevOps tools"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/tribe29/checkmk"
 readme = "README.rst"
 packages = [
   {include = "cmk_dev/**/*.py"}
 ]
```

### Comparing `checkmk_dev_tools-0.1.3/PKG-INFO` & `checkmk_dev_tools-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkmk-dev-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Checkmk DevOps tools
 Home-page: https://github.com/tribe29/checkmk
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

