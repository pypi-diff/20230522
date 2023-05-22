# Comparing `tmp/manhattan_comparable-0.0.8.tar.gz` & `tmp/manhattan_comparable-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manhattan_comparable-0.0.8.tar", last modified: Fri Sep 14 13:51:57 2018, max compression
+gzip compressed data, was "dist/manhattan_comparable-0.0.9.tar", last modified: Fri Sep 14 14:25:49 2018, max compression
```

## Comparing `manhattan_comparable-0.0.8.tar` & `manhattan_comparable-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       61 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/MANIFEST.in
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1101 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/LICENSE
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       79 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/setup.cfg
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1198 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/PKG-INFO
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     4042 2018-09-14 13:51:27.000000 manhattan_comparable-0.0.8/setup.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)      212 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/README.md
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan_comparable.egg-info/
--rw-rw-r--   0 anthony   (1001) anthony   (1001)      954 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan_comparable.egg-info/SOURCES.txt
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       10 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan_comparable.egg-info/top_level.txt
--rw-rw-r--   0 anthony   (1001) anthony   (1001)        1 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan_comparable.egg-info/dependency_links.txt
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1198 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan_comparable.egg-info/PKG-INFO
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       60 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan_comparable.egg-info/requires.txt
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       10 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan_comparable.egg-info/namespace_packages.txt
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       56 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/__init__.py
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     5251 2018-09-14 13:50:27.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/change_log.py
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 13:51:57.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/tests/
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     3506 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/tests/test_frames.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     4005 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/tests/test_change_log.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)      807 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/tests/__init__.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1230 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/tests/fixtures.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)      919 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/factory.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       35 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/__init__.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     5514 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/frames.py
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       61 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/MANIFEST.in
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1101 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/LICENSE
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       79 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/setup.cfg
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1198 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/PKG-INFO
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     4042 2018-09-14 14:24:43.000000 manhattan_comparable-0.0.9/setup.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)      212 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/README.md
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan_comparable.egg-info/
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)      954 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan_comparable.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       10 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan_comparable.egg-info/top_level.txt
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)        1 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan_comparable.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1198 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan_comparable.egg-info/PKG-INFO
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       60 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan_comparable.egg-info/requires.txt
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       10 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan_comparable.egg-info/namespace_packages.txt
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       56 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/__init__.py
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     5303 2018-09-14 14:24:37.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/change_log.py
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-09-14 14:25:49.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/tests/
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     3506 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/tests/test_frames.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     4005 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/tests/test_change_log.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)      807 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/tests/__init__.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1230 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/tests/fixtures.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)      919 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/factory.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       35 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/__init__.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     5514 2018-04-12 16:15:33.000000 manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/frames.py
```

### Comparing `manhattan_comparable-0.0.8/LICENSE` & `manhattan_comparable-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manhattan_comparable-0.0.8/PKG-INFO` & `manhattan_comparable-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manhattan_comparable
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tracking changes (who, what [from > to], when) to the database (via the mongoframes.Frame interface).
 Home-page: https://git.getme.co.uk/manhattan/manhattan_comparable
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: The Getme development team
 Maintainer-email: devs@getme.co.uk
 License: MIT
@@ -25,9 +25,9 @@
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-Provides-Extra: develop
 Provides-Extra: test
+Provides-Extra: develop
```

### Comparing `manhattan_comparable-0.0.8/setup.py` & `manhattan_comparable-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     name='manhattan_comparable',
     namespace_packages=['manhattan'],
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.8',
+    version='0.0.9',
 
     description='Tracking changes (who, what [from > to], when) to the database '
                 '(via the mongoframes.Frame interface).',
     long_description=long_description,
 
     # The project's main homepage (@@ add github url once public)
     url='https://git.getme.co.uk/manhattan/manhattan_comparable',
```

### Comparing `manhattan_comparable-0.0.8/manhattan_comparable/manhattan_comparable.egg-info/SOURCES.txt` & `manhattan_comparable-0.0.9/manhattan_comparable/manhattan_comparable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manhattan_comparable-0.0.8/manhattan_comparable/manhattan_comparable.egg-info/PKG-INFO` & `manhattan_comparable-0.0.9/manhattan_comparable/manhattan_comparable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manhattan-comparable
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tracking changes (who, what [from > to], when) to the database (via the mongoframes.Frame interface).
 Home-page: https://git.getme.co.uk/manhattan/manhattan_comparable
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: The Getme development team
 Maintainer-email: devs@getme.co.uk
 License: MIT
@@ -25,9 +25,9 @@
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-Provides-Extra: develop
 Provides-Extra: test
+Provides-Extra: develop
```

### Comparing `manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/change_log.py` & `manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/change_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
         'user',
         'user_sticky_label',
         'type',
         'details'
         }
 
     _indexes = [
-        IndexModel([('documents', ASC)])
+        IndexModel([
+            ('created', ASC),
+            ('documents', ASC)
+        ])
     ]
 
     @property
     def diff_html(self):
         """Return the entry's diff in HTML format"""
         return self.diff_to_html(self.details)
```

### Comparing `manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/tests/test_frames.py` & `manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/tests/test_frames.py`

 * *Files identical despite different names*

### Comparing `manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/tests/test_change_log.py` & `manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/tests/test_change_log.py`

 * *Files identical despite different names*

### Comparing `manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/tests/__init__.py` & `manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/tests/fixtures.py` & `manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/factory.py` & `manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/factory.py`

 * *Files identical despite different names*

### Comparing `manhattan_comparable-0.0.8/manhattan_comparable/manhattan/comparable/frames.py` & `manhattan_comparable-0.0.9/manhattan_comparable/manhattan/comparable/frames.py`

 * *Files identical despite different names*

