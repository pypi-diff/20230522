# Comparing `tmp/krutils-0.20230522.1320.tar.gz` & `tmp/krutils-0.20230522.1322.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230522.1320.tar", last modified: Mon May 22 04:20:05 2023, max compression
+gzip compressed data, was "krutils-0.20230522.1322.tar", last modified: Mon May 22 04:22:53 2023, max compression
```

## Comparing `krutils-0.20230522.1320.tar` & `krutils-0.20230522.1322.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 04:20:05.481603 krutils-0.20230522.1320/
--rw-rw-rw-   0        0        0      526 2023-05-22 04:20:05.478487 krutils-0.20230522.1320/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1320/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 04:20:05.302226 krutils-0.20230522.1320/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1320/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1320/krutils/CONST.py
--rw-rw-rw-   0        0        0       94 2023-05-22 04:01:49.000000 krutils-0.20230522.1320/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1320/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0    12538 2023-05-22 03:59:25.000000 krutils-0.20230522.1320/krutils/logger.py
--rw-rw-rw-   0        0        0    21458 2023-05-22 03:59:08.000000 krutils-0.20230522.1320/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:20:05.452315 krutils-0.20230522.1320/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-05-22 04:20:04.000000 krutils-0.20230522.1320/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-22 04:20:04.000000 krutils-0.20230522.1320/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 04:20:04.000000 krutils-0.20230522.1320/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-22 04:20:04.000000 krutils-0.20230522.1320/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 04:20:04.000000 krutils-0.20230522.1320/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 04:20:05.493827 krutils-0.20230522.1320/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-05-22 04:20:03.000000 krutils-0.20230522.1320/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:20:05.468407 krutils-0.20230522.1320/test/
--rw-rw-rw-   0        0        0      308 2023-05-22 03:42:17.000000 krutils-0.20230522.1320/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:22:53.301456 krutils-0.20230522.1322/
+-rw-rw-rw-   0        0        0      526 2023-05-22 04:22:53.299600 krutils-0.20230522.1322/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1322/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 04:22:53.101210 krutils-0.20230522.1322/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1322/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1322/krutils/CONST.py
+-rw-rw-rw-   0        0        0       96 2023-05-22 04:22:41.000000 krutils-0.20230522.1322/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1322/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0    12538 2023-05-22 03:59:25.000000 krutils-0.20230522.1322/krutils/logger.py
+-rw-rw-rw-   0        0        0    21458 2023-05-22 03:59:08.000000 krutils-0.20230522.1322/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:22:53.293029 krutils-0.20230522.1322/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-05-22 04:22:52.000000 krutils-0.20230522.1322/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-22 04:22:52.000000 krutils-0.20230522.1322/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 04:22:52.000000 krutils-0.20230522.1322/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-22 04:22:52.000000 krutils-0.20230522.1322/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 04:22:52.000000 krutils-0.20230522.1322/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 04:22:53.301456 krutils-0.20230522.1322/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-05-22 04:22:50.000000 krutils-0.20230522.1322/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:22:53.297032 krutils-0.20230522.1322/test/
+-rw-rw-rw-   0        0        0      308 2023-05-22 03:42:17.000000 krutils-0.20230522.1322/test/test_logger.py
```

### Comparing `krutils-0.20230522.1320/PKG-INFO` & `krutils-0.20230522.1322/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1320
+Version: 0.20230522.1322
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1320/krutils/CONST.py` & `krutils-0.20230522.1322/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1320/krutils/_dbmgr.py` & `krutils-0.20230522.1322/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1320/krutils/logger.py` & `krutils-0.20230522.1322/krutils/logger.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1320/krutils/utils.py` & `krutils-0.20230522.1322/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1320/krutils.egg-info/PKG-INFO` & `krutils-0.20230522.1322/krutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1320
+Version: 0.20230522.1322
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1320/setup.py` & `krutils-0.20230522.1322/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230522.1320",
+    version="0.20230522.1322",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

