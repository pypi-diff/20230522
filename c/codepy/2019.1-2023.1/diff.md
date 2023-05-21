# Comparing `tmp/codepy-2019.1.tar.gz` & `tmp/codepy-2023.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codepy-2019.1.tar", last modified: Sat Jul  6 17:18:00 2019, max compression
+gzip compressed data, was "codepy-2023.1.tar", last modified: Sun May 21 22:57:35 2023, max compression
```

## Comparing `codepy-2019.1.tar` & `codepy-2023.1.tar`

### file list

```diff
@@ -1,40 +1,36 @@
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-07-06 17:18:00.000000 codepy-2019.1/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      239 2015-10-17 19:25:54.000000 codepy-2019.1/MANIFEST.in
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1350 2019-07-06 17:18:00.000000 codepy-2019.1/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)      553 2015-10-17 19:25:54.000000 codepy-2019.1/README.rst
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-07-06 17:18:00.000000 codepy-2019.1/codepy/
--rw-r--r--   0 andreas   (1000) andreas   (1000)       40 2015-10-17 19:25:54.000000 codepy-2019.1/codepy/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     5473 2015-10-17 19:25:54.000000 codepy-2019.1/codepy/bpl.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-07-06 17:18:00.000000 codepy-2019.1/codepy/cgen/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      269 2015-10-17 19:25:54.000000 codepy-2019.1/codepy/cgen/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4408 2015-10-17 19:25:54.000000 codepy-2019.1/codepy/cuda.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     5824 2018-01-25 16:01:16.000000 codepy-2019.1/codepy/elementwise.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-07-06 17:18:00.000000 codepy-2019.1/codepy/include/
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-07-06 17:18:00.000000 codepy-2019.1/codepy/include/codepy/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      931 2015-10-17 19:25:54.000000 codepy-2019.1/codepy/include/codepy/bpl.hpp
--rw-r--r--   0 andreas   (1000) andreas   (1000)    16167 2018-11-10 22:23:31.000000 codepy-2019.1/codepy/jit.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     5159 2017-09-07 20:40:56.000000 codepy-2019.1/codepy/libraries.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    15820 2018-06-20 19:18:44.000000 codepy-2019.1/codepy/toolchain.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      850 2017-08-11 17:38:18.000000 codepy-2019.1/codepy/tools.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-07-06 17:18:00.000000 codepy-2019.1/codepy.egg-info/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1350 2019-07-06 17:18:00.000000 codepy-2019.1/codepy.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)      616 2019-07-06 17:18:00.000000 codepy-2019.1/codepy.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2019-07-06 17:18:00.000000 codepy-2019.1/codepy.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2019-01-02 17:19:50.000000 codepy-2019.1/codepy.egg-info/not-zip-safe
--rw-r--r--   0 andreas   (1000) andreas   (1000)       53 2019-07-06 17:18:00.000000 codepy-2019.1/codepy.egg-info/requires.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        7 2019-07-06 17:18:00.000000 codepy-2019.1/codepy.egg-info/top_level.txt
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-07-06 17:18:00.000000 codepy-2019.1/doc/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2344 2015-10-17 19:25:54.000000 codepy-2019.1/doc/Makefile
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-07-06 17:18:00.000000 codepy-2019.1/doc/source/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6850 2016-05-17 22:51:13.000000 codepy-2019.1/doc/source/conf.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1141 2015-10-17 19:25:54.000000 codepy-2019.1/doc/source/faq.rst
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2710 2015-10-17 19:25:54.000000 codepy-2019.1/doc/source/index.rst
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1347 2015-10-17 19:25:54.000000 codepy-2019.1/doc/source/jit.rst
--rw-r--r--   0 andreas   (1000) andreas   (1000)      189 2019-07-06 17:18:00.000000 codepy-2019.1/setup.cfg
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1253 2019-07-06 17:17:23.000000 codepy-2019.1/setup.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2019-07-06 17:18:00.000000 codepy-2019.1/test/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      391 2018-02-27 06:10:29.000000 codepy-2019.1/test/demo.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      474 2018-02-27 06:10:29.000000 codepy-2019.1/test/demo_plain.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4919 2018-02-27 06:10:29.000000 codepy-2019.1/test/nvcc-test.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      936 2018-02-27 06:10:29.000000 codepy-2019.1/test/test_identical_symbols.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      811 2018-02-27 06:10:29.000000 codepy-2019.1/test/test_two_stage_compile.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-21 22:57:35.354984 codepy-2023.1/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1091 2022-02-08 18:56:29.000000 codepy-2023.1/LICENSE
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      239 2019-10-01 22:43:51.000000 codepy-2023.1/MANIFEST.in
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1677 2023-05-21 22:57:35.354984 codepy-2023.1/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      954 2022-10-14 19:23:23.000000 codepy-2023.1/README.rst
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-21 22:57:35.354984 codepy-2023.1/codepy/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       40 2019-10-01 22:43:51.000000 codepy-2023.1/codepy/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5549 2022-02-08 18:56:29.000000 codepy-2023.1/codepy/bpl.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4575 2022-10-14 19:23:23.000000 codepy-2023.1/codepy/cuda.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5851 2022-02-08 18:56:29.000000 codepy-2023.1/codepy/elementwise.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-21 22:57:35.354984 codepy-2023.1/codepy/include/
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-21 22:57:35.354984 codepy-2023.1/codepy/include/codepy/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      931 2019-10-01 22:43:51.000000 codepy-2023.1/codepy/include/codepy/bpl.hpp
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    16291 2022-10-14 19:23:23.000000 codepy-2023.1/codepy/jit.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5081 2022-02-08 18:56:29.000000 codepy-2023.1/codepy/libraries.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    15082 2023-04-30 19:47:13.000000 codepy-2023.1/codepy/toolchain.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      818 2022-02-08 18:56:29.000000 codepy-2023.1/codepy/tools.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-21 22:57:35.354984 codepy-2023.1/codepy.egg-info/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1677 2023-05-21 22:57:35.000000 codepy-2023.1/codepy.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      546 2023-05-21 22:57:35.000000 codepy-2023.1/codepy.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2023-05-21 22:57:35.000000 codepy-2023.1/codepy.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2023-05-09 16:21:09.000000 codepy-2023.1/codepy.egg-info/not-zip-safe
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       54 2023-05-21 22:57:35.000000 codepy-2023.1/codepy.egg-info/requires.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       36 2023-05-21 22:57:35.000000 codepy-2023.1/codepy.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-21 22:57:35.354984 codepy-2023.1/doc/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      637 2022-02-08 18:56:29.000000 codepy-2023.1/doc/Makefile
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      763 2023-05-21 22:42:02.000000 codepy-2023.1/doc/conf.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-21 22:57:35.354984 codepy-2023.1/examples/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      391 2020-09-01 05:51:20.000000 codepy-2023.1/examples/demo.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      474 2020-09-01 05:51:20.000000 codepy-2023.1/examples/demo_plain.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4924 2022-02-08 18:56:29.000000 codepy-2023.1/examples/nvcc-test.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      197 2023-05-21 22:57:35.354984 codepy-2023.1/setup.cfg
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1185 2023-05-21 22:57:00.000000 codepy-2023.1/setup.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-21 22:57:35.354984 codepy-2023.1/test/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      936 2022-02-08 18:56:29.000000 codepy-2023.1/test/test_identical_symbols.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      799 2022-02-08 18:56:29.000000 codepy-2023.1/test/test_two_stage_compile.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `codepy-2019.1/PKG-INFO` & `codepy-2023.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,39 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: codepy
-Version: 2019.1
+Version: 2023.1
 Summary: Generate and execute native code at run time.
 Home-page: http://mathema.tician.de/software/codepy
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
-Description: .. image:: https://badge.fury.io/py/codepy.png
-            :target: http://pypi.python.org/pypi/codepy
-        
-        CodePy is a C/C++ metaprogramming toolkit for Python. It helps you compile
-        source code and dynamically load it into the Python interpreter.
-        This facility also works in conjunction with with `PyCuda
-        <http://mathema.tician.de/software/pycuda>`_.  Dynamic compilation and linking
-        are so far only supported in Linux with the GNU toolchain.
-        
-        See also the `documentation <http://documen.tician.de/codepy>`_ and the
-        `git tree <http://github.com/inducer/codepy>`_.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
+Requires-Python: ~=3.8
+License-File: LICENSE
+
+.. image:: https://gitlab.tiker.net/inducer/codepy/badges/main/pipeline.svg
+    :alt: Gitlab Build Status
+    :target: https://gitlab.tiker.net/inducer/codepy/commits/main
+.. image:: https://github.com/inducer/codepy/workflows/CI/badge.svg
+    :alt: Github Build Status
+    :target: https://github.com/inducer/codepy/actions?query=branch%3Amain+workflow%3ACI
+.. image:: https://badge.fury.io/py/codepy.svg
+    :alt: Python Package Index Release Page
+    :target: https://pypi.org/project/codepy/
+
+CodePy is a C/C++ metaprogramming toolkit for Python. It helps you compile
+source code and dynamically load it into the Python interpreter.
+This facility also works in conjunction with with `PyCuda
+<http://mathema.tician.de/software/pycuda>`_.  Dynamic compilation and linking
+are so far only supported in Linux with the GNU toolchain.
+
+See also the `documentation <http://documen.tician.de/codepy>`_ and the
+`git tree <http://github.com/inducer/codepy>`_.
```

### Comparing `codepy-2019.1/codepy/bpl.py` & `codepy-2023.1/codepy/bpl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 """Convenience interface for using CodePy with Boost.Python."""
 
