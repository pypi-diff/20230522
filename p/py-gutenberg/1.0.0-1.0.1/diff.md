# Comparing `tmp/py-gutenberg-1.0.0.tar.gz` & `tmp/py-gutenberg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-gutenberg-1.0.0.tar", last modified: Mon Apr  3 04:29:39 2023, max compression
+gzip compressed data, was "py-gutenberg-1.0.1.tar", last modified: Mon May 22 20:16:35 2023, max compression
```

## Comparing `py-gutenberg-1.0.0.tar` & `py-gutenberg-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:29:39.607360 py-gutenberg-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-03 04:29:18.000000 py-gutenberg-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-03 04:29:39.607360 py-gutenberg-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-03 04:29:18.000000 py-gutenberg-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-03 04:29:18.000000 py-gutenberg-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 04:29:39.607360 py-gutenberg-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:29:39.603360 py-gutenberg-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:29:39.607360 py-gutenberg-1.0.0/src/gutenberg/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-03 04:29:18.000000 py-gutenberg-1.0.0/src/gutenberg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-03 04:29:18.000000 py-gutenberg-1.0.0/src/gutenberg/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-03 04:29:18.000000 py-gutenberg-1.0.0/src/gutenberg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:29:39.607360 py-gutenberg-1.0.0/src/py_gutenberg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-03 04:29:39.000000 py-gutenberg-1.0.0/src/py_gutenberg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-03 04:29:39.000000 py-gutenberg-1.0.0/src/py_gutenberg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 04:29:39.000000 py-gutenberg-1.0.0/src/py_gutenberg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 04:29:39.000000 py-gutenberg-1.0.0/src/py_gutenberg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:29:39.607360 py-gutenberg-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-03 04:29:18.000000 py-gutenberg-1.0.0/tests/test_gutenberg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/src/gutenberg/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/src/gutenberg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/src/gutenberg/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/src/gutenberg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-22 20:16:35.000000 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-22 20:16:35.000000 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:16:35.000000 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 20:16:35.000000 py-gutenberg-1.0.1/src/py_gutenberg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:16:35.787004 py-gutenberg-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-22 20:16:15.000000 py-gutenberg-1.0.1/tests/test_gutenberg.py
```

### Comparing `py-gutenberg-1.0.0/LICENSE` & `py-gutenberg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-gutenberg-1.0.0/PKG-INFO` & `py-gutenberg-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-gutenberg
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library to access the Project Gutenberg API
 Author-email: Peter Rauscher <peterrauscher@protonmail.com>
 Project-URL: Homepage, https://github.com/peterrauscher/gutenberg-py
 Project-URL: Bug Tracker, https://github.com/peterrauscher/gutenberg-py/issues
 Project-URL: Source Code, https://github.com/peterrauscher/gutenberg-py
 Project-URL: Funding, https://ko-fi.com/peterrauscher
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-gutenberg
 
