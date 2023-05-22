# Comparing `tmp/pycufsm-0.1.0.tar.gz` & `tmp/pycufsm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycufsm-0.1.0.tar", last modified: Sat May  6 07:37:28 2023, max compression
+gzip compressed data, was "pycufsm-0.1.1.tar", last modified: Mon May 22 01:02:25 2023, max compression
```

## Comparing `pycufsm-0.1.0.tar` & `pycufsm-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:37:28.909180 pycufsm-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-05-06 07:35:08.000000 pycufsm-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-06 07:37:28.909180 pycufsm-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-06 07:35:08.000000 pycufsm-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-06 07:35:08.000000 pycufsm-0.1.0/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 07:35:08.000000 pycufsm-0.1.0/jupyter_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 07:35:08.000000 pycufsm-0.1.0/plot_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:37:28.909180 pycufsm-0.1.0/pycufsm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pycufsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pycufsm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    42540 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pycufsm/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)   108649 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pycufsm/cfsm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pycufsm/cutwp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pycufsm/fsm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pycufsm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pycufsm/plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pycufsm/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:37:28.909180 pycufsm-0.1.0/pycufsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-06 07:37:28.000000 pycufsm-0.1.0/pycufsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-06 07:37:28.000000 pycufsm-0.1.0/pycufsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 07:37:28.000000 pycufsm-0.1.0/pycufsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-06 07:37:28.000000 pycufsm-0.1.0/pycufsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 07:37:28.000000 pycufsm-0.1.0/pycufsm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-06 07:35:08.000000 pycufsm-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 07:35:08.000000 pycufsm-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 07:37:28.909180 pycufsm-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-06 07:35:08.000000 pycufsm-0.1.0/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:37:28.909180 pycufsm-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-06 07:35:08.000000 pycufsm-0.1.0/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:02:25.245726 pycufsm-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-05-22 00:58:26.000000 pycufsm-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-22 01:02:25.245726 pycufsm-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-22 00:58:26.000000 pycufsm-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 00:58:26.000000 pycufsm-0.1.1/_custom_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-22 00:58:26.000000 pycufsm-0.1.1/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 00:58:26.000000 pycufsm-0.1.1/jupyter_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 00:58:26.000000 pycufsm-0.1.1/plot_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:02:25.241726 pycufsm-0.1.1/pycufsm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1496999 2023-05-22 01:02:24.000000 pycufsm-0.1.1/pycufsm/analysis_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40997 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/analysis_p.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107945 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/cfsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/cutwp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/fsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pycufsm/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:02:25.241726 pycufsm-0.1.1/pycufsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-22 01:02:25.000000 pycufsm-0.1.1/pycufsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-22 01:02:25.000000 pycufsm-0.1.1/pycufsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 01:02:25.000000 pycufsm-0.1.1/pycufsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-22 01:02:25.000000 pycufsm-0.1.1/pycufsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 01:02:25.000000 pycufsm-0.1.1/pycufsm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-22 00:58:26.000000 pycufsm-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 00:58:26.000000 pycufsm-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 01:02:25.245726 pycufsm-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 00:58:26.000000 pycufsm-0.1.1/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:02:25.241726 pycufsm-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-22 00:58:26.000000 pycufsm-0.1.1/tests/test_e2e.py
```

### Comparing `pycufsm-0.1.0/LICENSE` & `pycufsm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycufsm-0.1.0/PKG-INFO` & `pycufsm-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycufsm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python CUFSM (Constrained and Unconstrained Finite Strip Method)
 Author-email: Brooks Smith <smith120bh@gmail.com>
 License: AFL-3.0
 Project-URL: Homepage, https://github.com/ClearCalcs/pyCUFSM
 Project-URL: Documentation, https://github.com/ClearCalcs/pyCUFSM/wiki
 Keywords: CUFSM,CFS,thin-walled,cold-formed steel,aluminium,structural engineering,structural analysis
 Classifier: Topic :: Scientific/Engineering
@@ -23,37 +23,40 @@
 Provides-Extra: jupyter
 License-File: LICENSE
 
 # pyCUFSM
 
 ## Description
 
-This is a port of the analysis portions of CUFSM v5.01, written by Benjamin Schafer PhD et al at Johns Hopkins University, from its original MATLAB language to Python v3, using the Numpy and Scipy packages for matrix manipulation and other advanced mathematics functionality. The goal of this project is to create a derivative of CUFSM which can be used in cloud-based applications. This project is not affiliated with Benjamin Schafer PhD or Johns Hopkins University in any way.
+This package is primarily a port of CUFSM v5.01, written by Benjamin Schafer PhD et al at Johns Hopkins University, from its original MATLAB language to Python v3, using the Numpy and Scipy packages for matrix manipulation and other advanced mathematics functionality. The goal of this project is to create a derivative of CUFSM which can be used either in Jupyter Notebooks or in headless (library) applications. This project is not affiliated with Benjamin Schafer PhD or Johns Hopkins University in any way.
 
-The original MATLAB CUFSM program may be accessed at the following address: https://www.ce.jhu.edu/bschafer/cufsm/
+The original MATLAB CUFSM program may be accessed at the following address: https://www.ce.jhu.edu/cufsm/
 
 ### Installation
 
-This package is still under check and development in its alpha state, therefore it has not yet been published to the Python's PyPI repository. Users may install clone and install the package on their systems using relevant codes the same as printed bellow:
+This package is still under heavy development, but it may be installed in several different possible forms, as described below:
+1. Minimal (headless) installation: `pip install pycufsm`
+2. Installation with plotting capabilities: `pip install pycufsm[plot]`
+3. Installation with Jupyter Notebooks: `pip install pycufsm[jupyter]`
+4. Installation with full development dependencies: `pip install pycufsm[dev]`
 
-`python -m pip install git+https://github.com/ClearCalcs/pyCUFSM.git`
+### Contributing
 
-### Limitations
-
--   **No GUI** - While the MATLAB version of CUFSM contains a full graphical user interface, I will be making no effort in this project to create anything more than a basic command-line interface (though other contributions will be welcome). I anticipate that users of this package will have their own user interface and that this package will function as something of a plug-in.
--   **No CUTWP** - The MATLAB version of CUFSM makes use of CUTWP code for calculating section properties (A, I, J, etc). There are already several mature, open-source Python section properties calculators available, and CUTWP is inherently less accurate because it is based upon section centerline calculations only. As such, I have no plans to port the CUTWP code and anticipate that users of this package will make use of other section properties calculators instead.
+If you would like to contribute to the pyCUFSM project, then please do - all productive contributions are welcome! However, please make sure that you're working off of the most recent development version of the pyCUFSM code, by cloning the [GitHub repository](https://github.com/ClearCalcs/pyCUFSM), and please review our wiki article on [Contributing to the Code](https://github.com/ClearCalcs/pyCUFSM/wiki/Contributing-to-the-Code).
 
 ## Current Status
 
 #### Complete and Generally Tested
 
 -   [x] Unconstrained FSM (signature curve generation)
 -   [x] Constrained FSM
 -   [x] Added template_path() function to define a complete arbitrary cross-section by simple paths
 -   [x] Add automated validation testing of FSM calculations via pytest
+-   [x] Various efficiency and readability improvements:
+    -   [x] Cythonise a few computation-heavy functions in analysis.py, including klocal(), kglocal(), and assemble()
 
 #### Complete But Untested
 
 -   [x] Equation constraints
 -   [x] Spring constraints
 -   [x] General boundary conditions
 
@@ -66,10 +69,10 @@
     -   [ ] Eliminate matrix columns which are nothing more than the index number of the row
     -   [ ] Review code for places where matrices can be preallocated rather than concatenated together
     -   [ ] Review code for function calls that are unnecessarily repeated (a couple of these have already been addressed, e.g. `base_properties()` did not need to be re-run for every half wavelength)
 -   [ ] Write API-style documentation (for now, generally refer to MATLAB CUFSM documentation and/or comments)
 
 ## Disclaimer
 
-While the original MATLAB CUFSM has been extensively tested, and best efforts have been made to check accuracy of this package against the original MATLAB CUFSM program, no warrant is made as to the accuracy of this package. The developers accept no liability for any errors or inaccuracies in this package, including, but not limited to, any problems which may stem from such errors or inaccuracies in this package such as under-conservative engineering designs or structural failures.
+While the original MATLAB CUFSM has been extensively tested, and best efforts have been made to check accuracy of this package against the original MATLAB CUFSM program, including via automated validation testing, no warrant is made as to the accuracy of this package. The developers accept no liability for any errors or inaccuracies in this package, including, but not limited to, any problems which may stem from such errors or inaccuracies in this package such as under-conservative engineering designs or structural failures.
 
 Always check your designs and never blindly trust any engineering program, including this one.
```

### Comparing `pycufsm-0.1.0/README.md` & `pycufsm-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # pyCUFSM
 
 ## Description
 
-This is a port of the analysis portions of CUFSM v5.01, written by Benjamin Schafer PhD et al at Johns Hopkins University, from its original MATLAB language to Python v3, using the Numpy and Scipy packages for matrix manipulation and other advanced mathematics functionality. The goal of this project is to create a derivative of CUFSM which can be used in cloud-based applications. This project is not affiliated with Benjamin Schafer PhD or Johns Hopkins University in any way.
+This package is primarily a port of CUFSM v5.01, written by Benjamin Schafer PhD et al at Johns Hopkins University, from its original MATLAB language to Python v3, using the Numpy and Scipy packages for matrix manipulation and other advanced mathematics functionality. The goal of this project is to create a derivative of CUFSM which can be used either in Jupyter Notebooks or in headless (library) applications. This project is not affiliated with Benjamin Schafer PhD or Johns Hopkins University in any way.
 
-The original MATLAB CUFSM program may be accessed at the following address: https://www.ce.jhu.edu/bschafer/cufsm/
+The original MATLAB CUFSM program may be accessed at the following address: https://www.ce.jhu.edu/cufsm/
 
 ### Installation
 
