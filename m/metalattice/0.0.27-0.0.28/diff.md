# Comparing `tmp/metalattice-0.0.27.tar.gz` & `tmp/metalattice-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalattice-0.0.27.tar", last modified: Sun May 21 17:46:39 2023, max compression
+gzip compressed data, was "metalattice-0.0.28.tar", last modified: Mon May 22 07:53:37 2023, max compression
```

## Comparing `metalattice-0.0.27.tar` & `metalattice-0.0.28.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.294357 metalattice-0.0.27/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.286357 metalattice-0.0.27/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-21 17:46:28.000000 metalattice-0.0.27/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-21 17:46:28.000000 metalattice-0.0.27/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-05-21 17:46:28.000000 metalattice-0.0.27/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-21 17:46:28.000000 metalattice-0.0.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-21 17:46:39.294357 metalattice-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-21 17:46:28.000000 metalattice-0.0.27/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-21 17:46:28.000000 metalattice-0.0.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:46:39.294357 metalattice-0.0.27/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.286357 metalattice-0.0.27/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/fortran/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/custom_lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/cylin_lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/kshape20h.f
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/kshape8h.f
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/mpc3d.f
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/namelist_element.f
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/namelist_info.f
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/code/rect_lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/fortran/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/abaqus/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/scripts/generate_inp.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/abaqus/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice/lattice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/lattice/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-21 17:46:28.000000 metalattice-0.0.27/src/metalattice/material.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.290357 metalattice-0.0.27/src/metalattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 17:46:39.000000 metalattice-0.0.27/src/metalattice.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:39.294357 metalattice-0.0.27/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/test_lattice_defination.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/test_math_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-21 17:46:28.000000 metalattice-0.0.27/tests/test_output_to_abaqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-22 07:53:23.000000 metalattice-0.0.28/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 07:53:23.000000 metalattice-0.0.28/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-05-22 07:53:23.000000 metalattice-0.0.28/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-22 07:53:23.000000 metalattice-0.0.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-22 07:53:37.016553 metalattice-0.0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 07:53:23.000000 metalattice-0.0.28/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-22 07:53:23.000000 metalattice-0.0.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:53:37.016553 metalattice-0.0.28/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/src/metalattice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/src/metalattice/abaqus/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/src/metalattice/abaqus/fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/custom_lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/cylin_lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/kshape20h.f
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/kshape8h.f
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/mpc3d.f
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/namelist_element.f
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/namelist_info.f
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/rect_lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/src/metalattice/abaqus/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/scripts/generate_beam_inp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/src/metalattice/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/lattice/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/material.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/src/metalattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-22 07:53:37.000000 metalattice-0.0.28/src/metalattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:23.000000 metalattice-0.0.28/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-22 07:53:23.000000 metalattice-0.0.28/tests/test_lattice_defination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-22 07:53:23.000000 metalattice-0.0.28/tests/test_math_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-22 07:53:23.000000 metalattice-0.0.28/tests/test_output_to_abaqus.py
```

### Comparing `metalattice-0.0.27/.github/workflows/python-package.yml` & `metalattice-0.0.28/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/.github/workflows/python-publish.yml` & `metalattice-0.0.28/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/.gitignore` & `metalattice-0.0.28/.gitignore`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/LICENSE` & `metalattice-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/PKG-INFO` & `metalattice-0.0.28/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.0.27
+Version: 0.0.28
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
+Maintainer-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (huang-lihao)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -24,13 +25,14 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: lattice metamaterial,micropolar,cosserat,abaqus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Fortran
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MetaLattice
 A Python package to model lattice metamaterials, using Abaqus.
```

### Comparing `metalattice-0.0.27/pyproject.toml` & `metalattice-0.0.28/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,28 +3,34 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metalattice"
 authors = [
     {name = "Huang Lihao", email = "huang-lihao@outlook.com"},
 ]
+maintainers = [
+    {name = "Huang Lihao", email = "huang-lihao@outlook.com"},
+]
 description = "A Python package to model lattice metamaterials, using Abaqus."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["lattice metamaterial", "micropolar", "cosserat", "abaqus"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Fortran",
 ]
 dependencies = [
     "cython",
     "f90nml",
     "gfort2py",
+    "meshio",
     "numpy",
+    "sympy",
 ]
 dynamic = ["version"]
 
 # pyproject.toml
 [tool.setuptools_scm]
 write_to = "src/metalattice/_version.py"
 local_scheme = "no-local-version"