-[![Install from pip](https://img.shields.io/badge/pip%20install-py--gutenberg-brightgreen)](https://pypi.org/project/py-gutenberg/) [![Tests Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/test.yml?branch=main&label=tests)](https://github.com/peterrauscher/py-gutenberg/actions) [![Build Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/release.yml?branch=main&label=build)](https://github.com/peterrauscher/py-gutenberg/actions) [![License](https://img.shields.io/github/license/peterrauscher/py-gutenberg)](https://github.com/peterrauscher/py-gutenberg/blob/main/LICENSE) [![Latest Release Version Number](https://img.shields.io/pypi/v/py-gutenberg)](https://pypi.org/project/py-gutenberg/releases) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/py-gutenberg)](https://pypi.org/project/py-gutenberg)
+[![Install from pip](https://img.shields.io/badge/pip%20install-py--gutenberg-orange)](https://pypi.org/project/py-gutenberg/) [![Tests Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/test.yml?branch=main&label=tests)](https://github.com/peterrauscher/py-gutenberg/actions) [![Build Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/release.yml?branch=main&label=build)](https://github.com/peterrauscher/py-gutenberg/actions) [![License](https://img.shields.io/github/license/peterrauscher/py-gutenberg)](https://github.com/peterrauscher/py-gutenberg/blob/main/LICENSE) [![Latest Release Version Number](https://img.shields.io/pypi/v/py-gutenberg)](https://pypi.org/project/py-gutenberg/releases) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/py-gutenberg)](https://pypi.org/project/py-gutenberg)
 
 ## Overview
 
 The **py-gutenberg** package is a Python library that provides methods to access the [Project Gutenberg](https://www.gutenberg.org/) library. Users can search for books based on a variety of metadata, get full texts in various formats, and retrieve metadata for books by their ID number.
 
 ## Installation
```

### Comparing `py-gutenberg-1.0.0/README.md` & `py-gutenberg-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # py-gutenberg
 
-[![Install from pip](https://img.shields.io/badge/pip%20install-py--gutenberg-brightgreen)](https://pypi.org/project/py-gutenberg/) [![Tests Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/test.yml?branch=main&label=tests)](https://github.com/peterrauscher/py-gutenberg/actions) [![Build Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/release.yml?branch=main&label=build)](https://github.com/peterrauscher/py-gutenberg/actions) [![License](https://img.shields.io/github/license/peterrauscher/py-gutenberg)](https://github.com/peterrauscher/py-gutenberg/blob/main/LICENSE) [![Latest Release Version Number](https://img.shields.io/pypi/v/py-gutenberg)](https://pypi.org/project/py-gutenberg/releases) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/py-gutenberg)](https://pypi.org/project/py-gutenberg)
+[![Install from pip](https://img.shields.io/badge/pip%20install-py--gutenberg-orange)](https://pypi.org/project/py-gutenberg/) [![Tests Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/test.yml?branch=main&label=tests)](https://github.com/peterrauscher/py-gutenberg/actions) [![Build Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/release.yml?branch=main&label=build)](https://github.com/peterrauscher/py-gutenberg/actions) [![License](https://img.shields.io/github/license/peterrauscher/py-gutenberg)](https://github.com/peterrauscher/py-gutenberg/blob/main/LICENSE) [![Latest Release Version Number](https://img.shields.io/pypi/v/py-gutenberg)](https://pypi.org/project/py-gutenberg/releases) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/py-gutenberg)](https://pypi.org/project/py-gutenberg)
 
 ## Overview
 
 The **py-gutenberg** package is a Python library that provides methods to access the [Project Gutenberg](https://www.gutenberg.org/) library. Users can search for books based on a variety of metadata, get full texts in various formats, and retrieve metadata for books by their ID number.
 
 ## Installation
```

### Comparing `py-gutenberg-1.0.0/pyproject.toml` & `py-gutenberg-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests>=2.28.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-gutenberg"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Peter Rauscher", email="peterrauscher@protonmail.com" },
 ]
 description = "A library to access the Project Gutenberg API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py-gutenberg-1.0.0/src/gutenberg/main.py` & `py-gutenberg-1.0.1/src/gutenberg/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import requests
-from models import APIException, Book
+
+from .models import APIException, Book
 
 
 class GutenbergAPI:
     # DISCLAIMER: PLEASE READ !!!
     # This library is built on the amazing Gutendex project,
     # but the public instance has limited bandwidth and the developer
     # does not make money on the project. If you are able, I HIGHLY encourage
     # you to host your own instance of the API, you will save the developers
     # lots of money and response times will be much faster for you.
     # The instructions for self-hosting can be found here:
     # https://github.com/garethbjohnson/gutendex/wiki/Installation-Guide
-    def __init__(self, instance_url="https://gutendex.com"):
+    def __init__(self, instance_url="https://gutendex.devbranch.co"):
         self.instance_url = instance_url
 
     # Methods for getting or searching for lists of books
     def __get_books(
         self,
         author_year_start: int = None,
         author_year_end: int = None,
```

### Comparing `py-gutenberg-1.0.0/src/gutenberg/models.py` & `py-gutenberg-1.0.1/src/gutenberg/models.py`

 * *Files identical despite different names*

### Comparing `py-gutenberg-1.0.0/src/py_gutenberg.egg-info/PKG-INFO` & `py-gutenberg-1.0.1/src/py_gutenberg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-gutenberg
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library to access the Project Gutenberg API
 Author-email: Peter Rauscher <peterrauscher@protonmail.com>
 Project-URL: Homepage, https://github.com/peterrauscher/gutenberg-py
 Project-URL: Bug Tracker, https://github.com/peterrauscher/gutenberg-py/issues
 Project-URL: Source Code, https://github.com/peterrauscher/gutenberg-py
 Project-URL: Funding, https://ko-fi.com/peterrauscher
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-gutenberg
 
-[![Install from pip](https://img.shields.io/badge/pip%20install-py--gutenberg-brightgreen)](https://pypi.org/project/py-gutenberg/) [![Tests Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/test.yml?branch=main&label=tests)](https://github.com/peterrauscher/py-gutenberg/actions) [![Build Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/release.yml?branch=main&label=build)](https://github.com/peterrauscher/py-gutenberg/actions) [![License](https://img.shields.io/github/license/peterrauscher/py-gutenberg)](https://github.com/peterrauscher/py-gutenberg/blob/main/LICENSE) [![Latest Release Version Number](https://img.shields.io/pypi/v/py-gutenberg)](https://pypi.org/project/py-gutenberg/releases) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/py-gutenberg)](https://pypi.org/project/py-gutenberg)
+[![Install from pip](https://img.shields.io/badge/pip%20install-py--gutenberg-orange)](https://pypi.org/project/py-gutenberg/) [![Tests Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/test.yml?branch=main&label=tests)](https://github.com/peterrauscher/py-gutenberg/actions) [![Build Status](https://img.shields.io/github/actions/workflow/status/peterrauscher/py-gutenberg/release.yml?branch=main&label=build)](https://github.com/peterrauscher/py-gutenberg/actions) [![License](https://img.shields.io/github/license/peterrauscher/py-gutenberg)](https://github.com/peterrauscher/py-gutenberg/blob/main/LICENSE) [![Latest Release Version Number](https://img.shields.io/pypi/v/py-gutenberg)](https://pypi.org/project/py-gutenberg/releases) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/py-gutenberg)](https://pypi.org/project/py-gutenberg)
 
 ## Overview
 
 The **py-gutenberg** package is a Python library that provides methods to access the [Project Gutenberg](https://www.gutenberg.org/) library. Users can search for books based on a variety of metadata, get full texts in various formats, and retrieve metadata for books by their ID number.
 
 ## Installation
```