-This package is still under check and development in its alpha state, therefore it has not yet been published to the Python's PyPI repository. Users may install clone and install the package on their systems using relevant codes the same as printed bellow:
+This package is still under heavy development, but it may be installed in several different possible forms, as described below:
+1. Minimal (headless) installation: `pip install pycufsm`
+2. Installation with plotting capabilities: `pip install pycufsm[plot]`
+3. Installation with Jupyter Notebooks: `pip install pycufsm[jupyter]`
+4. Installation with full development dependencies: `pip install pycufsm[dev]`
 
-`python -m pip install git+https://github.com/ClearCalcs/pyCUFSM.git`
+### Contributing
 
-### Limitations
-
--   **No GUI** - While the MATLAB version of CUFSM contains a full graphical user interface, I will be making no effort in this project to create anything more than a basic command-line interface (though other contributions will be welcome). I anticipate that users of this package will have their own user interface and that this package will function as something of a plug-in.
--   **No CUTWP** - The MATLAB version of CUFSM makes use of CUTWP code for calculating section properties (A, I, J, etc). There are already several mature, open-source Python section properties calculators available, and CUTWP is inherently less accurate because it is based upon section centerline calculations only. As such, I have no plans to port the CUTWP code and anticipate that users of this package will make use of other section properties calculators instead.
+If you would like to contribute to the pyCUFSM project, then please do - all productive contributions are welcome! However, please make sure that you're working off of the most recent development version of the pyCUFSM code, by cloning the [GitHub repository](https://github.com/ClearCalcs/pyCUFSM), and please review our wiki article on [Contributing to the Code](https://github.com/ClearCalcs/pyCUFSM/wiki/Contributing-to-the-Code).
 
 ## Current Status
 
 #### Complete and Generally Tested
 
 -   [x] Unconstrained FSM (signature curve generation)
 -   [x] Constrained FSM
 -   [x] Added template_path() function to define a complete arbitrary cross-section by simple paths
 -   [x] Add automated validation testing of FSM calculations via pytest
+-   [x] Various efficiency and readability improvements:
+    -   [x] Cythonise a few computation-heavy functions in analysis.py, including klocal(), kglocal(), and assemble()
 
 #### Complete But Untested
 
 -   [x] Equation constraints
 -   [x] Spring constraints
 -   [x] General boundary conditions
 
@@ -41,10 +44,10 @@
     -   [ ] Eliminate matrix columns which are nothing more than the index number of the row
     -   [ ] Review code for places where matrices can be preallocated rather than concatenated together
     -   [ ] Review code for function calls that are unnecessarily repeated (a couple of these have already been addressed, e.g. `base_properties()` did not need to be re-run for every half wavelength)
 -   [ ] Write API-style documentation (for now, generally refer to MATLAB CUFSM documentation and/or comments)
 
 ## Disclaimer
 
-While the original MATLAB CUFSM has been extensively tested, and best efforts have been made to check accuracy of this package against the original MATLAB CUFSM program, no warrant is made as to the accuracy of this package. The developers accept no liability for any errors or inaccuracies in this package, including, but not limited to, any problems which may stem from such errors or inaccuracies in this package such as under-conservative engineering designs or structural failures.
+While the original MATLAB CUFSM has been extensively tested, and best efforts have been made to check accuracy of this package against the original MATLAB CUFSM program, including via automated validation testing, no warrant is made as to the accuracy of this package. The developers accept no liability for any errors or inaccuracies in this package, including, but not limited to, any problems which may stem from such errors or inaccuracies in this package such as under-conservative engineering designs or structural failures.
 
 Always check your designs and never blindly trust any engineering program, including this one.
```

### Comparing `pycufsm-0.1.0/pycufsm/analysis.py` & `pycufsm-0.1.1/pycufsm/analysis_p.py`

 * *Files 12% similar despite different names*

```diff
@@ -147,27 +147,26 @@
     d_y = stiff_y * thick**3 / (12 * (1 - nu_x*nu_y))
     d_1 = nu_x * stiff_y * thick**3 / (12 * (1 - nu_x*nu_y))
     d_xy = bulk * thick**3 / 12
 
     total_m = len(m_a)  # Total number of longitudinal terms m
 
     k_local = np.zeros((8 * total_m, 8 * total_m))
-    zero_matrix = np.zeros((4, 4))
     for i in range(0, total_m):
         for j in range(0, total_m):
             km_mp = np.zeros((4, 4))
             kf_mp = np.zeros((4, 4))
             u_i = m_a[i] * np.pi
             u_j = m_a[j] * np.pi
             c_1 = u_i / length
             c_2 = u_j / length
 
             [i_1, i_2, i_3, i_4, i_5] = bc_i1_5(b_c, m_a[i], m_a[j], length)
 
-            # assemble the matrix of Km_mp
+            # assemble the matrix of Km_mp (membrane stiffness matrix)
             km_mp[0, 0] = e_1*i_1/b_strip + bulk*b_strip*i_5/3
             km_mp[0, 1] = e_2 * nu_x * (-1 / 2 / c_2) * i_3 - bulk*i_5/2/c_2
             km_mp[0, 2] = -e_1 * i_1 / b_strip + bulk*b_strip*i_5/6
             km_mp[0, 3] = e_2 * nu_x * (-1 / 2 / c_2) * i_3 + bulk*i_5/2/c_2
 
             km_mp[1, 0] = e_2 * nu_x * (-1 / 2 / c_1) * i_2 - bulk*i_5/2/c_1
             km_mp[1, 1] = e_2*b_strip*i_4/3/c_1/c_2 + bulk*i_5/b_strip/c_1/c_2
@@ -181,15 +180,15 @@
 
             km_mp[3, 0] = e_2 * nu_x * (-1 / 2 / c_1) * i_2 + bulk*i_5/2/c_1
             km_mp[3, 1] = e_2*b_strip*i_4/6/c_1/c_2 - bulk*i_5/b_strip/c_1/c_2
             km_mp[3, 2] = e_2 * nu_x * (1/2/c_1) * i_2 + bulk*i_5/2/c_1
             km_mp[3, 3] = e_2*b_strip*i_4/3/c_1/c_2 + bulk*i_5/b_strip/c_1/c_2
             km_mp = km_mp * thick
 
