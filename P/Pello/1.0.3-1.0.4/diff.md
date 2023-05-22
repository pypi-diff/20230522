# Comparing `tmp/Pello-1.0.3.tar.gz` & `tmp/Pello-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pello-1.0.3.tar", last modified: Wed Mar 30 17:55:44 2022, max compression
+gzip compressed data, was "Pello-1.0.4.tar", last modified: Mon May 22 12:52:44 2023, max compression
```

## Comparing `Pello-1.0.3.tar` & `Pello-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 churchyard  (1000) churchyard  (1000)        0 2022-03-30 17:55:44.576420 Pello-1.0.3/
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)     7049 2022-03-25 18:48:43.000000 Pello-1.0.3/LICENSE.txt
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       20 2022-03-25 18:48:43.000000 Pello-1.0.3/MANIFEST.in
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)     2217 2022-03-30 17:55:44.575420 Pello-1.0.3/PKG-INFO
-drwxrwxr-x   0 churchyard  (1000) churchyard  (1000)        0 2022-03-30 17:55:44.575420 Pello-1.0.3/Pello.egg-info/
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)     2217 2022-03-30 17:55:44.000000 Pello-1.0.3/Pello.egg-info/PKG-INFO
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)      321 2022-03-30 17:55:44.000000 Pello-1.0.3/Pello.egg-info/SOURCES.txt
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)        1 2022-03-30 17:55:44.000000 Pello-1.0.3/Pello.egg-info/dependency_links.txt
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       66 2022-03-30 17:55:44.000000 Pello-1.0.3/Pello.egg-info/entry_points.txt
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)        1 2022-03-30 17:55:44.000000 Pello-1.0.3/Pello.egg-info/not-zip-safe
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       19 2022-03-30 17:55:44.000000 Pello-1.0.3/Pello.egg-info/requires.txt
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)        6 2022-03-30 17:55:44.000000 Pello-1.0.3/Pello.egg-info/top_level.txt
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)     1718 2022-03-25 18:48:43.000000 Pello-1.0.3/README.md
-drwxrwxr-x   0 churchyard  (1000) churchyard  (1000)        0 2022-03-30 17:55:44.575420 Pello-1.0.3/pello/
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       66 2022-03-25 18:48:43.000000 Pello-1.0.3/pello/__init__.py
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       60 2022-03-25 18:48:43.000000 Pello-1.0.3/pello/__main__.py
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)      213 2022-03-25 18:48:43.000000 Pello-1.0.3/pello/pello_greeting.py
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)      365 2022-03-25 18:48:43.000000 Pello-1.0.3/pyproject.toml
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       38 2022-03-30 17:55:44.576420 Pello-1.0.3/setup.cfg
--rw-rw-r--   0 churchyard  (1000) churchyard  (1000)      916 2022-03-30 17:55:17.000000 Pello-1.0.3/setup.py
+drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2023-05-22 12:52:44.346704 Pello-1.0.4/
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)      878 2023-05-22 12:51:46.000000 Pello-1.0.4/LICENSE.txt
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)       49 2023-05-22 12:24:40.000000 Pello-1.0.4/MANIFEST.in
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)     2197 2023-05-22 12:52:44.346704 Pello-1.0.4/PKG-INFO
+drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2023-05-22 12:52:44.346704 Pello-1.0.4/Pello.egg-info/
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)     2197 2023-05-22 12:52:43.000000 Pello-1.0.4/Pello.egg-info/PKG-INFO
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)      350 2023-05-22 12:52:44.000000 Pello-1.0.4/Pello.egg-info/SOURCES.txt
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)        1 2023-05-22 12:52:44.000000 Pello-1.0.4/Pello.egg-info/dependency_links.txt
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       65 2023-05-22 12:52:44.000000 Pello-1.0.4/Pello.egg-info/entry_points.txt
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)        1 2022-03-30 17:55:44.000000 Pello-1.0.4/Pello.egg-info/not-zip-safe
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       19 2023-05-22 12:52:44.000000 Pello-1.0.4/Pello.egg-info/requires.txt
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)        6 2023-05-22 12:52:44.000000 Pello-1.0.4/Pello.egg-info/top_level.txt
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)     1718 2022-03-25 18:48:43.000000 Pello-1.0.4/README.md
+drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2023-05-22 12:52:44.346704 Pello-1.0.4/pello/
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       66 2022-03-25 18:48:43.000000 Pello-1.0.4/pello/__init__.py
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)       60 2022-03-25 18:48:43.000000 Pello-1.0.4/pello/__main__.py
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)      213 2022-03-25 18:48:43.000000 Pello-1.0.4/pello/pello_greeting.py
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)      365 2022-03-25 18:48:43.000000 Pello-1.0.4/pyproject.toml
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)       38 2023-05-22 12:52:44.346704 Pello-1.0.4/setup.cfg
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)      916 2023-05-22 12:51:46.000000 Pello-1.0.4/setup.py
+drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2023-05-22 12:52:44.346704 Pello-1.0.4/tests/
+-rw-rw-r--   0 churchyard  (1000) churchyard  (1000)      190 2022-03-25 18:48:43.000000 Pello-1.0.4/tests/test_pello_greeting.py
```

### Comparing `Pello-1.0.3/PKG-INFO` & `Pello-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: Pello
-Version: 1.0.3
+Version: 1.0.4
 Summary: An example Python Hello World package
 Home-page: https://github.com/fedora-python/Pello
 Author: Tomáš Hrnčiar
 Author-email: tomas.hrnciar@me.com
-License: CC0
-Platform: UNKNOWN
+License: MIT-0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: color
 License-File: LICENSE.txt
 
 
 # Pello
@@ -86,9 +85,7 @@
 metadata (in `pyproject.toml` and `setup.py`).
 This metadata should be converted, as automatically as possible,
 into RPM metadata.
 
 Thanks to the capital P, `Pello` differs from the
 [normalized name](https://www.python.org/dev/peps/pep-0503/#normalized-name)
 `pello`, so we can show where each of them is needed.
-
-
```

### Comparing `Pello-1.0.3/Pello.egg-info/PKG-INFO` & `Pello-1.0.4/Pello.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: Pello
-Version: 1.0.3
+Version: 1.0.4
 Summary: An example Python Hello World package
 Home-page: https://github.com/fedora-python/Pello
 Author: Tomáš Hrnčiar
 Author-email: tomas.hrnciar@me.com
-License: CC0
-Platform: UNKNOWN
+License: MIT-0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: color
 License-File: LICENSE.txt
 
 
 # Pello
@@ -86,9 +85,7 @@
 metadata (in `pyproject.toml` and `setup.py`).
 This metadata should be converted, as automatically as possible,
 into RPM metadata.
 
 Thanks to the capital P, `Pello` differs from the
 [normalized name](https://www.python.org/dev/peps/pep-0503/#normalized-name)
 `pello`, so we can show where each of them is needed.
-
-
```

### Comparing `Pello-1.0.3/README.md` & `Pello-1.0.4/README.md`

 * *Files identical despite different names*

