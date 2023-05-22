# Comparing `tmp/metalattice-0.0.26.tar.gz` & `tmp/metalattice-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalattice-0.0.26.tar", last modified: Fri May 19 02:19:18 2023, max compression
+gzip compressed data, was "metalattice-0.0.27.tar", last modified: Sun May 21 17:46:39 2023, max compression
```

## Comparing `metalattice-0.0.26.tar` & `metalattice-0.0.27.tar`

### file list

```diff
@@ -1,31 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.559301 metalattice-0.0.26/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.555300 metalattice-0.0.26/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.559301 metalattice-0.0.26/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-19 02:19:05.000000 metalattice-0.0.26/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-19 02:19:05.000000 metalattice-0.0.26/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-05-19 02:19:05.000000 metalattice-0.0.26/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-19 02:19:05.000000 metalattice-0.0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-19 02:19:18.559301 metalattice-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 02:19:05.000000 metalattice-0.0.26/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-19 02:19:05.000000 metalattice-0.0.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 02:19:18.559301 metalattice-0.0.26/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.555300 metalattice-0.0.26/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.559301 metalattice-0.0.26/src/metalattice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:05.000000 metalattice-0.0.26/src/metalattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-19 02:19:18.000000 metalattice-0.0.26/src/metalattice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.559301 metalattice-0.0.26/src/metalattice/abaqus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:05.000000 metalattice-0.0.26/src/metalattice/abaqus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.559301 metalattice-0.0.26/src/metalattice/abaqus/fortran/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-19 02:19:05.000000 metalattice-0.0.26/src/metalattice/abaqus/fortran/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.559301 metalattice-0.0.26/src/metalattice/abaqus/fortran/code/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 02:19:05.000000 metalattice-0.0.26/src/metalattice/abaqus/fortran/code/test.f
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:05.000000 metalattice-0.0.26/src/metalattice/abaqus/fortran/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.559301 metalattice-0.0.26/src/metalattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-19 02:19:18.000000 metalattice-0.0.26/src/metalattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-19 02:19:18.000000 metalattice-0.0.26/src/metalattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:19:18.000000 metalattice-0.0.26/src/metalattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 02:19:18.000000 metalattice-0.0.26/src/metalattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 02:19:18.000000 metalattice-0.0.26/src/metalattice.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:18.559301 metalattice-0.0.26/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 02:19:05.000000 metalattice-0.0.26/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-19 02:19:05.000000 metalattice-0.0.26/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.294357 metalattice-0.0.27/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.286357 metalattice-0.0.27/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-21 17:46:28.000000 metalattice-0.0.27/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-21 17:46:28.000000 metalattice-0.0.27/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-05-21 17:46:28.000000 metalattice-0.0.27/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-21 17:46:28.000000 metalattice-0.0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-21 17:46:39.294357 metalattice-0.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-21 17:46:28.000000 metalattice-0.0.27/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-21 17:46:28.000000 metalattice-0.0.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:46:39.294357 metalattice-0.0.27/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.286357 metalattice-0.0.27/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/custom_lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/cylin_lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/kshape20h.f
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/kshape8h.f
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/mpc3d.f
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/namelist_element.f
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/namelist_info.f
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/rect_lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/scripts/generate_inp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/lattice/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/material.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.294357 metalattice-0.0.27/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/test_lattice_defination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/test_math_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/test_output_to_abaqus.py
```

### Comparing `metalattice-0.0.26/.github/workflows/python-package.yml` & `metalattice-0.0.27/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.26/.github/workflows/python-publish.yml` & `metalattice-0.0.27/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.26/.gitignore` & `metalattice-0.0.27/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -614,8 +614,9 @@
 *.sln.iml
 
 ### VisualStudio Patch ###
 # Additional files built by Visual Studio
 
 # End of https://www.toptal.com/developers/gitignore/api/python,fortran,visualstudio,visualstudiocode
 src/metalattice/_version.py
-
+*.metalattice.*
+*.inp
```

### Comparing `metalattice-0.0.26/LICENSE` & `metalattice-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.26/PKG-INFO` & `metalattice-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.0.26
+Version: 0.0.27
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (huang-lihao)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `metalattice-0.0.26/pyproject.toml` & `metalattice-0.0.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "cython",
+    "f90nml",
     "gfort2py",
     "numpy",
 ]
 dynamic = ["version"]
 
 # pyproject.toml
 [tool.setuptools_scm]
```

### Comparing `metalattice-0.0.26/src/metalattice/abaqus/fortran/__init__.py` & `metalattice-0.0.27/src/metalattice/abaqus/fortran/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 import gfort2py as gf
 import os
 from pathlib import Path
 
 from metalattice.abaqus.fortran import lib
 
-# compile fortran code and use gfort2py
-cwd = os.getcwd()
+fortran_src = ["lattice.f"]
+
 current = Path(os.path.dirname(__file__))
 code_dir = current.joinpath("code")
 bin_dir = current.joinpath("bin")
 if not bin_dir.exists():
     os.mkdir(bin_dir)
-os.chdir(bin_dir)
-if code_dir.exists():
-    for f in code_dir.iterdir():
-        if f.suffix in [".f", ".for", ".f90"]:
-            os.system(f"gfortran -fPIC -shared -c {f.absolute()}")
-            os.system(f"gfortran -fPIC -shared -o {f.stem}.so {f.absolute()}")
-            libname = str(bin_dir.joinpath(f.with_suffix(".so").name))
-            mod_file = str(bin_dir.joinpath(f.with_suffix(".mod").name))
-            module = gf.fFort(libname=libname, mod_file=mod_file)
-            setattr(lib, str(f.stem), module)
-os.chdir(cwd)
+idx = 0
+bin_dir_tmp = bin_dir.joinpath(f"{idx}")
+
+
+def compile_fortran():  # compile fortran code and use gfort2py
+    cwd = os.getcwd()
+    if not bin_dir_tmp.exists():
+        os.mkdir(bin_dir_tmp)
+    os.chdir(bin_dir_tmp)
+    if code_dir.exists():
+        for f in code_dir.iterdir():
+            if f.name in fortran_src:
+                os.system(
+                    f"gfortran -fPIC -shared -c {f.absolute()}")
+                os.system(
+                    f"gfortran -fPIC -shared -o {f.stem}.so {f.absolute()}")
+        for f in code_dir.iterdir():
+            if f.name in fortran_src:
+                libname = str(bin_dir_tmp.joinpath(f.with_suffix(".so").name))
+                mod_file = str(bin_dir_tmp.joinpath(f.with_suffix(".mod").name))
+                module = gf.fFort(libname=libname, mod_file=mod_file)
+                setattr(lib, str(f.stem), module)
+    os.chdir(cwd)
+
+
+compile_fortran()
```

### Comparing `metalattice-0.0.26/src/metalattice.egg-info/PKG-INFO` & `metalattice-0.0.27/src/metalattice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.0.26
+Version: 0.0.27
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (huang-lihao)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