-            # assemble the matrix of Kf_mp
+            # assemble the matrix of Kf_mp (flexural stiffness matrix)
             kf_mp[0, 0] = (5040*d_x*i_1 - 504*b_strip**2*d_1*i_2 - 504*b_strip**2*d_1*i_3 \
                 + 156*b_strip**4*d_y*i_4 + 2016*b_strip**2*d_xy*i_5)/420/b_strip**3
             kf_mp[0, 1] = (2520*b_strip*d_x*i_1 - 462*b_strip**3*d_1*i_2 - 42*b_strip**3*d_1*i_3 \
                 + 22*b_strip**5*d_y*i_4 + 168*b_strip**3*d_xy*i_5)/420/b_strip**3
             kf_mp[0, 2] = (-5040*d_x*i_1 + 504*b_strip**2*d_1*i_2 + 504*b_strip**2*d_1*i_3 \
                 + 54*b_strip**4*d_y*i_4 - 2016*b_strip**2*d_xy*i_5)/420/b_strip**3
             kf_mp[0, 3] = (2520*b_strip*d_x*i_1 - 42*b_strip**3*d_1*i_2 - 42*b_strip**3*d_1*i_3 \
@@ -214,21 +213,17 @@
             kf_mp[3, 0] = kf_mp[0, 3]
             kf_mp[3, 1] = kf_mp[1, 3]
             kf_mp[3, 2] = (-2520*b_strip*d_x*i_1 + 462*b_strip**3*d_1*i_3 + 42*b_strip**3*d_1*i_2 \
                 - 22*b_strip**5*d_y*i_4 - 168*b_strip**3*d_xy*i_5)/420/b_strip**3 # not symmetric
             kf_mp[3, 3] = (1680*b_strip**2*d_x*i_1 - 56*b_strip**4*d_1*i_2 - 56*b_strip**4*d_1*i_3 \
                 + 4*b_strip**6*d_y*i_4 + 224*b_strip**4*d_xy*i_5)/420/b_strip**3
 
-            # assemble the membrane and flexural stiffness matrices
-            k_mp = np.concatenate((
-                np.concatenate((km_mp, zero_matrix),
-                               axis=1), np.concatenate((zero_matrix, kf_mp), axis=1)
-            ))
-            # add it into local element stiffness matrix by corresponding to i
-            k_local[8 * i:8 * (i+1), 8 * j:8 * (j+1)] = k_mp
+            k_local[8 * i:8*i + 4, 8 * j:8*j + 4] = km_mp
+            k_local[8*i + 4:8 * (i+1), 8*j + 4:8 * (j+1)] = kf_mp
+
     return k_local
 
 
 def bc_i1_5(b_c, m_i, m_j, length):
     # Calculate the 5 undetermined parameters i_1,i_2,i_3,i_4,i_5 for local elastic
     # and geometric stiffness matrices.
     # b_c: a string specifying boundary conditions to be analysed:
@@ -242,28 +237,28 @@
     # calculation of i_1 is the integration of y_m*Yn from 0 to length
     # calculation of i_2 is the integration of y_m''*Yn from 0 to length
     # calculation of i_3 is the integration of y_m*Yn'' from 0 to length
     # calculation of i_3 is the integration of y_m*Yn'' from 0 to length
     # calculation of i_4 is the integration of y_m''*Yn'' from 0 to length
     # calculation of i_5 is the integration of y_m'*Yn' from 0 to length
 
+    i_1 = 0
+    i_2 = 0
+    i_3 = 0
+    i_4 = 0
+    i_5 = 0
+
     if b_c == 'S-S':
         # For simply-pimply supported boundary condition at loaded edges
         if m_i == m_j:
             i_1 = length / 2
             i_2 = -m_i**2 * np.pi**2 / length / 2
             i_3 = -m_j**2 * np.pi**2 / length / 2
             i_4 = np.pi**4 * m_i**4 / 2 / length**3
             i_5 = np.pi**2 * m_i**2 / 2 / length
-        else:
-            i_1 = 0
-            i_2 = 0
-            i_3 = 0
-            i_4 = 0
-            i_5 = 0
 
     elif b_c == 'C-C':
         # For Clamped-clamped boundary condition at loaded edges
         # calculation of i_1 is the integration of y_m*Yn from 0 to length
         if m_i == m_j:
             if m_i == 1:
                 i_1 = 3 * length / 8
@@ -282,20 +277,14 @@
                 i_5 = -(1 + m_i*m_j) * np.pi**2 / 8 / length
             elif m_i - m_j == -2:
                 i_1 = -length / 8
                 i_2 = (m_i**2 + 1) * np.pi**2 / 8 / length + m_i * np.pi**2 / 4 / length
                 i_3 = (m_j**2 + 1) * np.pi**2 / 8 / length - m_j * np.pi**2 / 4 / length
                 i_4 = -(m_i + 1)**2 * (m_j - 1)**2 * np.pi**4 / 8 / length**3
                 i_5 = -(1 + m_i*m_j) * np.pi**2 / 8 / length
-            else:
-                i_1 = 0
-                i_2 = 0
-                i_3 = 0
-                i_4 = 0
-                i_5 = 0
 
     elif b_c == 'S-C' or b_c == 'C-S':
         # For simply-clamped supported boundary condition at loaded edges
         # calculation of i_1 is the integration of y_m*Yn from 0 to length
         if m_i == m_j:
             i_1 = (1 + (m_i + 1)**2 / m_i**2) * length / 2
             i_2 = -(m_i + 1)**2 * np.pi**2 / length
@@ -311,20 +300,14 @@
                 i_5 = (1+m_i) * (1+m_j) * np.pi**2 / 2 / length
             elif m_i - m_j == -1:
                 i_1 = (m_j+1) * length / 2 / m_j
                 i_2 = -(m_i + 1)**2 * np.pi**2 * (m_j+1) / 2 / length / m_j
                 i_3 = -(m_j + 1) * m_j * np.pi**2 / 2 / length
                 i_4 = (m_i + 1)**2 * m_j * (m_j+1) * np.pi**4 / 2 / length**3
                 i_5 = (1+m_i) * (1+m_j) * np.pi**2 / 2 / length
-            else:
-                i_1 = 0
-                i_2 = 0
-                i_3 = 0
-                i_4 = 0
-                i_5 = 0
 
     elif b_c == 'C-F' or b_c == 'F-C':
         # For clamped-free supported boundary condition at loaded edges
         # calculation of i_1 is the integration of y_m*Yn from 0 to length
         if m_i == m_j:
             i_1 = 3*length/2 - 2 * length * (-1)**(m_i - 1) / (m_i - 1/2) / np.pi
             i_2 = (m_i - 1/2)**2 * np.pi**2 * ((-1)**(m_i - 1) / (m_i - 1/2) / np.pi - 1/2) / length
@@ -332,16 +315,14 @@
             i_4 = (m_i - 1/2)**4 * np.pi**4 / 2 / length**3
             i_5 = (m_i - 1/2)**2 * np.pi**2 / 2 / length
         else:
             i_1 = length - length*(-1)**(m_i - 1) / (m_i - 1/2) / np.pi \
                 - length*(-1)**(m_j - 1) / (m_j - 1/2) / np.pi
             i_2 = (m_i - 1/2)**2 * np.pi**2 * ((-1)**(m_i - 1) / (m_i - 1/2) / np.pi) / length
             i_3 = (m_j - 1/2)**2 * np.pi**2 * ((-1)**(m_j - 1) / (m_j - 1/2) / np.pi) / length
-            i_4 = 0
-            i_5 = 0
 
     elif b_c == 'C-G' or b_c == 'G-C':
         # For clamped-guided supported boundary condition at loaded edges
         # calculation of i_1 is the integration of y_m*Yn from 0 to length
         if m_i == m_j:
             if m_i == 1:
                 i_1 = 3 * length / 8
@@ -365,20 +346,15 @@
                 i_1 = -length / 8
                 i_2 = ((m_i - 1/2)**2
                        + 1/4) * np.pi**2 / length / 8 + (m_i - 1/2) * np.pi**2 / length / 8
                 i_3 = ((m_j - 1/2)**2
                        + 1/4) * np.pi**2 / length / 8 - (m_j - 1/2) * np.pi**2 / length / 8
                 i_4 = -m_i**4 * np.pi**4 / 8 / length**3
                 i_5 = -m_i**2 * np.pi**2 / 8 / length
-            else:
-                i_1 = 0
-                i_2 = 0
-                i_3 = 0
-                i_4 = 0
-                i_5 = 0
+
     return [i_1, i_2, i_3, i_4, i_5]
 
 
 def kglocal(length, b_strip, ty_1, ty_2, b_c, m_a):
     # Generate geometric stiffness matrix (kg_local) in local coordinates
 
     # Inputs:
@@ -405,15 +381,14 @@
 
     total_m = len(m_a)  # Total number of longitudinal terms m
     kg_local = np.zeros((8 * total_m, 8 * total_m))
 
     for i in range(0, total_m):
         for j in range(0, total_m):
             gm_mp = np.zeros((4, 4))
-            zero_matrix = np.zeros((4, 4))
             gf_mp = np.zeros((4, 4))
             u_i = m_a[i] * np.pi
             u_j = m_a[j] * np.pi
 
             [_, _, _, i_4, i_5] = bc_i1_5(b_c, m_a[i], m_a[j], length)
 
             # assemble the matrix of gm_mp (symmetric membrane stability matrix)
@@ -440,22 +415,16 @@
             gf_mp[1, 3] = -(ty_1 + ty_2) * b_strip**3 * i_5 / 140 / 2
             gf_mp[3, 1] = gf_mp[1, 3]
             gf_mp[2, 2] = (3*ty_1 + 10*ty_2) * b_strip * i_5 / 35
             gf_mp[2, 3] = -(7*ty_1 + 15*ty_2) * b_strip**2 * i_5 / 420
             gf_mp[3, 2] = gf_mp[2, 3]
             gf_mp[3, 3] = (3*ty_1 + 5*ty_2) * b_strip**3 * i_5 / 420 / 2
 
-            # assemble the membrane and flexural stiffness matrices
-            kg_mp = np.concatenate((
-                np.concatenate((gm_mp, zero_matrix),
-                               axis=1), np.concatenate((zero_matrix, gf_mp), axis=1)
-            ))
-
-            # add it into local geometric stiffness matrix by corresponding to i
-            kg_local[8 * i:8 * (i+1), 8 * j:8 * (j+1)] = kg_mp
+            kg_local[8 * i:8*i + 4, 8 * j:8*j + 4] = gm_mp
+            kg_local[8*i + 4:8 * (i+1), 8*j + 4:8 * (j+1)] = gf_mp
     return kg_local
 
 
 def trans(alpha, k_local, kg_local, m_a):
     # Transfer the local stiffness into global stiffness
     # Zhanjie 2008
     # modified by Z. Li, Aug. 09, 2009
@@ -468,18 +437,18 @@
                     [np.sin(alpha), 0, 0, 0, np.cos(alpha), 0, 0, 0], [0, 0, 0, 0, 0, 1, 0, 0],
                     [0, 0, np.sin(alpha), 0, 0, 0, np.cos(alpha), 0], [0, 0, 0, 0, 0, 0, 0, 1]])
 
     # extend to multi-m
     for i in range(0, total_m):
         gamma[8 * i:8 * (i+1), 8 * i:8 * (i+1)] = gam
 
-    kglobal = gamma @ k_local @ gamma.conj().T
-    kgglobal = gamma @ kg_local @ gamma.conj().T
+    k_global = gamma @ k_local @ gamma.conj().T
+    kg_global = gamma @ kg_local @ gamma.conj().T
 
-    return [kglobal, kgglobal]
+    return [k_global, kg_global]
 
 
 def assemble(k_global, kg_global, k_local, kg_local, node_i, node_j, n_nodes, m_a):
     # Add the element contribution to the global stiffness matrix
 
     # Outputs:
     # k_global: global elastic stiffness matrix
@@ -489,16 +458,14 @@
     #[u1 v1...un vn w1 01...wn 0n]m'.
 
     # Z. Li, June 2008
     # modified by Z. Li, Aug. 09, 2009
     # Z. Li, June 2010
 
     total_m = len(m_a)  # Total number of longitudinal terms m
-    k_2_matrix = np.zeros((4 * n_nodes * total_m, 4 * n_nodes * total_m))
-    k_3_matrix = np.zeros((4 * n_nodes * total_m, 4 * n_nodes * total_m))
     skip = 2 * n_nodes
     for i in range(0, total_m):
         for j in range(0, total_m):
             # Submatrices for the initial stiffness
             k11 = k_local[8 * i:8*i + 2, 8 * j:8*j + 2]
             k12 = k_local[8 * i:8*i + 2, 8*j + 2:8*j + 4]
             k13 = k_local[8 * i:8*i + 2, 8*j + 4:8*j + 6]
@@ -512,49 +479,49 @@
             k33 = k_local[8*i + 4:8*i + 6, 8*j + 4:8*j + 6]
             k34 = k_local[8*i + 4:8*i + 6, 8*j + 6:8*j + 8]
             k41 = k_local[8*i + 6:8*i + 8, 8 * j:8*j + 2]
             k42 = k_local[8*i + 6:8*i + 8, 8*j + 2:8*j + 4]
             k43 = k_local[8*i + 6:8*i + 8, 8*j + 4:8*j + 6]
             k44 = k_local[8*i + 6:8*i + 8, 8*j + 6:8*j + 8]
 
