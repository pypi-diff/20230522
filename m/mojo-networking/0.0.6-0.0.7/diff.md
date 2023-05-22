# Comparing `tmp/mojo-networking-0.0.6.tar.gz` & `tmp/mojo_networking-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo-networking-0.0.6.tar", max compression
+gzip compressed data, was "mojo_networking-0.0.7.tar", max compression
```

## Comparing `mojo-networking-0.0.6.tar` & `mojo_networking-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-03-20 16:35:27.038935 mojo-networking-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0      117 2023-03-20 16:35:27.038935 mojo-networking-0.0.6/README.md
--rw-r--r--   0        0        0      732 2023-05-16 02:32:28.081996 mojo-networking-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      500 2023-03-18 15:00:54.917241 mojo-networking-0.0.6/source/packages/mojo/networking/__init__.py
--rw-r--r--   0        0        0      613 2023-03-16 19:03:22.304009 mojo-networking-0.0.6/source/packages/mojo/networking/broadcast.py
--rw-r--r--   0        0        0     6959 2023-03-21 03:13:45.813161 mojo-networking-0.0.6/source/packages/mojo/networking/constants.py
--rw-r--r--   0        0        0     2910 2023-03-21 03:23:12.561679 mojo-networking-0.0.6/source/packages/mojo/networking/exceptions.py
--rw-r--r--   0        0        0     9204 2023-03-16 19:03:34.088103 mojo-networking-0.0.6/source/packages/mojo/networking/interfaces.py
--rw-r--r--   0        0        0     8824 2023-03-20 16:43:41.819833 mojo-networking-0.0.6/source/packages/mojo/networking/multicast.py
--rw-r--r--   0        0        0     2381 2023-03-17 14:58:49.355462 mojo-networking-0.0.6/source/packages/mojo/networking/resolution.py
--rw-r--r--   0        0        0     1845 2023-03-19 21:36:12.292413 mojo-networking-0.0.6/source/packages/mojo/networking/trafficcapturecontext.py
--rw-r--r--   0        0        0     4543 2023-03-20 16:43:44.355824 mojo-networking-0.0.6/source/packages/mojo/networking/unicast.py
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 mojo-networking-0.0.6/setup.py
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 mojo-networking-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-20 16:35:27.038935 mojo_networking-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      117 2023-03-20 16:35:27.038935 mojo_networking-0.0.7/README.md
+-rw-r--r--   0        0        0      882 2023-05-21 03:45:55.343446 mojo_networking-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      500 2023-03-18 15:00:54.917241 mojo_networking-0.0.7/source/packages/mojo/networking/__init__.py
+-rw-r--r--   0        0        0      613 2023-03-16 19:03:22.304009 mojo_networking-0.0.7/source/packages/mojo/networking/broadcast.py
+-rw-r--r--   0        0        0     6959 2023-03-21 03:13:45.813161 mojo_networking-0.0.7/source/packages/mojo/networking/constants.py
+-rw-r--r--   0        0        0     2910 2023-03-21 03:23:12.561679 mojo_networking-0.0.7/source/packages/mojo/networking/exceptions.py
+-rw-r--r--   0        0        0     9204 2023-03-16 19:03:34.088103 mojo_networking-0.0.7/source/packages/mojo/networking/interfaces.py
+-rw-r--r--   0        0        0     8824 2023-03-20 16:43:41.819833 mojo_networking-0.0.7/source/packages/mojo/networking/multicast.py
+-rw-r--r--   0        0        0     2381 2023-03-17 14:58:49.355462 mojo_networking-0.0.7/source/packages/mojo/networking/resolution.py
+-rw-r--r--   0        0        0     1845 2023-03-19 21:36:12.292413 mojo_networking-0.0.7/source/packages/mojo/networking/trafficcapturecontext.py
+-rw-r--r--   0        0        0     4543 2023-03-20 16:43:44.355824 mojo_networking-0.0.7/source/packages/mojo/networking/unicast.py
+-rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 mojo_networking-0.0.7/setup.py
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 mojo_networking-0.0.7/PKG-INFO
```

### Comparing `mojo-networking-0.0.6/LICENSE.txt` & `mojo_networking-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo-networking-0.0.6/pyproject.toml` & `mojo_networking-0.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [tool.poetry]
 name = "mojo-networking"
 description = "Automation Mojo Netorking Package (mojo-networking)"
-version = "0.0.6"
-authors = []
+version = "0.0.7"
+authors = [
+    "Myron Walker <myron.walker@gmail.com>"
+]
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
 ]
 keywords = [
     "python"
 ]
 packages = [{include="mojo", from="source/packages"}]
 
+homepage = "http://automationmojo.com"
+repository = "https://github.com/automationmojo/mojo-networking"
+
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 netifaces = "^0.11.0"
 requests = "<=2.29.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
```

### Comparing `mojo-networking-0.0.6/source/packages/mojo/networking/broadcast.py` & `mojo_networking-0.0.7/source/packages/mojo/networking/broadcast.py`

 * *Files identical despite different names*

### Comparing `mojo-networking-0.0.6/source/packages/mojo/networking/constants.py` & `mojo_networking-0.0.7/source/packages/mojo/networking/constants.py`

 * *Files identical despite different names*

### Comparing `mojo-networking-0.0.6/source/packages/mojo/networking/exceptions.py` & `mojo_networking-0.0.7/source/packages/mojo/networking/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo-networking-0.0.6/source/packages/mojo/networking/interfaces.py` & `mojo_networking-0.0.7/source/packages/mojo/networking/interfaces.py`

 * *Files identical despite different names*

### Comparing `mojo-networking-0.0.6/source/packages/mojo/networking/multicast.py` & `mojo_networking-0.0.7/source/packages/mojo/networking/multicast.py`

 * *Files identical despite different names*

### Comparing `mojo-networking-0.0.6/source/packages/mojo/networking/resolution.py` & `mojo_networking-0.0.7/source/packages/mojo/networking/resolution.py`

 * *Files identical despite different names*

### Comparing `mojo-networking-0.0.6/source/packages/mojo/networking/trafficcapturecontext.py` & `mojo_networking-0.0.7/source/packages/mojo/networking/trafficcapturecontext.py`

 * *Files identical despite different names*

### Comparing `mojo-networking-0.0.6/source/packages/mojo/networking/unicast.py` & `mojo_networking-0.0.7/source/packages/mojo/networking/unicast.py`

 * *Files identical despite different names*

### Comparing `mojo-networking-0.0.6/setup.py` & `mojo_networking-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 {'': ['*']}
 
 install_requires = \
 ['netifaces>=0.11.0,<0.12.0', 'requests<=2.29.0']
 
 setup_kwargs = {
     'name': 'mojo-networking',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Automation Mojo Netorking Package (mojo-networking)',
     'long_description': '# python-package-template\nThis is a template repository that can be used to quickly create a python package project.\n',
-    'author': 'None',
-    'author_email': 'None',
+    'author': 'Myron Walker',
+    'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'http://automationmojo.com',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `mojo-networking-0.0.6/PKG-INFO` & `mojo_networking-0.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: mojo-networking
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automation Mojo Netorking Package (mojo-networking)
+Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python
+Author: Myron Walker
+Author-email: myron.walker@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: requests (<=2.29.0)
+Project-URL: Repository, https://github.com/automationmojo/mojo-networking
 Description-Content-Type: text/markdown
 
 # python-package-template
 This is a template repository that can be used to quickly create a python package project.
```

