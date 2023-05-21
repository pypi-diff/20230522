# Comparing `tmp/sagemath-meataxe-10.0.tar.gz` & `tmp/sagemath-meataxe-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath-meataxe-10.0.tar", last modified: Sun May 21 22:55:43 2023, max compression
+gzip compressed data, was "sagemath-meataxe-9.8b1.tar", last modified: Mon Nov 21 07:45:53 2022, max compression
```

## Comparing `sagemath-meataxe-10.0.tar` & `sagemath-meataxe-9.8b1.tar`

### file list

```diff
@@ -1,24 +1,18 @@
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:43.694017 sagemath-meataxe-10.0/
--rw-r--r--   0 mkoeppe    (502) staff       (20)      330 2023-05-21 22:55:30.000000 sagemath-meataxe-10.0/MANIFEST.in
--rw-r--r--   0 mkoeppe    (502) staff       (20)     2588 2023-05-21 22:55:43.694250 sagemath-meataxe-10.0/PKG-INFO
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1511 2023-05-21 19:28:13.000000 sagemath-meataxe-10.0/README.rst
--rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2023-05-21 19:35:13.000000 sagemath-meataxe-10.0/VERSION.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)      290 2023-05-21 22:14:22.000000 sagemath-meataxe-10.0/pyproject.toml
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:43.684945 sagemath-meataxe-10.0/sage/
--rw-r--r--   0 mkoeppe    (502) staff       (20)        0 2023-05-21 20:03:00.000000 sagemath-meataxe-10.0/sage/all__sagemath_meataxe.py
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:43.687250 sagemath-meataxe-10.0/sage/libs/
--rw-r--r--   0 mkoeppe    (502) staff       (20)        0 2023-05-21 20:01:38.000000 sagemath-meataxe-10.0/sage/libs/all__sagemath_meataxe.py
--rw-r--r--   0 mkoeppe    (502) staff       (20)     6644 2023-05-21 20:46:55.000000 sagemath-meataxe-10.0/sage/libs/meataxe.pxd
--rw-r--r--   0 mkoeppe    (502) staff       (20)     3576 2023-05-21 19:10:12.000000 sagemath-meataxe-10.0/sage/libs/meataxe.pyx
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:43.689418 sagemath-meataxe-10.0/sage/matrix/
--rw-r--r--   0 mkoeppe    (502) staff       (20)        0 2023-05-21 20:03:00.000000 sagemath-meataxe-10.0/sage/matrix/all__sagemath_meataxe.py
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1628 2023-05-21 20:49:00.000000 sagemath-meataxe-10.0/sage/matrix/matrix_gfpn_dense.pxd
--rw-r--r--   0 mkoeppe    (502) staff       (20)    71632 2023-05-21 19:10:21.000000 sagemath-meataxe-10.0/sage/matrix/matrix_gfpn_dense.pyx
-drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2023-05-21 22:55:43.693558 sagemath-meataxe-10.0/sagemath_meataxe.egg-info/
--rw-r--r--   0 mkoeppe    (502) staff       (20)     2588 2023-05-21 22:55:40.000000 sagemath-meataxe-10.0/sagemath_meataxe.egg-info/PKG-INFO
--rw-r--r--   0 mkoeppe    (502) staff       (20)      481 2023-05-21 22:55:43.000000 sagemath-meataxe-10.0/sagemath_meataxe.egg-info/SOURCES.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2023-05-21 22:55:40.000000 sagemath-meataxe-10.0/sagemath_meataxe.egg-info/dependency_links.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)       24 2023-05-21 22:55:40.000000 sagemath-meataxe-10.0/sagemath_meataxe.egg-info/requires.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2023-05-21 22:55:40.000000 sagemath-meataxe-10.0/sagemath_meataxe.egg-info/top_level.txt
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1220 2023-05-21 22:55:43.695185 sagemath-meataxe-10.0/setup.cfg
--rw-r--r--   0 mkoeppe    (502) staff       (20)     1948 2023-05-21 22:43:29.000000 sagemath-meataxe-10.0/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.708990 sagemath-meataxe-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:46:42.000000 sagemath-meataxe-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2589 2022-11-21 07:45:53.709134 sagemath-meataxe-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1511 2022-11-21 07:44:45.000000 sagemath-meataxe-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:43.000000 sagemath-meataxe-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.704823 sagemath-meataxe-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.706668 sagemath-meataxe-9.8b1/sage/libs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     3576 2022-10-12 20:41:10.000000 sagemath-meataxe-9.8b1/sage/libs/meataxe.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.706957 sagemath-meataxe-9.8b1/sage/matrix/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)    71714 2022-10-12 20:41:10.000000 sagemath-meataxe-9.8b1/sage/matrix/matrix_gfpn_dense.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:45:53.708719 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2589 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      311 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:45:53.000000 sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1097 2022-11-21 07:45:53.709827 sagemath-meataxe-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2061 2022-11-20 23:46:42.000000 sagemath-meataxe-9.8b1/setup.py
```

### Comparing `sagemath-meataxe-10.0/PKG-INFO` & `sagemath-meataxe-9.8b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-meataxe
-Version: 10.0
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with meataxe
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

### Comparing `sagemath-meataxe-10.0/README.rst` & `sagemath-meataxe-9.8b1/README.rst`

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

### Comparing `sagemath-meataxe-10.0/sage/libs/meataxe.pyx` & `sagemath-meataxe-9.8b1/sage/libs/meataxe.pyx`

 * *Files identical despite different names*