-            k_2_matrix[4*n_nodes*i+(node_i+1)*2-2:4*n_nodes*i+(node_i+1)*2, \
-                4*n_nodes*j+(node_i+1)*2-2:4*n_nodes*j+(node_i+1)*2] = k11
-            k_2_matrix[4*n_nodes*i+(node_i+1)*2-2:4*n_nodes*i+(node_i+1)*2, \
-                4*n_nodes*j+(node_j+1)*2-2:4*n_nodes*j+(node_j+1)*2] = k12
-            k_2_matrix[4*n_nodes*i+(node_j+1)*2-2:4*n_nodes*i+(node_j+1)*2, \
-                4*n_nodes*j+(node_i+1)*2-2:4*n_nodes*j+(node_i+1)*2] = k21
-            k_2_matrix[4*n_nodes*i+(node_j+1)*2-2:4*n_nodes*i+(node_j+1)*2, \
-                4*n_nodes*j+(node_j+1)*2-2:4*n_nodes*j+(node_j+1)*2] = k22
-
-            k_2_matrix[4*n_nodes*i+skip+(node_i+1)*2-2:4*n_nodes*i+skip+(node_i+1)*2, \
-                4*n_nodes*j+skip+(node_i+1)*2-2:4*n_nodes*j+skip+(node_i+1)*2] = k33
-            k_2_matrix[4*n_nodes*i+skip+(node_i+1)*2-2:4*n_nodes*i+skip+(node_i+1)*2, \
-                4*n_nodes*j+skip+(node_j+1)*2-2:4*n_nodes*j+skip+(node_j+1)*2] = k34
-            k_2_matrix[4*n_nodes*i+skip+(node_j+1)*2-2:4*n_nodes*i+skip+(node_j+1)*2, \
-                4*n_nodes*j+skip+(node_i+1)*2-2:4*n_nodes*j+skip+(node_i+1)*2] = k43
-            k_2_matrix[4*n_nodes*i+skip+(node_j+1)*2-2:4*n_nodes*i+skip+(node_j+1)*2, \
-                4*n_nodes*j+skip+(node_j+1)*2-2:4*n_nodes*j+skip+(node_j+1)*2] = k44
-
-            k_2_matrix[4*n_nodes*i+(node_i+1)*2-2:4*n_nodes*i+(node_i+1)*2, \
-                4*n_nodes*j+skip+(node_i+1)*2-2:4*n_nodes*j+skip+(node_i+1)*2] = k13
-            k_2_matrix[4*n_nodes*i+(node_i+1)*2-2:4*n_nodes*i+(node_i+1)*2, \
-                4*n_nodes*j+skip+(node_j+1)*2-2:4*n_nodes*j+skip+(node_j+1)*2] = k14
-            k_2_matrix[4*n_nodes*i+(node_j+1)*2-2:4*n_nodes*i+(node_j+1)*2, \
-                4*n_nodes*j+skip+(node_i+1)*2-2:4*n_nodes*j+skip+(node_i+1)*2] = k23
-            k_2_matrix[4*n_nodes*i+(node_j+1)*2-2:4*n_nodes*i+(node_j+1)*2, \
-                4*n_nodes*j+skip+(node_j+1)*2-2:4*n_nodes*j+skip+(node_j+1)*2] = k24
-
-            k_2_matrix[4*n_nodes*i+skip+(node_i+1)*2-2:4*n_nodes*i+skip+(node_i+1)*2, \
-                4*n_nodes*j+(node_i+1)*2-2:4*n_nodes*j+(node_i+1)*2] = k31
-            k_2_matrix[4*n_nodes*i+skip+(node_i+1)*2-2:4*n_nodes*i+skip+(node_i+1)*2, \
-                4*n_nodes*j+(node_j+1)*2-2:4*n_nodes*j+(node_j+1)*2] = k32
-            k_2_matrix[4*n_nodes*i+skip+(node_j+1)*2-2:4*n_nodes*i+skip+(node_j+1)*2, \
-                4*n_nodes*j+(node_i+1)*2-2:4*n_nodes*j+(node_i+1)*2] = k41
-            k_2_matrix[4*n_nodes*i+skip+(node_j+1)*2-2:4*n_nodes*i+skip+(node_j+1)*2, \
-                4*n_nodes*j+(node_j+1)*2-2:4*n_nodes*j+(node_j+1)*2] = k42
+            k_global[4*n_nodes*i+(node_i+1)*2-2:4*n_nodes*i+(node_i+1)*2, \
+                4*n_nodes*j+(node_i+1)*2-2:4*n_nodes*j+(node_i+1)*2] += k11
+            k_global[4*n_nodes*i+(node_i+1)*2-2:4*n_nodes*i+(node_i+1)*2, \
+                4*n_nodes*j+(node_j+1)*2-2:4*n_nodes*j+(node_j+1)*2] += k12
+            k_global[4*n_nodes*i+(node_j+1)*2-2:4*n_nodes*i+(node_j+1)*2, \
+                4*n_nodes*j+(node_i+1)*2-2:4*n_nodes*j+(node_i+1)*2] += k21
+            k_global[4*n_nodes*i+(node_j+1)*2-2:4*n_nodes*i+(node_j+1)*2, \
+                4*n_nodes*j+(node_j+1)*2-2:4*n_nodes*j+(node_j+1)*2] += k22
+
+            k_global[4*n_nodes*i+skip+(node_i+1)*2-2:4*n_nodes*i+skip+(node_i+1)*2, \
+                4*n_nodes*j+skip+(node_i+1)*2-2:4*n_nodes*j+skip+(node_i+1)*2] += k33
+            k_global[4*n_nodes*i+skip+(node_i+1)*2-2:4*n_nodes*i+skip+(node_i+1)*2, \
+                4*n_nodes*j+skip+(node_j+1)*2-2:4*n_nodes*j+skip+(node_j+1)*2] += k34
+            k_global[4*n_nodes*i+skip+(node_j+1)*2-2:4*n_nodes*i+skip+(node_j+1)*2, \
+                4*n_nodes*j+skip+(node_i+1)*2-2:4*n_nodes*j+skip+(node_i+1)*2] += k43
+            k_global[4*n_nodes*i+skip+(node_j+1)*2-2:4*n_nodes*i+skip+(node_j+1)*2, \
+                4*n_nodes*j+skip+(node_j+1)*2-2:4*n_nodes*j+skip+(node_j+1)*2] += k44
+
+            k_global[4*n_nodes*i+(node_i+1)*2-2:4*n_nodes*i+(node_i+1)*2, \
+                4*n_nodes*j+skip+(node_i+1)*2-2:4*n_nodes*j+skip+(node_i+1)*2] += k13
+            k_global[4*n_nodes*i+(node_i+1)*2-2:4*n_nodes*i+(node_i+1)*2, \
+                4*n_nodes*j+skip+(node_j+1)*2-2:4*n_nodes*j+skip+(node_j+1)*2] += k14
+            k_global[4*n_nodes*i+(node_j+1)*2-2:4*n_nodes*i+(node_j+1)*2, \
+                4*n_nodes*j+skip+(node_i+1)*2-2:4*n_nodes*j+skip+(node_i+1)*2] += k23
+            k_global[4*n_nodes*i+(node_j+1)*2-2:4*n_nodes*i+(node_j+1)*2, \
+                4*n_nodes*j+skip+(node_j+1)*2-2:4*n_nodes*j+skip+(node_j+1)*2] += k24
+
+            k_global[4*n_nodes*i+skip+(node_i+1)*2-2:4*n_nodes*i+skip+(node_i+1)*2, \
+                4*n_nodes*j+(node_i+1)*2-2:4*n_nodes*j+(node_i+1)*2] += k31
+            k_global[4*n_nodes*i+skip+(node_i+1)*2-2:4*n_nodes*i+skip+(node_i+1)*2, \
+                4*n_nodes*j+(node_j+1)*2-2:4*n_nodes*j+(node_j+1)*2] += k32
+            k_global[4*n_nodes*i+skip+(node_j+1)*2-2:4*n_nodes*i+skip+(node_j+1)*2, \
+                4*n_nodes*j+(node_i+1)*2-2:4*n_nodes*j+(node_i+1)*2] += k41
+            k_global[4*n_nodes*i+skip+(node_j+1)*2-2:4*n_nodes*i+skip+(node_j+1)*2, \
+                4*n_nodes*j+(node_j+1)*2-2:4*n_nodes*j+(node_j+1)*2] += k42
 
             # Submatrices for the initial stiffness
             kg11 = kg_local[8 * i:8*i + 2, 8 * j:8*j + 2]
             kg12 = kg_local[8 * i:8*i + 2, 8*j + 2:8*j + 4]
             kg13 = kg_local[8 * i:8*i + 2, 8*j + 4:8*j + 6]
             kg14 = kg_local[8 * i:8*i + 2, 8*j + 6:8*j + 8]
             kg21 = kg_local[8*i + 2:8*i + 4, 8 * j:8*j + 2]
@@ -566,56 +533,53 @@
             kg33 = kg_local[8*i + 4:8*i + 6, 8*j + 4:8*j + 6]
             kg34 = kg_local[8*i + 4:8*i + 6, 8*j + 6:8*j + 8]
             kg41 = kg_local[8*i + 6:8*i + 8, 8 * j:8*j + 2]
             kg42 = kg_local[8*i + 6:8*i + 8, 8*j + 2:8*j + 4]
             kg43 = kg_local[8*i + 6:8*i + 8, 8*j + 4:8*j + 6]
             kg44 = kg_local[8*i + 6:8*i + 8, 8*j + 6:8*j + 8]
 
