# Comparing `tmp/morpheus-mail-1.0.17.tar.gz` & `tmp/morpheus-mail-1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morpheus-mail-1.0.17.tar", last modified: Mon May 22 15:21:18 2023, max compression
+gzip compressed data, was "morpheus-mail-1.0.18.tar", last modified: Mon May 22 15:34:37 2023, max compression
```

## Comparing `morpheus-mail-1.0.17.tar` & `morpheus-mail-1.0.18.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.687962 morpheus-mail-1.0.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-22 15:21:18.687962 morpheus-mail-1.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.683962 morpheus-mail-1.0.17/morpheus_mail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-22 15:21:18.687962 morpheus-mail-1.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.683962 morpheus-mail-1.0.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.683962 morpheus-mail-1.0.17/src/render/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/src/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/src/render/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.683962 morpheus-mail-1.0.17/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)    31782 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_user_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:34:37.674341 morpheus-mail-1.0.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-22 15:34:37.674341 morpheus-mail-1.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:34:37.674341 morpheus-mail-1.0.18/morpheus_mail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-22 15:34:37.000000 morpheus-mail-1.0.18/morpheus_mail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-22 15:34:37.000000 morpheus-mail-1.0.18/morpheus_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:34:37.000000 morpheus-mail-1.0.18/morpheus_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 15:34:37.000000 morpheus-mail-1.0.18/morpheus_mail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 15:34:37.000000 morpheus-mail-1.0.18/morpheus_mail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:34:37.000000 morpheus-mail-1.0.18/morpheus_mail.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-22 15:34:37.674341 morpheus-mail-1.0.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:34:37.670340 morpheus-mail-1.0.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:34:37.674341 morpheus-mail-1.0.18/src/render/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/src/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/src/render/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:34:37.674341 morpheus-mail-1.0.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/tests/test_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31782 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/tests/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/tests/test_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-22 15:33:48.000000 morpheus-mail-1.0.18/tests/test_user_display.py
```

### Comparing `morpheus-mail-1.0.17/LICENSE` & `morpheus-mail-1.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.17/PKG-INFO` & `morpheus-mail-1.0.18/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: morpheus-mail
-Version: 1.0.17
+Version: 1.0.18
 Summary: Email rendering engine from morpheus
 Home-page: https://github.com/tutorcruncher/morpheus
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Internet
```

### Comparing `morpheus-mail-1.0.17/README.md` & `morpheus-mail-1.0.18/README.md`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.17/morpheus_mail.egg-info/PKG-INFO` & `morpheus-mail-1.0.18/morpheus_mail.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: morpheus-mail
-Version: 1.0.17
+Version: 1.0.18
 Summary: Email rendering engine from morpheus
 Home-page: https://github.com/tutorcruncher/morpheus
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Internet
```

### Comparing `morpheus-mail-1.0.17/setup.cfg` & `morpheus-mail-1.0.18/setup.cfg`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.17/setup.py` & `morpheus-mail-1.0.18/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         'Environment :: Console',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Unix',
         'Operating System :: POSIX :: Linux',
         'Topic :: Internet',
```

### Comparing `morpheus-mail-1.0.17/src/render/main.py` & `morpheus-mail-1.0.18/src/render/main.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.17/tests/test_aux.py` & `morpheus-mail-1.0.18/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.17/tests/test_email.py` & `morpheus-mail-1.0.18/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.17/tests/test_render.py` & `morpheus-mail-1.0.18/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.17/tests/test_sms.py` & `morpheus-mail-1.0.18/tests/test_sms.py`

 * *Files identical despite different names*

### Comparing `morpheus-mail-1.0.17/tests/test_user_display.py` & `morpheus-mail-1.0.18/tests/test_user_display.py`

 * *Files identical despite different names*

