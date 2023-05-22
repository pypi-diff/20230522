# Comparing `tmp/otools-rpc-0.2.2.tar.gz` & `tmp/otools-rpc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otools-rpc-0.2.2.tar", last modified: Mon May 22 12:08:19 2023, max compression
+gzip compressed data, was "otools-rpc-0.2.3.tar", last modified: Mon May 22 12:30:55 2023, max compression
```

## Comparing `otools-rpc-0.2.2.tar` & `otools-rpc-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:08:19.763942 otools-rpc-0.2.2/
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     1074 2023-05-22 09:23:28.000000 otools-rpc-0.2.2/LICENSE.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     2791 2023-05-22 12:08:19.763942 otools-rpc-0.2.2/PKG-INFO
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     2297 2023-05-22 09:12:06.000000 otools-rpc-0.2.2/README.md
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:08:19.763942 otools-rpc-0.2.2/otools_rpc/
--rw-rw-r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 09:21:22.000000 otools-rpc-0.2.2/otools_rpc/__init__.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:08:19.763942 otools-rpc-0.2.2/otools_rpc.egg-info/
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     2791 2023-05-22 12:08:19.000000 otools-rpc-0.2.2/otools_rpc.egg-info/PKG-INFO
--rw-rw-r--   0 opennet   (1000) opennet   (1000)      222 2023-05-22 12:08:19.000000 otools-rpc-0.2.2/otools_rpc.egg-info/SOURCES.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)        1 2023-05-22 12:08:19.000000 otools-rpc-0.2.2/otools_rpc.egg-info/dependency_links.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       46 2023-05-22 12:08:19.000000 otools-rpc-0.2.2/otools_rpc.egg-info/requires.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       11 2023-05-22 12:08:19.000000 otools-rpc-0.2.2/otools_rpc.egg-info/top_level.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-05-22 12:08:19.763942 otools-rpc-0.2.2/setup.cfg
--rw-rw-r--   0 opennet   (1000) opennet   (1000)      833 2023-05-22 12:08:18.000000 otools-rpc-0.2.2/setup.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:30:55.079167 otools-rpc-0.2.3/
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     1074 2023-05-22 09:23:28.000000 otools-rpc-0.2.3/LICENSE.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     2791 2023-05-22 12:30:55.079167 otools-rpc-0.2.3/PKG-INFO
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     2297 2023-05-22 12:30:12.000000 otools-rpc-0.2.3/README.md
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:30:55.075167 otools-rpc-0.2.3/otools_rpc/
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 09:21:22.000000 otools-rpc-0.2.3/otools_rpc/__init__.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:30:55.079167 otools-rpc-0.2.3/otools_rpc/external_api/
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)       39 2023-05-22 09:24:49.000000 otools-rpc-0.2.3/otools_rpc/external_api/__init__.py
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)      959 2023-05-22 08:31:48.000000 otools-rpc-0.2.3/otools_rpc/external_api/common.py
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     4816 2023-05-22 08:38:48.000000 otools-rpc-0.2.3/otools_rpc/external_api/environment.py
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     6037 2023-05-22 09:13:04.000000 otools-rpc-0.2.3/otools_rpc/external_api/recordset.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:30:55.075167 otools-rpc-0.2.3/otools_rpc.egg-info/
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     2791 2023-05-22 12:30:55.000000 otools-rpc-0.2.3/otools_rpc.egg-info/PKG-INFO
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)      368 2023-05-22 12:30:55.000000 otools-rpc-0.2.3/otools_rpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)        1 2023-05-22 12:30:55.000000 otools-rpc-0.2.3/otools_rpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)       46 2023-05-22 12:30:55.000000 otools-rpc-0.2.3/otools_rpc.egg-info/requires.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)       11 2023-05-22 12:30:55.000000 otools-rpc-0.2.3/otools_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-05-22 12:30:55.079167 otools-rpc-0.2.3/setup.cfg
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)      828 2023-05-22 12:29:44.000000 otools-rpc-0.2.3/setup.py
```

### Comparing `otools-rpc-0.2.2/LICENSE.txt` & `otools-rpc-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.2.2/PKG-INFO` & `otools-rpc-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # otools-rpc
 
-[![Version](https://img.shields.io/badge/version-0.2.1-blue.svg)](https://pypi.org/project/otools-rpc/)
+[![Version](https://img.shields.io/badge/version-0.2.3-blue.svg)](https://pypi.org/project/otools-rpc/)
 [![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://pypi.org/project/otools-rpc/)
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
```

### Comparing `otools-rpc-0.2.2/README.md` & `otools-rpc-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # otools-rpc
 
-[![Version](https://img.shields.io/badge/version-0.2.1-blue.svg)](https://pypi.org/project/otools-rpc/)
+[![Version](https://img.shields.io/badge/version-0.2.3-blue.svg)](https://pypi.org/project/otools-rpc/)
 [![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://pypi.org/project/otools-rpc/)
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
```

### Comparing `otools-rpc-0.2.2/otools_rpc.egg-info/PKG-INFO` & `otools-rpc-0.2.3/otools_rpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # otools-rpc
 
-[![Version](https://img.shields.io/badge/version-0.2.1-blue.svg)](https://pypi.org/project/otools-rpc/)
+[![Version](https://img.shields.io/badge/version-0.2.3-blue.svg)](https://pypi.org/project/otools-rpc/)
 [![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://pypi.org/project/otools-rpc/)
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
```

### Comparing `otools-rpc-0.2.2/setup.py` & `otools-rpc-0.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="otools-rpc",
-    version="0.2.2",
+    version="0.2.3",
     description="A tool to interact with Odoo's external API.",
-    packages=find_packages(include=["otools_rpc"]),
+    packages=find_packages(exclude=["tests"]),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MrFaBemol/otools-rpc",
     author="Gautier Casabona",
     author_email="gcasabona.pro@gmail.com",
     license="MIT",
     classifiers=[
```