-            k_3_matrix[4*n_nodes*i + (node_i+1) * 2 - 2:4*n_nodes*i + (node_i+1) * 2,
-                       4*n_nodes*j + (node_i+1) * 2 - 2:4*n_nodes*j + (node_i+1) * 2] = kg11
-            k_3_matrix[4*n_nodes*i + (node_i+1) * 2 - 2:4*n_nodes*i + (node_i+1) * 2,
-                       4*n_nodes*j + (node_j+1) * 2 - 2:4*n_nodes*j + (node_j+1) * 2] = kg12
-            k_3_matrix[4*n_nodes*i + (node_j+1) * 2 - 2:4*n_nodes*i + (node_j+1) * 2,
-                       4*n_nodes*j + (node_i+1) * 2 - 2:4*n_nodes*j + (node_i+1) * 2] = kg21
-            k_3_matrix[4*n_nodes*i + (node_j+1) * 2 - 2:4*n_nodes*i + (node_j+1) * 2,
-                       4*n_nodes*j + (node_j+1) * 2 - 2:4*n_nodes*j + (node_j+1) * 2] = kg22
-
-            k_3_matrix[4*n_nodes*i + skip + (node_i+1) * 2 - 2:4*n_nodes*i + skip + (node_i+1) * 2,
-                       4*n_nodes*j + skip + (node_i+1) * 2 - 2:4*n_nodes*j + skip
-                       + (node_i+1) * 2] = kg33
-            k_3_matrix[4*n_nodes*i + skip + (node_i+1) * 2 - 2:4*n_nodes*i + skip + (node_i+1) * 2,
-                       4*n_nodes*j + skip + (node_j+1) * 2 - 2:4*n_nodes*j + skip
-                       + (node_j+1) * 2] = kg34
-            k_3_matrix[4*n_nodes*i + skip + (node_j+1) * 2 - 2:4*n_nodes*i + skip + (node_j+1) * 2,
-                       4*n_nodes*j + skip + (node_i+1) * 2 - 2:4*n_nodes*j + skip
-                       + (node_i+1) * 2] = kg43
-            k_3_matrix[4*n_nodes*i + skip + (node_j+1) * 2 - 2:4*n_nodes*i + skip + (node_j+1) * 2,
-                       4*n_nodes*j + skip + (node_j+1) * 2 - 2:4*n_nodes*j + skip
-                       + (node_j+1) * 2] = kg44
-
-            k_3_matrix[4*n_nodes*i + (node_i+1) * 2 - 2:4*n_nodes*i + (node_i+1) * 2, 4*n_nodes*j
-                       + skip + (node_i+1) * 2 - 2:4*n_nodes*j + skip + (node_i+1) * 2] = kg13
-            k_3_matrix[4*n_nodes*i + (node_i+1) * 2 - 2:4*n_nodes*i + (node_i+1) * 2, 4*n_nodes*j
-                       + skip + (node_j+1) * 2 - 2:4*n_nodes*j + skip + (node_j+1) * 2] = kg14
-            k_3_matrix[4*n_nodes*i + (node_j+1) * 2 - 2:4*n_nodes*i + (node_j+1) * 2, 4*n_nodes*j
-                       + skip + (node_i+1) * 2 - 2:4*n_nodes*j + skip + (node_i+1) * 2] = kg23
-            k_3_matrix[4*n_nodes*i + (node_j+1) * 2 - 2:4*n_nodes*i + (node_j+1) * 2, 4*n_nodes*j
-                       + skip + (node_j+1) * 2 - 2:4*n_nodes*j + skip + (node_j+1) * 2] = kg24
-
-            k_3_matrix[4*n_nodes*i + skip + (node_i+1) * 2 - 2:4*n_nodes*i + skip + (node_i+1) * 2,
-                       4*n_nodes*j + (node_i+1) * 2 - 2:4*n_nodes*j + (node_i+1) * 2] = kg31
-            k_3_matrix[4*n_nodes*i + skip + (node_i+1) * 2 - 2:4*n_nodes*i + skip + (node_i+1) * 2,
-                       4*n_nodes*j + (node_j+1) * 2 - 2:4*n_nodes*j + (node_j+1) * 2] = kg32
-            k_3_matrix[4*n_nodes*i + skip + (node_j+1) * 2 - 2:4*n_nodes*i + skip + (node_j+1) * 2,
-                       4*n_nodes*j + (node_i+1) * 2 - 2:4*n_nodes*j + (node_i+1) * 2] = kg41
-            k_3_matrix[4*n_nodes*i + skip + (node_j+1) * 2 - 2:4*n_nodes*i + skip + (node_j+1) * 2,
-                       4*n_nodes*j + (node_j+1) * 2 - 2:4*n_nodes*j + (node_j+1) * 2] = kg42
-
-    k_global = k_global + k_2_matrix
-    kg_global = kg_global + k_3_matrix
+            kg_global[4*n_nodes*i + (node_i+1) * 2 - 2:4*n_nodes*i + (node_i+1) * 2,
+                      4*n_nodes*j + (node_i+1) * 2 - 2:4*n_nodes*j + (node_i+1) * 2] += kg11
+            kg_global[4*n_nodes*i + (node_i+1) * 2 - 2:4*n_nodes*i + (node_i+1) * 2,
+                      4*n_nodes*j + (node_j+1) * 2 - 2:4*n_nodes*j + (node_j+1) * 2] += kg12
+            kg_global[4*n_nodes*i + (node_j+1) * 2 - 2:4*n_nodes*i + (node_j+1) * 2,
+                      4*n_nodes*j + (node_i+1) * 2 - 2:4*n_nodes*j + (node_i+1) * 2] += kg21
+            kg_global[4*n_nodes*i + (node_j+1) * 2 - 2:4*n_nodes*i + (node_j+1) * 2,
+                      4*n_nodes*j + (node_j+1) * 2 - 2:4*n_nodes*j + (node_j+1) * 2] += kg22
+
+            kg_global[4*n_nodes*i + skip + (node_i+1) * 2 - 2:4*n_nodes*i + skip + (node_i+1) * 2,
+                      4*n_nodes*j + skip + (node_i+1) * 2 - 2:4*n_nodes*j + skip
+                      + (node_i+1) * 2] += kg33
+            kg_global[4*n_nodes*i + skip + (node_i+1) * 2 - 2:4*n_nodes*i + skip + (node_i+1) * 2,
+                      4*n_nodes*j + skip + (node_j+1) * 2 - 2:4*n_nodes*j + skip
+                      + (node_j+1) * 2] += kg34
+            kg_global[4*n_nodes*i + skip + (node_j+1) * 2 - 2:4*n_nodes*i + skip + (node_j+1) * 2,
+                      4*n_nodes*j + skip + (node_i+1) * 2 - 2:4*n_nodes*j + skip
+                      + (node_i+1) * 2] += kg43
+            kg_global[4*n_nodes*i + skip + (node_j+1) * 2 - 2:4*n_nodes*i + skip + (node_j+1) * 2,
+                      4*n_nodes*j + skip + (node_j+1) * 2 - 2:4*n_nodes*j + skip
+                      + (node_j+1) * 2] += kg44
+
+            kg_global[4*n_nodes*i + (node_i+1) * 2 - 2:4*n_nodes*i + (node_i+1) * 2, 4*n_nodes*j
+                      + skip + (node_i+1) * 2 - 2:4*n_nodes*j + skip + (node_i+1) * 2] += kg13
+            kg_global[4*n_nodes*i + (node_i+1) * 2 - 2:4*n_nodes*i + (node_i+1) * 2, 4*n_nodes*j
+                      + skip + (node_j+1) * 2 - 2:4*n_nodes*j + skip + (node_j+1) * 2] += kg14
+            kg_global[4*n_nodes*i + (node_j+1) * 2 - 2:4*n_nodes*i + (node_j+1) * 2, 4*n_nodes*j
+                      + skip + (node_i+1) * 2 - 2:4*n_nodes*j + skip + (node_i+1) * 2] += kg23
+            kg_global[4*n_nodes*i + (node_j+1) * 2 - 2:4*n_nodes*i + (node_j+1) * 2, 4*n_nodes*j
+                      + skip + (node_j+1) * 2 - 2:4*n_nodes*j + skip + (node_j+1) * 2] += kg24
+
+            kg_global[4*n_nodes*i + skip + (node_i+1) * 2 - 2:4*n_nodes*i + skip + (node_i+1) * 2,
+                      4*n_nodes*j + (node_i+1) * 2 - 2:4*n_nodes*j + (node_i+1) * 2] += kg31
+            kg_global[4*n_nodes*i + skip + (node_i+1) * 2 - 2:4*n_nodes*i + skip + (node_i+1) * 2,
+                      4*n_nodes*j + (node_j+1) * 2 - 2:4*n_nodes*j + (node_j+1) * 2] += kg32
+            kg_global[4*n_nodes*i + skip + (node_j+1) * 2 - 2:4*n_nodes*i + skip + (node_j+1) * 2,
+                      4*n_nodes*j + (node_i+1) * 2 - 2:4*n_nodes*j + (node_i+1) * 2] += kg41
+            kg_global[4*n_nodes*i + skip + (node_j+1) * 2 - 2:4*n_nodes*i + skip + (node_j+1) * 2,
+                      4*n_nodes*j + (node_j+1) * 2 - 2:4*n_nodes*j + (node_j+1) * 2] += kg42
 
     return [k_global, kg_global]
 
 
 def spring_klocal(k_u, k_v, k_w, k_q, length, b_c, m_a, discrete, y_s):
     # Generate spring stiffness matrix (k_local) in local coordinates, modified from
     # klocal
@@ -637,45 +601,40 @@
     # Output:
     # k_local: local stiffness matrix, a total_m x total_m matrix of 8 by 8 submatrices.
     # k_local=[k_mp]total_m x total_m block matrix
     # each k_mp is the 8 x 8 submatrix in the DOF order [u1 v1 u2 v2 w1 theta1 w2 theta2]'
 
     total_m = len(m_a)  # Total number of longitudinal terms m
     k_local = np.zeros(8 * total_m, 8 * total_m)
-    z_0 = np.zeros(4, 4)
     for i in range(0, total_m):
         for j in range(0, total_m):
             km_mp = np.zeros(4, 4)
             kf_mp = np.zeros(4, 4)
             u_i = m_a[i] * np.pi
             u_j = m_a[j] * np.pi
 
             if discrete:
                 [i_1, i_5] = bc_i1_5_atpoint(
                     b_c=b_c, m_i=m_a[i], m_j=m_a[j], length=length, y_s=y_s
                 )
             else:  # foundation spring
                 [i_1, _, _, _, i_5] = bc_i1_5(b_c=b_c, m_i=m_a[i], m_j=m_a[j], length=length)
-            # assemble the matrix of km_mp
+            # assemble the matrix of km_mp (membrane stiffness)
             km_mp = np.array(
                 [[k_u * i_1, 0, -k_u * i_1, 0],
                  [0, k_v * i_5 * length**2 / (u_i*u_j), 0, -k_v * i_5 * length**2 / (u_i*u_j)],
                  [-k_u * i_1, 0, k_u * i_1, 0],
                  [0, -k_v * i_5 * length**2 / (u_i*u_j), 0, k_v * i_5 * length**2 / (u_i*u_j)]]
             )
-            # assemble the matrix of kf_mp
+            # assemble the matrix of kf_mp (flexural stiffness)
             kf_mp = np.array([[k_w * i_1, 0, -k_w * i_1, 0], [0, k_q * i_1, 0, -k_q * i_1],
                               [-k_w * i_1, 0, k_w * i_1, 0], [0, -k_q * i_1, 0, k_q * i_1]])
-            # assemble the membrane and flexural stiffness matrices
-            k_mp = np.concatenate(
-                (np.concatenate((km_mp, z_0), axis=1), np.concatenate((z_0, kf_mp), axis=1))
-            )
 