```

### Comparing `metalattice-0.0.27/src/metalattice/abaqus/fortran/__init__.py` & `metalattice-0.0.28/src/metalattice/abaqus/fortran/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 current = Path(os.path.dirname(__file__))
 code_dir = current.joinpath("code")
 bin_dir = current.joinpath("bin")
 if not bin_dir.exists():
     os.mkdir(bin_dir)
 idx = 0
-bin_dir_tmp = bin_dir.joinpath(f"{idx}")
 
 
 def compile_fortran():  # compile fortran code and use gfort2py
     cwd = os.getcwd()
+    global idx
+    bin_dir_tmp = bin_dir.joinpath(f"{idx}")
+    idx += 1
     if not bin_dir_tmp.exists():
         os.mkdir(bin_dir_tmp)
     os.chdir(bin_dir_tmp)
     if code_dir.exists():
         for f in code_dir.iterdir():
             if f.name in fortran_src:
                 os.system(
```

### Comparing `metalattice-0.0.27/src/metalattice/abaqus/fortran/code/custom_lattice.f` & `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/custom_lattice.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/src/metalattice/abaqus/fortran/code/cylin_lattice.f` & `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/cylin_lattice.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/src/metalattice/abaqus/fortran/code/kshape20h.f` & `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/kshape20h.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/src/metalattice/abaqus/fortran/code/kshape8h.f` & `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/kshape8h.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/src/metalattice/abaqus/fortran/code/lattice.f` & `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/lattice.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/src/metalattice/abaqus/fortran/code/mpc3d.f` & `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/mpc3d.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/src/metalattice/abaqus/fortran/code/rect_lattice.f` & `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/rect_lattice.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/src/metalattice/lattice/lattice.py` & `metalattice-0.0.28/src/metalattice/lattice/lattice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from f90nml.namelist import Namelist
 import meshio
 from meshio.abaqus._abaqus import meshio_to_abaqus_type, abaqus_to_meshio_type
 import numpy as np
+from numpy.typing import ArrayLike
 from shutil import copyfile
 
 from metalattice.material import Material
 from metalattice.abaqus import fortran
 from metalattice.abaqus.fortran import compile_fortran
 from metalattice.abaqus.fortran import lib
 from metalattice.abaqus.scripts import run_abaqus_script
@@ -29,16 +30,14 @@
 
         self.custom_lattice_f = custom_lattice_f
         target = "custom_lattice.f"
         src = fortran.code_dir.joinpath(custom_lattice_f)
         dst = fortran.code_dir.joinpath(target)
         assert src.is_file()
         copyfile(src=src, dst=dst)
-        fortran.idx += 1
-        fortran.bin_dir_tmp = fortran.bin_dir.joinpath(f"{fortran.idx}")
         compile_fortran()
 
         self.nodes: dict[tuple(int), np.ndarray] = None
         self.beams: dict[tuple(int), lib.lattice.Beam] = None
         self.continuum_mesh: dict = None
         self.base_indices: list[list[int]] = None
         self.iel2ijk: np.ndarray = None
@@ -297,24 +296,26 @@
     def write_beam_job(
         self,
         job_name: str,
     ) -> None:
         self.generate_nodes()
         self.generate_beams()
 
+        node_ns = self.node_ns
+
         inp_file_name = job_name + ".inp"
         points = list(self.nodes.values())
 
         conn = []
         ijk_list = list(self.nodes.keys())
         for beam in self.beams.values():
             conn.append(
                 [
                     ijk_list.index(tuple([
-                        (ijk[d] - 1) % self.node_ns[d]
+                        (ijk[d] - 1) % node_ns[d]
                         for d in range(3)
                     ]))
                     for ijk in beam["indices"].T
                 ]
             )
 
         element_type = beam["element"]
@@ -326,17 +327,43 @@
             meshio_to_abaqus_type[meshio_type] = "B33"
         else:
             raise Exception(
                 f"Beam element type {element_type} is not supported!")
         cells = [
             (meshio_type, conn),
         ]
-        meshio.write_points_cells(inp_file_name, points, cells)
 
-        run_abaqus_script("generate_inp")
+        point_sets: dict[str, ArrayLike] = {}
+        sign = {0: "-", 1: "+"}
+        for d in range(3):
+            if not self.periodic[d]:
+                for pn in range(2):
+                    indices = [
+                        [i for i in range(0, node_ns[j])]
+                        for j in range(3)
+                    ]
+                    indices[d] = [pn * node_ns[d]]
+                    point_sets[f"SURFACE-{d}{sign[pn]}"] = [
+                        ijk_list.index(tuple(i, j, k))
+                        for i in range(0, node_ns[0])
+                        for j in range(0, node_ns[1])
+                        for k in range(0, node_ns[2])
+                    ]
+
+        meshio.write_points_cells(
+            filename=inp_file_name,
+            points=points,
+            cells=cells,
+            point_sets=point_sets,
+        )
+
+        run_abaqus_script(
+            script_file="generate_beam_inp",
+            option=f"main_{job_name} main_{job_name} {inp_file_name} {self.material.E} {self.material.nu} {self.material.rho}"
+        )
 
     def write_micropolar_job(
         self,
         job_name: str,
         element_type: str = "MPC3D8",
         regenerate: bool = False,
     ):
```

### Comparing `metalattice-0.0.27/src/metalattice.egg-info/PKG-INFO` & `metalattice-0.0.28/src/metalattice.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.0.27
+Version: 0.0.28
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
+Maintainer-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (huang-lihao)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -24,13 +25,14 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: lattice metamaterial,micropolar,cosserat,abaqus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Fortran
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MetaLattice
 A Python package to model lattice metamaterials, using Abaqus.
```

### Comparing `metalattice-0.0.27/src/metalattice.egg-info/SOURCES.txt` & `metalattice-0.0.28/src/metalattice.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 src/metalattice/abaqus/fortran/code/kshape8h.f
 src/metalattice/abaqus/fortran/code/lattice.f
 src/metalattice/abaqus/fortran/code/mpc3d.f
 src/metalattice/abaqus/fortran/code/namelist_element.f
 src/metalattice/abaqus/fortran/code/namelist_info.f
 src/metalattice/abaqus/fortran/code/rect_lattice.f
 src/metalattice/abaqus/scripts/__init__.py
-src/metalattice/abaqus/scripts/generate_inp.py
+src/metalattice/abaqus/scripts/generate_beam_inp.py
 src/metalattice/lattice/__init__.py
 src/metalattice/lattice/lattice.py
 tests/__init__.py
 tests/test_lattice_defination.py
 tests/test_math_constants.py
 tests/test_output_to_abaqus.py
```

### Comparing `metalattice-0.0.27/tests/test_lattice_defination.py` & `metalattice-0.0.28/tests/test_lattice_defination.py`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/tests/test_math_constants.py` & `metalattice-0.0.28/tests/test_math_constants.py`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.27/tests/test_output_to_abaqus.py` & `metalattice-0.0.28/tests/test_output_to_abaqus.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
         la = Lattice(
             ns=[7, 7, 7],
             strides=[2, 2, 2],
             custom_lattice_f="rect_lattice.f"
         )
         la.write_beam_job(
-            job_name="test_beam"
+            job_name="test_rect_beam"
         )
         la.write_micropolar_job(
             job_name="test_rect__micropolar_mpc3d8",
             element_type="MPC3D8",
             regenerate=True,
         )
         la.write_micropolar_job(
@@ -35,15 +35,15 @@
         la = Lattice(
             ns=[8, 48, 4],
             strides=[2, 2, 2],
             periodic=[False, True, False],
             custom_lattice_f="cylin_lattice.f"
         )
         la.write_beam_job(
-            job_name="test_beam"
+            job_name="test_cylin_beam"
         )
         la.write_micropolar_job(
             job_name="test_cylin_micropolar_mpc3d8",
             element_type="MPC3D8",
             regenerate=True,
         )
         la.write_micropolar_job(
```

