# Comparing `tmp/pybaht-0.1.1.tar.gz` & `tmp/pybaht-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaht-0.1.1.tar", last modified: Mon May 22 09:54:45 2023, max compression
+gzip compressed data, was "pybaht-0.2.0.tar", last modified: Mon May 22 10:10:06 2023, max compression
```

## Comparing `pybaht-0.1.1.tar` & `pybaht-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:54:45.545077 pybaht-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     1077 2023-05-22 09:54:35.000000 pybaht-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1954 2023-05-22 09:54:45.545077 pybaht-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1542 2023-05-22 09:54:35.000000 pybaht-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:54:45.545077 pybaht-0.1.1/pybaht/
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-22 09:54:35.000000 pybaht-0.1.1/pybaht/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-22 09:54:35.000000 pybaht-0.1.1/pybaht/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2634 2023-05-22 09:54:35.000000 pybaht-0.1.1/pybaht/bahttext.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:54:45.545077 pybaht-0.1.1/pybaht.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1954 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-05-22 09:54:45.545077 pybaht-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-22 09:54:43.000000 pybaht-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:10:06.347061 pybaht-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-05-22 10:10:02.000000 pybaht-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2131 2023-05-22 10:10:06.347061 pybaht-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-05-22 10:10:02.000000 pybaht-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:10:06.347061 pybaht-0.2.0/pybaht/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-22 10:10:02.000000 pybaht-0.2.0/pybaht/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-22 10:10:02.000000 pybaht-0.2.0/pybaht/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-05-22 10:10:02.000000 pybaht-0.2.0/pybaht/bahttext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:10:06.347061 pybaht-0.2.0/pybaht.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2131 2023-05-22 10:10:06.000000 pybaht-0.2.0/pybaht.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-22 10:10:06.000000 pybaht-0.2.0/pybaht.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 10:10:06.000000 pybaht-0.2.0/pybaht.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-22 10:10:06.000000 pybaht-0.2.0/pybaht.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 10:10:06.000000 pybaht-0.2.0/pybaht.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-22 10:10:06.347061 pybaht-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-22 10:10:03.000000 pybaht-0.2.0/setup.py
```

### Comparing `pybaht-0.1.1/LICENSE` & `pybaht-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybaht-0.1.1/PKG-INFO` & `pybaht-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,11 @@
-Metadata-Version: 2.1
-Name: pybaht
-Version: 0.1.1
-Summary: Baht library for Python
-Home-page: https://github.com/jojoee/pybaht
-Author: Nathachai Thongniran
-Author-email: inid3a@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pybaht
 
-[![CI and CD](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml)
+[![continuous-integration](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml)
+[![release](https://github.com/jojoee/pybaht/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/jojoee/pybaht/actions/workflows/release.yml)
 [![PyPI version fury.io](https://badge.fury.io/py/pybaht.svg)](https://pypi.python.org/pypi/pybaht/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![codecov](https://codecov.io/gh/jojoee/pybaht/branch/main/graph/badge.svg)](https://codecov.io/gh/jojoee/pybaht)
 
 Baht library for Python
 
 ## Installation
@@ -50,7 +37,8 @@
 ```
 
 ## Other languages
 - JavaScript: [jojoee/bahttext](https://github.com/jojoee/bahttext)
 
 ## Reference
 - [Google Sheets BAHTTEXT function](https://support.google.com/docs/answer/9982303?hl=en)
+
```

### Comparing `pybaht-0.1.1/README.md` & `pybaht-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+Metadata-Version: 2.1
+Name: pybaht
+Version: 0.2.0
+Summary: Baht library for Python
+Home-page: https://github.com/jojoee/pybaht
+Author: Nathachai Thongniran
+Author-email: inid3a@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pybaht
 
-[![CI and CD](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml)
+[![continuous-integration](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml)
+[![release](https://github.com/jojoee/pybaht/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/jojoee/pybaht/actions/workflows/release.yml)
 [![PyPI version fury.io](https://badge.fury.io/py/pybaht.svg)](https://pypi.python.org/pypi/pybaht/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![codecov](https://codecov.io/gh/jojoee/pybaht/branch/main/graph/badge.svg)](https://codecov.io/gh/jojoee/pybaht)
 
 Baht library for Python
 
 ## Installation
@@ -36,7 +51,8 @@
 ```
 
 ## Other languages
 - JavaScript: [jojoee/bahttext](https://github.com/jojoee/bahttext)
 
 ## Reference
 - [Google Sheets BAHTTEXT function](https://support.google.com/docs/answer/9982303?hl=en)
+
```

### Comparing `pybaht-0.1.1/pybaht/bahttext.py` & `pybaht-0.2.0/pybaht/bahttext.py`

 * *Files identical despite different names*

### Comparing `pybaht-0.1.1/pybaht.egg-info/PKG-INFO` & `pybaht-0.2.0/pybaht.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pybaht
-Version: 0.1.1
+Version: 0.2.0
 Summary: Baht library for Python
 Home-page: https://github.com/jojoee/pybaht
 Author: Nathachai Thongniran
 Author-email: inid3a@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pybaht
 
-[![CI and CD](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml)
+[![continuous-integration](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/jojoee/pybaht/actions/workflows/continuous-integration.yml)
+[![release](https://github.com/jojoee/pybaht/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/jojoee/pybaht/actions/workflows/release.yml)
 [![PyPI version fury.io](https://badge.fury.io/py/pybaht.svg)](https://pypi.python.org/pypi/pybaht/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![codecov](https://codecov.io/gh/jojoee/pybaht/branch/main/graph/badge.svg)](https://codecov.io/gh/jojoee/pybaht)
 
 Baht library for Python
 
 ## Installation
@@ -50,7 +51,8 @@
 ```
 
 ## Other languages
 - JavaScript: [jojoee/bahttext](https://github.com/jojoee/bahttext)
 
 ## Reference
 - [Google Sheets BAHTTEXT function](https://support.google.com/docs/answer/9982303?hl=en)
+
```

### Comparing `pybaht-0.1.1/setup.py` & `pybaht-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 # This call to setup() does all the work
 setup(
     name="pybaht",
     version=__version__,
     description="Baht library for Python",
     long_description=README,
```

