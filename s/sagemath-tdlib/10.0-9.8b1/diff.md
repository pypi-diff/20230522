# Comparing `tmp/sagemath-tdlib-10.0.tar.gz` & `tmp/sagemath-tdlib-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath-tdlib-10.0.tar", last modified: Sun May 21 22:55:47 2023, max compression
+gzip compressed data, was "sagemath-tdlib-9.8b1.tar", last modified: Mon Nov 21 07:31:30 2022, max compression
```

## Comparing `sagemath-tdlib-10.0.tar` & `sagemath-tdlib-9.8b1.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:47.308095 sagemath-tdlib-10.0/
--rw-r--r--   0 mkoeppe    (502) staff       (20)      302 2023-05-21 22:46:00.000000 sagemath-tdlib-10.0/MANIFEST.in
--rw-r--r--   0 mkoeppe    (502) staff       (20)     2349 2023-05-21 22:55:47.308340 sagemath-tdlib-10.0/PKG-INFO
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1276 2023-05-21 19:28:13.000000 sagemath-tdlib-10.0/README.rst
--rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2023-05-21 19:35:13.000000 sagemath-tdlib-10.0/VERSION.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)      290 2023-05-21 22:14:21.000000 sagemath-tdlib-10.0/pyproject.toml
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:47.302735 sagemath-tdlib-10.0/sage/
--rw-r--r--   0 mkoeppe    (502) staff       (20)        0 2023-05-21 19:59:00.000000 sagemath-tdlib-10.0/sage/all__sagemath_tdlib.py
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:47.303177 sagemath-tdlib-10.0/sage/graphs/
--rw-r--r--   0 mkoeppe    (502) staff       (20)        0 2023-05-21 19:59:00.000000 sagemath-tdlib-10.0/sage/graphs/all__sagemath_tdlib.py
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:47.304712 sagemath-tdlib-10.0/sage/graphs/graph_decompositions/
--rw-r--r--   0 mkoeppe    (502) staff       (20)        0 2023-05-21 19:59:00.000000 sagemath-tdlib-10.0/sage/graphs/graph_decompositions/all__sagemath_tdlib.py
--rw-r--r--   0 mkoeppe    (502) staff       (20)     2643 2021-12-20 22:27:44.000000 sagemath-tdlib-10.0/sage/graphs/graph_decompositions/sage_tdlib.cpp
--rw-r--r--   0 mkoeppe    (502) staff       (20)     5663 2022-10-12 20:41:10.000000 sagemath-tdlib-10.0/sage/graphs/graph_decompositions/tdlib.pyx
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:47.307579 sagemath-tdlib-10.0/sagemath_tdlib.egg-info/
--rw-r--r--   0 mkoeppe    (502) staff       (20)     2349 2023-05-21 22:55:40.000000 sagemath-tdlib-10.0/sagemath_tdlib.egg-info/PKG-INFO
--rw-r--r--   0 mkoeppe    (502) staff       (20)      467 2023-05-21 22:55:47.000000 sagemath-tdlib-10.0/sagemath_tdlib.egg-info/SOURCES.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2023-05-21 22:55:40.000000 sagemath-tdlib-10.0/sagemath_tdlib.egg-info/dependency_links.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)       24 2023-05-21 22:55:40.000000 sagemath-tdlib-10.0/sagemath_tdlib.egg-info/requires.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2023-05-21 22:55:40.000000 sagemath-tdlib-10.0/sagemath_tdlib.egg-info/top_level.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1092 2023-05-21 22:55:47.309328 sagemath-tdlib-10.0/setup.cfg
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1944 2023-05-21 22:43:29.000000 sagemath-tdlib-10.0/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.702261 sagemath-tdlib-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-tdlib-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2350 2022-11-21 07:31:30.702399 sagemath-tdlib-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1276 2022-11-20 23:46:42.000000 sagemath-tdlib-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-tdlib-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.698530 sagemath-tdlib-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.698631 sagemath-tdlib-9.8b1/sage/graphs/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.700524 sagemath-tdlib-9.8b1/sage/graphs/graph_decompositions/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     5663 2022-10-12 20:41:10.000000 sagemath-tdlib-9.8b1/sage/graphs/graph_decompositions/tdlib.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.702002 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2350 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      288 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1093 2022-11-21 07:31:30.702993 sagemath-tdlib-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2057 2022-11-20 23:45:29.000000 sagemath-tdlib-9.8b1/setup.py
```

### Comparing `sagemath-tdlib-10.0/PKG-INFO` & `sagemath-tdlib-9.8b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-tdlib
-Version: 10.0
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with tdlib
 Home-page: https://www.sagemath.org
 Author: The Sage Developers
 Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
@@ -28,15 +28,15 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
 macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
```

### Comparing `sagemath-tdlib-10.0/README.rst` & `sagemath-tdlib-9.8b1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
 macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
```

### Comparing `sagemath-tdlib-10.0/sage/graphs/graph_decompositions/tdlib.pyx` & `sagemath-tdlib-9.8b1/sage/graphs/graph_decompositions/tdlib.pyx`

 * *Files identical despite different names*

### Comparing `sagemath-tdlib-10.0/sagemath_tdlib.egg-info/PKG-INFO` & `sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-tdlib
-Version: 10.0
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with tdlib
 Home-page: https://www.sagemath.org
 Author: The Sage Developers
 Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
@@ -28,15 +28,15 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
 macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
```

### Comparing `sagemath-tdlib-10.0/setup.cfg` & `sagemath-tdlib-9.8b1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
 python_requires = >=3.8, <3.12
 install_requires = 
-	sagemath-standard ~= 10.0
+	sagemath-standard ~= 9.8b3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sagemath-tdlib-10.0/setup.py` & `sagemath-tdlib-9.8b1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-tdlib']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-tdlib'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-tdlib'])
 
-log.warn('python_packages = {0}'.format(python_packages))
-log.warn('python_modules = {0}'.format(python_modules))
-log.warn('cython_modules = {0}'.format(cython_modules))
+    log.warn('python_packages = {0}'.format(python_packages))
+    log.warn('python_modules = {0}'.format(python_modules))
+    log.warn('cython_modules = {0}'.format(cython_modules))
 
 setup(
     cmdclass = cmdclass,
     packages = python_packages,
     py_modules  = python_modules,
     ext_modules = cython_modules,
 )
```