-            # add it into local element stiffness matrix by corresponding to m
-            k_local[8 * i:8 * (i+1), 8 * j:8 * (j+1)] = k_mp
+            k_local[8 * i:8*i + 4, 8 * j:8*j + 4] = km_mp
+            k_local[8*i + 4:8 * (i+1), 8*j + 4:8 * (j+1)] = kf_mp
 
     return k_local
 
 
 def bc_i1_5_atpoint(b_c, m_i, m_j, length, y_s):
     # Calculate the value of the longitudinal shape functions for discrete springs
```

### Comparing `pycufsm-0.1.0/pycufsm/cfsm.py` & `pycufsm-0.1.1/pycufsm/cfsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import deepcopy
 from scipy import linalg as spla
 import numpy as np
-import pycufsm.analysis
+from pycufsm.analysis import analysis
 
 # Originally developed for MATLAB by Benjamin Schafer PhD et al
 # Ported to Python by Brooks Smith MEng, PE, CPEng
 #
 # Each function within this file was originally its own separate file.
 # Original MATLAB comments, especially those retaining to authorship or
 # change history, have been generally retained unaltered
@@ -298,15 +298,15 @@
                 row = int((np.argwhere(props[:, 0] == mat_num)).reshape(1))
                 mat = props[row]
                 stiff_x = mat[1]
                 stiff_y = mat[2]
                 nu_x = mat[3]
                 nu_y = mat[4]
                 bulk = mat[5]