### Comparing `sagemath-meataxe-10.0/sage/matrix/matrix_gfpn_dense.pyx` & `sagemath-meataxe-9.8b1/sage/matrix/matrix_gfpn_dense.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 
 AUTHORS:
 
 - Simon King (2015-09): initial version
 
 """
 
-# ***************************************************************************
+#*****************************************************************************
 #       Copyright (C) 2015 Simon King <simon.king@uni-jena.de>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 2 of the License, or
 # (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-# ***************************************************************************
+#                  http://www.gnu.org/licenses/
+#*****************************************************************************
 
 from cysignals.memory cimport check_realloc, check_malloc, sig_free
 from cpython.bytes cimport PyBytes_AsString, PyBytes_FromStringAndSize
+from sage.cpython.string cimport str_to_bytes
 from cysignals.signals cimport sig_on, sig_off, sig_check
 cimport cython
 
 import os
 
 ####################
 #
@@ -100,19 +101,19 @@
 
         sage: from sage.matrix.matrix_gfpn_dense import Matrix_gfpn_dense
         sage: F.<y> = GF(125)
         sage: M = MatrixSpace(F, 2, 2, implementation=Matrix_gfpn_dense).one()
         sage: C = M._converter
         sage: C.fel_to_field(15)
         3*y
-        sage: F.from_integer(15)
+        sage: F.fetch_int(15)
         3*y
         sage: C.field_to_fel(y)
         5
-        sage: y.to_integer()
+        sage: y.integer_representation()
         5
     """
     def __init__(self, field):
         """
         INPUT:
 
         A finite field with Givaro implementation and at most 251
@@ -134,15 +135,15 @@
         EXAMPLES::
 
             sage: from sage.matrix.matrix_gfpn_dense import FieldConverter_class
             sage: F.<y> = GF(125)
             sage: C = FieldConverter_class(F)
             sage: C.fel_to_field(15)
             3*y
-            sage: F.from_integer(15)
+            sage: F.fetch_int(15)
             3*y
         """
         return self.field(FfToInt(x))
 
     cpdef FEL field_to_fel(self, x) except 255:
         """
         Represent a field element by a python int.
@@ -150,27 +151,27 @@
         EXAMPLES::
 
             sage: from sage.matrix.matrix_gfpn_dense import FieldConverter_class
             sage: F.<y> = GF(125)
             sage: C = FieldConverter_class(F)
             sage: C.field_to_fel(y)
             5
-            sage: y.to_integer()
+            sage: y.integer_representation()
             5
 
         TESTS:
 
         Test invalid input::
 
             sage: C.field_to_fel('foo')
             Traceback (most recent call last):
             ...
-            AttributeError: 'str' object has no attribute 'to_integer'
+            AttributeError: 'str' object has no attribute 'integer_representation'
         """
-        return FfFromInt(x.to_integer())
+        return FfFromInt(x.integer_representation())
 
 
 cdef class PrimeFieldConverter_class(FieldConverter_class):
     """
     An auxiliary class, used to convert between meataxe ``FEL`` and
     finite field elements.
 
@@ -1880,15 +1881,15 @@
         sage: t = b'Uq\x82\x00\x00\x00\x00\x00\xa7\x8bh\x00\x00\x00\x00\x00'
         sage: len(t)
         16
         sage: N == mtx_unpickle(MS, 2, 5, t, True)
         doctest:warning
         ...
         DeprecationWarning: Reading this pickle may be machine dependent
-        See https://github.com/sagemath/sage/issues/23411 for details.
+        See http://trac.sagemath.org/23411 for details.
         True
 
     Unpickling would even work in the case that the machine creating
     the deprecated pickle had ``sizeof(long)==9``::
 
         sage: t = b'Uq\x82\x00\x00\x00\x00\x00\x00\xa7\x8bh\x00\x00\x00\x00\x00\x00'
         sage: len(t)
@@ -1932,15 +1933,15 @@
     """
     # The expected input type is bytes. However, Python-2 legacy pickles do
     # not distinguish between str and bytes. If such pickle is unpickled
     # in Python-3, Sage will receive a str in `latin1` encoding. Therefore,
     # in the following line, we use a helper function that would return bytes,
     # regardless whether the input is bytes or str.
     cdef bytes Data = str_to_bytes(data, encoding='latin1')
-    if isinstance(f, int):
+    if isinstance(f, (int, long)):
         # This is for old pickles created with the group cohomology spkg
         MS = MatrixSpace(GF(f, 'z'), nr, nc, implementation=Matrix_gfpn_dense)
     else:
         MS = f
         if MS.nrows() != nr or MS.ncols() != nc:
             raise ValueError("Inconsistent dimensions in this matrix pickle")
         f = MS.base_ring().order()
```

### Comparing `sagemath-meataxe-10.0/sagemath_meataxe.egg-info/PKG-INFO` & `sagemath-meataxe-9.8b1/sagemath_meataxe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-meataxe
-Version: 10.0
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with meataxe
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

### Comparing `sagemath-meataxe-10.0/setup.cfg` & `sagemath-meataxe-9.8b1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -22,22 +22,13 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
 python_requires = >=3.8, <3.12
 install_requires = 
-	sagemath-standard ~= 10.0
-packages = 
-	sage.libs
-	sage.matrix
-
-[options.package_data]
-sage.libs = 
-	meataxe.pxd
-sage.matrix = 
-	matrix_gfpn_dense.pxd
+	sagemath-standard ~= 9.8b3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sagemath-meataxe-10.0/setup.py` & `sagemath-meataxe-9.8b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-meataxe']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-meataxe'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-meataxe'])
 
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