-from __future__ import absolute_import
 
-
-
-
-class BoostPythonModule(object):
+class BoostPythonModule:
     def __init__(self, name="module", max_arity=None,
             use_private_namespace=True):
         self.name = name
         self.preamble = []
         self.mod_body = []
         self.init_body = []
 
@@ -65,69 +61,75 @@
         from cgen import (Block, Typedef, Line, Statement, Value)
 
         self.init_body.append(
             Block([
                 Typedef(Value(name, "cl")),
                 Line(),
                 Statement(
-                    "boost::python::class_<cl>(\"%s\")"
-                    ".def(codepy::no_compare_indexing_suite<cl>())" % py_name),
+                    f'boost::python::class_<cl>("{py_name}")'
+                    ".def(codepy::no_compare_indexing_suite<cl>())"),
                 ]))
 
     def add_function(self, func):
         """Add a function to be exposed. *func* is expected to be a
         :class:`cgen.FunctionBody`.
         """
 
         self.mod_body.append(func)
         from cgen import Statement
         self.init_body.append(
                 Statement(
-                    "boost::python::def(\"%s\", &%s)" % (
+                    'boost::python::def("{}", &{})'.format(
                         func.fdecl.name, func.fdecl.name)))
 
     def add_raw_function(self, func):
         """Add a function to be exposed using boost::python::raw_function.
         *func* is expected to be a :class:`cgen.FunctionBody`.
         """
         self.mod_body.append(func)
         from cgen import Statement
         self.add_raw_function_include()
-        raw_function = "boost::python::raw_function(&%s)" % func.fdecl.name
+        raw_function = f"boost::python::raw_function(&{func.fdecl.name})"
         self.init_body.append(
             Statement(
-                "boost::python::def(\"%s\", %s)" % (
+                'boost::python::def("{}", {})'.format(
                     func.fdecl.name, raw_function)))
 
-    def add_struct(self, struct, py_name=None, py_member_name_transform=lambda x: x,
-            by_value_members=set()):
+    def add_struct(self,
+            struct, py_name=None, py_member_name_transform=lambda x: x,
+            by_value_members=None):
+        if by_value_members is None:
+            by_value_members = set()
+
         from cgen import Block, Line, Statement, Typedef, Value
 
         if py_name is None:
             py_name = struct.tpname
 
         self.mod_body.append(struct)
 
         member_defs = []
         for f in struct.fields:
             py_f_name = py_member_name_transform(f.name)
             tp_lines, declarator = f.get_decl_pair()
             if f.name in by_value_members or tp_lines[0].startswith("numpy_"):
-                member_defs.append(".def(pyublas::by_value_rw_member(\"%s\", &cl::%s))"
-                        % (py_f_name, f.name))
+                member_defs.append(
+                        ".def(pyublas::by_value_rw_member"
+                        f'("{py_f_name}", &cl::{f.name}))')
             else:
-                member_defs.append(".def_readwrite(\"%s\", &cl::%s)"
-                        % (py_f_name, f.name))
+                member_defs.append(
+                        f'.def_readwrite("{py_f_name}", &cl::{f.name})'
+                        )
 
         self.init_body.append(
             Block([
                 Typedef(Value(struct.tpname, "cl")),
                 Line(),
                 Statement(
-                    "boost::python::class_<cl>(\"%s\")%s" % (
+                    'boost::python::class_<cl>("{}"){}'.format(
                         py_name, "".join(member_defs))),
                 ]))
 
     def generate(self):
         """Generate (i.e. yield) the source code of the
         module line-by-line.
         """
@@ -144,15 +146,15 @@
             mod_body = [PrivateNamespace(self.mod_body)]
         else:
             mod_body = self.mod_body
 
         body += ([Include("boost/python.hpp")]
                 + self.preamble + [Line()]
                 + mod_body
-                + [Line(), Line("BOOST_PYTHON_MODULE(%s)" % self.name)]
+                + [Line(), Line(f"BOOST_PYTHON_MODULE({self.name})")]
                 + [Block(self.init_body)])
 
         return Module(body)
 
     def compile(self, toolchain, **kwargs):
         """Return the extension module generated from the code described
         by *self*. If necessary, build the code using *toolchain* with
@@ -162,9 +164,8 @@
 
         from codepy.libraries import add_boost_python
         toolchain = toolchain.copy()
         add_boost_python(toolchain)
 
         from codepy.jit import extension_from_string
         return extension_from_string(toolchain, self.name,
-                str(self.generate())+"\n", **kwargs)
-
+                "{}\n".format(self.generate()), **kwargs)
```

### Comparing `codepy-2019.1/codepy/cuda.py` & `codepy-2023.1/codepy/cuda.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import cgen
 """Convenience interface for using CodePy with CUDA"""
 
 
-
-
-class CudaModule(object):
+class CudaModule:
     def __init__(self, boost_module, name="module"):
         """*boost_module* is a codepy.BoostPythonModule containing host code
         which calls CUDA code.
         Current limitations of nvcc preclude compiling anything which
         references Boost by nvcc, so the code needs to be split in two pieces:
-        a BoostPythonModule compiled by the host c++ compiler, as well as CUDA
+        a BoostPythonModule compiled by the host C++ compiler, as well as CUDA
         code which is compiled by nvcc.  This module allows the construction of
         CUDA code to be compiled by nvcc, as well as bridges between the CUDA
         code and the BoostPythonModule.
         """
         self.name = name
 
         self.preamble = []
         self.body = []
         self.boost_module = boost_module
-        self.boost_module.add_to_preamble([cgen.Include('cuda.h')])
+        self.boost_module.add_to_preamble([cgen.Include("cuda.h")])
 
     def add_to_preamble(self, pa):
         self.preamble.extend(pa)
 
     def add_to_module(self, body):
         """Add the :class:`cgen.Generable` instances in the iterable
         *body* to the body of the module *self*.
@@ -41,68 +39,74 @@
         self.body.append(func)
 
     def generate(self):
         """Generate (i.e. yield) the source code of the
         module line-by-line.
         """
         body = []
-        body += (self.preamble + [cgen.Line()]
-                + self.body)
+        body += (self.preamble + [cgen.Line()] + self.body)
         return cgen.Module(body)
 
-    def compile(self, host_toolchain, nvcc_toolchain, host_kwargs={},
-                nvcc_kwargs={}, **kwargs):
+    def compile(self, host_toolchain, nvcc_toolchain,
+            host_kwargs=None, nvcc_kwargs=None, **kwargs):
         """Return the extension module generated from the code described
         by *self*. If necessary, build the code using *toolchain* with
         :func:`codepy.jit.extension_from_string`. Any keyword arguments
         accept by that latter function may be passed in *kwargs*.
         """
+        if host_kwargs is None:
+            host_kwargs = {}
+
+        if nvcc_kwargs is None:
+            nvcc_kwargs = {}
 
         from codepy.libraries import add_boost_python, add_cuda
         host_toolchain = host_toolchain.copy()
         add_boost_python(host_toolchain)
         add_cuda(host_toolchain)
 
         nvcc_toolchain = nvcc_toolchain.copy()
         add_cuda(nvcc_toolchain)
 
-        host_code = str(self.boost_module.generate()) + "\n"
-        device_code = str(self.generate()) + "\n"
+        host_code = "{}\n".format(self.boost_module.generate())
+        device_code = "{}\n".format(self.generate())
 
-        from codepy.jit import compile_from_string, extension_from_string
+        from codepy.jit import compile_from_string
         from codepy.jit import link_extension
 
         local_host_kwargs = kwargs.copy()
         local_host_kwargs.update(host_kwargs)
         local_nvcc_kwargs = kwargs.copy()
         local_nvcc_kwargs.update(nvcc_kwargs)
 
         # Don't compile shared objects, just normal objects
         # (on some platforms, they're different)
-        host_checksum, host_mod_name, host_object, host_compiled = compile_from_string(
-            host_toolchain, self.boost_module.name, host_code,
-            object=True, **local_host_kwargs)
-        device_checksum, device_mod_name, device_object, device_compiled = compile_from_string(
-            nvcc_toolchain, 'gpu', device_code, 'gpu.cu',
-            object=True, **local_nvcc_kwargs)
+        host_checksum, host_mod_name, host_object, host_compiled = \
+                compile_from_string(
+                        host_toolchain, self.boost_module.name, host_code,
+                        object=True, **local_host_kwargs)
+        device_checksum, device_mod_name, device_object, device_compiled = \
+                compile_from_string(
+                        nvcc_toolchain, "gpu", device_code, "gpu.cu",
+                        object=True, **local_nvcc_kwargs)
         # The name of the shared lib depends on the hex checksums of both
-        # host and device code to prevent accidentially returned a cached
+        # host and device code to prevent accidentally returned a cached
         # module with wrong linkage
-        mod_name = "codepy.temp.%s.%s.module" % (host_checksum, device_checksum)
+        mod_name = f"codepy.temp.{host_checksum}.{device_checksum}.module"
 
         if host_compiled or device_compiled:
             return link_extension(host_toolchain,
                                   [host_object, device_object],
                                   mod_name, **kwargs)
         else:
             import os.path
 
             destination_base, first_object = os.path.split(host_object)
             module_path = os.path.join(destination_base, mod_name
                                        + host_toolchain.so_ext)
             try:
                 from imp import load_dynamic
                 return load_dynamic(mod_name, module_path)
-            except:
+            except Exception:
                 return link_extension(host_toolchain,
                                       [host_object, device_object],
                                       mod_name, **kwargs)
```

### Comparing `codepy-2019.1/codepy/elementwise.py` & `codepy-2023.1/codepy/elementwise.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,100 +1,97 @@
 """Elementwise functionality."""
 
-from __future__ import division
 
 __copyright__ = "Copyright (C) 2009 Andreas Kloeckner"
 
 
-
-
 from pytools import memoize
 import numpy
 from cgen import POD, Value, dtype_to_ctype
 
 
-
-
 class Argument:
     def __init__(self, dtype, name):
         self.dtype = numpy.dtype(dtype)
         self.name = name
 
     def __repr__(self):
-        return "%s(%r, %s)" % (
+        return "{}({!r}, {})".format(
                 self.__class__.__name__,
                 self.name,
                 self.dtype)
 
+
 class VectorArg(Argument):
     def declarator(self):
-        return Value("numpy_array<%s >" % dtype_to_ctype(self.dtype),
-                self.name+"_ary")
+        return Value(
+                "numpy_array<{} >".format(dtype_to_ctype(self.dtype)),
+                f"{self.name}_ary")
 
     def arg_name(self):
-        return self.name + "_ary"
+        return f"{self.name}_ary"
 
     struct_char = "P"
 
+
 class ScalarArg(Argument):
     def declarator(self):
         return POD(self.dtype, self.name)
 
     def arg_name(self):
         return self.name
 
     @property
     def struct_char(self):
         return self.dtype.char
 
 
-
-
 def get_elwise_module_descriptor(arguments, operation, name="kernel"):
     from codepy.bpl import BoostPythonModule
 
     from cgen import FunctionBody, FunctionDeclaration, \
             Value, POD, Struct, For, Initializer, Include, Statement, \
             Line, Block
 
-    S = Statement
+    S = Statement  # noqa: N806
 
     mod = BoostPythonModule()
     mod.add_to_preamble([
         Include("pyublas/numpy.hpp"),
         ])
 
     mod.add_to_module([
         S("namespace ublas = boost::numeric::ublas"),
         S("using namespace pyublas"),
         Line(),
         ])
 
     body = Block([
         Initializer(
-            Value("numpy_array<%s >::iterator"
-                % dtype_to_ctype(varg.dtype),
+            Value(
+                "numpy_array<{} >::iterator".format(dtype_to_ctype(varg.dtype)),
                 varg.name),
-            "args.%s_ary.begin()" % varg.name)
+            f"args.{varg.name}_ary.begin()")
         for varg in arguments if isinstance(varg, VectorArg)]
-        +[Initializer(
-            sarg.declarator(), "args." + sarg.name)
-        for sarg in arguments if isinstance(sarg, ScalarArg)]
+        + [
+            Initializer(
+                sarg.declarator(), f"args.{sarg.name}")
+            for sarg in arguments if isinstance(sarg, ScalarArg)]
         )
 
     body.extend([
         Line(),
         For("unsigned i = 0",
             "i < codepy_length",
             "++i",
             Block([S(operation)])
             )
         ])
 
-    arg_struct = Struct("arg_struct", 
+    arg_struct = Struct("arg_struct",
             [arg.declarator() for arg in arguments])
     mod.add_struct(arg_struct, "ArgStruct")
     mod.add_to_module([Line()])
 
     mod.add_function(
             FunctionBody(
                 FunctionDeclaration(
@@ -102,15 +99,14 @@
                     [POD(numpy.uintp, "codepy_length"),
                         Value("arg_struct", "args")]),
                 body))
 
     return mod
 
 
-
 def get_elwise_module_binary(arguments, operation, name="kernel", toolchain=None):
     if toolchain is None:
         from codepy.toolchain import guess_toolchain
         toolchain = guess_toolchain()
 
     toolchain = toolchain.copy()
 
@@ -118,39 +114,34 @@
     toolchain = toolchain.copy()
     add_pyublas(toolchain)
 
     return get_elwise_module_descriptor(arguments, operation, name) \
             .compile(toolchain)
 
 
-
-
 def get_elwise_kernel(arguments, operation, name="kernel", toolchain=None):
     return getattr(get_elwise_module_binary(
         arguments, operation, name, toolchain), name)
 
 
-
-
 class ElementwiseKernel:
     def __init__(self, arguments, operation, name="kernel", toolchain=None):
         self.arguments = arguments
         self.module = get_elwise_module_binary(
                 arguments, operation, name, toolchain)
         self.func = getattr(self.module, name)
 
         self.vec_arg_indices = [i for i, arg in enumerate(arguments)
                 if isinstance(arg, VectorArg)]
 
         assert self.vec_arg_indices, \
-                "ElementwiseKernel can only be used with functions that have at least one " \
-                "vector argument"
+                "ElementwiseKernel can only be used with functions " \
+                "that have at least one vector argument"
 
     def __call__(self, *args):
-        vectors = []
         args = list(args)
 
         from pytools import single_valued
         size = single_valued(args[i].size for i in self.vec_arg_indices
                 if not (isinstance(args[i], (int, float)) and args[i] == 0))
         for i in self.vec_arg_indices:
             if isinstance(args[i], (int, float)) and args[i] == 0:
@@ -162,42 +153,39 @@
             setattr(arg_struct, arg_descr.arg_name(), arg)
 
         assert not arg_struct.__dict__
 
         self.func(size, arg_struct)
 
 
-
-
 @memoize
 def make_linear_comb_kernel_with_result_dtype(
         result_dtype, scalar_dtypes, vector_dtypes):
     comp_count = len(vector_dtypes)
     from pytools import flatten
     return ElementwiseKernel([VectorArg(result_dtype, "result")] + list(flatten(
-            (ScalarArg(scalar_dtypes[i], "a%d_fac" % i), 
-                VectorArg(vector_dtypes[i], "a%d" % i))
+            (ScalarArg(scalar_dtypes[i], f"a{i}_fac"),
+                VectorArg(vector_dtypes[i], f"a{i}"))
             for i in range(comp_count))),
-            "result[i] = " + " + ".join("a%d_fac*a%d[i]" % (i, i) 
-                for i in range(comp_count)))
-
-
+            "result[i] = " + " + ".join(
+                f"a{i}_fac*a{i}[i]" for i in range(comp_count)
+                ))
 
 
 @memoize
 def make_linear_comb_kernel(scalar_dtypes, vector_dtypes):
     from pytools import common_dtype
-    result_dtype = common_dtype(scalar_dtypes+vector_dtypes)
+    result_dtype = common_dtype(scalar_dtypes + vector_dtypes)
 
     return make_linear_comb_kernel_with_result_dtype(
             result_dtype, scalar_dtypes, vector_dtypes), result_dtype
 
 
 if __name__ == "__main__":
-    import pyublas
+    import pyublas  # noqa: F401
 
     a = numpy.random.rand(50000)
     b = numpy.random.rand(50000)
 
     dtype = a.dtype
 
     lin_comb = ElementwiseKernel([
```

### Comparing `codepy-2019.1/codepy/include/codepy/bpl.hpp` & `codepy-2023.1/codepy/include/codepy/bpl.hpp`

 * *Files identical despite different names*

### Comparing `codepy-2019.1/codepy/jit.py` & `codepy-2023.1/codepy/jit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Just-in-time Python extension compilation."""
 
-from __future__ import division
 
 __copyright__ = """
 Copyright (C) 2009-17 Andreas Kloeckner
 Copyright (C) 2017 Nick Curtis
 """
 
 __license__ = """
@@ -25,15 +24,14 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
 from codepy import CompileError
 from pytools import Record
-import six
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 def _erase_dir(dir):
     from os import listdir, unlink, rmdir
@@ -63,15 +61,15 @@
 
     try:
         toolchain.build_extension(ext_file, [source_file], debug=debug)
     finally:
         _erase_dir(src_dir)
 
 
-class CleanupBase(object):
+class CleanupBase:
     pass
 
 
 class CleanupManager(CleanupBase):
     def __init__(self):
         self.cleanups = []
 
@@ -123,16 +121,16 @@
                 from time import sleep
                 sleep(sleep_delay)
 
                 attempts += 1
 
                 if attempts > 10:
                     from warnings import warn
-                    warn("could not obtain lock--delete '%s' if necessary"
-                            % self.lock_file)
+                    warn("could not obtain lock -- "
+                            f"delete '{self.lock_file}' if necessary")
 
             cleanup_m.register(self)
 
     def clean_up(self):
         import os
         os.close(self.fd)
         os.unlink(self.lock_file)
@@ -214,15 +212,15 @@
 
 
 class _SourceInfo(Record):
     pass
 
 
 def compile_from_string(toolchain, name, source_string,
-                        source_name=["module.cpp"], cache_dir=None,
+                        source_name=None, cache_dir=None,
                         debug=False, wait_on_error=None, debug_recompile=True,
                         object=False, source_is_binary=False, sleep_delay=1):
     """Returns a tuple: mod_name, file_name, recompiled.
     mod_name is the name of the module represented by a compiled object,
     file_name is the name of the compiled object, which can be built from the
     source code(s) in *source_strings* if necessary,
     recompiled is True if the object had to be recompiled, False if the cache
@@ -231,15 +229,15 @@
     are designed to be used with load_dynamic to load a python module from
     this object, if desired.
 
     Compiled code is cached in *cache_dir* and available immediately if it has
     been compiled at some point in the past.  Compiler and Python API versions
     as well as versions of include files are taken into account when examining
     the cache. If *cache_dir* is ``None``, a default location is assumed. If it
-    is ``False``, no caching is perfomed.  Proper locking is performed on the
+    is ``False``, no caching is performed.  Proper locking is performed on the
     cache directory.  Simultaneous use of the cache by multiple processes works
     as expected, but may lead to delays because of locking. By default, a
     process waits for 1 second before reattempting to acquire the *cache_dir*
     lock. A different waiting time can be specified through *sleep_delay*.
 
     The code in *source_string* will be saved to a temporary file named
     *source_name* if it needs to be compiled.
@@ -253,38 +251,43 @@
 
     If *debug_recompile*, messages are printed indicating whether a
     recompilation is taking place.
 
     If *source_is_binary*, the source string is a compile object file and
     should be treated as binary for read/write purposes
     """
+    if source_name is None:
+        source_name = ["module.cpp"]
 
     # first ensure that source strings and names are lists
-    if isinstance(source_string, six.string_types) \
-            or (source_is_binary and isinstance(source_string, six.binary_type)):
+    if isinstance(source_string, str) \
+            or (source_is_binary and isinstance(source_string, bytes)):
         source_string = [source_string]
 
     if isinstance(source_name, str):
         source_name = [source_name]
 
     if wait_on_error is not None:
         from warnings import warn
         warn("wait_on_error is deprecated and has no effect",
                 DeprecationWarning)
 
     import os
-    from os.path import join
 
     if cache_dir is None:
-        import appdirs
+        try:
+            import platformdirs as appdirs
+        except ImportError:
+            import appdirs
+
         import sys
-        cache_dir = join(
+        cache_dir = os.path.join(
                 appdirs.user_cache_dir("codepy", "codepy"),
-                "codepy-compiler-cache-v5-py%s" % (
-                    ".".join(str(i) for i in sys.version_info),))
+                "codepy-compiler-cache-v5-py{}".format(
+                    ".".join(str(i) for i in sys.version_info)))
 
         try:
             os.makedirs(cache_dir)
         except OSError as e:
             from errno import EEXIST
             if e.errno != EEXIST:
                 raise
@@ -325,61 +328,64 @@
             import md5
             checksum = md5.new()
 
         for source in source_string:
             if source_is_binary:
                 checksum.update(source)
             else:
-                checksum.update(source.encode('utf-8'))
-        checksum.update(str(toolchain.abi_id()).encode('utf-8'))
+                checksum.update(source.encode("utf-8"))
+        checksum.update(str(toolchain.abi_id()).encode("utf-8"))
         return checksum.hexdigest()
 
     def load_info(info_path):
-        from six.moves.cPickle import load
+        import pickle
 
         try:
-            info_file = open(info_path, 'rb')
-        except IOError:
+            info_file = open(info_path, "rb")
+        except OSError:
             raise _InvalidInfoFile()
 
         try:
-            return load(info_file)
+            return pickle.load(info_file)
         except EOFError:
             raise _InvalidInfoFile()
         finally:
             info_file.close()
 
     def check_deps(deps):
         for name, date, md5sum in deps:
             try:
                 possibly_updated = os.stat(name).st_mtime != date
             except OSError as e:
                 if debug_recompile:
-                    logger.info("recompiling because dependency %s is "
-                    "inaccessible (%s)." % (name, e))
+                    logger.info(
+                            "recompiling because dependency %s is "
+                            "inaccessible (%s).", name, e)
                 return False
             else:
                 if possibly_updated and md5sum != get_file_md5sum(name):
                     if debug_recompile:
-                        logger.info("recompiling because dependency %s was "
-                        "updated." % name)
+                        logger.info(
+                                "recompiling because dependency %s was "
+                                "updated.", name)
                     return False
 
         return True
 
     def check_source(source_path):
         valid = True
         for i, path in enumerate(source_path):
             source = source_string[i]
             try:
                 src_f = open(path, "r" if not source_is_binary else "rb")
-            except IOError:
+            except OSError:
                 if debug_recompile:
-                    logger.info("recompiling because cache directory does "
-                            "not contain source file '%s'." % path)
+                    logger.info(
+                            "recompiling because cache directory does "
+                            "not contain source file '%s'.", path)
                 return False
 
             valid = valid and src_f.read() == source
             src_f.close()
 
             if not valid:
                 from warnings import warn
@@ -390,63 +396,63 @@
 
     try:
         # Variable 'lock_m' is used for no other purpose than
         # to keep lock manager alive.
         lock_m = CacheLockManager(cleanup_m, cache_dir, sleep_delay)  # noqa
 
         hex_checksum = calculate_hex_checksum()
-        mod_name = "codepy.temp.%s.%s" % (hex_checksum, name)
+        mod_name = f"codepy.temp.{hex_checksum}.{name}"
         if object:
             suffix = toolchain.o_ext
         else:
             suffix = toolchain.so_ext
 
         mod_cache_dir_m = ModuleCacheDirManager(cleanup_m,
-                join(cache_dir, hex_checksum))
+                os.path.join(cache_dir, hex_checksum))
         info_path = mod_cache_dir_m.sub("info")
-        ext_file = mod_cache_dir_m.sub(name+suffix)
+        ext_file = mod_cache_dir_m.sub(name + suffix)
 
         if mod_cache_dir_m.existed:
             try:
                 info = load_info(info_path)
             except _InvalidInfoFile:
                 mod_cache_dir_m.reset()
 
                 if debug_recompile:
-                    logger.info("recompiling for invalid cache dir (%s)." % (
-                            mod_cache_dir_m.path))
+                    logger.info("recompiling for invalid cache dir (%s).",
+                            mod_cache_dir_m.path)
             else:
                 if check_deps(info.dependencies) and check_source(
                         [mod_cache_dir_m.sub(x) for x in info.source_name]):
                     return hex_checksum, mod_name, ext_file, False
         else:
             if debug_recompile:
-                logger.info("recompiling for non-existent cache dir (%s)." % (
-                        mod_cache_dir_m.path))
+                logger.info("recompiling for non-existent cache dir (%s).",
+                        mod_cache_dir_m.path)
 
         source_paths = [mod_cache_dir_m.sub(source) for source in source_name]
 
         write_source(source_paths)
 
         if object:
             toolchain.build_object(ext_file, source_paths, debug=debug)
         else:
             toolchain.build_extension(ext_file, source_paths, debug=debug)
 
         if info_path is not None:
-            from six.moves.cPickle import dump
+            import pickle
 
             info_file = open(info_path, "wb")
-            dump(_SourceInfo(
+            pickle.dump(_SourceInfo(
                 dependencies=get_dep_structure(source_paths),
                 source_name=source_name), info_file)
             info_file.close()
 
         return hex_checksum, mod_name, ext_file, True
-    except:
+    except Exception:
         cleanup_m.error_clean_up()
         raise
     finally:
         cleanup_m.clean_up()
 
 
 def link_extension(toolchain, objects, mod_name, cache_dir=None,
@@ -460,15 +466,15 @@
         destination = os.path.join(
                 destination_base,
                 mod_name + toolchain.so_ext)
     try:
         toolchain.link_extension(destination, objects, debug=debug)
     except CompileError:
         if wait_on_error:
-            six.moves.input("Link error, examine %s, then press [Enter]" % objects)
+            input(f"Link error, examine {objects}, then press [Enter]")
             raise
 
     # try loading it
     from imp import load_dynamic
     return load_dynamic(mod_name, destination)
```

### Comparing `codepy-2019.1/codepy/libraries.py` & `codepy-2023.1/codepy/libraries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Configure JIT platforms to link with external libraries."""
 
-from __future__ import division
-
 __copyright__ = "Copyright (C) 2008 Andreas Kloeckner"
 
 
 from pytools import memoize
-import six
 
 
 def search_on_path(filenames):
     """Find file on system path."""
     # http://aspn.activestate.com/ASPN/Cookbook/Python/Recipe/52224
 
     from os.path import exists, join, abspath
@@ -40,15 +37,15 @@
 
         return expand_str(repl, options)
 
     return re.subn(r"\$\{([a-zA-Z0-9_]+)\}", my_repl, s)[0]
 
 
 def expand_value(v, options):
-    if isinstance(v, (str, six.text_type)):
+    if isinstance(v, str):
         return expand_str(v, options)
     elif isinstance(v, list):
         return [expand_value(i, options) for i in v]
     else:
         return v
 
 
@@ -61,19 +58,19 @@
 @memoize
 def get_aksetup_config():
     def update_config(fname):
         import os
         if os.access(fname, os.R_OK):
             filevars = {}
 
-            with open(fname, "r") as cf_file:
+            with open(fname) as cf_file:
                 file_contents = cf_file.read()
-            exec(compile(file_contents, fname, 'exec'), filevars)
+            exec(compile(file_contents, fname, "exec"), filevars)
 
-            for key, value in six.iteritems(filevars):
+            for key, value in filevars.items():
                 if key != "__builtins__":
                     config[key] = value
 
     config = {}
     from os.path import expanduser
     update_config(expanduser("~/.aksetup-defaults.py"))
 
@@ -86,30 +83,30 @@
 # }}}
 
 
 # {{{ libraries
 
 def get_boost_libname(basename, aksetup):
     try:
-        return aksetup["BOOST_%s_LIBNAME" % basename.upper()]
+        return aksetup[f"BOOST_{basename.upper()}_LIBNAME"]
     except KeyError:
-        return ["boost_%s" % (basename)]
+        return [f"boost_{basename}"]
 
 
 def add_boost_python(toolchain):
     aksetup = get_aksetup_config()
     import sys
     toolchain.add_library(
             "boost-python",
             aksetup.get("BOOST_INC_DIR", []),
             aksetup.get("BOOST_LIB_DIR", []),
-            get_boost_libname("python-py%d%d" % sys.version_info[:2], aksetup)
-            + ["python%d.%d%s" % (
-                sys.version_info[:2] + (
-                    "m" if sys.version_info[0] >= 3 else "",))]
+            get_boost_libname("python-py{}{}".format(*sys.version_info[:2]), aksetup)
+            + ["python{}.{}{}".format(
+                *sys.version_info[:2],
+                "m" if sys.version_info[0] >= 3 else "")]
             )
 
 
 def add_boost_numeric_bindings(toolchain):
     aksetup = get_aksetup_config()
     toolchain.add_library(
             "boost-numeric-bindings",
@@ -125,15 +122,15 @@
 
     toolchain.add_library("numpy", [get_numpy_incpath()], [], [])
 
 
 def add_py_module(toolchain, name):
     def get_module_include_path(name):
         from pkg_resources import Requirement, resource_filename
-        return resource_filename(Requirement.parse(name), "%s/include" % name)
+        return resource_filename(Requirement.parse(name), f"{name}/include")
 
     toolchain.add_library(name, [get_module_include_path(name)], [], [])
 
 
 def add_codepy(toolchain):
     add_py_module(toolchain, "codepy")
 
@@ -148,17 +145,17 @@
     add_pyublas(toolchain)
     add_boost_numeric_bindings(toolchain)
     add_py_module(toolchain, "hedge")
 
 
 def add_cuda(toolchain):
     conf = get_aksetup_config()
-    cuda_lib_path = conf.get('CUDADRV_LIB_DIR', [])
-    cuda_library = conf.get('CUDADRV_LIBNAME', ['cuda'])
-    cuda_include_path = conf.get('CUDA_INC_DIR', [])
+    cuda_lib_path = conf.get("CUDADRV_LIB_DIR", [])
+    cuda_library = conf.get("CUDADRV_LIBNAME", ["cuda"])
+    cuda_include_path = conf.get("CUDA_INC_DIR", [])
 
     if not cuda_include_path or not cuda_lib_path:
         from os.path import dirname, join, normpath
 
         cuda_root = conf.get("CUDA_ROOT")
 
         if cuda_root is None:
@@ -171,17 +168,17 @@
             cuda_root = normpath(join(dirname(nvcc_path), ".."))
 
         if not cuda_include_path:
             cuda_include_path = [join(cuda_root, "include")]
         if not cuda_lib_path:
             cuda_lib_path = [join(cuda_root, "lib"), join(cuda_root, "lib64")]
 
-    cuda_rt_path = conf.get('CUDART_LIB_DIR', cuda_lib_path)
-    cuda_rt_library = conf.get('CUDART_LIBNAME', ['cudart'])
+    cuda_rt_path = conf.get("CUDART_LIB_DIR", cuda_lib_path)
+    cuda_rt_library = conf.get("CUDART_LIBNAME", ["cudart"])
 
-    toolchain.add_library('cuda', cuda_include_path,
+    toolchain.add_library("cuda", cuda_include_path,
                           cuda_lib_path + cuda_rt_path,
                           cuda_library + cuda_rt_library)
 
 # }}}
 
 # vim:foldmethod=marker
```

### Comparing `codepy-2019.1/codepy/toolchain.py` & `codepy-2023.1/codepy/toolchain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Toolchains for Just-in-time Python extension compilation."""
 
-from __future__ import division, print_function
 
 __copyright__ = """
 "Copyright (C) 2008,9 Andreas Kloeckner, Bryan Catanzaro
 """
 
 __license__ = """
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,16 +30,16 @@
 from pytools import Record
 
 
 class Toolchain(Record):
     """Abstract base class for tools used to link dynamic Python modules."""
 
     def __init__(self, *args, **kwargs):
-        if 'features' not in kwargs:
-            kwargs['features'] = set()
+        if "features" not in kwargs:
+            kwargs["features"] = set()
         Record.__init__(self, *args, **kwargs)
 
     def get_version(self):
         """Return a string describing the exact version of the tools (compilers etc.)
         involved in this toolchain.
 
         Implemented by subclasses.
@@ -87,15 +86,15 @@
         Implemented by subclasses.
         """
 
         raise NotImplementedError
 
     def build_extension(self, ext_file, source_files, debug=False):
         """Create the extension file *ext_file* from *source_files*
-        by invoking the toolchain. Raise :exc:`CompileError` in
+        by invoking the toolchain. Raise :exc:`~codepy.jit.CompileError` in
         case of error.
 
         If *debug* is True, print the commands executed.
 
         Implemented by subclasses.
         """
 
@@ -129,50 +128,52 @@
         """Return a new Toolchain object with the optimization level
         set to `level` , on the scale defined by the gcc -O option.
         Levels greater than four may be defined to perform certain, expensive
         optimizations. Further, extra keyword arguments may be defined.
         If a subclass doesn't understand an "extra" argument, it should
         simply ignore it.
 
-        Level may also be "debug" to specifiy a debug build.
+        Level may also be "debug" to specify a debug build.
 
         Implemented by subclasses.
         """
 
         raise NotImplementedError
 
 
 # {{{ gcc-like tool chain
 
 class GCCLikeToolchain(Toolchain):
     def get_version(self):
         result, stdout, stderr = call_capture_output([self.cc, "--version"])
         if result != 0:
-            raise RuntimeError("version query failed: "+stderr)
+            raise RuntimeError(f"version query failed: {stderr}")
         return stdout
 
     def enable_debugging(self):
         self.cflags = [f for f in self.cflags if not f.startswith("-O")] + ["-g"]
 
     def get_dependencies(self, source_files):
         from codepy.tools import join_continued_lines
         result, stdout, stderr = call_capture_output(
                 [self.cc]
                 + ["-M"]
-                + ["-D%s" % define for define in self.defines]
-                + ["-U%s" % undefine for undefine in self.undefines]
-                + ["-I%s" % idir for idir in self.include_dirs]
+                + [f"-D{define}" for define in self.defines]
+                + [f"-U{undefine}" for undefine in self.undefines]
+                + [f"-I{idir}" for idir in self.include_dirs]
                 + self.cflags
                 + source_files
                 )
 
         if result != 0:
-            raise CompileError("getting dependencies failed: "+stderr)
+            raise CompileError(f"getting dependencies failed: {stderr}")
 
         lines = join_continued_lines(stdout.split("\n"))
+        lines = [line for line in lines
+                 if not (line.strip() and line.strip()[0] == "#")]
         from pytools import flatten
         return set(flatten(
             line.split()[2:] for line in lines))
 
     def build_object(self, ext_file, source_files, debug=False):
         cc_cmdline = (
                 self._cmdline(source_files, True)
@@ -183,16 +184,16 @@
         if debug:
             print(" ".join(cc_cmdline))
 
         result = call(cc_cmdline)
 
         if result != 0:
             import sys
-            print("FAILED compiler invocation:" +
-                  " ".join(cc_cmdline), file=sys.stderr)
+            print("FAILED compiler invocation: {}".format(" ".join(cc_cmdline)),
+                  file=sys.stderr)
             raise CompileError("module compilation failed")
 
     def build_extension(self, ext_file, source_files, debug=False):
         cc_cmdline = (
                 self._cmdline(source_files, False)
                 + ["-o", ext_file]
                 )
@@ -201,15 +202,15 @@
         if debug:
             print(" ".join(cc_cmdline))
 
         result = call(cc_cmdline)
 
         if result != 0:
             import sys
-            print("FAILED compiler invocation:" + " ".join(cc_cmdline),
+            print("FAILED compiler invocation: {}".format(" ".join(cc_cmdline)),
                   file=sys.stderr)
             raise CompileError("module compilation failed")
 
     def link_extension(self, ext_file, object_files, debug=False):
         cc_cmdline = (
                 self._cmdline(object_files, False)
                 + ["-o", ext_file]
@@ -219,15 +220,15 @@
         if debug:
             print(" ".join(cc_cmdline))
 
         result = call(cc_cmdline)
 
         if result != 0:
             import sys
-            print("FAILED compiler invocation:" + " ".join(cc_cmdline),
+            print("FAILED compiler invocation: {}".format(" ".join(cc_cmdline)),
                   file=sys.stderr)
             raise CompileError("module compilation failed")
 
 # }}}
 
 
 # {{{ gcc toolchain
@@ -247,46 +248,46 @@
                 # not an integer? too bad.
                 break
 
         return tuple(result)
 
     def _cmdline(self, files, object=False):
         if object:
-            ld_options = ['-c']
+            ld_options = ["-c"]
             link = []
         else:
             ld_options = self.ldflags
-            link = ["-L%s" % ldir for ldir in self.library_dirs]
-            link.extend(["-l%s" % lib for lib in self.libraries])
+            link = [f"-L{ldir}" for ldir in self.library_dirs]
+            link.extend([f"-l{lib}" for lib in self.libraries])
         return (
             [self.cc]
             + self.cflags
             + ld_options
-            + ["-D%s" % define for define in self.defines]
-            + ["-U%s" % undefine for undefine in self.undefines]
-            + ["-I%s" % idir for idir in self.include_dirs]
+            + [f"-D{define}" for define in self.defines]
+            + [f"-U{undefine}" for undefine in self.undefines]
+            + [f"-I{idir}" for idir in self.include_dirs]
             + files
             + link
             )
 
     def abi_id(self):
         return Toolchain.abi_id(self) + [self._cmdline([])]
 
     def with_optimization_level(self, level, debug=False, **extra):
-        def remove_prefix(l, prefix):
-            return [f for f in l if not f.startswith(prefix)]
+        def remove_prefix(flags, prefix):
+            return [f for f in flags if not f.startswith(prefix)]
 
         cflags = self.cflags
         for pfx in ["-O", "-g", "-march", "-mtune", "-DNDEBUG"]:
             cflags = remove_prefix(cflags, pfx)
 
         if level == "debug":
             oflags = ["-g"]
         else:
-            oflags = ["-O%d" % level, "-DNDEBUG"]
+            oflags = [f"-O{level}", "-DNDEBUG"]
 
             if level >= 2 and self.get_version_tuple() >= (4, 3):
                 oflags.extend(["-march=native", "-mtune=native", ])
 
         return self.copy(cflags=cflags + oflags)
 
 # }}}
@@ -295,41 +296,41 @@
 # {{{ nvcc
 
 class NVCCToolchain(GCCLikeToolchain):
     def get_version_tuple(self):
         ver = self.get_version()
         lines = ver.split("\n")
         words = lines[3].split()
-        numbers = words[4].split('.') + words[5].split('.')
+        numbers = words[4].split(".") + words[5].split(".")
 
         result = []
         for n in numbers:
             try:
                 result.append(int(n))
             except ValueError:
                 # not an integer? too bad.
                 break
 
         return tuple(result)
 
     def _cmdline(self, files, object=False):
         if object:
-            ldflags = ['-c']
+            ldflags = ["-c"]
             load = []
         else:
             ldflags = self.ldflags
-            load = ["-L%s" % ldir for ldir in self.library_dirs]
-            load.extend(["-l%s" % lib for lib in self.libraries])
+            load = [f"-L{ldir}" for ldir in self.library_dirs]
+            load.extend([f"-l{lib}" for lib in self.libraries])
         return (
                 [self.cc]
                 + self.cflags
                 + ldflags
-                + ["-D%s" % define for define in self.defines]
-                + ["-U%s" % undefine for undefine in self.undefines]
-                + ["-I%s" % idir for idir in self.include_dirs]
+                + [f"-D{define}" for define in self.defines]
+                + [f"-U{undefine}" for undefine in self.undefines]
+                + [f"-I{idir}" for idir in self.include_dirs]
                 + files
                 + load
                 )
 
     def abi_id(self):
         return Toolchain.abi_id(self) + [self._cmdline([])]
 
@@ -349,45 +350,38 @@
         if "error" in stderr:
             # work around a bug in nvcc, which doesn't provide a non-zero
             # return code even if it failed.
             result = 1
 
         if result != 0:
             import sys
-            print("FAILED compiler invocation:" + " ".join(cc_cmdline),
+            print("FAILED compiler invocation: {}".format(" ".join(cc_cmdline)),
                   file=sys.stderr)
             raise CompileError("module compilation failed")
 
 # }}}
 
 
 # {{{ configuration
 
 class ToolchainGuessError(Exception):
     pass
 
 
 def _guess_toolchain_kwargs_from_python_config():
-    def strip_prefix(pfx, value):
-        if value.startswith(pfx):
-            return value[len(pfx):]
-        else:
-            return value
-
-    from distutils.sysconfig import parse_makefile, get_makefile_filename
-    make_vars = parse_makefile(get_makefile_filename())
-
-    cc_cmdline = (make_vars["CXX"].split()
-            + make_vars["CFLAGS"].split()
-            + make_vars["CFLAGSFORSHARED"].split())
-    object_names = [
-            oname for oname in make_vars['OBJECT_OBJS'].split()
-            if "(" not in oname and ")" not in oname]
-
-    object_suffix = '.' + object_names[0].split('.')[1]
+    import os
+    import sysconfig
+    config_vars = sysconfig.get_config_vars()
+
+    cc_cmdline = (
+            config_vars["CXX"].split()
+            + config_vars["CFLAGS"].split()
+            + config_vars["CFLAGSFORSHARED"].split()
+            )
+    object_suffix = os.path.splitext(config_vars["MODOBJS"].split()[0])[-1]
 
     cflags = []
     defines = []
     undefines = []
 
     for cflag in cc_cmdline[1:]:
         if cflag.startswith("-D"):
@@ -395,38 +389,34 @@
         elif cflag.startswith("-U"):
             undefines.append(cflag[2:])
         else:
             cflags.append(cflag)
 
     # on Mac OS X, "libraries" can also be "frameworks"
     libraries = []
-    for lib in make_vars["LIBS"].split():
+    for lib in config_vars["LIBS"].split():
         if lib.startswith("-l"):
-            libraries.append(strip_prefix("-l", lib))
+            libraries.append(lib[2:])
         else:
             cflags.append(lib)
 
-    return dict(
-            cc=cc_cmdline[0],
-            ld=make_vars["LDSHARED"].split()[0],
-            cflags=cflags,
-            ldflags=(
-                make_vars["LDSHARED"].split()[1:]
-                + make_vars["LINKFORSHARED"].split()
-                ),
-            libraries=libraries,
-            include_dirs=[
-                make_vars["INCLUDEPY"]
-                ],
-            library_dirs=[make_vars["LIBDIR"]],
-            so_ext=make_vars["SO"] if 'SO' in make_vars else '.so',
-            o_ext=object_suffix,
-            defines=defines,
-            undefines=undefines,
-            )
+    ld, *ldflags = config_vars["LDSHARED"].split()
+    return {
+            "cc": cc_cmdline[0],
+            "ld": ld,
+            "cflags": cflags,
+            "ldflags": ldflags + config_vars["LINKFORSHARED"].split(),
+            "libraries": libraries,
+            "include_dirs": [config_vars["INCLUDEPY"]],
+            "library_dirs": [config_vars["LIBDIR"]],
+            "so_ext": config_vars.get("EXT_SUFFIX", ".so"),
+            "o_ext": object_suffix,
+            "defines": defines,
+            "undefines": undefines,
+            }
 
 
 def call_capture_output(*args):
     from pytools.prefork import call_capture_output
     import sys
 
     encoding = sys.getdefaultencoding()
@@ -438,61 +428,50 @@
     """Guess and return a :class:`Toolchain` instance.
 
     Raise :exc:`ToolchainGuessError` if no toolchain could be found.
     """
     kwargs = _guess_toolchain_kwargs_from_python_config()
     result, version, stderr = call_capture_output([kwargs["cc"], "--version"])
     if result != 0:
-        raise ToolchainGuessError("compiler version query failed: "+stderr)
+        raise ToolchainGuessError(f"compiler version query failed: {stderr}")
 
     if "Free Software Foundation" in version:
         if "-Wstrict-prototypes" in kwargs["cflags"]:
             kwargs["cflags"].remove("-Wstrict-prototypes")
         if "darwin" in version:
             # Are we running in 32-bit mode?
             # The python interpreter may have been compiled as a Fat binary
             # So we need to check explicitly how we're running
             # And update the cflags accordingly
             import sys
             if sys.maxsize == 0x7fffffff:
-                kwargs["cflags"].extend(['-arch', 'i386'])
-
-        return GCCToolchain(**kwargs)
-    elif "Apple LLVM" in version and "clang" in version:
-        if "-Wstrict-prototypes" in kwargs["cflags"]:
-            kwargs["cflags"].remove("-Wstrict-prototypes")
-        if "darwin" in version:
-            # Are we running in 32-bit mode?
-            # The python interpreter may have been compiled as a Fat binary
-            # So we need to check explicitly how we're running
-            # And update the cflags accordingly
-            import sys
-            if sys.maxsize == 0x7fffffff:
-                kwargs["cflags"].extend(['-arch', 'i386'])
+                kwargs["cflags"].extend(["-arch", "i386"])
 
         return GCCToolchain(**kwargs)
     else:
-        raise ToolchainGuessError("unknown compiler")
+        raise ToolchainGuessError(
+                "Unable to determine compiler. Tried running "
+                f"'{kwargs['cc']} --version' and failed.")
 
 
 def guess_nvcc_toolchain():
     gcc_kwargs = _guess_toolchain_kwargs_from_python_config()
 
-    kwargs = dict(
-            cc="nvcc",
-            ldflags=[],
-            libraries=gcc_kwargs["libraries"],
-            cflags=["-Xcompiler", ",".join(gcc_kwargs["cflags"])],
-            include_dirs=gcc_kwargs["include_dirs"],
-            library_dirs=gcc_kwargs["library_dirs"],
-            so_ext=gcc_kwargs["so_ext"],
-            o_ext=gcc_kwargs["o_ext"],
-            defines=gcc_kwargs["defines"],
-            undefines=gcc_kwargs["undefines"],
-            )
+    kwargs = {
+            "cc": "nvcc",
+            "ldflags": [],
+            "libraries": gcc_kwargs["libraries"],
+            "cflags": ["-Xcompiler", ",".join(gcc_kwargs["cflags"])],
+            "include_dirs": gcc_kwargs["include_dirs"],
+            "library_dirs": gcc_kwargs["library_dirs"],
+            "so_ext": gcc_kwargs["so_ext"],
+            "o_ext": gcc_kwargs["o_ext"],
+            "defines": gcc_kwargs["defines"],
+            "undefines": gcc_kwargs["undefines"],
+            }
     kwargs.setdefault("undefines", []).append("__BLOCKS__")
     kwargs["cc"] = "nvcc"
 
     return NVCCToolchain(**kwargs)
 
 # }}}
```

### Comparing `codepy-2019.1/codepy/tools.py` & `codepy-2023.1/codepy/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Random bits of usefulness."""
 
-from __future__ import division
 
 __copyright__ = "Copyright (C) 2009 Andreas Kloeckner"
 
 
 def join_continued_lines(lines):
     result = []
     it = iter(lines)
```

### Comparing `codepy-2019.1/codepy.egg-info/PKG-INFO` & `codepy-2023.1/codepy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,39 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: codepy
-Version: 2019.1
+Version: 2023.1
 Summary: Generate and execute native code at run time.
 Home-page: http://mathema.tician.de/software/codepy
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
-Description: .. image:: https://badge.fury.io/py/codepy.png
-            :target: http://pypi.python.org/pypi/codepy
-        
-        CodePy is a C/C++ metaprogramming toolkit for Python. It helps you compile
-        source code and dynamically load it into the Python interpreter.
-        This facility also works in conjunction with with `PyCuda
-        <http://mathema.tician.de/software/pycuda>`_.  Dynamic compilation and linking
-        are so far only supported in Linux with the GNU toolchain.
-        
-        See also the `documentation <http://documen.tician.de/codepy>`_ and the
-        `git tree <http://github.com/inducer/codepy>`_.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
+Requires-Python: ~=3.8
+License-File: LICENSE
+
+.. image:: https://gitlab.tiker.net/inducer/codepy/badges/main/pipeline.svg
+    :alt: Gitlab Build Status
+    :target: https://gitlab.tiker.net/inducer/codepy/commits/main
+.. image:: https://github.com/inducer/codepy/workflows/CI/badge.svg
+    :alt: Github Build Status
+    :target: https://github.com/inducer/codepy/actions?query=branch%3Amain+workflow%3ACI
+.. image:: https://badge.fury.io/py/codepy.svg
+    :alt: Python Package Index Release Page
+    :target: https://pypi.org/project/codepy/
+
+CodePy is a C/C++ metaprogramming toolkit for Python. It helps you compile
+source code and dynamically load it into the Python interpreter.
+This facility also works in conjunction with with `PyCuda
+<http://mathema.tician.de/software/pycuda>`_.  Dynamic compilation and linking
+are so far only supported in Linux with the GNU toolchain.
+
+See also the `documentation <http://documen.tician.de/codepy>`_ and the
+`git tree <http://github.com/inducer/codepy>`_.
```

### Comparing `codepy-2019.1/codepy.egg-info/SOURCES.txt` & `codepy-2023.1/codepy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 codepy/__init__.py
 codepy/bpl.py
 codepy/cuda.py
@@ -12,19 +13,15 @@
 codepy/tools.py
 codepy.egg-info/PKG-INFO
 codepy.egg-info/SOURCES.txt
 codepy.egg-info/dependency_links.txt
 codepy.egg-info/not-zip-safe
 codepy.egg-info/requires.txt
 codepy.egg-info/top_level.txt
-codepy/cgen/__init__.py
 codepy/include/codepy/bpl.hpp
 doc/Makefile
-doc/source/conf.py
-doc/source/faq.rst
-doc/source/index.rst
-doc/source/jit.rst
-test/demo.py
-test/demo_plain.py
-test/nvcc-test.py
+doc/conf.py
+examples/demo.py
+examples/demo_plain.py
+examples/nvcc-test.py
 test/test_identical_symbols.py
 test/test_two_stage_compile.py
```

### Comparing `codepy-2019.1/setup.py` & `codepy-2023.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
-from setuptools import setup
+from setuptools import setup, find_namespace_packages
 
-setup(name="codepy",
-      version="2019.1",
-      description="Generate and execute native code at run time.",
-      long_description=open("README.rst", "rt").read(),
-      classifiers=[
-          'Development Status :: 4 - Beta',
-          'Intended Audience :: Developers',
-          'Intended Audience :: Other Audience',
-          'Intended Audience :: Science/Research',
-          'License :: OSI Approved :: MIT License',
-          'Natural Language :: English',
-          'Programming Language :: Python',
-          'Topic :: Scientific/Engineering',
-          'Topic :: Software Development :: Libraries',
-          'Topic :: Utilities',
-          ],
-
-      author=u"Andreas Kloeckner",
-      url="http://mathema.tician.de/software/codepy",
-      author_email="inform@tiker.net",
-      license="MIT",
-
-      packages=["codepy", "codepy.cgen"],
-      install_requires=[
-          "pytools>=2015.1.2",
-          "numpy>=1.6",
-          "appdirs>=1.4.0",
-          "six",
-          "cgen",
-          ],
-
-      include_package_data=True,
-      package_data={
-          "codepy": [
-              "include/codepy/*.hpp",
-              ]
-          },
-
-      zip_safe=False)
+setup(
+    name="codepy",
+    version="2023.1",
+    description="Generate and execute native code at run time.",
+    long_description=open("README.rst").read(),
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Other Audience",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Utilities",
+    ],
+    author="Andreas Kloeckner",
+    url="http://mathema.tician.de/software/codepy",
+    author_email="inform@tiker.net",
+    license="MIT",
+    packages=find_namespace_packages(),
+    python_requires="~=3.8",
+    install_requires=[
+        "pytools>=2015.1.2",
+        "numpy>=1.6",
+        "platformdirs>=2.2.0",
+        "cgen",
+    ],
+    include_package_data=True,
+    package_data={
+        "codepy": [
+            "include/codepy/*.hpp",
+        ]
+    },
+    zip_safe=False,
+)
```

### Comparing `codepy-2019.1/test/nvcc-test.py` & `codepy-2023.1/examples/nvcc-test.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,89 +11,89 @@
 # The host module should include a function which is callable from Python
 host_mod = BoostPythonModule()
 
 # Are we on a 32 or 64 bit platform?
 import sys
 import math
 bitness = math.log(sys.maxsize) + 1
-ptr_sz_uint_conv = 'K' if bitness > 32 else 'I'
+ptr_sz_uint_conv = "K" if bitness > 32 else "I"
 
 # This host function extracts a pointer and shape information from a PyCUDA
 # GPUArray, and then sends them to a CUDA function.  The CUDA function
 # returns a pointer to an array of the same type and shape as the input array.
 # The host function then constructs a GPUArray with the result.
 
 statements = [
     # Extract information from incoming GPUArray
     'PyObject* shape = PyObject_GetAttrString(gpuArray, "shape")',
     'PyObject* type = PyObject_GetAttrString(gpuArray, "dtype")',
     'PyObject* pointer = PyObject_GetAttrString(gpuArray, "gpudata")',
-    'CUdeviceptr cudaPointer = boost::python::extract<CUdeviceptr>(pointer)',
-    'PyObject* length = PySequence_GetItem(shape, 0)',
-    'int intLength = boost::python::extract<int>(length)',
+    "CUdeviceptr cudaPointer = boost::python::extract<CUdeviceptr>(pointer)",
+    "PyObject* length = PySequence_GetItem(shape, 0)",
+    "int intLength = boost::python::extract<int>(length)",
     # Call CUDA function
-    'CUdeviceptr diffResult = diffInstance(cudaPointer, intLength)',
+    "CUdeviceptr diffResult = diffInstance(cudaPointer, intLength)",
     # Build resulting GPUArray
     'PyObject* args = Py_BuildValue("()")',
     'PyObject* newShape = Py_BuildValue("(i)", intLength)',
 
-    'PyObject* kwargs = Py_BuildValue('
+    "PyObject* kwargs = Py_BuildValue("
     '"{sOsOs%s}", "shape", newShape, "dtype", type, "gpudata", diffResult)'
     % ptr_sz_uint_conv,
 
     'PyObject* GPUArrayClass = PyObject_GetAttrString(gpuArray, "__class__")',
-    'PyObject* remoteResult = PyObject_Call(GPUArrayClass, args, kwargs)',
-    'return remoteResult']
+    "PyObject* remoteResult = PyObject_Call(GPUArrayClass, args, kwargs)",
+    "return remoteResult"]
 
 
 host_mod.add_function(
     c.FunctionBody(
         c.FunctionDeclaration(c.Pointer(c.Value("PyObject", "adjacentDifference")),
                             [c.Pointer(c.Value("PyObject", "gpuArray"))]),
         c.Block([c.Statement(x) for x in statements])))
-host_mod.add_to_preamble([c.Include('boost/python/extract.hpp')])
+host_mod.add_to_preamble([c.Include("boost/python/extract.hpp")])
 
 
 cuda_mod = CudaModule(host_mod)
-cuda_mod.add_to_preamble([c.Include('cuda.h')])
+cuda_mod.add_to_preamble([c.Include("cuda.h")])
 
-globalIndex = 'int index = blockIdx.x * blockDim.x + threadIdx.x'
-compute_diff = 'outputPtr[index] = inputPtr[index] - inputPtr[index-1]'
-launch = ['CUdeviceptr output',
-          'cuMemAlloc(&output, sizeof(T) * length)',
-          'int bSize = 256',
-          'int gSize = (length-1)/bSize + 1',
-          'diffKernel<<<gSize, bSize>>>((T*)inputPtr, length, (T*)output)',
-          'return output']
+global_index = "int index = blockIdx.x * blockDim.x + threadIdx.x"
+compute_diff = "outputPtr[index] = inputPtr[index] - inputPtr[index-1]"
+launch = ["CUdeviceptr output",
+          "cuMemAlloc(&output, sizeof(T) * length)",
+          "int bSize = 256",
+          "int gSize = (length-1)/bSize + 1",
+          "diffKernel<<<gSize, bSize>>>((T*)inputPtr, length, (T*)output)",
+          "return output"]
 
 diff = [
-    c.Template('typename T',
-             CudaGlobal(c.FunctionDeclaration(c.Value('void', 'diffKernel'),
-                [c.Value('T*', 'inputPtr'),
-                 c.Value('int', 'length'),
-                 c.Value('T*', 'outputPtr')]))),
-    c.Block([c.Statement(globalIndex),
-           c.If('index == 0',
-              c.Statement('outputPtr[0] = inputPtr[0]'),
-              c.If('index < length',
+    c.Template("typename T",
+             CudaGlobal(c.FunctionDeclaration(c.Value("void", "diffKernel"),
+                [c.Value("T*", "inputPtr"),
+                 c.Value("int", "length"),
+                 c.Value("T*", "outputPtr")]))),
+    c.Block([c.Statement(global_index),
+           c.If("index == 0",
+              c.Statement("outputPtr[0] = inputPtr[0]"),
+              c.If("index < length",
                  c.Statement(compute_diff),
-                 c.Statement('')))]),
+                 c.Statement("")))]),
 
-    c.Template('typename T',
-                c.FunctionDeclaration(c.Value('CUdeviceptr', 'difference'),
-                                          [c.Value('CUdeviceptr', 'inputPtr'),
-                                           c.Value('int', 'length')])),
+    c.Template("typename T",
+                c.FunctionDeclaration(c.Value("CUdeviceptr", "difference"),
+                                          [c.Value("CUdeviceptr", "inputPtr"),
+                                           c.Value("int", "length")])),
     c.Block([c.Statement(x) for x in launch])]
 
 cuda_mod.add_to_module(diff)
 diff_instance = c.FunctionBody(
-    c.FunctionDeclaration(c.Value('CUdeviceptr', 'diffInstance'),
-                        [c.Value('CUdeviceptr', 'inputPtr'),
-                         c.Value('int', 'length')]),
-    c.Block([c.Statement('return difference<int>(inputPtr, length)')]))
+    c.FunctionDeclaration(c.Value("CUdeviceptr", "diffInstance"),
+                        [c.Value("CUdeviceptr", "inputPtr"),
+                         c.Value("int", "length")]),
+    c.Block([c.Statement("return difference<int>(inputPtr, length)")]))
 
 # CudaModule.add_function also adds a declaration of this
 # function to the BoostPythonModule which
 # is responsible for the host function.
 cuda_mod.add_function(diff_instance)
 
 import codepy.jit
@@ -106,25 +106,25 @@
 import pycuda.autoinit
 import pycuda.driver
 
 
 import pycuda.gpuarray
 import numpy as np
 length = 25
-constantValue = 2
+constant_value = 2
 # This is a strange way to create a GPUArray, but is meant to illustrate
 # how to construct a GPUArray if the GPU buffer it owns has been
 # created by something else
 
 pointer = pycuda.driver.mem_alloc(length * 4)
-pycuda.driver.memset_d32(pointer, constantValue, length)
+pycuda.driver.memset_d32(pointer, constant_value, length)
 a = pycuda.gpuarray.GPUArray((length,), np.int32, gpudata=pointer)
 b = module.adjacentDifference(a).get()
 
-golden = [constantValue] + [0] * (length - 1)
+golden = [constant_value] + [0] * (length - 1)
 difference = [(x-y)*(x-y) for x, y in zip(b, golden)]
 error = sum(difference)
 if error == 0:
     print("Test passed!")
 else:
     print("Error should be 0, but is: %s" % error)
     print("Test failed")
```

### Comparing `codepy-2019.1/test/test_identical_symbols.py` & `codepy-2023.1/test/test_identical_symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     us = make_greet_mod("Hi there")
     aussie = make_greet_mod("G'day")
 
     assert us.greet() != aussie.greet()
     print(us.greet(), aussie.greet())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test_identical_symbols()
```

### Comparing `codepy-2019.1/test/test_two_stage_compile.py` & `codepy-2023.1/test/test_two_stage_compile.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,22 +11,22 @@
         int const greet()
         {
             return 1;
         }
     }
     """
     # compile to object file
-    _, _, obj_path, _ = compile_from_string(toolchain, 'module', module_code,
+    _, _, obj_path, _ = compile_from_string(toolchain, "module", module_code,
                                             object=True)
     # and then to shared lib
-    with open(obj_path, 'rb') as file:
+    with open(obj_path, "rb") as file:
         obj = file.read()
 
     _, _, ext_file, _ = compile_from_string(
-        toolchain, 'module', obj, source_name=['module.o'],
+        toolchain, "module", obj, source_name=["module.o"],
         object=False, source_is_binary=True)
 
     # test module
     dll = CDLL(ext_file)
-    _fn = getattr(dll, 'greet')
+    _fn = dll.greet
     _fn.restype = int
     assert _fn() == 1
```

