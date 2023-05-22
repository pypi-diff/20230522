# Comparing `tmp/krutils-0.20230522.1259.tar.gz` & `tmp/krutils-0.20230522.1301.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230522.1259.tar", last modified: Mon May 22 03:59:42 2023, max compression
+gzip compressed data, was "krutils-0.20230522.1301.tar", last modified: Mon May 22 04:01:57 2023, max compression
```

## Comparing `krutils-0.20230522.1259.tar` & `krutils-0.20230522.1301.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 03:59:42.799221 krutils-0.20230522.1259/
--rw-rw-rw-   0        0        0      526 2023-05-22 03:59:42.782029 krutils-0.20230522.1259/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1259/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 03:59:42.604765 krutils-0.20230522.1259/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1259/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1259/krutils/CONST.py
--rw-rw-rw-   0        0        0       71 2023-04-11 07:37:54.000000 krutils-0.20230522.1259/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1259/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0    12538 2023-05-22 03:59:25.000000 krutils-0.20230522.1259/krutils/logger.py
--rw-rw-rw-   0        0        0    21458 2023-05-22 03:59:08.000000 krutils-0.20230522.1259/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:59:42.756961 krutils-0.20230522.1259/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 03:59:42.800279 krutils-0.20230522.1259/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-05-22 03:59:40.000000 krutils-0.20230522.1259/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:59:42.776612 krutils-0.20230522.1259/test/
--rw-rw-rw-   0        0        0      308 2023-05-22 03:42:17.000000 krutils-0.20230522.1259/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:01:57.323566 krutils-0.20230522.1301/
+-rw-rw-rw-   0        0        0      526 2023-05-22 04:01:57.322137 krutils-0.20230522.1301/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1301/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 04:01:57.202510 krutils-0.20230522.1301/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1301/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1301/krutils/CONST.py
+-rw-rw-rw-   0        0        0       94 2023-05-22 04:01:49.000000 krutils-0.20230522.1301/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1301/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0    12538 2023-05-22 03:59:25.000000 krutils-0.20230522.1301/krutils/logger.py
+-rw-rw-rw-   0        0        0    21458 2023-05-22 03:59:08.000000 krutils-0.20230522.1301/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:01:57.297044 krutils-0.20230522.1301/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-05-22 04:01:56.000000 krutils-0.20230522.1301/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-22 04:01:56.000000 krutils-0.20230522.1301/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 04:01:56.000000 krutils-0.20230522.1301/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-22 04:01:56.000000 krutils-0.20230522.1301/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 04:01:56.000000 krutils-0.20230522.1301/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 04:01:57.323566 krutils-0.20230522.1301/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-05-22 04:01:55.000000 krutils-0.20230522.1301/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:01:57.319590 krutils-0.20230522.1301/test/
+-rw-rw-rw-   0        0        0      308 2023-05-22 03:42:17.000000 krutils-0.20230522.1301/test/test_logger.py
```

### Comparing `krutils-0.20230522.1259/PKG-INFO` & `krutils-0.20230522.1301/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1259
+Version: 0.20230522.1301
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1259/krutils/CONST.py` & `krutils-0.20230522.1301/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1259/krutils/_dbmgr.py` & `krutils-0.20230522.1301/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1259/krutils/logger.py` & `krutils-0.20230522.1301/krutils/logger.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1259/krutils/utils.py` & `krutils-0.20230522.1301/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1259/krutils.egg-info/PKG-INFO` & `krutils-0.20230522.1301/krutils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1259
+Version: 0.20230522.1301
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1259/setup.py` & `krutils-0.20230522.1301/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230522.1259",
+    version="0.20230522.1301",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