-                k_l = pycufsm.analysis.klocal(
+                k_l = analysis.klocal(
                     stiff_x=stiff_x,
                     stiff_y=stiff_y,
                     nu_x=nu_x,
                     nu_y=nu_y,
                     bulk=bulk,
                     thick=thick,
                     length=length,
@@ -315,26 +315,26 @@
                     m_a=m_a
                 )
                 # Generate geometric stiffness matrix (kg_local) in local coordinates
                 node_i = int(elem[1])
                 node_j = int(elem[2])
                 ty_1 = nodes_base[node_i][7] * thick
                 ty_2 = nodes_base[node_j][7] * thick
-                kg_l = pycufsm.analysis.kglocal(
+                kg_l = analysis.kglocal(
                     length=length, b_strip=b_strip, ty_1=ty_1, ty_2=ty_2, b_c=b_c, m_a=m_a
                 )
                 # Transform k_local and kg_local into global coordinates
                 alpha = el_props[i, 2]
-                [k_local, kg_local] = pycufsm.analysis.trans(
+                [k_local, kg_local] = analysis.trans(
                     alpha=alpha, k_local=k_l, kg_local=kg_l, m_a=m_a
                 )
 
                 # Add element contribution of k_local to full matrix k_global
                 # and kg_local to kg_global
-                [k_global, kg_global] = pycufsm.analysis.assemble(
+                [k_global, kg_global] = analysis.assemble(
                     k_global=k_global,
                     kg_global=kg_global,
                     k_local=k_local,
                     kg_local=kg_local,
                     node_i=node_i,
                     node_j=node_j,
                     n_nodes=n_nodes,
@@ -1873,26 +1873,25 @@
     e_1 = stiff_x / (1 - nu_x*nu_y)
     e_2 = stiff_y / (1 - nu_x*nu_y)
     d_x = stiff_x * thick**3 / (12 * (1 - nu_x*nu_y))
     d_y = stiff_y * thick**3 / (12 * (1 - nu_x*nu_y))
     d_1 = nu_x * stiff_y * thick**3 / (12 * (1 - nu_x*nu_y))
     d_xy = bulk * thick**3 / 12
     #
-    # k_local = sparse(np.zeros(8*m_i, 8*m_i))
-    z_0 = np.zeros((4, 4))
+    k_local = np.zeros(8 * m_i, 8 * m_i)
     i = m_i
     j = m_i
     km_mp = np.zeros((4, 4))
     kf_mp = np.zeros((4, 4))
     u_m = i * np.pi
     u_p = j * np.pi
     c_1 = u_m / length
     c_2 = u_p / length
     #
-    [i_1, i_2, i_3, i_4, i_5] = pycufsm.analysis.bc_i1_5(b_c, i, j, length)
+    [i_1, i_2, i_3, i_4, i_5] = analysis.bc_i1_5(b_c, i, j, length)
     #
     # assemble the matrix of Km_mp
     km_mp[0, 0] = e_1*i_1/b_strip + bulk*b_strip*i_5/3
     km_mp[0, 1] = e_2 * nu_x * (-1 / 2 / c_2) * i_3 - bulk*i_5/2/c_2
     km_mp[0, 2] = -e_1 * i_1 / b_strip + bulk*b_strip*i_5/6
     km_mp[0, 3] = e_2 * nu_x * (-1 / 2 / c_2) * i_3 + bulk*i_5/2/c_2
 
@@ -1942,40 +1941,35 @@
     kf_mp[3, 0] = kf_mp[0, 3]
     kf_mp[3, 1] = kf_mp[1, 3]
     kf_mp[3, 2] = (-2520*b_strip*d_x*i_1 + 462*b_strip**3*d_1*i_3 + 42*b_strip**3*d_1*i_2 \
         - 22*b_strip**5*d_y*i_4 - 168*b_strip**3*d_xy*i_5) / 420/b_strip**3 # not symmetric
     kf_mp[3, 3] = (1680*b_strip**2*d_x*i_1 - 56*b_strip**4*d_1*i_2 - 56*b_strip**4*d_1*i_3 \
         + 4*b_strip**6*d_y*i_4 + 224*b_strip**4*d_xy*i_5) / 420/b_strip**3
 
-    # assemble the membrane and flexural stiffness matrices
-    kmp = np.concatenate(
-        (np.concatenate((km_mp, z_0), axis=1), np.concatenate((z_0, kf_mp), axis=1))
-    )
-    # add it into local element stiffness matrix by corresponding to m_i
-    k_local = kmp
+    k_local[0:4, 0:4] = km_mp
+    k_local[4:8, 4:8] = kf_mp
 
     return k_local
 
 
 def kglocal_m(length, b_strip, m_i, ty_1, ty_2, b_c):
     # assemble local geometric stiffness matrix for a single longitudinal term m_i
 
     # created on Jul 10, 2009 by Z. Li
 
     # Generate geometric stiffness matrix (kg_local) in local coordinates
-    # kg_local = sparse(np.zeros(8*m_i, 8*m_i))
+    kg_local = np.zeros((8 * m_i, 8 * m_i))
     i = m_i
     j = m_i
     gm_mp = np.zeros((4, 4))
-    z_0 = np.zeros((4, 4))
     gf_mp = np.zeros((4, 4))
     u_m = i * np.pi
     u_p = j * np.pi
     #
-    [_, _, _, i_4, i_5] = pycufsm.analysis.bc_i1_5(b_c, i, j, length)
+    [_, _, _, i_4, i_5] = analysis.bc_i1_5(b_c, i, j, length)
     #
     # assemble the matrix of gm_mp (symmetric membrane stability matrix)
     gm_mp[0, 0] = b_strip * (3*ty_1 + ty_2) * i_5 / 12
     gm_mp[0, 2] = b_strip * (ty_1+ty_2) * i_5 / 12
     gm_mp[2, 0] = gm_mp[0, 2]
     gm_mp[1, 1] = b_strip * length**2 * (3*ty_1 + ty_2) * i_4 / 12 / u_m / u_p
     gm_mp[1, 3] = b_strip * length**2 * (ty_1+ty_2) * i_4 / 12 / u_m / u_p
@@ -1996,20 +1990,17 @@
     gf_mp[2, 1] = gf_mp[1, 2]
     gf_mp[1, 3] = -(ty_1 + ty_2) * b_strip**3 * i_5 / 140 / 2
     gf_mp[3, 1] = gf_mp[1, 3]
     gf_mp[2, 2] = (3*ty_1 + 10*ty_2) * b_strip * i_5 / 35
     gf_mp[2, 3] = -(7*ty_1 + 15*ty_2) * b_strip**2 * i_5 / 420
     gf_mp[3, 2] = gf_mp[2, 3]
     gf_mp[3, 3] = (3*ty_1 + 5*ty_2) * b_strip**3 * i_5 / 420 / 2
-    # assemble the membrane and flexural stiffness matrices
-    kg_mp = np.concatenate(
-        (np.concatenate((gm_mp, z_0), axis=1), np.concatenate((z_0, gf_mp), axis=1))
-    )
-    # add it into local geometric stiffness matrix by corresponding to m_i
-    kg_local = kg_mp
+
+    kg_local[0:4, 0:4] = gm_mp
+    kg_local[4:8, 4:8] = gf_mp
     return kg_local
 
 
 def trans_m(alpha, k_local, kg_local):
     # transfer the local stiffness into global stiffness
 
     # created on Jul 10, 2009 by Z. Li
@@ -2207,25 +2198,25 @@
     e_1 = stiff_x / (1 - nu_x*nu_y) * 100000000
     e_2 = stiff_y / (1 - nu_x*nu_y)
     d_x = stiff_x * thick**3 / (12 * (1 - nu_x*nu_y))
     d_y = stiff_y * thick**3 / (12 * (1 - nu_x*nu_y))
     d_1 = nu_x * stiff_y * thick**3 / (12 * (1 - nu_x*nu_y))
     d_xy = bulk * thick**3 / 12
 
-    z_0 = np.zeros((4, 4))
+    k_local = np.zeros((8, 8))
     i = m_i
     j = m_i
     km_mp = np.zeros((4, 4))
     kf_mp = np.zeros((4, 4))
     u_m = i * np.pi
     u_p = j * np.pi
     c_1 = u_m / length
     c_2 = u_p / length
 
-    [i_1, _, _, _, _] = pycufsm.analysis.bc_i1_5(b_c, i, j, length)
+    [i_1, _, _, _, _] = analysis.bc_i1_5(b_c, i, j, length)
     i_2 = 0
     i_3 = 0
     i_4 = 0
     i_5 = 0
 
     # assemble in-plane stiffness matrix of Km_mp
     km_mp[0, 0] = e_1*i_1/b_strip + bulk*b_strip*i_5/3
@@ -2278,21 +2269,16 @@
     kf_mp[3, 0] = kf_mp[0, 3]
     kf_mp[3, 1] = kf_mp[1, 3]
     kf_mp[3, 2] = (-2520*b_strip*d_x*i_1 + 462*b_strip**3*d_1*i_3 + 42*b_strip**3*d_1*i_2 \
         - 22*b_strip**5*d_y*i_4 - 168*b_strip**3*d_xy*i_5) / 420/b_strip**3 # not symmetric
     kf_mp[3, 3] = (1680*b_strip**2*d_x*i_1 - 56*b_strip**4*d_1*i_2 - 56*b_strip**4*d_1*i_3 \
         + 4*b_strip**6*d_y*i_4 + 224*b_strip**4*d_xy*i_5) / 420/b_strip**3
 
-    # assemble the membrane and flexural stiffness matrices
-    kmp = np.concatenate(
-        (np.concatenate((km_mp, z_0), axis=1), np.concatenate((z_0, kf_mp), axis=1))
-    )
-
-    # local stiffness matrix:
-    k_local = kmp
+    k_local[0:4, 0:4] = km_mp
+    k_local[4:8, 4:8] = kf_mp
     return k_local
 
 
 def assemble_single(k_global, k_local, node_i, node_j, n_nodes):
     #
     # this routine adds the element contribution to the global stiffness matrix
     # basically it does the same as routine 'assemble', however:
@@ -2371,18 +2357,18 @@
     # modified SA, Oct 10, 2006
     # Z.Li, June 2010
     n_nodes = len(nodes)
     n_dof_m = 4 * n_nodes
 
     # CLEAN UP INPUT
     # clean u_p 0's, multiple terms. or out-of-order terms in m_all
-    m_all = pycufsm.analysis.m_sort(m_all)
+    m_all = analysis.m_sort(m_all)
 
     # FIND BASE PROPERTIES
-    el_props = pycufsm.analysis.elem_prop(nodes=nodes, elements=elements)
+    el_props = analysis.elem_prop(nodes=nodes, elements=elements)
     # set u_p stress to 1.0 for finding kg_global and k_global for axial modes
     nodes_base = deepcopy(nodes)
     nodes_base[:, 7] = np.ones_like(nodes[:, 7])
 
     # natural base first
     # properties all the longitudinal terms share
     [main_nodes, meta_elements, node_props, n_main_nodes, \
```

### Comparing `pycufsm-0.1.0/pycufsm/cutwp.py` & `pycufsm-0.1.1/pycufsm/cutwp.py`

 * *Files identical despite different names*

### Comparing `pycufsm-0.1.0/pycufsm/fsm.py` & `pycufsm-0.1.1/pycufsm/fsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import deepcopy
 from scipy import linalg as spla
 import numpy as np
-import pycufsm.analysis
+from pycufsm.analysis import analysis
 import pycufsm.cfsm
 # from scipy.sparse.linalg import eigs
 # Originally developed for MATLAB by Benjamin Schafer PhD et al
 # Ported to Python by Brooks Smith MEng, PE, CPEng
 #
 # Each function within this file was originally its own separate file.
 # Original MATLAB comments, especially those retaining to authorship or
@@ -70,21 +70,21 @@
     n_nodes = len(nodes)
     curve = []
     shapes = []
     signature = np.zeros((len(lengths), 1))
 
     # CLEAN UP INPUT
     # clean u_j 0's, multiple terms. or out-of-order terms in m_all
-    m_all = pycufsm.analysis.m_sort(m_all)
+    m_all = analysis.m_sort(m_all)
 
     # DETERMINE FLAGS FOR USER CONSTRAINTS AND INTERNAL (AT NODE) B.C.'s
-    bc_flag = pycufsm.analysis.constr_bc_flag(nodes=nodes, constraints=constraints)
+    bc_flag = analysis.constr_bc_flag(nodes=nodes, constraints=constraints)
 
     # GENERATE STRIP WIDTH AND DIRECTION ANGLE
-    el_props = pycufsm.analysis.elem_prop(nodes=nodes, elements=elements)
+    el_props = analysis.elem_prop(nodes=nodes, elements=elements)
 
     # ENABLE cFSM ANALYSIS IF APPLICABLE, AND FIND BASE PROPERTIES
     if sum(gbt_con['glob']) + sum(gbt_con['dist']) \
                 + sum(gbt_con['local']) + sum(gbt_con['other']) > 0:
         # turn on modal classification analysis
         cfsm_analysis = 1
         # set u_p stress to 1.0 for finding kg_global and k_global for axial modes
@@ -163,15 +163,15 @@
             row = int((np.argwhere(props[:, 0] == mat_num)).reshape(1))
             mat = props[row]
             stiff_x = mat[1]
             stiff_y = mat[2]
             nu_x = mat[3]
             nu_y = mat[4]
             bulk = mat[5]
-            k_l = pycufsm.analysis.klocal(
+            k_l = analysis.klocal(
                 stiff_x=stiff_x,
                 stiff_y=stiff_y,
                 nu_x=nu_x,
                 nu_y=nu_y,
                 bulk=bulk,
                 thick=thick,
                 length=length,
@@ -181,26 +181,24 @@
             )
             node_i = int(elem[1])
             node_j = int(elem[2])
 
             # Generate geometric stiffness matrix (kg_local) in local coordinates
             ty_1 = nodes[node_i][7] * thick
             ty_2 = nodes[node_j][7] * thick
-            kg_l = pycufsm.analysis.kglocal(
+            kg_l = analysis.kglocal(
                 length=length, b_strip=b_strip, ty_1=ty_1, ty_2=ty_2, b_c=b_c, m_a=m_a
             )
 
             # Transform k_local and kg_local into global coordinates
             alpha = el_props[j, 2]
-            [k_local, kg_local] = pycufsm.analysis.trans(
-                alpha=alpha, k_local=k_l, kg_local=kg_l, m_a=m_a
-            )
+            [k_local, kg_local] = analysis.trans(alpha=alpha, k_local=k_l, kg_local=kg_l, m_a=m_a)
 
             # Add element contribution of k_local to full matrix k_global and kg_local to kg_global
-            [k_global, kg_global] = pycufsm.analysis.assemble(
+            [k_global, kg_global] = analysis.assemble(
                 k_global=k_global,
                 kg_global=kg_global,
                 k_local=k_local,
                 kg_local=kg_local,
                 node_i=node_i,
                 node_j=node_j,
                 n_nodes=n_nodes,
@@ -219,15 +217,15 @@
                 # Generate spring stiffness matrix (k_s) in local coordinates
                 k_u = spring[3]
                 k_v = spring[4]
                 k_w = spring[5]
                 k_q = spring[6]
                 discrete = spring[8]
                 y_s = spring[9] * length
-                ks_l = pycufsm.analysis.spring_klocal(
+                ks_l = analysis.spring_klocal(
                     k_u=k_u,
                     k_v=k_v,
                     k_w=k_w,
                     k_q=k_q,
                     length=length,
                     b_c=b_c,
                     m_a=m_a,
@@ -249,17 +247,17 @@
                     d_y = y_j - y_i
                     width = np.sqrt(d_x**2 + d_y**2)
                     if width < 1E-10:  # coincident nodes
                         alpha = 0  # use global coordinates for spring
                     else:
                         # local orientation for spring
                         alpha = np.arctan2(d_y, d_x)
-                k_s = pycufsm.analysis.spring_trans(alpha=alpha, k_s=ks_l, m_a=m_a)
+                k_s = analysis.spring_trans(alpha=alpha, k_s=ks_l, m_a=m_a)
                 # Add element contribution of k_s to full matrix k_global
-                k_global = pycufsm.analysis.spring_assemble(
+                k_global = analysis.spring_assemble(
                     k_global=k_global,
                     k_local=k_s,
                     node_i=node_i,
                     node_j=node_j,
                     n_nodes=n_nodes,
                     m_a=m_a
                 )
```

### Comparing `pycufsm-0.1.0/pycufsm/helpers.py` & `pycufsm-0.1.1/pycufsm/helpers.py`

 * *Files identical despite different names*

### Comparing `pycufsm-0.1.0/pycufsm/plotters.py` & `pycufsm-0.1.1/pycufsm/plotters.py`

 * *Files identical despite different names*

### Comparing `pycufsm-0.1.0/pycufsm/preprocess.py` & `pycufsm-0.1.1/pycufsm/preprocess.py`

 * *Files identical despite different names*

### Comparing `pycufsm-0.1.0/pycufsm.egg-info/PKG-INFO` & `pycufsm-0.1.1/pycufsm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycufsm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python CUFSM (Constrained and Unconstrained Finite Strip Method)
 Author-email: Brooks Smith <smith120bh@gmail.com>
 License: AFL-3.0
 Project-URL: Homepage, https://github.com/ClearCalcs/pyCUFSM
 Project-URL: Documentation, https://github.com/ClearCalcs/pyCUFSM/wiki
 Keywords: CUFSM,CFS,thin-walled,cold-formed steel,aluminium,structural engineering,structural analysis
 Classifier: Topic :: Scientific/Engineering
@@ -23,37 +23,40 @@
 Provides-Extra: jupyter
 License-File: LICENSE
 
 # pyCUFSM
 
 ## Description
 
-This is a port of the analysis portions of CUFSM v5.01, written by Benjamin Schafer PhD et al at Johns Hopkins University, from its original MATLAB language to Python v3, using the Numpy and Scipy packages for matrix manipulation and other advanced mathematics functionality. The goal of this project is to create a derivative of CUFSM which can be used in cloud-based applications. This project is not affiliated with Benjamin Schafer PhD or Johns Hopkins University in any way.
+This package is primarily a port of CUFSM v5.01, written by Benjamin Schafer PhD et al at Johns Hopkins University, from its original MATLAB language to Python v3, using the Numpy and Scipy packages for matrix manipulation and other advanced mathematics functionality. The goal of this project is to create a derivative of CUFSM which can be used either in Jupyter Notebooks or in headless (library) applications. This project is not affiliated with Benjamin Schafer PhD or Johns Hopkins University in any way.
 
-The original MATLAB CUFSM program may be accessed at the following address: https://www.ce.jhu.edu/bschafer/cufsm/
+The original MATLAB CUFSM program may be accessed at the following address: https://www.ce.jhu.edu/cufsm/
 
 ### Installation
 
-This package is still under check and development in its alpha state, therefore it has not yet been published to the Python's PyPI repository. Users may install clone and install the package on their systems using relevant codes the same as printed bellow:
+This package is still under heavy development, but it may be installed in several different possible forms, as described below:
+1. Minimal (headless) installation: `pip install pycufsm`
+2. Installation with plotting capabilities: `pip install pycufsm[plot]`
+3. Installation with Jupyter Notebooks: `pip install pycufsm[jupyter]`
+4. Installation with full development dependencies: `pip install pycufsm[dev]`
 
-`python -m pip install git+https://github.com/ClearCalcs/pyCUFSM.git`
+### Contributing
 
-### Limitations
-
--   **No GUI** - While the MATLAB version of CUFSM contains a full graphical user interface, I will be making no effort in this project to create anything more than a basic command-line interface (though other contributions will be welcome). I anticipate that users of this package will have their own user interface and that this package will function as something of a plug-in.
--   **No CUTWP** - The MATLAB version of CUFSM makes use of CUTWP code for calculating section properties (A, I, J, etc). There are already several mature, open-source Python section properties calculators available, and CUTWP is inherently less accurate because it is based upon section centerline calculations only. As such, I have no plans to port the CUTWP code and anticipate that users of this package will make use of other section properties calculators instead.
+If you would like to contribute to the pyCUFSM project, then please do - all productive contributions are welcome! However, please make sure that you're working off of the most recent development version of the pyCUFSM code, by cloning the [GitHub repository](https://github.com/ClearCalcs/pyCUFSM), and please review our wiki article on [Contributing to the Code](https://github.com/ClearCalcs/pyCUFSM/wiki/Contributing-to-the-Code).
 
 ## Current Status
 
 #### Complete and Generally Tested
 
 -   [x] Unconstrained FSM (signature curve generation)
 -   [x] Constrained FSM
 -   [x] Added template_path() function to define a complete arbitrary cross-section by simple paths
 -   [x] Add automated validation testing of FSM calculations via pytest
+-   [x] Various efficiency and readability improvements:
+    -   [x] Cythonise a few computation-heavy functions in analysis.py, including klocal(), kglocal(), and assemble()
 
 #### Complete But Untested
 
 -   [x] Equation constraints
 -   [x] Spring constraints
 -   [x] General boundary conditions
 
@@ -66,10 +69,10 @@
     -   [ ] Eliminate matrix columns which are nothing more than the index number of the row
     -   [ ] Review code for places where matrices can be preallocated rather than concatenated together
     -   [ ] Review code for function calls that are unnecessarily repeated (a couple of these have already been addressed, e.g. `base_properties()` did not need to be re-run for every half wavelength)
 -   [ ] Write API-style documentation (for now, generally refer to MATLAB CUFSM documentation and/or comments)
 
 ## Disclaimer
 
-While the original MATLAB CUFSM has been extensively tested, and best efforts have been made to check accuracy of this package against the original MATLAB CUFSM program, no warrant is made as to the accuracy of this package. The developers accept no liability for any errors or inaccuracies in this package, including, but not limited to, any problems which may stem from such errors or inaccuracies in this package such as under-conservative engineering designs or structural failures.
+While the original MATLAB CUFSM has been extensively tested, and best efforts have been made to check accuracy of this package against the original MATLAB CUFSM program, including via automated validation testing, no warrant is made as to the accuracy of this package. The developers accept no liability for any errors or inaccuracies in this package, including, but not limited to, any problems which may stem from such errors or inaccuracies in this package such as under-conservative engineering designs or structural failures.
 
 Always check your designs and never blindly trust any engineering program, including this one.
```

### Comparing `pycufsm-0.1.0/pyproject.toml` & `pycufsm-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.0", "cython"]
+requires = ["setuptools>=61.0", "cython", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycufsm"
 authors = [
     {name = "Brooks Smith", email = "smith120bh@gmail.com"}
 ]
@@ -38,14 +38,18 @@
 "Homepage" = "https://github.com/ClearCalcs/pyCUFSM"
 "Documentation" = "https://github.com/ClearCalcs/pyCUFSM/wiki"
 
 [tool.setuptools]
 packages = [
     "pycufsm",
 ]
+py-modules = ["_custom_build"]
+
+[tool.setuptools.cmdclass]
+build_py = "_custom_build.build_py"
 
 [tool.pylint.messages_control]
 disable = [
     "R",
     "missing-docstring",
     "too-many-lines",
     "bad-continuation",
```

### Comparing `pycufsm-0.1.0/tests/test_e2e.py` & `pycufsm-0.1.1/tests/test_e2e.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     )
     lengths = list(cufsm_input["lengths"])
     return lengths, mat["curve"], sect_props_cutwp, signature, curve, shapes
 
 
 def describe_end_to_end_tests():
 
-    @pspec_context("End-to-End Tests (i.e. original unittest tests)")
+    @pspec_context("End-to-End Tests")
     def describe():
         pass
 
     def context_example_1():
 
         @pspec_context("Example 1")
         def describe():
@@ -58,15 +58,15 @@
                 4.75, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 22, 24, 26, 28, 30,
                 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 66, 72, 78, 84, 90, 96,
                 102, 108, 114, 120, 132, 144, 156, 168, 180, 204, 228, 252, 276, 300
             ]
 
     def context_dsm_3_2_1_c_with_lips_Mx():
 
-        @pspec_context("DSM Guide Jan 2006, Ex 3.2.1")
+        @pspec_context("DSM Guide Jan 2006, Ex 3.2.1: C-Section with Lips (Mx)")
         def describe():
             pass
 
         lengths, expected_curve, sect_props, signature, curve, _ = mat_file_test("cwlip_Mx.mat")
 
         expected = {"xcrl": 5, "Mcrl": 0.67, "xcrd": 26.6, "Mcrd": 0.85, "A": 0.880, "Ixx": 10.285}
 
@@ -79,15 +79,15 @@
             assert signature[lengths.index(expected["xcrd"])] == approx(expected["Mcrd"], abs=0.01)
 
         def it_results_in_correct_signature_curve():
             assert np.allclose(expected_curve[:, 1, 0], curve[:, 0], rtol=1.e-4)
 
     def context_dsm_3_2_1_c_with_lips_P():
 
-        @pspec_context("DSM Guide Jan 2006, Ex 3.2.1")
+        @pspec_context("DSM Guide Jan 2006, Ex 3.2.1: C-Section with Lips (P)")
         def describe():
             pass
 
         lengths, expected_curve, sect_props, signature, curve, _ = mat_file_test("cwlip_P.mat")
 
         expected = {
             "xcrl": 6.6,
@@ -107,15 +107,15 @@
             assert signature[lengths.index(expected["xcrd"])] == approx(expected["Pcrd"], abs=0.01)
 
         def it_results_in_correct_signature_curve():
             assert np.allclose(expected_curve[:, 1, 0], curve[:, 0], rtol=1.e-4)
 
     def context_dsm_3_2_2_c_with_lips_modified_Mx():
 
-        @pspec_context("DSM Guide Jan 2006, Ex 3.2.2")
+        @pspec_context("DSM Guide Jan 2006, Ex 3.2.2: Modified C-Section with Lips (Mx)")
         def describe():
             pass
 
         lengths, expected_curve, sect_props, signature, curve, _ = mat_file_test(
             "cwlip_modified_Mx.mat"
         )
 
@@ -133,19 +133,19 @@
             assert expected["Ixx"] == approx(sect_props["Ixx"], abs=0.001)
 
         def it_results_in_correct_Mcr():
             assert signature[lengths.index(expected["xcrl"])] == approx(expected["Mcrl"], abs=0.01)
             assert signature[lengths.index(expected["xcrd"])] == approx(expected["Mcrd"], abs=0.01)
 
         def it_results_in_correct_signature_curve():
-            assert np.allclose(expected_curve[:, 1, 0], curve[:, 0], rtol=1.e-4)
+            assert np.allclose(expected_curve[:, 1, 0], curve[:, 0], rtol=1.e-3)
 
     def context_dsm_3_2_2_c_with_lips_modified_P():
 
-        @pspec_context("DSM Guide Jan 2006, Ex 3.2.2")
+        @pspec_context("DSM Guide Jan 2006, Ex 3.2.2: Modified C-Section with Lips (P)")
         def describe():
             pass
 
         lengths, expected_curve, sect_props, signature, curve, _ = mat_file_test(
             "cwlip_modified_P.mat"
         )
 
@@ -167,15 +167,15 @@
             assert signature[lengths.index(expected["xcrd"])] == approx(expected["Pcrd"], abs=0.01)
 
         def it_results_in_correct_signature_curve():
             assert np.allclose(expected_curve[:, 1, 0], curve[:, 0], rtol=1.e-4)
 
     def context_dsm_3_2_5_z_with_lips_Mx():
 
-        @pspec_context("DSM Guide Jan 2006, Ex 3.2.2")
+        @pspec_context("DSM Guide Jan 2006, Ex 3.2.2: Z-Section with Lips (Mx)")
         def describe():
             pass
 
         lengths, expected_curve, sect_props, signature, curve, _ = mat_file_test("zwlip_Mxr.mat")
 
         expected = {"xcrl": 4.1, "Mcrl": 0.85, "xcrd": 22.1, "Mcrd": 0.77, "A": 0.822, "Ixx": 7.762}
 
@@ -189,15 +189,15 @@
 
         def it_results_in_correct_signature_curve():
             # TODO: Investigate why the signature curve starts mismatching at the tail end...
             assert np.allclose(expected_curve[0:-10, 1, 0], curve[0:-10, 0], rtol=1.e-3)
 
     def context_dsm_3_2_5_z_with_lips_P():
 
-        @pspec_context("DSM Guide Jan 2006, Ex 3.2.2")
+        @pspec_context("DSM Guide Jan 2006, Ex 3.2.2: Z-Section with Lips (P)")
         def describe():
             pass
 
         lengths, expected_curve, sect_props, signature, curve, _ = mat_file_test("zwlip_P.mat")
 
         expected = {"xcrl": 5.9, "Pcrl": 0.16, "xcrd": 18.3, "Pcrd": 0.29, "A": 0.822, "Ixx": 7.762}
```

