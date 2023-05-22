# Comparing `tmp/pybaht-0.1.0.tar.gz` & `tmp/pybaht-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaht-0.1.0.tar", last modified: Wed Jun  1 10:37:27 2022, max compression
+gzip compressed data, was "pybaht-0.1.1.tar", last modified: Mon May 22 09:54:45 2023, max compression
```

## Comparing `pybaht-0.1.0.tar` & `pybaht-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 10:37:27.498155 pybaht-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1077 2022-06-01 10:37:12.000000 pybaht-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1974 2022-06-01 10:37:27.498155 pybaht-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1542 2022-06-01 10:37:12.000000 pybaht-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 10:37:27.498155 pybaht-0.1.0/pybaht/
--rw-r--r--   0 root         (0) root         (0)       69 2022-06-01 10:37:12.000000 pybaht-0.1.0/pybaht/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2022-06-01 10:37:12.000000 pybaht-0.1.0/pybaht/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2598 2022-06-01 10:37:12.000000 pybaht-0.1.0/pybaht/bahttext.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 10:37:27.498155 pybaht-0.1.0/pybaht.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1974 2022-06-01 10:37:27.000000 pybaht-0.1.0/pybaht.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2022-06-01 10:37:27.000000 pybaht-0.1.0/pybaht.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-01 10:37:27.000000 pybaht-0.1.0/pybaht.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-06-01 10:37:27.000000 pybaht-0.1.0/pybaht.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-06-01 10:37:27.000000 pybaht-0.1.0/pybaht.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      112 2022-06-01 10:37:27.502155 pybaht-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      892 2022-06-01 10:37:25.000000 pybaht-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:54:45.545077 pybaht-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-05-22 09:54:35.000000 pybaht-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-05-22 09:54:45.545077 pybaht-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-22 09:54:35.000000 pybaht-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:54:45.545077 pybaht-0.1.1/pybaht/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-22 09:54:35.000000 pybaht-0.1.1/pybaht/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-22 09:54:35.000000 pybaht-0.1.1/pybaht/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-05-22 09:54:35.000000 pybaht-0.1.1/pybaht/bahttext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:54:45.545077 pybaht-0.1.1/pybaht.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 09:54:45.000000 pybaht-0.1.1/pybaht.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-22 09:54:45.545077 pybaht-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-22 09:54:43.000000 pybaht-0.1.1/setup.py
```

### Comparing `pybaht-0.1.0/LICENSE` & `pybaht-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybaht-0.1.0/PKG-INFO` & `pybaht-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pybaht
-Version: 0.1.0
+Version: 0.1.1
 Summary: Baht library for Python
 Home-page: https://github.com/jojoee/pybaht
 Author: Nathachai Thongniran
 Author-email: inid3a@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pybaht
@@ -51,9 +50,7 @@
 ```
 
 ## Other languages
 - JavaScript: [jojoee/bahttext](https://github.com/jojoee/bahttext)
 
 ## Reference
 - [Google Sheets BAHTTEXT function](https://support.google.com/docs/answer/9982303?hl=en)
-
-
```

### Comparing `pybaht-0.1.0/README.md` & `pybaht-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pybaht-0.1.0/pybaht.egg-info/PKG-INFO` & `pybaht-0.1.1/pybaht.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pybaht
-Version: 0.1.0
+Version: 0.1.1
 Summary: Baht library for Python
 Home-page: https://github.com/jojoee/pybaht
 Author: Nathachai Thongniran
 Author-email: inid3a@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pybaht
@@ -51,9 +50,7 @@
 ```
 
 ## Other languages
 - JavaScript: [jojoee/bahttext](https://github.com/jojoee/bahttext)
 
 ## Reference
 - [Google Sheets BAHTTEXT function](https://support.google.com/docs/answer/9982303?hl=en)
-
-
```

### Comparing `pybaht-0.1.0/setup.py` & `pybaht-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 # This call to setup() does all the work
 setup(
     name="pybaht",
     version=__version__,
     description="Baht library for Python",
     long_description=README,
```

