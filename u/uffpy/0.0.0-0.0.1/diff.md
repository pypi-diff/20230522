# Comparing `tmp/uffpy-0.0.0.tar.gz` & `tmp/uffpy-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uffpy-0.0.0.tar", last modified: Fri May  6 11:03:34 2022, max compression
+gzip compressed data, was "uffpy-0.0.1.tar", last modified: Mon May 22 08:05:33 2023, max compression
```

## Comparing `uffpy-0.0.0.tar` & `uffpy-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 jaesus     (501) staff       (20)        0 2022-05-06 11:03:34.000000 uffpy-0.0.0/
--rw-r--r--   0 jaesus     (501) staff       (20)     1770 2022-05-06 11:03:34.000000 uffpy-0.0.0/PKG-INFO
--rw-r--r--   0 jaesus     (501) staff       (20)      122 2022-05-06 10:01:34.000000 uffpy-0.0.0/pyproject.toml
-drwxr-xr-x   0 jaesus     (501) staff       (20)        0 2022-05-06 11:03:34.000000 uffpy-0.0.0/uffpy.egg-info/
--rw-r--r--   0 jaesus     (501) staff       (20)     1770 2022-05-06 11:03:34.000000 uffpy-0.0.0/uffpy.egg-info/PKG-INFO
--rw-r--r--   0 jaesus     (501) staff       (20)        1 2022-05-06 10:17:16.000000 uffpy-0.0.0/uffpy.egg-info/not-zip-safe
--rw-r--r--   0 jaesus     (501) staff       (20)      250 2022-05-06 11:03:34.000000 uffpy-0.0.0/uffpy.egg-info/SOURCES.txt
--rw-r--r--   0 jaesus     (501) staff       (20)        6 2022-05-06 11:03:34.000000 uffpy-0.0.0/uffpy.egg-info/requires.txt
--rw-r--r--   0 jaesus     (501) staff       (20)        6 2022-05-06 11:03:34.000000 uffpy-0.0.0/uffpy.egg-info/top_level.txt
--rw-r--r--   0 jaesus     (501) staff       (20)        1 2022-05-06 11:03:34.000000 uffpy-0.0.0/uffpy.egg-info/dependency_links.txt
--rw-r--r--   0 jaesus     (501) staff       (20)     1061 2022-05-06 11:03:08.000000 uffpy-0.0.0/README.md
--rw-r--r--   0 jaesus     (501) staff       (20)     1250 2022-05-06 10:39:50.000000 uffpy-0.0.0/setup.py
--rw-r--r--   0 jaesus     (501) staff       (20)       38 2022-05-06 11:03:34.000000 uffpy-0.0.0/setup.cfg
--rw-r--r--   0 jaesus     (501) staff       (20)     1082 2022-05-03 07:24:59.000000 uffpy-0.0.0/LICENSE.txt
-drwxr-xr-x   0 jaesus     (501) staff       (20)        0 2022-05-06 11:03:34.000000 uffpy-0.0.0/src/
-drwxr-xr-x   0 jaesus     (501) staff       (20)        0 2022-05-06 11:03:34.000000 uffpy-0.0.0/src/python/
--rw-r--r--   0 jaesus     (501) staff       (20)     2982 2022-05-06 10:03:55.000000 uffpy-0.0.0/src/python/uffpy.cpp
--rw-r--r--   0 jaesus     (501) staff       (20)     4476 2022-05-06 09:23:27.000000 uffpy-0.0.0/src/uff.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:05:33.451288 uffpy-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-22 08:05:25.000000 uffpy-0.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-22 08:05:33.447288 uffpy-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-22 08:05:25.000000 uffpy-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-22 08:05:25.000000 uffpy-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:05:33.451288 uffpy-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-22 08:05:25.000000 uffpy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:05:33.447288 uffpy-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:05:33.447288 uffpy-0.0.1/src/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-22 08:05:25.000000 uffpy-0.0.1/src/python/uffpy.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:05:33.447288 uffpy-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-22 08:05:25.000000 uffpy-0.0.1/tests/test_uffpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:05:33.447288 uffpy-0.0.1/uffpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-22 08:05:33.000000 uffpy-0.0.1/uffpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-22 08:05:33.000000 uffpy-0.0.1/uffpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:05:33.000000 uffpy-0.0.1/uffpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:05:33.000000 uffpy-0.0.1/uffpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 08:05:33.000000 uffpy-0.0.1/uffpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 08:05:33.000000 uffpy-0.0.1/uffpy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `uffpy-0.0.0/PKG-INFO` & `uffpy-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: uffpy
-Version: 0.0.0
+Version: 0.0.1
 Summary: Unique vertices finder
 Home-page: https://github.com/tataratat/uff
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # uff
 _`U`ff, once upon a time, I've created a mesh with a lot of duplicating vertices and needed to `F`ind unique vertices `F`ast._
@@ -61,9 +62,7 @@
 _option2: DIY_
 ```
 git clone git@github.com:tataratat/uff.git
 cd uff
 pip install -r requirements.txt
 python3 setup.py install   # or `pip install .`
 ```
-
-
```

### Comparing `uffpy-0.0.0/uffpy.egg-info/PKG-INFO` & `uffpy-0.0.1/uffpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: uffpy
-Version: 0.0.0
+Version: 0.0.1
 Summary: Unique vertices finder
 Home-page: https://github.com/tataratat/uff
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # uff
 _`U`ff, once upon a time, I've created a mesh with a lot of duplicating vertices and needed to `F`ind unique vertices `F`ast._
@@ -61,9 +62,7 @@
 _option2: DIY_
 ```
 git clone git@github.com:tataratat/uff.git
 cd uff
 pip install -r requirements.txt
 python3 setup.py install   # or `pip install .`
 ```
-
-
```

### Comparing `uffpy-0.0.0/README.md` & `uffpy-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `uffpy-0.0.0/LICENSE.txt` & `uffpy-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

