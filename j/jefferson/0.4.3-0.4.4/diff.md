# Comparing `tmp/jefferson-0.4.3.tar.gz` & `tmp/jefferson-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jefferson-0.4.3.tar", max compression
+gzip compressed data, was "jefferson-0.4.4.tar", max compression
```

## Comparing `jefferson-0.4.3.tar` & `jefferson-0.4.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1083 2023-05-10 06:39:36.328341 jefferson-0.4.3/LICENSE
--rwxr-xr-x   0        0        0      965 2023-05-10 06:39:36.328341 jefferson-0.4.3/README.md
--rw-r--r--   0        0        0        0 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/__init__.py
--rw-r--r--   0        0        0     1792 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/cli.py
--rw-r--r--   0        0        0        0 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/compression/__init__.py
--rw-r--r--   0        0        0      395 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/compression/jffs2_lzma.py
--rw-r--r--   0        0        0      829 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/compression/rtime.py
--rw-r--r--   0        0        0        0 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/core/__init__.py
--rw-r--r--   0        0        0    16776 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/jffs2.py
--rw-r--r--   0        0        0      825 2023-05-10 06:39:36.328341 jefferson-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 jefferson-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-22 19:56:39.859706 jefferson-0.4.4/LICENSE
+-rwxr-xr-x   0        0        0      965 2023-05-22 19:56:39.863706 jefferson-0.4.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/__init__.py
+-rw-r--r--   0        0        0     1792 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/cli.py
+-rw-r--r--   0        0        0        0 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/compression/__init__.py
+-rw-r--r--   0        0        0      395 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/compression/jffs2_lzma.py
+-rw-r--r--   0        0        0      829 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/compression/rtime.py
+-rw-r--r--   0        0        0        0 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/core/__init__.py
+-rw-r--r--   0        0        0    16776 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/jffs2.py
+-rw-r--r--   0        0        0      825 2023-05-22 19:56:39.863706 jefferson-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 jefferson-0.4.4/PKG-INFO
```

### Comparing `jefferson-0.4.3/LICENSE` & `jefferson-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.3/README.md` & `jefferson-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.3/jefferson/cli.py` & `jefferson-0.4.4/jefferson/cli.py`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.3/jefferson/compression/rtime.py` & `jefferson-0.4.4/jefferson/compression/rtime.py`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.3/jefferson/jffs2.py` & `jefferson-0.4.4/jefferson/jffs2.py`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.3/pyproject.toml` & `jefferson-0.4.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "jefferson"
-version = "0.4.3"
+version = "0.4.4"
 description = "JFFS2 filesystem extraction tool."
 authors = ["ONEKEY <support@onekey.com>", "Stefan Viehböck <support@onekey.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "jefferson" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 cstruct = "^5.2"
 click = "^8.1.3"
-lzallright = "^0.1.0"
+lzallright = "^0.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `jefferson-0.4.3/PKG-INFO` & `jefferson-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: jefferson
-Version: 0.4.3
+Version: 0.4.4
 Summary: JFFS2 filesystem extraction tool.
 License: MIT
 Author: ONEKEY
 Author-email: support@onekey.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cstruct (>=5.2,<6.0)
-Requires-Dist: lzallright (>=0.1.0,<0.2.0)
+Requires-Dist: lzallright (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 ## Jefferson
 
 JFFS2 filesystem extraction tool.
 
 ### Installation
```

