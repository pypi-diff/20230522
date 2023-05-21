# Comparing `tmp/sagemath-bliss-10.0.tar.gz` & `tmp/sagemath-bliss-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath-bliss-10.0.tar", last modified: Sun May 21 22:55:43 2023, max compression
+gzip compressed data, was "sagemath-bliss-9.8b1.tar", last modified: Mon Nov 21 07:31:28 2022, max compression
```

## Comparing `sagemath-bliss-10.0.tar` & `sagemath-bliss-9.8b1.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:43.688439 sagemath-bliss-10.0/
--rw-r--r--   0 mkoeppe    (502) staff       (20)      245 2023-05-21 22:13:07.000000 sagemath-bliss-10.0/MANIFEST.in
--rw-r--r--   0 mkoeppe    (502) staff       (20)     2369 2023-05-21 22:55:43.688661 sagemath-bliss-10.0/PKG-INFO
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1296 2023-05-21 19:28:13.000000 sagemath-bliss-10.0/README.rst
--rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2023-05-21 19:35:13.000000 sagemath-bliss-10.0/VERSION.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)      290 2023-05-21 22:14:21.000000 sagemath-bliss-10.0/pyproject.toml
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:43.683415 sagemath-bliss-10.0/sage/
--rw-r--r--   0 mkoeppe    (502) staff       (20)        0 2023-05-21 19:57:48.000000 sagemath-bliss-10.0/sage/all__sagemath_bliss.py
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:43.684517 sagemath-bliss-10.0/sage/graphs/
--rw-r--r--   0 mkoeppe    (502) staff       (20)        0 2023-05-21 19:57:48.000000 sagemath-bliss-10.0/sage/graphs/all__sagemath_bliss.py
--rw-r--r--   0 mkoeppe    (502) staff       (20)    34209 2023-05-21 19:10:21.000000 sagemath-bliss-10.0/sage/graphs/bliss.pyx
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:43.687973 sagemath-bliss-10.0/sagemath_bliss.egg-info/
--rw-r--r--   0 mkoeppe    (502) staff       (20)     2369 2023-05-21 22:55:40.000000 sagemath-bliss-10.0/sagemath_bliss.egg-info/PKG-INFO
--rw-r--r--   0 mkoeppe    (502) staff       (20)      342 2023-05-21 22:55:43.000000 sagemath-bliss-10.0/sagemath_bliss.egg-info/SOURCES.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2023-05-21 22:55:40.000000 sagemath-bliss-10.0/sagemath_bliss.egg-info/dependency_links.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)       24 2023-05-21 22:55:40.000000 sagemath-bliss-10.0/sagemath_bliss.egg-info/requires.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2023-05-21 22:55:40.000000 sagemath-bliss-10.0/sagemath_bliss.egg-info/top_level.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1092 2023-05-21 22:55:43.689479 sagemath-bliss-10.0/setup.cfg
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1944 2023-05-21 22:43:29.000000 sagemath-bliss-10.0/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.289780 sagemath-bliss-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-bliss-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2370 2022-11-21 07:31:28.289916 sagemath-bliss-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1296 2022-11-20 23:45:29.000000 sagemath-bliss-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-bliss-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.285772 sagemath-bliss-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.287619 sagemath-bliss-9.8b1/sage/graphs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)    34899 2022-11-16 06:02:58.000000 sagemath-bliss-9.8b1/sage/graphs/bliss.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.289510 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2370 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      267 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1093 2022-11-21 07:31:28.290521 sagemath-bliss-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2057 2022-11-20 23:45:29.000000 sagemath-bliss-9.8b1/setup.py
```

### Comparing `sagemath-bliss-10.0/PKG-INFO` & `sagemath-bliss-9.8b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-bliss
-Version: 10.0
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
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

### Comparing `sagemath-bliss-10.0/README.rst` & `sagemath-bliss-9.8b1/README.rst`

 * *Files 0% similar despite different names*

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

### Comparing `sagemath-bliss-10.0/sage/graphs/bliss.pyx` & `sagemath-bliss-9.8b1/sage/graphs/bliss.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -704,20 +704,20 @@
         sage: automorphism_group(G,partition=[[1,2],[0,3],[4]]).cardinality()   # optional - bliss
         2
 
     Partitioning the edges into classes::
 
         sage: G = Graph(graphs.CompleteMultipartiteGraph([8, 2]), sparse=True)  # optional - bliss
         sage: for i,j in G.edges(labels=False, sort=False):                     # optional - bliss
-        ....:     if 0 <= i < 3:
-        ....:         G.set_edge_label(i, j, "A")
-        ....:     if 3 <= i < 6:
-        ....:         G.set_edge_label(i, j, "B")
-        ....:     if 6 <= i < 8:
-        ....:         G.set_edge_label(i, j, "C")
+        ....:     if 0 <= i < 3:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "A")                               # optional - bliss
+        ....:     if 3 <= i < 6:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "B")                               # optional - bliss
+        ....:     if 6 <= i < 8:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "C")                               # optional - bliss
 
         sage: factor(automorphism_group(G).cardinality())                       # optional - bliss
         2^4 * 3^2
         sage: automorphism_group(G,[[0],[1],[2,3],[4,5],[6,7],[8],[9]]).cardinality()   # optional - bliss
         4
 
     TESTS::
@@ -736,20 +736,20 @@
         sage: G = graphs.CompleteMultipartiteGraph([5,7,11])
         sage: B = automorphism_group(G)                                         # optional - bliss
         sage: B.cardinality() == prod(factorial(n) for n in [5,7,11])           # optional - bliss
         True
 
         sage: G = Graph(graphs.CompleteMultipartiteGraph([8,8,8,5]),sparse=True)# optional - bliss
         sage: for i,j in G.edges(labels=False, sort=False):                     # optional - bliss
-        ....:     if 0 <= i < 3:
-        ....:         G.set_edge_label(i, j, "A")
-        ....:     if 3 <= i < 6:
-        ....:         G.set_edge_label(i, j, "B")
-        ....:     if 6 <= i < 8:
-        ....:         G.set_edge_label(i, j, "C")
+        ....:     if 0 <= i < 3:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "A")                               # optional - bliss
+        ....:     if 3 <= i < 6:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "B")                               # optional - bliss
+        ....:     if 6 <= i < 8:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "C")                               # optional - bliss
         sage: automorphism_group(G).cardinality() == prod( factorial(n) for n in [3,3,2,8,8,5,2] )  # optional - bliss
         True
         sage: automorphism_group(G, use_edge_labels=False).cardinality() == prod( factorial(n) for n in [8,8,8,5,3] )  # optional - bliss
         True
         sage: automorphism_group(G,[[0 .. 7],[8 .. 11],[12 .. 28]]).cardinality() == prod( factorial(n) for n in [3,3,2,4,4,8,5] )  # optional - bliss
         True
```

### Comparing `sagemath-bliss-10.0/sagemath_bliss.egg-info/PKG-INFO` & `sagemath-bliss-9.8b1/sagemath_bliss.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-bliss
-Version: 10.0
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
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

### Comparing `sagemath-bliss-10.0/setup.cfg` & `sagemath-bliss-9.8b1/setup.cfg`

 * *Files 2% similar despite different names*

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

### Comparing `sagemath-bliss-10.0/setup.py` & `sagemath-bliss-9.8b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-bliss']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-bliss'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-bliss'])
 
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

