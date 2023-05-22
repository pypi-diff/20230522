# Comparing `tmp/morpheus-mail-1.0.19.tar.gz` & `tmp/morpheus-mail-1.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morpheus-mail-1.0.19.tar", last modified: Mon May 22 15:49:57 2023, max compression
+gzip compressed data, was "morpheus-mail-1.0.22.tar", last modified: Mon May 22 16:15:30 2023, max compression
```

## Comparing `morpheus-mail-1.0.19.tar` & `morpheus-mail-1.0.22.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:49:57.587863 morpheus-mail-1.0.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-22 15:49:57.587863 morpheus-mail-1.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:49:57.583863 morpheus-mail-1.0.19/morpheus_mail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-22 15:49:57.000000 morpheus-mail-1.0.19/morpheus_mail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-22 15:49:57.000000 morpheus-mail-1.0.19/morpheus_mail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:49:57.000000 morpheus-mail-1.0.19/morpheus_mail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 15:49:57.000000 morpheus-mail-1.0.19/morpheus_mail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 15:49:57.000000 morpheus-mail-1.0.19/morpheus_mail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:49:57.000000 morpheus-mail-1.0.19/morpheus_mail.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-22 15:49:57.587863 morpheus-mail-1.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:49:57.579863 morpheus-mail-1.0.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:49:57.583863 morpheus-mail-1.0.19/src/render/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/src/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/src/render/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:49:57.587863 morpheus-mail-1.0.19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/tests/test_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)    31782 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/tests/test_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/tests/test_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-22 15:49:18.000000 morpheus-mail-1.0.19/tests/test_user_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:15:30.004717 morpheus-mail-1.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-22 16:15:30.004717 morpheus-mail-1.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:15:30.000717 morpheus-mail-1.0.22/morpheus_mail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-22 16:15:29.000000 morpheus-mail-1.0.22/morpheus_mail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-22 16:15:29.000000 morpheus-mail-1.0.22/morpheus_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:15:29.000000 morpheus-mail-1.0.22/morpheus_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 16:15:29.000000 morpheus-mail-1.0.22/morpheus_mail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 16:15:29.000000 morpheus-mail-1.0.22/morpheus_mail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:15:29.000000 morpheus-mail-1.0.22/morpheus_mail.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-22 16:15:30.004717 morpheus-mail-1.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:15:30.000717 morpheus-mail-1.0.22/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:15:30.000717 morpheus-mail-1.0.22/src/render/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/src/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/src/render/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:15:30.004717 morpheus-mail-1.0.22/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/tests/test_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31782 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/tests/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/tests/test_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-22 16:14:45.000000 morpheus-mail-1.0.22/tests/test_user_display.py
```

### Comparing `morpheus-mail-1.0.19/LICENSE` & `morpheus-mail-1.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.19/PKG-INFO` & `morpheus-mail-1.0.22/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morpheus-mail
-Version: 1.0.19
+Version: 1.0.22
 Summary: Email rendering engine from morpheus
 Home-page: https://github.com/tutorcruncher/morpheus
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `morpheus-mail-1.0.19/README.md` & `morpheus-mail-1.0.22/README.md`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.19/morpheus_mail.egg-info/PKG-INFO` & `morpheus-mail-1.0.22/morpheus_mail.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morpheus-mail
-Version: 1.0.19
+Version: 1.0.22
 Summary: Email rendering engine from morpheus
 Home-page: https://github.com/tutorcruncher/morpheus
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `morpheus-mail-1.0.19/setup.cfg` & `morpheus-mail-1.0.22/setup.cfg`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.19/setup.py` & `morpheus-mail-1.0.22/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         'Operating System :: POSIX :: Linux',
         'Topic :: Internet',
     ],
     author='Samuel Colvin',
     author_email='s@muelcolvin.com',
     url='https://github.com/tutorcruncher/morpheus',
     license='MIT',
-    packages=['src.render'],
-    package_dir={'src.render': 'src/render'},
+    packages=['morpheus.render'],
+    package_dir={'morpheus.render': 'src/render'},
     python_requires='>=3.6',
     zip_safe=True,
     install_requires=[
         'chevron>=0.11.1',
         'libsass>=0.13.2',
         'misaka>=2.1.1',
     ],
```

### Comparing `morpheus-mail-1.0.19/src/render/main.py` & `morpheus-mail-1.0.22/src/render/main.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.19/tests/test_aux.py` & `morpheus-mail-1.0.22/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.19/tests/test_email.py` & `morpheus-mail-1.0.22/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.19/tests/test_render.py` & `morpheus-mail-1.0.22/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.19/tests/test_sms.py` & `morpheus-mail-1.0.22/tests/test_sms.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.19/tests/test_user_display.py` & `morpheus-mail-1.0.22/tests/test_user_display.py`

 * *Files identical despite different names*

