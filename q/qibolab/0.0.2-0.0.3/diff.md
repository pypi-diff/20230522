# Comparing `tmp/qibolab-0.0.2.tar.gz` & `tmp/qibolab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibolab-0.0.2.tar", last modified: Sat Mar 18 10:12:00 2023, max compression
+gzip compressed data, was "qibolab-0.0.3.tar", max compression
```

## Comparing `qibolab-0.0.2.tar` & `qibolab-0.0.3.tar`

### file list

```diff
@@ -1,60 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:12:00.121435 qibolab-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-18 10:11:57.000000 qibolab-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-03-18 10:12:00.121435 qibolab-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-18 10:11:57.000000 qibolab-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-18 10:11:57.000000 qibolab-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 10:12:00.121435 qibolab-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-18 10:11:57.000000 qibolab-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:12:00.117435 qibolab-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:12:00.117435 qibolab-0.0.2/src/qibolab/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:12:00.121435 qibolab-0.0.2/src/qibolab/designs/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/designs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/designs/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/designs/design.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:12:00.121435 qibolab-0.0.2/src/qibolab/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/dummy_oscillator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/icarusq.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/icarusqfpga.py
--rw-r--r--   0 runner    (1001) docker     (123)   148469 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/qblox.py
--rw-r--r--   0 runner    (1001) docker     (123)    34053 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/qm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/qmsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/qutech.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/instruments/rohde_schwarz.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:12:00.121435 qibolab-0.0.2/src/qibolab/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/platforms/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/platforms/icplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/platforms/multiqubit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/platforms/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)    64427 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/pulses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:12:00.121435 qibolab-0.0.2/src/qibolab/runcards/
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/runcards/dummy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/runcards/icarusq.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/runcards/multiqubit_icarusq.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/runcards/multiqubit_icarusqfpga.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/runcards/qili1q_os2.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/runcards/qw5q_gold.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/sweeper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19598 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/symbolic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:12:00.121435 qibolab-0.0.2/src/qibolab/transpilers/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/transpilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/transpilers/connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/transpilers/gate_decompositions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/transpilers/general_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/transpilers/transpile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-03-18 10:11:57.000000 qibolab-0.0.2/src/qibolab/transpilers/unitary_decompositions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 10:12:00.121435 qibolab-0.0.2/src/qibolab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-03-18 10:12:00.000000 qibolab-0.0.2/src/qibolab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-18 10:12:00.000000 qibolab-0.0.2/src/qibolab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 10:12:00.000000 qibolab-0.0.2/src/qibolab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 10:12:00.000000 qibolab-0.0.2/src/qibolab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-18 10:12:00.000000 qibolab-0.0.2/src/qibolab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-18 10:12:00.000000 qibolab-0.0.2/src/qibolab.egg-info/top_level.txt
+-rw-r--r--   0        0        0      204 2023-05-22 11:44:47.469454 qibolab-0.0.3/.readthedocs.yml
+-rw-r--r--   0        0        0    11357 2023-05-22 11:44:47.469454 qibolab-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3266 2023-05-22 11:44:47.469454 qibolab-0.0.3/README.md
+-rw-r--r--   0        0        0     1992 2023-05-22 11:44:47.529459 qibolab-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/__init__.py
+-rw-r--r--   0        0        0     6327 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/backends.py
+-rw-r--r--   0        0        0      109 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/designs/__init__.py
+-rw-r--r--   0        0        0     4890 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/designs/channels.py
+-rw-r--r--   0        0        0     3021 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/designs/design.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/__init__.py
+-rw-r--r--   0        0        0     2714 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/abstract.py
+-rw-r--r--   0        0        0     7736 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/dummy.py
+-rw-r--r--   0        0        0      726 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/dummy_oscillator.py
+-rw-r--r--   0        0        0     8021 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/erasynth.py
+-rw-r--r--   0        0        0    12572 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/icarusq.py
+-rw-r--r--   0        0        0     9126 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/icarusqfpga.py
+-rw-r--r--   0        0        0   147723 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/qblox.py
+-rw-r--r--   0        0        0    42699 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/qm.py
+-rw-r--r--   0        0        0     2144 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/qmsim.py
+-rw-r--r--   0        0        0     6466 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/qutech.py
+-rw-r--r--   0        0        0    20329 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/rfsoc.py
+-rw-r--r--   0        0        0     5034 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/rohde_schwarz.py
+-rw-r--r--   0        0        0      272 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/paths.py
+-rw-r--r--   0        0        0     9354 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platform.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/__init__.py
+-rw-r--r--   0        0        0    29895 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/abstract.py
+-rw-r--r--   0        0        0     6646 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/icplatform.py
+-rw-r--r--   0        0        0    26191 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/multiqubit.py
+-rw-r--r--   0        0        0     3112 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/platform.py
+-rw-r--r--   0        0        0    68007 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/pulses.py
+-rw-r--r--   0        0        0     3020 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/result.py
+-rw-r--r--   0        0        0     8260 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/dummy.yml
+-rw-r--r--   0        0        0     2057 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/icarusq.yml
+-rw-r--r--   0        0        0     4751 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/multiqubit_icarusq.yml
+-rw-r--r--   0        0        0     4423 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/multiqubit_icarusqfpga.yml
+-rw-r--r--   0        0        0     4033 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/qili1q_os2.yml
+-rw-r--r--   0        0        0     8282 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/qw5q_gold.yml
+-rw-r--r--   0        0        0    15895 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/qw5q_gold_qblox.yml
+-rw-r--r--   0        0        0      946 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/tii1q_b1.yml
+-rw-r--r--   0        0        0     2937 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/sweeper.py
+-rw-r--r--   0        0        0    19979 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/symbolic.py
+-rw-r--r--   0        0        0      311 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/abstract.py
+-rw-r--r--   0        0        0      977 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/fusion.py
+-rw-r--r--   0        0        0    14368 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/gate_decompositions.py
+-rw-r--r--   0        0        0    19396 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/general_connectivity.py
+-rw-r--r--   0        0        0     1932 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/pipeline.py
+-rw-r--r--   0        0        0     6247 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/star_connectivity.py
+-rw-r--r--   0        0        0     8264 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/unitary_decompositions.py
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 qibolab-0.0.3/PKG-INFO
```

### Comparing `qibolab-0.0.2/LICENSE` & `qibolab-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/PKG-INFO` & `qibolab-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: qibolab
-Version: 0.0.2
+Version: 0.0.3
 Summary: Quantum hardware module and drivers for Qibo
-Home-page: https://github.com/qiboteam/qibolab
+Home-page: https://qibo.science/
+License: Apache-2.0
 Author: The Qibo team
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8.0
+Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
+Requires-Dist: networkx (>=3.0,<4.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: qibo (>=0.1.12,<0.2.0)
+Project-URL: Documentation, https://qibo.science/docs/qibolab/stable
+Project-URL: Repository, https://github.com/qiboteam/qibolab/
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: analysis
-Provides-Extra: tiiq
-License-File: LICENSE
 
 # Qibolab
 
 ![Tests](https://github.com/qiboteam/qibolab/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/qiboteam/qibolab/branch/main/graph/badge.svg?token=11UENAPBPH)](https://codecov.io/gh/qiboteam/qibolab)
 [![Documentation Status](https://readthedocs.org/projects/qibolab/badge/?version=latest)](https://qibolab.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/241307936.svg)](https://zenodo.org/badge/latestdoi/241307936)
@@ -117,8 +121,7 @@
 ## Citation policy
 
 If you use the package please cite the following references:
 - https://arxiv.org/abs/2009.01845
 - https://doi.org/10.5281/zenodo.3997194
 - DOI paper and zenodo
 
-
```

### Comparing `qibolab-0.0.2/README.md` & `qibolab-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/backends.py` & `qibolab-0.0.3/src/qibolab/backends.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from qibo.backends import NumpyBackend
 from qibo.config import log, raise_error
 from qibo.states import CircuitResult
 
 from qibolab import __version__ as qibolab_version
 from qibolab.platform import Platform
 from qibolab.platforms.abstract import AbstractPlatform
-from qibolab.transpilers import can_execute, transpile
+from qibolab.transpilers import Pipeline
 
 
 class QibolabBackend(NumpyBackend):
     def __init__(self, platform, runcard=None):
         super().__init__()
         self.name = "qibolab"
         if isinstance(platform, AbstractPlatform):
@@ -22,14 +22,15 @@
         else:
             self.platform = Platform(platform, runcard)
         self.versions = {
             "qibo": qibo_version,
             "numpy": self.np.__version__,
             "qibolab": qibolab_version,
         }
+        self.transpiler = Pipeline.default(self.platform.two_qubit_natives)
 
     def apply_gate(self, gate, state, nqubits):  # pragma: no cover
         raise_error(NotImplementedError, "Qibolab cannot apply gates directly.")
 
     def apply_gate_density_matrix(self, gate, state, nqubits):  # pragma: no cover
         raise_error(NotImplementedError, "Qibolab cannot apply gates directly.")
 
@@ -62,28 +63,22 @@
             )
         elif initial_state is not None:
             raise_error(
                 ValueError,
                 "Hardware backend only supports circuits as initial states.",
             )
 
-        two_qubit_natives = self.platform.two_qubit_natives
-        if can_execute(circuit, two_qubit_natives, verbose=False):
+        if self.transpiler is None or self.transpiler.is_satisfied(circuit):
             native_circuit = circuit
         else:
             # Transform a circuit into proper connectivity and native gates
-            log.info("Transpiling circuit.")
-            native_circuit, _ = transpile(circuit, two_qubit_natives)
+            native_circuit, qubit_map = self.transpiler.transpile(circuit)
+            # TODO: Use the qubit map to properly map measurements
             if check_transpiled:
-                backend = NumpyBackend()
-                target_state = backend.execute_circuit(circuit).state()
-                final_state = backend.execute_circuit(native_circuit).state()
-                fidelity = np.abs(np.dot(np.conj(target_state), final_state))
-                np.testing.assert_allclose(fidelity, 1.0)
-                log.info("Transpiler test passed.")
+                self.transpiler.check_execution(circuit, native_circuit)
 
         # Transpile the native circuit into a sequence of pulses ``PulseSequence``
         sequence = self.platform.transpile(native_circuit)
 
         if not self.platform.is_connected:
             self.platform.connect()
             self.platform.setup()
```

### Comparing `qibolab-0.0.2/src/qibolab/designs/channels.py` & `qibolab-0.0.3/src/qibolab/designs/channels.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,28 +2,38 @@
 from typing import List, Optional
 
 from qibo.config import raise_error
 
 from qibolab.instruments.abstract import LocalOscillator
 
 
+def check_max_bias(bias, max_bias):
+    """Checks if a given bias value exceeds the maximum supported bias.
+
+    This is to avoid sending high currents that could damage lab equipment
+    such as amplifiers.
+    """
+    if max_bias is not None and abs(bias) > max_bias:
+        raise_error(ValueError, f"{bias} exceeds the maximum allowed bias {max_bias}.")
+
+
 @dataclass
 class Channel:
     """Representation of physical wire connection (channel)."""
 
     name: str
     """Name of the channel from the lab schematics."""
 
     qubit: Optional["Qubit"] = field(default=None, repr=False)
     """Qubit connected to this channel.
     Used to read the sweetspot and filters for flux channels only. ``None`` for non-flux channels.
     """
     ports: List[tuple] = field(default_factory=list)
     """List of tuples (controller, port) connected to this channel."""
-    local_oscillator: Optional[LocalOscillator] = None
+    _local_oscillator: Optional[LocalOscillator] = None
     """Instrument object controlling the local oscillator connected to this channel.
     Not applicable for setups that do not use local oscillators because the controller
     can send sufficiently high frequencies
     """
     _bias: Optional[float] = None
     """DC offset that should be applied in the channel in order to shift the
     frequency of the qubit, usually to put it in its sweetspot.
@@ -31,27 +41,49 @@
     """
     _filter: Optional[dict] = None
     """Filter to be applied to the channel to reduce the distortions when sending
     flux pulses. Useful for two-qubit gates.
     Quantum Machines associate filters to channels but this may not be the case
     in other instruments.
     """
+    max_bias: Optional[float] = None
+    """Maximum voltage that we can send for flux bias without damaging amplifiers.
+    If the user attempts to send a higher value the platform will raise an error
+    to avoid the operation of being executed in the real instruments.
+    """
+
+    @property
+    def local_oscillator(self):
+        """LocalOscillator object connnected to this channel."""
+        if self._local_oscillator is None:
+            raise_error(NotImplementedError, f"Channel {self.name} does not have a local oscillator")
+        return self._local_oscillator
+
+    @local_oscillator.setter
+    def local_oscillator(self, local_oscillator):
+        if not isinstance(local_oscillator, LocalOscillator):
+            raise_error(TypeError, "Attempting to set LocalOscillator failed.")
+        self._local_oscillator = local_oscillator
 
     @property
     def bias(self):
         """Bias offset for flux channels."""
         if self._bias is None:
+            if self.qubit.flux is None:
+                raise_error(NotImplementedError, f"Channel {self.name} is not connected to a flux qubit")
             # operate qubits at their sweetspot unless otherwise stated
+            check_max_bias(self.qubit.sweetspot, self.max_bias)
             return self.qubit.sweetspot
         return self._bias
 
     @bias.setter
     def bias(self, bias):
         if not isinstance(bias, (int, float)):
             raise_error(TypeError, f"Attempting to set non-float bias {bias}.")
+        check_max_bias(bias, self.max_bias)
         self._bias = bias
 
     @property
     def filter(self):
         """Filters for sending flux pulses through a flux channel."""
         if self._filter is None:
             return self.qubit.filter
```

### Comparing `qibolab-0.0.2/src/qibolab/designs/design.py` & `qibolab-0.0.3/src/qibolab/designs/design.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/instruments/abstract.py` & `qibolab-0.0.3/src/qibolab/instruments/abstract.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/instruments/dummy.py` & `qibolab-0.0.3/src/qibolab/instruments/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
     def stop(self):
         log.info("Stopping dummy instrument.")
 
     def disconnect(self):
         log.info("Disconnecting dummy instrument.")
 
-    def play(self, qubits, sequence, nshots, relaxation_time):
-        time.sleep(relaxation_time)
+    def play(self, qubits, sequence, nshots, relaxation_time, raw_adc=False):
+        time.sleep(relaxation_time * 1e-9)
 
         ro_pulses = {pulse.qubit: pulse.serial for pulse in sequence.ro_pulses}
 
         results = {}
         for qubit, serial in ro_pulses.items():
             i = np.random.rand(nshots)
             q = np.random.rand(nshots)
@@ -118,45 +118,43 @@
                     results=results,
                     sweeper_pulses=sweeper_pulses,
                     map_original_shifted=map_original_shifted
                 )
             else:
                 new_sequence = copy.deepcopy(sequence)
                 result = self.play(qubits, new_sequence, nshots, relaxation_time)
+
                 # colllect result and append to original pulse
                 for original_pulse, new_serial in map_original_shifted.items():
-                    acquisition = result[new_serial].compute_average() if average else result[new_serial]
-
-                    if results:
+                    acquisition = result[new_serial].average if average else result[new_serial]
+                    if original_pulse.serial in results:
                         results[original_pulse.serial] += acquisition
                         results[original_pulse.qubit] += acquisition
                     else:
                         results[original_pulse.serial] = acquisition
                         results[original_pulse.qubit] = copy.copy(results[original_pulse.serial])
-
         # restore initial value of the pulse
         if sweeper.pulses is not None:
             self._restore_initial_value(sweeper, sweeper_pulses, original_value)
 
     def _save_original_value(self, sweeper, sweeper_pulses):
         """Helper method for _sweep_recursion"""
         original_value = {}
         pulses = sweeper_pulses[sweeper.parameter]
         # save original value of the parameter swept
         for pulse in pulses:
-            if sweeper.parameter not in [Parameter.attenuation, Parameter.gain, Parameter.bias]:
+            if sweeper.parameter not in [Parameter.attenuation, Parameter.gain, Parameter.bias, Parameter.delay]:
                 original_value[pulse] = getattr(pulses[pulse], sweeper.parameter.name)
-
         return original_value
 
     def _restore_initial_value(self, sweeper, sweeper_pulses, original_value):
         """Helper method for _sweep_recursion"""
         pulses = sweeper_pulses[sweeper.parameter]
         for pulse in pulses:
-            if sweeper.parameter not in [Parameter.attenuation, Parameter.gain, Parameter.bias]:
+            if sweeper.parameter not in [Parameter.attenuation, Parameter.gain, Parameter.bias, Parameter.delay]:
                 setattr(pulses[pulse], sweeper.parameter.name, original_value[pulse])
 
     def _update_pulse_sequence_parameters(
         self, qubits, sweeper, sweeper_pulses, original_sequence, map_original_shifted, value
     ):
         """Helper method for _sweep_recursion"""
         if sweeper.pulses is not None:
@@ -167,14 +165,16 @@
                         value += qubits[pulses[pulse].qubit].readout_frequency
                     else:
                         value += qubits[pulses[pulse].qubit].drive_frequency
                     setattr(pulses[pulse], sweeper.parameter.name, value)
                 elif sweeper.parameter is Parameter.amplitude:
                     current_amplitude = pulses[pulse].amplitude
                     setattr(pulses[pulse], sweeper.parameter.name, float(current_amplitude * value))
+                elif sweeper.parameter is Parameter.delay:
+                    pulses[pulse].start += value
                 else:
                     setattr(pulses[pulse], sweeper.parameter.name, value)
                 if pulses[pulse].type is PulseType.READOUT:
                     to_modify = [
                         pulse1 for pulse1 in original_sequence.ro_pulses if pulse1.qubit == pulses[pulse].qubit
                     ]
                     if to_modify:
```

### Comparing `qibolab-0.0.2/src/qibolab/instruments/dummy_oscillator.py` & `qibolab-0.0.3/src/qibolab/instruments/dummy_oscillator.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/instruments/icarusq.py` & `qibolab-0.0.3/src/qibolab/instruments/icarusq.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/instruments/icarusqfpga.py` & `qibolab-0.0.3/src/qibolab/instruments/icarusqfpga.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/instruments/qblox.py` & `qibolab-0.0.3/src/qibolab/instruments/qblox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Qblox instruments driver.
 
 Supports the following Instruments:
     Cluster
     Cluster QRM-RF
     Cluster QCM-RF
-Compatible with qblox-instruments driver 0.7.0 (8/8/2022).
+Compatible with qblox-instruments driver 0.9.0 (28/2/2023).
 It does not support the operation of multiple clusters symultaneously.
 https://qblox-qblox-instruments.readthedocs-hosted.com/en/master/
 """
 
 import json
 
 import numpy as np
@@ -369,15 +369,15 @@
         Sequencer 1 to 6 are used as needed to sinthesise simultaneous pulses on the same channel
         or when the memory of the default sequencers rans out.
 
     """
 
     DEFAULT_SEQUENCERS: dict = {"o1": 0, "i1": 0}
     SAMPLING_RATE: int = 1e9  # 1 GSPS
-    FREQUENCY_LIMIT = 300e6
+    FREQUENCY_LIMIT = 500e6
 
     property_wrapper = lambda parent, *parameter: property(
         lambda self: parent.device.get(parameter[0]),
         lambda self, x: parent._set_device_parameter(parent.device, *parameter, value=x),
     )
     property_wrapper.__doc__ = """A lambda function used to create properties that wrap around the device parameters and
     caches their value using `_set_device_parameter()`.
@@ -626,38 +626,40 @@
             Exception = If attempting to set a parameter without a connection to the instrument.
         """
 
         # select a new sequencer and configure it as required
         next_sequencer_number = self._free_sequencers_numbers.pop(0)
         if next_sequencer_number != self.DEFAULT_SEQUENCERS[port]:
             for parameter in self.device.sequencers[self.DEFAULT_SEQUENCERS[port]].parameters:
-                value = self.device.sequencers[self.DEFAULT_SEQUENCERS[port]].get(param_name=parameter)
-                if not value is None:
-                    target = self.device.sequencers[next_sequencer_number]
-                    self._set_device_parameter(target, parameter, value=value)
+                # exclude read-only parameter `sequence` and others that have wrong default values (qblox bug)
+                if not parameter in ["sequence", "thresholded_acq_marker_address", "thresholded_acq_trigger_address"]:
+                    value = self.device.sequencers[self.DEFAULT_SEQUENCERS[port]].get(param_name=parameter)
+                    if value:
+                        target = self.device.sequencers[next_sequencer_number]
+                        self._set_device_parameter(target, parameter, value=value)
 
         # if hardware demodulation is enabled, configure nco_frequency and classification parameters
         if self.ports["i1"].hardware_demod_en or self.ports["o1"].hardware_mod_en:
             self._set_device_parameter(
                 self.device.sequencers[next_sequencer_number],
                 "nco_freq",
                 value=frequency,  # Assumes all pulses in non_overlapping_pulses set
                 # have the same frequency. Non-overlapping pulses of different frequencies on the same
                 # qubit channel with hardware_demod_en would lead to wrong results.
                 # TODO: Throw error in that event or implement for non_overlapping_same_frequency_pulses
             )
         if self.ports["i1"].hardware_demod_en and qubit in self.classification_parameters:
             self._set_device_parameter(
                 self.device.sequencers[next_sequencer_number],
-                "phase_rotation_acq",
+                "thresholded_acq_rotation",
                 value=self.classification_parameters[qubit]["rotation_angle"],
             )
             self._set_device_parameter(
                 self.device.sequencers[next_sequencer_number],
-                "discretization_threshold_acq",
+                "thresholded_acq_threshold",
                 value=self.classification_parameters[qubit]["threshold"] * self.acquisition_duration,
             )
         # create sequencer wrapper
         sequencer = Sequencer(next_sequencer_number)
         # add the sequencer to the list of sequencers required by the port
         self._sequencers[port].append(sequencer)
         return sequencer
@@ -861,22 +863,17 @@
                     body += initial_wait_instruction
 
                     for n in range(pulses.count):
                         if (self.ports["i1"].hardware_demod_en or self.ports["o1"].hardware_mod_en) and pulses[
                             n
                         ].relative_phase != 0:
                             # Set phase
-                            p = 10
                             phase = (pulses[n].relative_phase * 360 / (2 * np.pi)) % 360
-                            coarse = int(round(phase / 0.9, p))
-                            fine = int(round((phase - coarse * 0.9) / 2.25e-3, p))
-                            ultra_fine = int(round((phase - coarse * 0.9 - fine * 2.25e-3) / 3.6e-7, p))
-                            error = abs(phase - coarse * 0.9 - fine * 2.25e-3 - ultra_fine * 3.6e-7)
-                            assert error < 3.6e-7
-                            set_ph_instruction = f"                    set_ph {coarse}, {fine}, {ultra_fine}"
+                            phase = int(phase / 360 * 1e9)
+                            set_ph_instruction = f"                    set_ph {phase}"
                             set_ph_instruction += (
                                 " " * (45 - len(set_ph_instruction))
                                 + f"# set relative phase {pulses[n].relative_phase} rads"
                             )
                             body += "\n" + set_ph_instruction
                         if pulses[n].type == PulseType.READOUT:
                             delay_after_play = self.acquisition_hold_off
@@ -1694,18 +1691,20 @@
             Exception = If attempting to set a parameter without a connection to the instrument.
         """
 
         # select a new sequencer and configure it as required
         next_sequencer_number = self._free_sequencers_numbers.pop(0)
         if next_sequencer_number != self.DEFAULT_SEQUENCERS[port]:
             for parameter in self.device.sequencers[self.DEFAULT_SEQUENCERS[port]].parameters:
-                value = self.device.sequencers[self.DEFAULT_SEQUENCERS[port]].get(param_name=parameter)
-                if not value is None:
-                    target = self.device.sequencers[next_sequencer_number]
-                    self._set_device_parameter(target, parameter, value=value)
+                # exclude read-only parameter `sequence`
+                if not parameter in ["sequence"]:
+                    value = self.device.sequencers[self.DEFAULT_SEQUENCERS[port]].get(param_name=parameter)
+                    if value:
+                        target = self.device.sequencers[next_sequencer_number]
+                        self._set_device_parameter(target, parameter, value=value)
 
         # if hardware modulation is enabled configure nco_frequency
         if self.ports[port].hardware_mod_en:
             self._set_device_parameter(
                 self.device.sequencers[next_sequencer_number],
                 "nco_freq",
                 value=frequency,  # Assumes all pulses in non_overlapping_pulses set
@@ -1926,22 +1925,17 @@
 
                         if delay_after_play < minimum_delay_between_instructions:
                             raise Exception(
                                 f"The minimum delay between pulses is {minimum_delay_between_instructions}ns."
                             )
                         if self.ports[port].hardware_mod_en and pulses[n].relative_phase != 0:
                             # Set phase
-                            p = 10
                             phase = (pulses[n].relative_phase * 360 / (2 * np.pi)) % 360
-                            coarse = int(round(phase / 0.9, p))
-                            fine = int(round((phase - coarse * 0.9) / 2.25e-3, p))
-                            ultra_fine = int(round((phase - coarse * 0.9 - fine * 2.25e-3) / 3.6e-7, p))
-                            error = abs(phase - coarse * 0.9 - fine * 2.25e-3 - ultra_fine * 3.6e-7)
-                            assert error < 3.6e-7
-                            set_ph_instruction = f"                    set_ph {coarse}, {fine}, {ultra_fine}"
+                            phase = int(phase / 360 * 1e9)
+                            set_ph_instruction = f"                    set_ph {phase}"
                             set_ph_instruction += (
                                 " " * (45 - len(set_ph_instruction))
                                 + f"# set relative phase {pulses[n].relative_phase} rads"
                             )
                             body += "\n" + set_ph_instruction
 
                         # Prepare play instruction: play wave_i_index, wave_q_index, delay_next_instruction
@@ -2398,18 +2392,20 @@
             Exception = If attempting to set a parameter without a connection to the instrument.
         """
 
         # select a new sequencer and configure it as required
         next_sequencer_number = self._free_sequencers_numbers.pop(0)
         if next_sequencer_number != self.DEFAULT_SEQUENCERS[port]:
             for parameter in self.device.sequencers[self.DEFAULT_SEQUENCERS[port]].parameters:
-                value = self.device.sequencers[self.DEFAULT_SEQUENCERS[port]].get(param_name=parameter)
-                if not value is None:
-                    target = self.device.sequencers[next_sequencer_number]
-                    self._set_device_parameter(target, parameter, value=value)
+                # exclude read-only parameter `sequence`
+                if not parameter in ["sequence"]:
+                    value = self.device.sequencers[self.DEFAULT_SEQUENCERS[port]].get(param_name=parameter)
+                    if value:
+                        target = self.device.sequencers[next_sequencer_number]
+                        self._set_device_parameter(target, parameter, value=value)
 
         # if hardware modulation is enabled configure nco_frequency
         if self.ports[port].hardware_mod_en:
             self._set_device_parameter(
                 self.device.sequencers[next_sequencer_number],
                 "nco_freq",
                 value=frequency,  # Assumes all pulses in non_overlapping_pulses set
@@ -2631,22 +2627,17 @@
 
                         if delay_after_play < minimum_delay_between_instructions:
                             raise Exception(
                                 f"The minimum delay between pulses is {minimum_delay_between_instructions}ns."
                             )
                         if self.ports[port].hardware_mod_en and pulses[n].relative_phase != 0:
                             # Set phase
-                            p = 10
                             phase = (pulses[n].relative_phase * 360 / (2 * np.pi)) % 360
-                            coarse = int(round(phase / 0.9, p))
-                            fine = int(round((phase - coarse * 0.9) / 2.25e-3, p))
-                            ultra_fine = int(round((phase - coarse * 0.9 - fine * 2.25e-3) / 3.6e-7, p))
-                            error = abs(phase - coarse * 0.9 - fine * 2.25e-3 - ultra_fine * 3.6e-7)
-                            assert error < 3.6e-7
-                            set_ph_instruction = f"                    set_ph {coarse}, {fine}, {ultra_fine}"
+                            phase = int(phase / 360 * 1e9)
+                            set_ph_instruction = f"                    set_ph {phase}"
                             set_ph_instruction += (
                                 " " * (45 - len(set_ph_instruction))
                                 + f"# set relative phase {pulses[n].relative_phase} rads"
                             )
                             body += "\n" + set_ph_instruction
 
                         # Prepare play instruction: play wave_i_index, wave_q_index, delay_next_instruction
```

### Comparing `qibolab-0.0.2/src/qibolab/instruments/qm.py` & `qibolab-0.0.3/src/qibolab/instruments/qm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import collections
+import math
 from dataclasses import dataclass, field
+from typing import Dict, List, Optional
 
 import numpy as np
 from qibo.config import log, raise_error
+from qm import qua
 from qm.qua import (
     align,
     assign,
     declare,
     declare_stream,
     dual_demod,
     fixed,
     for_,
     frame_rotation_2pi,
     measure,
     play,
     program,
     reset_frame,
     reset_phase,
-    save,
     stream_processing,
     wait,
 )
+from qm.qua._dsl import _ResultSource, _Variable  # for type declaration only
 from qm.QuantumMachinesManager import QuantumMachinesManager
 from qualang_tools.bakery import baking
 from qualang_tools.loops import from_array
+from qualang_tools.units import unit
 
+from qibolab.designs.channels import check_max_bias
 from qibolab.instruments.abstract import AbstractInstrument
 from qibolab.pulses import Pulse, PulseType, Rectangular
-from qibolab.result import ExecutionResults
+from qibolab.result import AveragedResults, ExecutionResults
 from qibolab.sweeper import Parameter
 
 
 @dataclass
 class QMConfig:
     """Configuration for communicating with the ``QuantumMachinesManager``."""
 
@@ -50,17 +55,14 @@
         Args:
             ports (list): List of tuples ``(conX, port)``.
             offset (float): Constant offset to be played in the given ports.
                 Relevant for ports connected to flux channels.
             filter (dict): Pulse shape filters. Relevant for ports connected to flux channels.
                 QM syntax should be followed for the filters.
         """
-        if abs(offset) > 0.2:
-            raise_error(ValueError, f"DC offset for Quantum Machines cannot exceed 0.1V but is {offset}.")
-
         for con, port in ports:
             if con not in self.controllers:
                 self.controllers[con] = {"analog_outputs": {}}
             self.controllers[con]["analog_outputs"][port] = {"offset": offset}
             if filter is not None:
                 self.controllers[con]["analog_outputs"][port]["filter"] = filter
 
@@ -91,15 +93,15 @@
                 will send to this qubit. This frequency will be mixed with the
                 LO connected to the same channel.
         """
         if f"drive{qubit.name}" not in self.elements:
             # register drive controllers
             self.register_analog_output_controllers(qubit.drive.ports)
             # register element
-            lo_frequency = int(qubit.drive.local_oscillator.frequency)
+            lo_frequency = math.floor(qubit.drive.local_oscillator.frequency)
             self.elements[f"drive{qubit.name}"] = {
                 "mixInputs": {
                     "I": qubit.drive.ports[0],
                     "Q": qubit.drive.ports[1],
                     "lo_frequency": lo_frequency,
                     "mixer": f"mixer_drive{qubit.name}",
                 },
@@ -147,15 +149,15 @@
                         1: {},
                     }
                 if "analog_inputs" not in controllers[con]:
                     controllers[con]["analog_inputs"] = {}
                 controllers[con]["analog_inputs"][port] = {"offset": 0.0, "gain_db": 0}
 
             # register element
-            lo_frequency = int(qubit.readout.local_oscillator.frequency)
+            lo_frequency = math.floor(qubit.readout.local_oscillator.frequency)
             self.elements[f"readout{qubit.name}"] = {
                 "mixInputs": {
                     "I": qubit.readout.ports[0],
                     "Q": qubit.readout.ports[1],
                     "lo_frequency": lo_frequency,
                     "mixer": f"mixer_readout{qubit.name}",
                 },
@@ -214,46 +216,46 @@
         Returns:
             element (str): Name of the element this pulse will be played on.
                 Elements are a part of the QM config and are generated during
                 instantiation of the Qubit objects. They are named as
                 "drive0", "drive1", "flux0", "readout0", ...
         """
         if pulse.serial not in self.pulses:
-            if pulse.type.name == "DRIVE":
+            if pulse.type is PulseType.DRIVE:
                 serial_i = self.register_waveform(pulse, "i")
                 serial_q = self.register_waveform(pulse, "q")
                 self.pulses[pulse.serial] = {
                     "operation": "control",
                     "length": pulse.duration,
                     "waveforms": {"I": serial_i, "Q": serial_q},
                 }
                 # register drive element (if it does not already exist)
-                if_frequency = pulse.frequency - int(qubit.drive.local_oscillator.frequency)
+                if_frequency = pulse.frequency - math.floor(qubit.drive.local_oscillator.frequency)
                 self.register_drive_element(qubit, if_frequency)
                 # register flux element (if available)
                 if qubit.flux:
                     self.register_flux_element(qubit)
                 # register drive pulse in elements
                 self.elements[f"drive{qubit.name}"]["operations"][pulse.serial] = pulse.serial
 
-            elif pulse.type.name == "FLUX":
+            elif pulse.type is PulseType.FLUX:
                 serial = self.register_waveform(pulse)
                 self.pulses[pulse.serial] = {
                     "operation": "control",
                     "length": pulse.duration,
                     "waveforms": {
                         "single": serial,
                     },
                 }
                 # register flux element (if it does not already exist)
                 self.register_flux_element(qubit, pulse.frequency)
                 # register flux pulse in elements
                 self.elements[f"flux{qubit.name}"]["operations"][pulse.serial] = pulse.serial
 
-            elif pulse.type.name == "READOUT":
+            elif pulse.type is PulseType.READOUT:
                 serial_i = self.register_waveform(pulse, "i")
                 serial_q = self.register_waveform(pulse, "q")
                 self.register_integration_weights(qubit, pulse.duration)
                 self.pulses[pulse.serial] = {
                     "operation": "measurement",
                     "length": pulse.duration,
                     "waveforms": {
@@ -264,15 +266,15 @@
                         "cos": f"cosine_weights{qubit.name}",
                         "sin": f"sine_weights{qubit.name}",
                         "minus_sin": f"minus_sine_weights{qubit.name}",
                     },
                     "digital_marker": "ON",
                 }
                 # register readout element (if it does not already exist)
-                if_frequency = pulse.frequency - int(qubit.readout.local_oscillator.frequency)
+                if_frequency = pulse.frequency - math.floor(qubit.readout.local_oscillator.frequency)
                 self.register_readout_element(qubit, if_frequency, time_of_flight, smearing)
                 # register flux element (if available)
                 if qubit.flux:
                     self.register_flux_element(qubit)
                 # register readout pulse in elements
                 self.elements[f"readout{qubit.name}"]["operations"][pulse.serial] = pulse.serial
 
@@ -314,68 +316,134 @@
         """Registers integration weights in QM config.
 
         Args:
             qubit (:class:`qibolab.platforms.quantum_machines.Qubit`): Qubit
                 object that the integration weights will be used for.
             readout_len (int): Duration of the readout pulse in ns.
         """
-        rotation_angle = qubit.rotation_angle
+        iq_angle = qubit.iq_angle
         self.integration_weights.update(
             {
                 f"cosine_weights{qubit.name}": {
-                    "cosine": [(np.cos(rotation_angle), readout_len)],
-                    "sine": [(-np.sin(rotation_angle), readout_len)],
+                    "cosine": [(np.cos(iq_angle), readout_len)],
+                    "sine": [(-np.sin(iq_angle), readout_len)],
                 },
                 f"sine_weights{qubit.name}": {
-                    "cosine": [(np.sin(rotation_angle), readout_len)],
-                    "sine": [(np.cos(rotation_angle), readout_len)],
+                    "cosine": [(np.sin(iq_angle), readout_len)],
+                    "sine": [(np.cos(iq_angle), readout_len)],
                 },
                 f"minus_sine_weights{qubit.name}": {
-                    "cosine": [(-np.sin(rotation_angle), readout_len)],
-                    "sine": [(-np.cos(rotation_angle), readout_len)],
+                    "cosine": [(-np.sin(iq_angle), readout_len)],
+                    "sine": [(-np.cos(iq_angle), readout_len)],
                 },
             }
         )
 
 
+@dataclass
+class AcquisitionVariables:
+    """QUA variables used for saving of acquisition results.
+    This class can be instantiated only within a QUA program scope.
+    Each readout pulse is associated with its own set of acquisition variables.
+    """
+
+    I: _Variable = field(default_factory=lambda: declare(fixed))
+    Q: _Variable = field(default_factory=lambda: declare(fixed))
+    """Variables to save the (I, Q) values acquired from a single shot."""
+    I_stream: _ResultSource = field(default_factory=lambda: declare_stream())
+    Q_stream: _ResultSource = field(default_factory=lambda: declare_stream())
+    """Streams to collect the results of all shots."""
+
+    raw_adc: bool = False
+    """Flag to select whether we are acquiring raw ADC data."""
+    adc_stream: Optional[_ResultSource] = None
+    """Stream to collect raw ADC data."""
+
+    threshold: Optional[float] = None
+    """Threshold to be used for classification of single shots."""
+    angle: Optional[float] = None
+    """Angle in the IQ plane to be used for classification of single shots."""
+    shot: Optional[_Variable] = None
+    shots: Optional[_ResultSource] = None
+    """Variable and stream to collect the classified shots.
+    Used only if a threshold and angle is given.
+    """
+
+    def __post_init__(self):
+        """Create QUA variables needed for single shot classification."""
+        if self.raw_adc:
+            self.adc_stream = declare_stream(adc_trace=True)
+
+        if self.threshold is not None and self.angle is not None:
+            self.shot = declare(bool)
+            self.shots = declare_stream()
+            self.cos = np.cos(self.angle)
+            self.sin = np.sin(self.angle)
+
+    def save(self):
+        """QUA instruction to save acquired results from variables to streams."""
+        qua.save(self.I, self.I_stream)
+        qua.save(self.Q, self.Q_stream)
+        if self.shot is not None:
+            qua.save(self.shot, self.shots)
+
+    def classify_shots(self):
+        """QUA instruction to classify shots in real time and save the result to a variable."""
+        if self.threshold is not None and self.angle is not None:
+            assign(self.shot, self.I * self.cos - self.Q * self.sin > self.threshold)
+
+
 class QMPulse:
-    def __init__(self, pulse):
-        self.pulse = pulse
-        self.element = f"{pulse.type.name.lower()}{pulse.qubit}"
-        self.operation = pulse.serial
-        self.relative_phase = pulse.relative_phase / (2 * np.pi)
-        self.duration = pulse.duration
+    """Wrapper around :class:`qibolab.pulses.Pulse` for easier translation to QUA program."""
+
+    def __init__(self, pulse: Pulse):
+        self.pulse: Pulse = pulse
+        """:class:`qibolab.pulses.Pulse` implemting the current pulse."""
+        self.element: str = f"{pulse.type.name.lower()}{pulse.qubit}"
+        """Element that the pulse will be played on, as defined in the QM config."""
+        self.operation: str = pulse.serial
+        """Name of the operation that is implementing the pulse in the QM config."""
+        self.relative_phase: float = pulse.relative_phase / (2 * np.pi)
+        """Relative phase of the pulse normalized to follow QM convention.
+        May be overrident when sweeping phase."""
+        self.duration: int = pulse.duration
+        """Duration of the pulse. May be overrident when sweeping duration."""
+        self.wait_time: int = 0
+        """Time (in clock cycles) to wait before playing this pulse.
+        Calculated and assigned by :meth:`qibolab.instruments.qm.Sequence.add`."""
+        self.wait_time_variable: Optional[_Variable] = None
+        """Time (in clock cycles) to wait before playing this pulse when we are sweeping delay."""
+        self.acquisition: AcquisitionVariables = None
+        """Data class containing the variables required for data acquisition for the instrument."""
+
+        self.next: set = set()
+        """Pulses that will be played after the current pulse.
+        These pulses need to be re-aligned if we are sweeping the delay or duration."""
 
-        # Stores the baking object (for pulses that need 1ns resolution)
         self.baked = None
+        """Baking object implementing the pulse when 1ns resolution is needed."""
         self.baked_amplitude = None
+        """Amplitude of the baked pulse."""
 
-        self.I = None
-        self.Q = None
-        self.shot = None
-        self.I_st = None
-        self.Q_st = None
-        self.shots = None
-        self.threshold = None
-        self.cos = None
-        self.sin = None
-
-    def declare_output(self, threshold=None, iq_angle=None):
-        self.I = declare(fixed)
-        self.Q = declare(fixed)
-        self.I_st = declare_stream()
-        self.Q_st = declare_stream()
+    @property
+    def wait_cycles(self):
+        """Instrument clock cycles (1 cycle = 4ns) to wait before playing the pulse.
+
+        This property will be used in the QUA ``wait`` command, so that it is compatible
+        with and without delay sweepers.
+        """
+        if self.wait_time_variable is not None:
+            return self.wait_time_variable + self.wait_time
+        elif self.wait_time >= 4:
+            return self.wait_time
+        else:
+            return None
 
-        if threshold is not None:
-            # QUA variables used for single shot classification
-            self.shot = declare(bool)
-            self.shots = declare_stream()
-            self.threshold = threshold
-            self.cos = np.cos(iq_angle)
-            self.sin = np.sin(iq_angle)
+    def declare_output(self, threshold=None, angle=None, raw_adc=False):
+        self.acquisition = AcquisitionVariables(threshold=threshold, angle=angle, raw_adc=raw_adc)
 
     def bake(self, config: QMConfig):
         if self.baked is not None:
             raise_error(RuntimeError, f"Bake was already called for {self.pulse}.")
         # ! Only works for flux pulses that have zero Q waveform
 
         # Create the different baked sequences, each one corresponding to a different truncated duration
@@ -393,31 +461,64 @@
             self.baked.play(self.pulse.serial, self.element)
             # Append the baking object in the list to call it from the QUA program
             # self.segments.append(b)
 
         self.duration = self.baked.get_op_length()
 
 
-class QMSequence(list):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        # keep track of readout pulses for registering outputs
-        self.ro_pulses = []
-        # map from qibolab pulses to QMPulses (useful when sweeping)
-        self.pulse_to_qmpulse = {}
+@dataclass
+class Sequence:
+    """Pulse sequence containing QM specific pulses (``qmpulse``).
+    Defined in :meth:`qibolab.instruments.qm.QMOPX.play`.
+    Holds attributes for the ``element`` and ``operation`` that
+    corresponds to each pulse, as defined in the QM config.
+    """
+
+    qmpulses: List[QMPulse] = field(default_factory=list)
+    """List of :class:`qibolab.instruments.qm.QMPulse` objects corresponding to the original pulses."""
+    ro_pulses: List[QMPulse] = field(default_factory=list)
+    """List of readout pulses used for registering outputs."""
+    pulse_to_qmpulse: Dict[Pulse, QMPulse] = field(default_factory=dict)
+    """Map from qibolab pulses to QMPulses (useful when sweeping)."""
+    clock: Dict[str, int] = field(default_factory=lambda: collections.defaultdict(int))
+    """Dictionary used to keep track of times of each element, in order to calculate wait times."""
+    pulse_finish: Dict[int, List[QMPulse]] = field(default_factory=lambda: collections.defaultdict(list))
+    """Map to find all pulses that finish at a given time (useful for ``_find_previous``)."""
+
+    def _find_previous(self, pulse):
+        for finish in reversed(sorted(self.pulse_finish.keys())):
+            if finish <= pulse.start:
+                # first try to find a previous pulse targeting the same qubit
+                last_pulses = self.pulse_finish[finish]
+                for previous in reversed(last_pulses):
+                    if previous.pulse.qubit == pulse.qubit:
+                        return previous
+        return None
 
-    def add(self, pulse):
+    def add(self, pulse: Pulse):
         if not isinstance(pulse, Pulse):
             raise_error(TypeError, f"Pulse {pulse} has invalid type {type(pulse)}.")
 
         qmpulse = QMPulse(pulse)
         self.pulse_to_qmpulse[pulse.serial] = qmpulse
-        if pulse.type.name == "READOUT":
+        if pulse.type is PulseType.READOUT:
             self.ro_pulses.append(qmpulse)
-        super().append(qmpulse)
+
+        previous = self._find_previous(pulse)
+        if previous is not None:
+            previous.next.add(qmpulse)
+
+        wait_time = pulse.start - self.clock[qmpulse.element]
+        if wait_time >= 12:
+            qmpulse.wait_time = wait_time // 4 + 1
+            self.clock[qmpulse.element] += 4 * qmpulse.wait_time
+        self.clock[qmpulse.element] += qmpulse.duration
+
+        self.pulse_finish[pulse.finish].append(qmpulse)
+        self.qmpulses.append(qmpulse)
         return qmpulse
 
 
 class QMOPX(AbstractInstrument):
     """Instrument object for controlling Quantum Machines (QM) OPX controllers.
 
     Playing pulses on QM controllers requires a ``config`` dictionary and a program
@@ -499,166 +600,199 @@
         from qm import generate_qua_script
 
         with open("qua_script.txt", "w") as file:
             file.write(generate_qua_script(program, self.config.__dict__))
 
         return machine.execute(program)
 
+    def create_qmsequence(self, qubits, sequence):
+        """Translates a :class:`qibolab.pulses.PulseSequence` to a :class:`qibolab.instruments.qm.Sequence`.
+        Also register flux elements for all qubits (if applicable) so that all qubits are operated at their
+        sweetspot.
+        Args:
+            qubits (list): List of :class:`qibolab.platforms.abstract.Qubit` objects
+                passed from the platform.
+            sequence (:class:`qibolab.pulses.PulseSequence`). Pulse sequence to translate.
+        Returns:
+            (:class:`qibolab.instruments.qm.Sequence`) containing the pulses from given pulse sequence.
+        """
+        # register flux elements for all qubits so that they are
+        # always at sweetspot even when they are not used
+        for qubit in qubits.values():
+            if qubit.flux:
+                self.config.register_flux_element(qubit)
+
+        # Current driver cannot play overlapping pulses on drive and flux channels
+        # If we want to play overlapping pulses we need to define different elements on the same ports
+        # like we do for readout multiplex
+        qmsequence = Sequence()
+        for pulse in sorted(sequence.pulses, key=lambda pulse: (pulse.start, pulse.duration)):
+            qmpulse = qmsequence.add(pulse)
+            if pulse.type is PulseType.FLUX:
+                # register flux element (if it does not already exist)
+                self.config.register_flux_element(qubits[pulse.qubit], pulse.frequency)
+                qmpulse.bake(self.config)
+            else:
+                if pulse.duration % 4 != 0 or pulse.duration < 16:
+                    raise_error(NotImplementedError, "1ns resolution is available for flux pulses only.")
+                self.config.register_pulse(qubits[pulse.qubit], pulse, self.time_of_flight, self.smearing)
+        return qmsequence
+
+    @staticmethod
+    def readout(qmpulse, raw_adc):
+        """Plays a readout pulse and assigns the acquired results in QUA variables.
+
+        Args:
+            qmpulse (:class:`qibolab.instruments.qm.QMPulse`): Readout pulse to play.
+            raw_adc (bool): If ``True`` it captures the raw ADC signal, otherwise it integrates.
+        """
+        acquisition = qmpulse.acquisition
+        if raw_adc:
+            measure(qmpulse.operation, qmpulse.element, acquisition.adc_stream)
+        else:
+            measure(
+                qmpulse.operation,
+                qmpulse.element,
+                None,
+                dual_demod.full("cos", "out1", "sin", "out2", acquisition.I),
+                dual_demod.full("minus_sin", "out1", "cos", "out2", acquisition.Q),
+            )
+            acquisition.classify_shots()
+
     @staticmethod
-    def play_pulses(qmsequence, relaxation_time=0):
+    def play_pulses(qmsequence, relaxation_time=0, raw_adc=False):
         """Part of QUA program that plays an arbitrary pulse sequence.
 
         Should be used inside a ``program()`` context.
 
         Args:
             qmsequence (list): Pulse sequence containing QM specific pulses (``qmpulse``).
                 These pulses are defined in :meth:`qibolab.instruments.qm.QMOPX.play` and
                 hold attributes for the ``element`` and ``operation`` that corresponds to
                 each pulse, as defined in the QM config.
         """
         needs_reset = False
         align()
-        clock = collections.defaultdict(int)
-        for qmpulse in qmsequence:
+        for qmpulse in qmsequence.qmpulses:
             pulse = qmpulse.pulse
-            wait_time = pulse.start - clock[qmpulse.element]
-            if wait_time >= 12:
-                wait_cycles = wait_time // 4 + 1
-                wait(wait_cycles, qmpulse.element)
-                clock[qmpulse.element] += 4 * wait_cycles
-            clock[qmpulse.element] += qmpulse.duration
-            if pulse.type.name == "READOUT":
-                measure(
-                    qmpulse.operation,
-                    qmpulse.element,
-                    None,
-                    dual_demod.full("cos", "out1", "sin", "out2", qmpulse.I),
-                    dual_demod.full("minus_sin", "out1", "cos", "out2", qmpulse.Q),
-                )
-                if qmpulse.threshold is not None:
-                    assign(qmpulse.shot, qmpulse.I * qmpulse.cos - qmpulse.Q * qmpulse.sin > qmpulse.threshold)
+            if qmpulse.wait_cycles is not None:
+                wait(qmpulse.wait_cycles, qmpulse.element)
+            if pulse.type is PulseType.READOUT:
+                QMOPX.readout(qmpulse, raw_adc)
             else:
                 if not isinstance(qmpulse.relative_phase, float) or qmpulse.relative_phase != 0:
                     frame_rotation_2pi(qmpulse.relative_phase, qmpulse.element)
                     needs_reset = True
                 if qmpulse.baked is not None:
                     if qmpulse.baked_amplitude is not None:
                         qmpulse.baked.run(amp_array=[(qmpulse.element, qmpulse.baked_amplitude)])
                     else:
                         qmpulse.baked.run()
                 else:
                     play(qmpulse.operation, qmpulse.element)
                 if needs_reset:
                     reset_frame(qmpulse.element)
+                    needs_reset = False
 
         # for Rabi-length?
         if relaxation_time > 0:
-            wait(relaxation_time // 4, *clock.keys())
+            wait(relaxation_time // 4)
 
         # Save data to the stream processing
-        for qmpulse in qmsequence.ro_pulses:
-            save(qmpulse.I, qmpulse.I_st)
-            save(qmpulse.Q, qmpulse.Q_st)
-            if qmpulse.threshold is not None:
-                save(qmpulse.shot, qmpulse.shots)
+        if not raw_adc:
+            for qmpulse in qmsequence.ro_pulses:
+                qmpulse.acquisition.save()
 
     @staticmethod
-    def fetch_results(result, ro_pulses):
+    def fetch_results(result, ro_pulses, average, raw_adc=False):
         """Fetches results from an executed experiment."""
         # TODO: Update result asynchronously instead of waiting
         # for all values, in order to allow live plotting
         # import time
         # for _ in range(5):
         #    handles.is_processing()
         #    time.sleep(1)
         handles = result.result_handles
         handles.wait_for_all_values()
         results = {}
         for pulse in ro_pulses:
             serial = pulse.serial
             ires = handles.get(f"{serial}_I").fetch_all()
             qres = handles.get(f"{serial}_Q").fetch_all()
+            if raw_adc:
+                # convert raw ADC signal to volts
+                u = unit()
+                ires = u.raw2volts(ires)
+                qres = u.raw2volts(qres)
+
             if f"{serial}_shots" in handles:
                 shots = handles.get(f"{serial}_shots").fetch_all().astype(int)
             else:
                 shots = None
-            results[pulse.qubit] = results[serial] = ExecutionResults.from_components(ires, qres, shots)
+            results[pulse.qubit] = results[serial] = (
+                AveragedResults.from_components(ires, qres)
+                if average
+                else ExecutionResults.from_components(ires, qres, shots)
+            )
         return results
 
-    def play(self, qubits, sequence, nshots, relaxation_time):
+    @staticmethod
+    def save_streams(qmpulse, nshots, raw_adc):
+        """Saves streams acquired from readout."""
+        serial = qmpulse.pulse.serial
+        acquisition = qmpulse.acquisition
+        if raw_adc:
+            acquisition.adc_stream.input1().average().save(f"{serial}_I")
+            acquisition.adc_stream.input2().average().save(f"{serial}_Q")
+        else:
+            acquisition.I_stream.buffer(nshots).save(f"{serial}_I")
+            acquisition.Q_stream.buffer(nshots).save(f"{serial}_Q")
+            if acquisition.threshold is not None:
+                acquisition.shots.buffer(nshots).save(f"{serial}_shots")
+
+    def play(self, qubits, sequence, nshots, relaxation_time, average=False, raw_adc=False):
         """Plays an arbitrary pulse sequence using QUA program.
 
         Args:
             qubits (list): List of :class:`qibolab.platforms.utils.Qubit` objects
                 passed from the platform.
             sequence (:class:`qibolab.pulses.PulseSequence`). Pulse sequence to play.
             nshots (int): Number of repetitions (shots) of the experiment.
             relaxation_time (int): Time to wait for the qubit to relax to its ground state between shots in ns.
+            average (bool): If True the return type is :class:`qibolab.result.AveragedResults` which includes
+                averaged values of i and q. If False the return type is :class:`qibolab.result.ExecutionResults`
+                which includes i, q and shot for each shots.
         """
-        # register flux elements for all qubits so that they are
-        # always at sweetspot even when they are not used
-        for qubit in qubits.values():
-            if qubit.flux:
-                self.config.register_flux_element(qubit)
-
         if not sequence:
             return {}
-        # Current driver cannot play overlapping pulses on drive and flux channels
-        # If we want to play overlapping pulses we need to define different elements on the same ports
-        # like we do for readout multiplex
-        qmsequence = QMSequence()
-        for pulse in sequence:
-            qmpulse = qmsequence.add(pulse)
-            if pulse.duration % 4 or pulse.duration < 16:
-                if pulse.type.name != "FLUX":
-                    raise_error(NotImplementedError, "1ns resolution is available for flux pulses only.")
-                # register flux element (if it does not already exist)
-                self.config.register_flux_element(qubits[pulse.qubit], pulse.frequency)
-                qmpulse.bake(self.config)
-            else:
-                self.config.register_pulse(qubits[pulse.qubit], pulse, self.time_of_flight, self.smearing)
 
+        qmsequence = self.create_qmsequence(qubits, sequence)
         # play pulses using QUA
         with program() as experiment:
             n = declare(int)
             for qmpulse in qmsequence.ro_pulses:
                 threshold = qubits[qmpulse.pulse.qubit].threshold
                 iq_angle = qubits[qmpulse.pulse.qubit].iq_angle
-                qmpulse.declare_output(threshold, iq_angle)
+                qmpulse.declare_output(threshold, iq_angle, raw_adc)
 
             with for_(n, 0, n < nshots, n + 1):
-                self.play_pulses(qmsequence, relaxation_time)
+                self.play_pulses(qmsequence, relaxation_time, raw_adc)
 
             with stream_processing():
-                # I_st.average().save("I")
-                # Q_st.average().save("Q")
-                # n_st.buffer().save_all("n")
                 for qmpulse in qmsequence.ro_pulses:
-                    serial = qmpulse.pulse.serial
-                    qmpulse.I_st.buffer(nshots).save(f"{serial}_I")
-                    qmpulse.Q_st.buffer(nshots).save(f"{serial}_Q")
-                    if qmpulse.threshold is not None:
-                        qmpulse.shots.buffer(nshots).save(f"{serial}_shots")
+                    self.save_streams(qmpulse, nshots, raw_adc)
 
         result = self.execute_program(experiment)
-        return self.fetch_results(result, sequence.ro_pulses)
+        return self.fetch_results(result, sequence.ro_pulses, average, raw_adc)
 
     def sweep(self, qubits, sequence, *sweepers, nshots, relaxation_time, average=True):
-        qmsequence = QMSequence()
-        for pulse in sequence:
-            qmpulse = qmsequence.add(pulse)
-            if pulse.duration % 4 or pulse.duration < 16:
-                if pulse.type.name != "FLUX":
-                    raise_error(NotImplementedError, "1ns resolution is available for flux pulses only.")
-                # register flux element (if it does not already exist)
-                self.config.register_flux_element(qubits[pulse.qubit], pulse.frequency)
-                qmpulse.bake(self.config)
-            else:
-                self.config.register_pulse(qubits[pulse.qubit], pulse, self.time_of_flight, self.smearing)
+        if not sequence:
+            return {}
 
+        qmsequence = self.create_qmsequence(qubits, sequence)
         # play pulses using QUA
         with program() as experiment:
             n = declare(int)
             for qmpulse in qmsequence.ro_pulses:
                 if average:
                     # not calculating single shots when averaging
                     # during sweep so we do not pass ``threshold`` here
@@ -669,119 +803,160 @@
                     qmpulse.declare_output(threshold, iq_angle)
 
             with for_(n, 0, n < nshots, n + 1):
                 self.sweep_recursion(list(sweepers), qubits, qmsequence, relaxation_time)
 
             with stream_processing():
                 for qmpulse in qmsequence.ro_pulses:
-                    Ist_temp = qmpulse.I_st
-                    Qst_temp = qmpulse.Q_st
-                    if not average and qmpulse.threshold is not None:
-                        shots_temp = qmpulse.shots
+                    acquisition = qmpulse.acquisition
+                    Ist_temp = acquisition.I_stream
+                    Qst_temp = acquisition.Q_stream
+                    if not average and acquisition.threshold is not None:
+                        shots_temp = acquisition.shots
                     for sweeper in reversed(sweepers):
                         Ist_temp = Ist_temp.buffer(len(sweeper.values))
                         Qst_temp = Qst_temp.buffer(len(sweeper.values))
-                        if not average and qmpulse.threshold is not None:
+                        if not average and acquisition.threshold is not None:
                             shots_temp = shots_temp.buffer(len(sweeper.values))
                     serial = qmpulse.pulse.serial
                     if average:
                         Ist_temp.average().save(f"{serial}_I")
                         Qst_temp.average().save(f"{serial}_Q")
                     else:
                         Ist_temp.buffer(nshots).save(f"{serial}_I")
                         Qst_temp.buffer(nshots).save(f"{serial}_Q")
-                        if qmpulse.threshold is not None:
+                        if acquisition.threshold is not None:
                             shots_temp.buffer(nshots).save(f"{serial}_shots")
 
         result = self.execute_program(experiment)
-        return self.fetch_results(result, sequence.ro_pulses)
+        return self.fetch_results(result, sequence.ro_pulses, average, raw_adc=False)
+
+    @staticmethod
+    def maximum_sweep_value(values, value0):
+        """Calculates maximum value that is reached during a sweep.
+
+        Useful to check whether a sweep exceeds the range of allowed values.
+        Note that both the array of values we sweep and the center value can
+        be negative, so we need to make sure that the maximum absolute value
+        is within range.
+
+        Args:
+            values (np.ndarray): Array of values we will sweep over.
+            value0 (float, int): Center value of the sweep.
+        """
+        return max(abs(min(values) + value0), abs(max(values) + value0))
 
     def sweep_frequency(self, sweepers, qubits, qmsequence, relaxation_time):
         from qm.qua import update_frequency
 
         sweeper = sweepers[0]
         freqs0 = []
         for pulse in sweeper.pulses:
             qubit = qubits[pulse.qubit]
             if pulse.type is PulseType.DRIVE:
-                lo_frequency = int(qubit.drive.local_oscillator.frequency)
+                lo_frequency = math.floor(qubit.drive.local_oscillator.frequency)
             elif pulse.type is PulseType.READOUT:
-                lo_frequency = int(qubit.readout.local_oscillator.frequency)
+                lo_frequency = math.floor(qubit.readout.local_oscillator.frequency)
             else:
                 raise_error(NotImplementedError, f"Cannot sweep frequency of pulse of type {pulse.type}.")
             # convert to IF frequency for readout and drive pulses
-            freqs0.append(declare(int, value=int(pulse.frequency - lo_frequency)))
+            f0 = math.floor(pulse.frequency - lo_frequency)
+            freqs0.append(declare(int, value=f0))
+            # check if sweep is within the supported bandwidth [-400, 400] MHz
+            max_freq = self.maximum_sweep_value(sweeper.values, f0)
+            if max_freq > 4e8:
+                raise_error(ValueError, f"Frequency {max_freq} for qubit {qubit.name} is beyond instrument bandwidth.")
 
         # is it fine to have this declaration inside the ``nshots`` QUA loop?
         f = declare(int)
         with for_(*from_array(f, sweeper.values.astype(int))):
             for pulse, f0 in zip(sweeper.pulses, freqs0):
                 qmpulse = qmsequence.pulse_to_qmpulse[pulse.serial]
                 update_frequency(qmpulse.element, f + f0)
 
             self.sweep_recursion(sweepers[1:], qubits, qmsequence, relaxation_time)
-            if relaxation_time > 0:
-                wait(relaxation_time // 4)
 
     def sweep_amplitude(self, sweepers, qubits, qmsequence, relaxation_time):
         from qm.qua import amp
 
-        # TODO: It should be -2 < amp(a) < 2 otherwise the we get weird results
-        # without an error. Amplitude should be fixed to allow arbitrary values
-        # in qibocal
-
         sweeper = sweepers[0]
+        # TODO: Consider sweeping amplitude without multiplication
+        if min(sweeper.values) < -2:
+            raise_error(ValueError, "Amplitude sweep values are <-2 which is not supported.")
+        if max(sweeper.values) > 2:
+            raise_error(ValueError, "Amplitude sweep values are >2 which is not supported.")
+
         a = declare(fixed)
         with for_(*from_array(a, sweeper.values)):
             for pulse in sweeper.pulses:
                 qmpulse = qmsequence.pulse_to_qmpulse[pulse.serial]
                 if qmpulse.baked is None:
                     qmpulse.operation = qmpulse.operation * amp(a)
                 else:
                     qmpulse.baked_amplitude = a
 
             self.sweep_recursion(sweepers[1:], qubits, qmsequence, relaxation_time)
-            if relaxation_time > 0:
-                wait(relaxation_time // 4)
 
     def sweep_relative_phase(self, sweepers, qubits, qmsequence, relaxation_time):
         sweeper = sweepers[0]
         relphase = declare(fixed)
         with for_(*from_array(relphase, sweeper.values / (2 * np.pi))):
             for pulse in sweeper.pulses:
                 qmpulse = qmsequence.pulse_to_qmpulse[pulse.serial]
                 qmpulse.relative_phase = relphase
 
             self.sweep_recursion(sweepers[1:], qubits, qmsequence, relaxation_time)
-            if relaxation_time > 0:
-                wait(relaxation_time // 4)
 
     def sweep_bias(self, sweepers, qubits, qmsequence, relaxation_time):
         from qm.qua import set_dc_offset
 
         sweeper = sweepers[0]
-        bias0 = [declare(fixed, value=qubits[q].flux.bias) for q in sweeper.qubits]
+        bias0 = []
+        for q in sweeper.qubits:
+            b0 = qubits[q].flux.bias
+            max_bias = qubits[q].flux.max_bias
+            max_value = self.maximum_sweep_value(sweeper.values, b0)
+            check_max_bias(max_value, max_bias)
+            bias0.append(declare(fixed, value=b0))
         b = declare(fixed)
         with for_(*from_array(b, sweeper.values)):
             for q, b0 in zip(sweeper.qubits, bias0):
                 set_dc_offset(f"flux{q}", "single", b + b0)
 
             self.sweep_recursion(sweepers[1:], qubits, qmsequence, relaxation_time)
-            if relaxation_time > 0:
-                wait(relaxation_time // 4)
+
+    def sweep_delay(self, sweepers, qubits, qmsequence, relaxation_time):
+        sweeper = sweepers[0]
+        if min(sweeper.values) < 16:
+            raise_error(ValueError, "Cannot sweep delay less than 16ns.")
+
+        delay = declare(int)
+        values = np.array(sweeper.values) // 4
+        with for_(*from_array(delay, values.astype(int))):
+            for pulse in sweeper.pulses:
+                qmpulse = qmsequence.pulse_to_qmpulse[pulse.serial]
+                # find all pulses that are connected to ``qmpulse`` and update their delays
+                to_process = {qmpulse}
+                while to_process:
+                    next_qmpulse = to_process.pop()
+                    to_process |= next_qmpulse.next
+                    next_qmpulse.wait_time_variable = delay
+
+            self.sweep_recursion(sweepers[1:], qubits, qmsequence, relaxation_time)
 
     SWEEPERS = {
         Parameter.frequency: sweep_frequency,
         Parameter.amplitude: sweep_amplitude,
         Parameter.relative_phase: sweep_relative_phase,
         Parameter.bias: sweep_bias,
+        Parameter.delay: sweep_delay,
     }
 
     def sweep_recursion(self, sweepers, qubits, qmsequence, relaxation_time):
         if len(sweepers) > 0:
             parameter = sweepers[0].parameter
             if parameter in self.SWEEPERS:
                 self.SWEEPERS[parameter](self, sweepers, qubits, qmsequence, relaxation_time)
             else:
                 raise_error(NotImplementedError, f"Sweeper for {parameter} is not implemented.")
         else:
-            self.play_pulses(qmsequence)
+            self.play_pulses(qmsequence, relaxation_time)
```

### Comparing `qibolab-0.0.2/src/qibolab/instruments/qmsim.py` & `qibolab-0.0.3/src/qibolab/instruments/qmsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             from qm.simulate.credentials import create_credentials
 
             self.manager = QuantumMachinesManager(host, int(port), credentials=create_credentials())
         else:
             self.manager = QuantumMachinesManager(host, int(port))
 
     @staticmethod
-    def fetch_results(result, ro_pulses):
+    def fetch_results(result, ro_pulses, average, raw_adc=False):
         return result
 
     def execute_program(self, program):
         ncontrollers = len(self.config.controllers)
 
         # for debugging only
         from qm import generate_qua_script
```

### Comparing `qibolab-0.0.2/src/qibolab/instruments/qutech.py` & `qibolab-0.0.3/src/qibolab/instruments/qutech.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/instruments/rohde_schwarz.py` & `qibolab-0.0.3/src/qibolab/instruments/rohde_schwarz.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/platform.py` & `qibolab-0.0.3/src/qibolab/platform.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 
 from qibolab.designs import Channel, ChannelMap, InstrumentDesign
 from qibolab.platforms.platform import DesignPlatform
 
 
 def create_dummy(runcard):
     """Create a dummy platform using the dummy instrument.
-
     Useful for testing.
     """
     from qibolab.instruments.dummy import DummyInstrument
 
     # Create channel objects
     channels = ChannelMap()
-    channels |= ChannelMap.from_names("readout", "drive", "flux")
+    channels |= ChannelMap.from_names("readout", "drive")
+    channels |= ChannelMap.from_names(*(f"flux-{i}" for i in range(6)))
 
     # Create dummy controller
     instrument = DummyInstrument("dummy", 0)
     # Create design
     design = InstrumentDesign([instrument], channels)
     # Create platform
     platform = DesignPlatform("dummy", design, runcard)
 
     # map channels to qubits
     for qubit in platform.qubits:
         platform.qubits[qubit].readout = channels["readout"]
         platform.qubits[qubit].drive = channels["drive"]
-        platform.qubits[qubit].flux = channels["flux"]
+        platform.qubits[qubit].flux = channels[f"flux-{qubit}"]
+        channels[f"flux-{qubit}"].qubit = platform.qubits[qubit]
+        channels["readout"].qubit = platform.qubits[qubit]
 
     return platform
 
 
 def create_tii_qw5q_gold(runcard, simulation_duration=None, address=None, cloud=False):
     """Create platform using Quantum Machines (QM) OPXs and Rohde Schwarz local oscillators.
-
     IPs and other instrument related parameters are hardcoded in ``__init__`` and ``setup``.
-
     Args:
         runcard (str): Path to the runcard file.
         simulation_duration (int): Duration for the simulation in ns.
             If given the compiler simulator will be used instead of the actual hardware.
             Default is ``None`` which falls back to the hardware.
         address (str): Address and port for the QM OPX cluster.
             If ``None`` it will attempt to connect to TII instruments.
@@ -146,14 +146,18 @@
     qubits[0].flux = channels["L4-5"]
     channels["L4-5"].qubit = qubits[0]
     for q in range(1, 5):
         qubits[q].drive = channels[f"L3-{10 + q}"]
         qubits[q].flux = channels[f"L4-{q}"]
         channels[f"L4-{q}"].qubit = qubits[q]
 
+    # set maximum allowed bias values to protect amplifier
+    # relevant only for qubits where an amplifier is used
+    for q in range(5):
+        platform.qubits[q].flux.max_bias = 0.2
     # Platfom topology
     Q = [f"q{i}" for i in range(5)]
     chip = nx.Graph()
     chip.add_nodes_from(Q)
     graph_list = [
         (Q[0], Q[2]),
         (Q[1], Q[2]),
@@ -162,23 +166,66 @@
     ]
     chip.add_edges_from(graph_list)
     platform.topology = chip
 
     return platform
 
 
+def create_tii_rfsoc4x2(runcard, address=None):
+    """Create platform using QICK project on the RFSoC4x2 board
+    IPs and other instrument related parameters are hardcoded in ``__init__`` and ``setup``.
+    Args:
+        runcard (str): Path to the runcard file.
+        address (str): Address and port for the QICK board.
+            If ``None`` it will attempt to connect to TII instruments.
+    """
+    from qibolab.instruments.rfsoc import TII_RFSOC4x2
+    from qibolab.instruments.rohde_schwarz import SGS100A as LocalOscillator
+
+    # Create channel objects
+    channels = ChannelMap()
+    channels |= ChannelMap.from_names("L3-18_ro")  # readout (DAC)
+    channels |= ChannelMap.from_names("L2-RO")  # feedback (readout DAC)
+    channels |= ChannelMap.from_names("L3-18_qd")  # drive
+
+    # Map controllers to qubit channels (HARDCODED)
+    channels["L3-18_ro"].ports = [("o0", 0)]  # readout
+    channels["L2-RO"].ports = [("i0", 0)]  # feedback
+    channels["L3-18_qd"].ports = [("o1", 1)]  # drive
+
+    local_oscillators = [
+        LocalOscillator("twpa_a", "192.168.0.32"),
+    ]
+    local_oscillators[0].frequency = 6_200_000_000
+    local_oscillators[0].power = -1
+
+    # Instantiate QICK instruments
+    if address is None:
+        address = "192.168.0.72:6000"
+    controller = TII_RFSOC4x2("tii_rfsoc4x2", address)
+    design = InstrumentDesign([controller] + local_oscillators, channels)
+
+    platform = DesignPlatform("tii_rfsoc4x2", design, runcard)
+
+    # assign channels to qubits
+    qubits = platform.qubits
+    qubits[0].readout = channels["L3-18_ro"]
+    qubits[0].feedback = channels["L2-RO"]
+    qubits[0].drive = channels["L3-18_qd"]  # Create channel objects
+
+    return platform
+
+
 def Platform(name, runcard=None, design=None):
     """Platform for controlling quantum devices.
-
     Args:
         name (str): name of the platform. Options are 'tiiq', 'qili' and 'icarusq'.
         runcard (str): path to the yaml file containing the platform setup.
         design (:class:`qibolab.designs.abstract.AbstractInstrumentDesign`): Instrument
             design to use for the platform.
-
     Returns:
         The plaform class.
     """
     if not runcard:
         from os.path import exists
 
         from qibolab.paths import qibolab_folder
@@ -189,11 +236,13 @@
 
     if name == "dummy":
         return create_dummy(runcard)
     elif name == "icarusq":
         from qibolab.platforms.icplatform import ICPlatform as Device
     elif name == "qw5q_gold":
         return create_tii_qw5q_gold(runcard)
+    elif name == "tii1q_b1":
+        return create_tii_rfsoc4x2(runcard)
     else:
         from qibolab.platforms.multiqubit import MultiqubitPlatform as Device
 
     return Device(name, runcard)
```

### Comparing `qibolab-0.0.2/src/qibolab/platforms/abstract.py` & `qibolab-0.0.3/src/qibolab/platforms/abstract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import math
+import re
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass, field
+from pathlib import Path
 from typing import Any, List, Optional
 
 import numpy as np
 import yaml
 from qibo import gates
 from qibo.config import log, raise_error
 from qibo.models import Circuit
 
 from qibolab.designs.channels import Channel
 from qibolab.pulses import FluxPulse, Pulse, PulseSequence, ReadoutPulse
-from qibolab.transpilers import can_execute, transpile
+from qibolab.transpilers.gate_decompositions import TwoQubitNatives
 
 
 @dataclass
 class Qubit:
     """Representation of a physical qubit.
 
     Qubit objects are instantiated by :class:`qibolab.platforms.platform.Platform`
@@ -31,35 +34,34 @@
             send drive pulses to the qubit.
         flux (:class:`qibolab.platforms.utils.Channel`): Channel used to
             send flux pulses to the qubit.
         Other characterization parameters for the qubit, loaded from the runcard.
     """
 
     name: str
-
-    readout_frequency: int = 0
+    bare_resonator_frequency: int = 0
+    readout_frequency: int = 0  # this is the dressed frequency
     drive_frequency: int = 0
     sweetspot: float = 0
     peak_voltage: float = 0
     pi_pulse_amplitude: float = 0
     T1: int = 0
     T2: int = 0
+    T2_spin_echo: int = 0
     state0_voltage: int = 0
     state1_voltage: int = 0
     mean_gnd_states: complex = 0 + 0.0j
     mean_exc_states: complex = 0 + 0.0j
     resonator_polycoef_flux: List[float] = field(default_factory=list)
 
     # filters used for applying CZ gate
     filter: dict = field(default_factory=dict)
     # parameters for single shot classification
     threshold: Optional[float] = None
     iq_angle: float = 0.0
-    # required for integration weights (not sure if it should be here)
-    rotation_angle: float = 0.0
     # required for mixers (not sure if it should be here)
     mixer_drive_g: float = 0.0
     mixer_drive_phi: float = 0.0
     mixer_readout_g: float = 0.0
     mixer_readout_phi: float = 0.0
 
     readout: Optional[Channel] = None
@@ -101,62 +103,220 @@
         self.is_connected = False
         self.nqubits = None
         self.resonator_type = None
         self.topology = None
         self.relaxation_time = None
         self.sampling_rate = None
 
-        self.native_single_qubit_gates = {}
-        self.native_two_qubit_gates = {}
-        self.two_qubit_natives = set()
+        self.single_qubit_natives = {}
+        self.two_qubit_natives = TwoQubitNatives(0)
         # Load platform settings
         self.reload_settings()
 
     def __repr__(self):
         return self.name
 
     def _check_connected(self):
         if not self.is_connected:  # pragma: no cover
             raise_error(RuntimeError, "Cannot access instrument because it is not connected.")
 
     def reload_settings(self):
         # TODO: Remove ``self.settings``
-        with open(self.runcard) as file:
-            settings = self.settings = yaml.safe_load(file)
+        if self.settings == None:
+            # Load initial configuration
+            with open(self.runcard) as file:
+                settings = self.settings = yaml.safe_load(file)
+        else:
+            # Load current configuration
+            settings = self.settings
 
         self.nqubits = settings["nqubits"]
         if "resonator_type" in self.settings:
             self.resonator_type = self.settings["resonator_type"]
         else:
             self.resonator_type = "3D" if self.nqubits == 1 else "2D"
 
         self.topology = settings["topology"]
 
-        self.relaxation_time = settings["settings"]["repetition_duration"]
+        self.relaxation_time = settings["settings"]["relaxation_time"]
         self.sampling_rate = settings["settings"]["sampling_rate"]
 
-        # TODO: Create better data structures for native gates
+        # Load native gates
         self.native_gates = settings["native_gates"]
-        self.native_single_qubit_gates = self.native_gates["single_qubit"]
+        self.single_qubit_natives = self.native_gates["single_qubit"]
         if "two_qubit" in self.native_gates:
-            self.native_two_qubit_gates = self.native_gates["two_qubit"]
-            for gates in self.native_gates["two_qubit"].values():
-                self.two_qubit_natives |= set(gates.keys())
+            for gate in self.native_gates["two_qubit"].values():
+                self.two_qubit_natives |= TwoQubitNatives[list(gate)[0]]
         else:
             # dummy value to avoid transpiler failure for single qubit devices
-            self.two_qubit_natives = {"CZ"}
+            self.two_qubit_natives = TwoQubitNatives.CZ
 
         # Load characterization settings and create ``Qubit`` and ``Channel`` objects
         for q in settings["qubits"]:
             if q in self.qubits:
                 for name, value in settings["characterization"]["single_qubit"][q].items():
                     setattr(self.qubits[q], name, value)
             else:
                 self.qubits[q] = Qubit(q, **settings["characterization"]["single_qubit"][q])
 
+    def dump(self, path: Path):
+        with open(path, "w") as file:
+            yaml.dump(self.settings, file, sort_keys=False, indent=4, default_flow_style=None)
+
+    def update(self, updates: dict):
+        r"""Updates platform common runcard parameters after calibration actions.
+
+        Args:
+
+            updates (dict): Dictionary containing the parameters to update the runcard. A typical dictionary should be of the following form
+                            {`parameter_to_update_in_runcard`:{`qubit0`:`par_value_qubit0`, ..., `qubit_i`:`par_value_qubit_i`, ...}}.
+                            The parameters that can be updated by this method are:
+                                - readout_frequency (GHz)
+                                - readout_attenuation (dimensionless)
+                                - bare_resonator_frequency (GHz)
+                                - sweetspot(V)
+                                - drive_frequency (GHz)
+                                - readout_amplitude (dimensionless)
+                                - drive_amplitude (dimensionless)
+                                - drive_length
+                                - t2 (ns)
+                                - t2_spin_echo (ns)
+                                - t1 (ns)
+                                - thresold(V)
+                                - iq_angle(deg)
+                                - mean_gnd_states(V)
+                                - mean_exc_states(V)
+                                - beta(dimensionless)
+
+
+
+        """
+
+        for par, values in updates.items():
+            for qubit, value in values.items():
+                # resonator_spectroscopy / resonator_spectroscopy_flux / resonator_punchout_attenuation
+                if par == "readout_frequency":
+                    freq = int(value * 1e9)
+                    self.single_qubit_natives[qubit]["MZ"]["frequency"] = freq
+                    self.settings["native_gates"]["single_qubit"][qubit]["MZ"]["frequency"] = freq
+
+                    if "if_frequency" in self.single_qubit_natives[qubit]["MZ"]:
+                        self.single_qubit_natives[qubit]["MZ"]["if_frequency"] = freq - self.get_lo_readout_frequency(
+                            qubit
+                        )
+                        self.settings["native_gates"]["single_qubit"][qubit]["MZ"][
+                            "if_frequency"
+                        ] = freq - self.get_lo_readout_frequency(qubit)
+
+                    self.qubits[qubit].readout_frequency = freq
+                    self.settings["characterization"]["single_qubit"][qubit]["readout_frequency"] = freq
+
+                # resonator_punchout_attenuation
+                elif par == "readout_attenuation":
+                    # TODO: Are we going to save the attenuation somwhere in the native_gates or characterization
+                    # in all platforms?
+                    True
+
+                # resonator_punchout_attenuation
+                elif par == "bare_resonator_frequency":
+                    freq = int(value * 1e9)
+                    self.qubits[qubit].bare_resonator_frequency = freq
+                    self.settings["characterization"]["single_qubit"][qubit]["bare_resonator_frequency"] = freq
+
+                # resonator_spectroscopy_flux / qubit_spectroscopy_flux
+                elif par == "sweetspot":
+                    sweetspot = float(value)
+                    self.qubits[qubit].sweetspot = sweetspot
+                    self.settings["characterization"]["single_qubit"][qubit]["sweetspot"] = sweetspot
+
+                # qubit_spectroscopy / qubit_spectroscopy_flux / ramsey
+                elif par == "drive_frequency":
+                    freq = int(value * 1e9)
+                    self.single_qubit_natives[qubit]["RX"]["frequency"] = freq
+                    self.settings["native_gates"]["single_qubit"][qubit]["RX"]["frequency"] = freq
+
+                    self.qubits[qubit].drive_frequency = freq
+                    self.settings["characterization"]["single_qubit"][qubit]["drive_frequency"] = freq
+
+                elif "amplitude" in par:
+                    amplitude = float(value)
+                    # resonator_spectroscopy
+                    if par == "readout_amplitude" and not math.isnan(amplitude):
+                        self.single_qubit_natives[qubit]["MZ"]["amplitude"] = amplitude
+                        self.settings["native_gates"]["single_qubit"][qubit]["MZ"]["amplitude"] = amplitude
+
+                    # rabi_amplitude / flipping
+                    if par == "drive_amplitude" or par == "amplitudes":
+                        self.single_qubit_natives[qubit]["RX"]["amplitude"] = amplitude
+                        self.settings["native_gates"]["single_qubit"][qubit]["RX"]["amplitude"] = amplitude
+                        self.settings["characterization"]["single_qubit"][qubit]["pi_pulse_amplitude"] = amplitude
+
+                # rabi_duration
+                elif par == "drive_length":
+                    duration = int(value)
+                    self.single_qubit_natives[qubit]["RX"]["duration"] = duration
+                    self.settings["native_gates"]["single_qubit"][qubit]["RX"]["duration"] = duration
+
+                # ramsey
+                elif par == "t2":
+                    t2 = float(value)
+                    self.qubits[qubit].T2 = t2
+                    self.settings["characterization"]["single_qubit"][qubit]["T2"] = t2
+
+                # spin_echo
+                elif par == "t2_spin_echo":
+                    t2_spin_echo = float(value)
+                    self.qubits[qubit].T2_spin_echo = t2_spin_echo
+                    self.settings["characterization"]["single_qubit"][qubit]["T2_spin_echo"] = t2_spin_echo
+
+                # t1
+                elif par == "t1":
+                    t1 = float(value)
+                    self.qubits[qubit].T1 = t1
+                    self.settings["characterization"]["single_qubit"][qubit]["T1"] = t1
+
+                # classification
+                elif par == "threshold":
+                    threshold = float(value)
+                    self.qubits[qubit].thresold = threshold
+                    self.settings["characterization"]["single_qubit"][qubit]["threshold"] = threshold
+
+                # classification
+                elif par == "iq_angle":
+                    iq_angle = float(value)
+                    self.qubits[qubit].iq_angle = iq_angle
+                    self.settings["characterization"]["single_qubit"][qubit]["iq_angle"] = iq_angle
+
+                # classification
+                elif par == "mean_gnd_states":
+                    mean_gnd_states = str(value)
+                    self.qubits[qubit].mean_gnd_states = mean_gnd_states
+                    self.settings["characterization"]["single_qubit"][qubit]["mean_gnd_states"] = mean_gnd_states
+
+                # classification
+                elif par == "mean_exc_states":
+                    mean_exc_states = str(value)
+                    self.qubits[qubit].mean_exc_states = mean_exc_states
+                    self.settings["characterization"]["single_qubit"][qubit]["mean_exc_states"] = mean_exc_states
+
+                # drag pulse tunning
+                elif "beta" in par:
+                    shape = self.single_qubit_natives[qubit]["RX"]["shape"]
+                    rel_sigma = re.findall(r"[\d]+[.\d]+|[\d]*[.][\d]+|[\d]+", shape)[0]
+                    self.single_qubit_natives[qubit]["RX"]["shape"] = f"Drag({rel_sigma}, {float(value)})"
+                    self.settings["native_gates"]["single_qubit"][qubit]["RX"][
+                        "shape"
+                    ] = f"Drag({rel_sigma}, {float(value)})"
+
+                else:
+                    raise_error(ValueError, f"Unknown parameter {par} for qubit {qubit}")
+
+        # reload_settings after execute any calibration routine keeping fitted parameters
+        self.reload_settings()
+
     @abstractmethod
     def connect(self):
         """Connects to instruments."""
 
     @abstractmethod
     def setup(self):
         """Prepares instruments to execute experiments."""
@@ -180,17 +340,14 @@
             circuit (qibo.models.Circuit): Qibo circuit that respects the platform's
                 connectivity and native gates.
 
         Returns:
             sequence (qibolab.pulses.PulseSequence): Pulse sequence that implements the
                 circuit on the qubit.
         """
-        if not can_execute(circuit, self.two_qubit_natives):
-            circuit, _ = transpile(circuit, self.two_qubit_natives)
-
         sequence = PulseSequence()
         virtual_z_phases = defaultdict(int)
 
         # keep track of gates that were already added to avoid adding them twice
         already_processed = set()
         # process circuit gates
         for moment in circuit.queue.moments:
@@ -266,29 +423,29 @@
                         f"Transpilation of {gate.__class__.__name__} gate has not been implemented yet.",
                     )
 
                 already_processed.add(gate)
         return sequence
 
     @abstractmethod
-    def execute_pulse_sequence(self, sequence, nshots=1024, relaxation_time=None):
+    def execute_pulse_sequence(self, sequence, nshots=1024, relaxation_time=None, raw_adc=False):
         """Executes a pulse sequence.
 
         Args:
             sequence (:class:`qibolab.pulses.PulseSequence`): Pulse sequence to execute.
             nshots (int): Number of shots to sample from the experiment. Default is 1024.
             relaxation_time (int): Time to wait for the qubit to relax to its ground state between shots in ns.
                 If ``None`` the default value provided as ``repetition_duration`` in the runcard will be used.
 
         Returns:
             Readout results acquired by after execution.
         """
 
-    def __call__(self, sequence, nshots=1024, relaxation_time=None):
-        return self.execute_pulse_sequence(sequence, nshots, relaxation_time)
+    def __call__(self, sequence, nshots=1024, relaxation_time=None, raw_adc=False):
+        return self.execute_pulse_sequence(sequence, nshots, relaxation_time, raw_adc=raw_adc)
 
     def sweep(self, sequence, *sweepers, nshots=1024, average=True, relaxation_time=None):
         """Executes a pulse sequence for different values of sweeped parameters.
         Useful for performing chip characterization.
 
         Example:
             .. testcode::
@@ -325,26 +482,25 @@
 
     def get_qd_channel(self, qubit):
         if self.qubits[qubit].drive:
             return self.qubits[qubit].drive.name
         else:
             return self.settings["qubit_channel_map"][qubit][1]
 
-    # TODO: Maybe create a dataclass for native gates
     def create_RX90_pulse(self, qubit, start=0, relative_phase=0):
-        pulse_kwargs = self.native_single_qubit_gates[qubit]["RX"]
+        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
         qd_duration = pulse_kwargs["duration"]
         qd_frequency = pulse_kwargs["frequency"]
         qd_amplitude = pulse_kwargs["amplitude"] / 2.0
         qd_shape = pulse_kwargs["shape"]
         qd_channel = self.get_qd_channel(qubit)
         return Pulse(start, qd_duration, qd_amplitude, qd_frequency, relative_phase, qd_shape, qd_channel, qubit=qubit)
 
     def create_RX_pulse(self, qubit, start=0, relative_phase=0):
-        pulse_kwargs = self.native_single_qubit_gates[qubit]["RX"]
+        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
         qd_duration = pulse_kwargs["duration"]
         qd_frequency = pulse_kwargs["frequency"]
         qd_amplitude = pulse_kwargs["amplitude"]
         qd_shape = pulse_kwargs["shape"]
         qd_channel = self.get_qd_channel(qubit)
         return Pulse(start, qd_duration, qd_amplitude, qd_frequency, relative_phase, qd_shape, qd_channel, qubit=qubit)
 
@@ -390,55 +546,55 @@
                 raise NotImplementedError(
                     "Implementation of CZ gates using pulses of types other than `qf` or `virtual_z` is not supported yet."
                 )
 
         return sequence, virtual_z_phases
 
     def create_MZ_pulse(self, qubit, start):
-        pulse_kwargs = self.native_single_qubit_gates[qubit]["MZ"]
+        pulse_kwargs = self.single_qubit_natives[qubit]["MZ"]
         ro_duration = pulse_kwargs["duration"]
         ro_frequency = pulse_kwargs["frequency"]
         ro_amplitude = pulse_kwargs["amplitude"]
         ro_shape = pulse_kwargs["shape"]
         if self.qubits[qubit].readout:
             ro_channel = self.qubits[qubit].readout.name
         else:
             ro_channel = self.settings["qubit_channel_map"][qubit][0]
         return ReadoutPulse(start, ro_duration, ro_amplitude, ro_frequency, 0, ro_shape, ro_channel, qubit=qubit)
 
     def create_qubit_drive_pulse(self, qubit, start, duration, relative_phase=0):
-        pulse_kwargs = self.native_single_qubit_gates[qubit]["RX"]
+        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
         qd_frequency = pulse_kwargs["frequency"]
         qd_amplitude = pulse_kwargs["amplitude"]
         qd_shape = pulse_kwargs["shape"]
         qd_channel = self.get_qd_channel(qubit)
         return Pulse(start, duration, qd_amplitude, qd_frequency, relative_phase, qd_shape, qd_channel, qubit=qubit)
 
     def create_qubit_readout_pulse(self, qubit, start):
         return self.create_MZ_pulse(qubit, start)
 
     # TODO Remove RX90_drag_pulse and RX_drag_pulse, replace them with create_qubit_drive_pulse
     # TODO Add RY90 and RY pulses
 
     def create_RX90_drag_pulse(self, qubit, start, relative_phase=0, beta=None):
         # create RX pi/2 pulse with drag shape
-        pulse_kwargs = self.native_single_qubit_gates[qubit]["RX"]
+        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
         qd_duration = pulse_kwargs["duration"]
         qd_frequency = pulse_kwargs["frequency"]
         qd_amplitude = pulse_kwargs["amplitude"] / 2.0
         qd_shape = pulse_kwargs["shape"]
         if beta != None:
             qd_shape = "Drag(5," + str(beta) + ")"
 
         qd_channel = self.get_qd_channel(qubit)
         return Pulse(start, qd_duration, qd_amplitude, qd_frequency, relative_phase, qd_shape, qd_channel, qubit=qubit)
 
     def create_RX_drag_pulse(self, qubit, start, relative_phase=0, beta=None):
         # create RX pi pulse with drag shape
-        pulse_kwargs = self.native_single_qubit_gates[qubit]["RX"]
+        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
         qd_duration = pulse_kwargs["duration"]
         qd_frequency = pulse_kwargs["frequency"]
         qd_amplitude = pulse_kwargs["amplitude"]
         qd_shape = pulse_kwargs["shape"]
         if beta != None:
             qd_shape = "Drag(5," + str(beta) + ")"
 
@@ -468,14 +624,40 @@
         """
 
     @abstractmethod
     def get_lo_readout_frequency(self, qubit):
         """Get frequency of the qubit readout local oscillator in Hz."""
 
     @abstractmethod
+    def set_lo_twpa_frequency(self, qubit, freq):
+        """Set frequency of the local oscillator of the TWPA to which the qubit's feedline is connected to.
+
+        Args:
+            qubit (int): qubit whose local oscillator will be modified.
+            freq (int): new value of the frequency in Hz.
+        """
+
+    @abstractmethod
+    def get_lo_twpa_frequency(self, qubit):
+        """Get frequency of the local oscillator of the TWPA to which the qubit's feedline is connected to in Hz."""
+
+    @abstractmethod
+    def set_lo_twpa_power(self, qubit, power):
+        """Set power of the local oscillator of the TWPA to which the qubit's feedline is connected to.
+
+        Args:
+            qubit (int): qubit whose local oscillator will be modified.
+            power (int): new value of the power in dBm.
+        """
+
+    @abstractmethod
+    def get_lo_twpa_power(self, qubit):
+        """Get power of the local oscillator of the TWPA to which the qubit's feedline is connected to in dBm."""
+
+    @abstractmethod
     def set_attenuation(self, qubit, att):
         """Set attenuation value. Usefeul for calibration routines such as punchout.
 
         Args:
             qubit (int): qubit whose attenuation will be modified.
             att (int): new value of the attenuation (dB).
         Returns:
```

### Comparing `qibolab-0.0.2/src/qibolab/platforms/icplatform.py` & `qibolab-0.0.3/src/qibolab/platforms/icplatform.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/platforms/multiqubit.py` & `qibolab-0.0.3/src/qibolab/platforms/multiqubit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 
 import numpy as np
 import yaml
 from qibo.config import log, raise_error
 
-from qibolab.platforms.abstract import AbstractPlatform
+from qibolab.platforms.abstract import AbstractPlatform, Qubit
 from qibolab.pulses import PulseSequence, PulseType
 from qibolab.result import ExecutionResults
 from qibolab.sweeper import Parameter
 
 
 class MultiqubitPlatform(AbstractPlatform):
     def __init__(self, name, runcard):
@@ -40,42 +40,161 @@
                             self.qubit_instrument_map[qubit][self.qubit_channel_map[qubit].index(channel)] = name
 
     def reload_settings(self):
         super().reload_settings()
         self.characterization = self.settings["characterization"]
         self.qubit_channel_map = self.settings["qubit_channel_map"]
         self.hardware_avg = self.settings["settings"]["hardware_avg"]
-        self.repetition_duration = self.settings["settings"]["repetition_duration"]
+        self.relaxation_time = self.settings["settings"]["relaxation_time"]
+
+        # FIX: Set attenuation again to the original value after sweep attenuation in punchout
+        if hasattr(self, "qubit_instrument_map"):
+            for qubit in range(self.nqubits):
+                instrument_name = self.qubit_instrument_map[qubit][0]
+                port = self.qrm[qubit].channel_port_map[self.qubit_channel_map[qubit][0]]
+                att = self.settings["instruments"][instrument_name]["settings"]["ports"][port]["attenuation"]
+                self.ro_port[qubit].attenuation = att
+
+    def update(self, updates: dict):
+        r"""Updates platform dependent runcard parameters and set up platform instruments if needed.
+
+        Args:
+
+            updates (dict): Dictionary containing the parameters to update the runcard.
+        """
+        for par, values in updates.items():
+            for qubit, value in values.items():
+                # resonator_punchout_attenuation
+                if par == "readout_attenuation":
+                    attenuation = int(value)
+                    # save settings
+                    instrument_name = self.qubit_instrument_map[qubit][0]
+                    port = self.qrm[qubit].channel_port_map[self.qubit_channel_map[qubit][0]]
+                    self.settings["instruments"][instrument_name]["settings"]["ports"][port][
+                        "attenuation"
+                    ] = attenuation
+                    # configure RO attenuation
+                    self.ro_port[qubit].attenuation = attenuation
+
+                # resonator_spectroscopy_flux / qubit_spectroscopy_flux
+                if par == "sweetspot":
+                    sweetspot = float(value)
+                    # save settings
+                    instrument_name = self.qubit_instrument_map[qubit][2]
+                    port = self.qrm[qubit].channel_port_map[self.qubit_channel_map[qubit][2]]
+                    self.settings["instruments"][instrument_name]["settings"]["ports"][port]["offset"] = sweetspot
+                    # configure instrument qcm_bb offset
+                    self.qb_port[qubit].current = sweetspot
+
+                # qubit_spectroscopy / qubit_spectroscopy_flux / ramsey
+                if par == "drive_frequency":
+                    freq = int(value * 1e9)
+
+                    # update Qblox qubit LO drive frequency config
+                    instrument_name = self.qubit_instrument_map[qubit][1]
+                    port = self.qdm[qubit].channel_port_map[self.qubit_channel_map[qubit][1]]
+                    drive_if = self.single_qubit_natives[qubit]["RX"]["if_frequency"]
+                    self.settings["instruments"][instrument_name]["settings"]["ports"][port]["lo_frequency"] = (
+                        freq - drive_if
+                    )
+
+                    # set Qblox qubit LO drive frequency
+                    self.qd_port[qubit].lo_frequency = freq - drive_if
+
+                # classification
+                if par == "threshold":
+                    threshold = float(value)
+                    # update Qblox qubit classification threshold
+                    instrument_name = self.qubit_instrument_map[qubit][0]
+                    self.settings["instruments"][instrument_name]["settings"]["classification_parameters"][qubit][
+                        "threshold"
+                    ] = threshold
+
+                    self.instruments[instrument_name].setup(
+                        **self.settings["settings"],
+                        **self.settings["instruments"][instrument_name]["settings"],
+                    )
+
+                # classification
+                if par == "iq_angle":
+                    rotation_angle = float(value)
+                    rotation_angle = (
+                        rotation_angle * 360 / (2 * np.pi)
+                    ) % 360  # save rotation angle in degrees for qblox
+                    # update Qblox qubit classification iq angle
+                    instrument_name = self.qubit_instrument_map[qubit][0]
+                    self.settings["instruments"][instrument_name]["settings"]["classification_parameters"][qubit][
+                        "rotation_angle"
+                    ] = rotation_angle
+
+                    self.instruments[instrument_name].setup(
+                        **self.settings["settings"],
+                        **self.settings["instruments"][instrument_name]["settings"],
+                    )
+
+                super().update(updates)
 
     def set_lo_drive_frequency(self, qubit, freq):
         self.qd_port[qubit].lo_frequency = freq
 
     def get_lo_drive_frequency(self, qubit):
         return self.qd_port[qubit].lo_frequency
 
     def set_lo_readout_frequency(self, qubit, freq):
         self.ro_port[qubit].lo_frequency = freq
 
     def get_lo_readout_frequency(self, qubit):
         return self.ro_port[qubit].lo_frequency
 
-    def set_attenuation(self, qubit, att):
-        self.ro_port[qubit].attenuation = att
+    def set_lo_twpa_frequency(self, qubit, freq):
+        for instrument in self.instruments:
+            if "twpa" in instrument:
+                self.instruments[instrument].frequency = freq
+                return None
+        raise_error(NotImplementedError, "No twpa instrument found in the platform. ")
+
+    def get_lo_twpa_frequency(self, qubit):
+        for instrument in self.instruments:
+            if "twpa" in instrument:
+                return self.instruments[instrument].frequency
+        raise_error(NotImplementedError, "No twpa instrument found in the platform. ")
+
+    def set_lo_twpa_power(self, qubit, power):
+        for instrument in self.instruments:
+            if "twpa" in instrument:
+                self.instruments[instrument].power = power
+                return None
+        raise_error(NotImplementedError, "No twpa instrument found in the platform. ")
+
+    def get_lo_twpa_power(self, qubit):
+        for instrument in self.instruments:
+            if "twpa" in instrument:
+                return self.instruments[instrument].power
+        raise_error(NotImplementedError, "No twpa instrument found in the platform. ")
+
+    def set_attenuation(self, qubit: Qubit, att):
+        self.ro_port[qubit.name].attenuation = att
 
     def set_gain(self, qubit, gain):
         self.qd_port[qubit].gain = gain
 
-    def set_bias(self, qubit, bias):
-        self.qb_port[qubit].current = bias
-
-    def get_attenuation(self, qubit):
-        return self.ro_port[qubit].attenuation
-
-    def get_bias(self, qubit):
-        return self.qb_port[qubit].current
+    def set_bias(self, qubit: Qubit, bias):
+        if qubit.name in self.qbm:
+            self.qb_port[qubit.name].current = bias
+        elif qubit.name in self.qfm:
+            self.qf_port[qubit.name].offset = bias
+
+    def get_attenuation(self, qubit: Qubit):
+        return self.ro_port[qubit.name].attenuation
+
+    def get_bias(self, qubit: Qubit):
+        if qubit.name in self.qbm:
+            return self.qb_port[qubit.name].current
+        elif qubit.name in self.qfm:
+            return self.qf_port[qubit.name].offset
 
     def get_gain(self, qubit):
         return self.qd_port[qubit].gain
 
     def connect(self):
         """Connects to lab instruments using the details specified in the calibration settings."""
         if not self.is_connected:
@@ -160,109 +279,75 @@
 
     def execute_pulse_sequence(self, sequence: PulseSequence, nshots=None):
         if not self.is_connected:
             raise_error(RuntimeError, "Execution failed because instruments are not connected.")
         if nshots is None:
             nshots = self.hardware_avg
 
-        # DEBUG: Plot Pulse Sequence
-        # sequence.plot('plot.png')
-        # DEBUG: sync_en
-        # from qblox_instruments.qcodes_drivers.cluster import Cluster
-        # cluster:Cluster = self.instruments['cluster'].device
-        # for module in cluster.modules:
-        #     if module.get("present"):
-        #         for sequencer in module.sequencers:
-        #             if sequencer.get('sync_en'):
-        #                 print(f"type: {module.module_type}, sequencer: {sequencer.name}, sync_en: True")
-
-        # Process Pulse Sequence. Assign pulses to instruments and generate waveforms & program
         instrument_pulses = {}
-        roles = {}
-        ro_pulses = {}
         changed = {}
-        data = {}
-        for name in self.instruments:
-            roles[name] = self.settings["instruments"][name]["roles"]
-            if "control" in roles[name] or "readout" in roles[name]:
-                instrument_pulses[name] = sequence.get_channel_pulses(*self.instruments[name].channels)
-                # Change pulses frequency to if and correct lo accordingly (before was done in qibolab)
-
-                if "readout" in roles[name]:
-                    for pulse in instrument_pulses[name]:
-                        ro_pulses[pulse.serial] = pulse
-                        if abs(pulse.frequency) > self.instruments[name].FREQUENCY_LIMIT:
-                            # TODO: implement algorithm to find correct LO
-                            if_frequency = self.native_gates["single_qubit"][pulse.qubit]["MZ"]["if_frequency"]
-                            self.set_lo_readout_frequency(pulse.qubit, pulse.frequency - if_frequency)
-                            pulse.frequency = if_frequency
-                            changed[pulse.serial] = True
-                elif "control" in roles[name]:
-                    for pulse in instrument_pulses[name]:
-                        if abs(pulse.frequency) > self.instruments[name].FREQUENCY_LIMIT:
-                            # TODO: implement algorithm to find correct LO
-                            if_frequency = self.native_gates["single_qubit"][pulse.qubit]["RX"]["if_frequency"]
-                            self.set_lo_drive_frequency(pulse.qubit, pulse.frequency - if_frequency)
-                            pulse.frequency = if_frequency
-                            changed[pulse.serial] = True
-
-                self.instruments[name].process_pulse_sequence(instrument_pulses[name], nshots, self.repetition_duration)
-                self.instruments[name].upload()
-        for name in self.instruments:
-            if "control" in roles[name] or "readout" in roles[name]:
-                if not instrument_pulses[name].is_empty:
-                    self.instruments[name].play_sequence()
 
+        readout_instruments = [
+            self.instruments[instrument]
+            for instrument in self.instruments
+            if self.settings["instruments"][instrument]["roles"] == ["readout"]
+        ]
+
+        control_instruments = [
+            self.instruments[instrument]
+            for instrument in self.instruments
+            if self.settings["instruments"][instrument]["roles"] == ["control"]
+        ]
+
+        # STEP 1: upload sequence
+        for instrument in readout_instruments + control_instruments:
+            instrument_pulses[instrument.name] = copy.deepcopy(sequence.get_channel_pulses(*instrument.channels))
+            for pulse in instrument_pulses[instrument.name]:
+                # FIXME: this will not work with arbitrary frequencies
+                if abs(pulse.frequency) > instrument.FREQUENCY_LIMIT:
+                    changed[pulse] = pulse.serial
+                    if instrument in readout_instruments:
+                        if_frequency = self.native_gates["single_qubit"][pulse.qubit]["MZ"]["if_frequency"]
+                        self.set_lo_readout_frequency(pulse.qubit, pulse.frequency - if_frequency)
+                    elif instrument in control_instruments:
+                        if_frequency = self.native_gates["single_qubit"][pulse.qubit]["RX"]["if_frequency"]
+                        self.set_lo_drive_frequency(pulse.qubit, pulse.frequency - if_frequency)
+                    pulse.frequency = if_frequency
+            instrument.process_pulse_sequence(instrument_pulses[instrument.name], nshots, self.relaxation_time)
+            instrument.upload()
+
+        # STEP 2: play sequence
+        for instrument in readout_instruments + control_instruments:
+            if instrument_pulses[instrument.name]:
+                instrument.play_sequence()
+        # STEP 3: acquire results
         acquisition_results = {}
-        for name in self.instruments:
-            if "readout" in roles[name]:
-                if not instrument_pulses[name].is_empty:
-                    if not instrument_pulses[name].ro_pulses.is_empty:
-                        if all([pulse.serial in changed for pulse in instrument_pulses[name].ro_pulses]):
-                            # FIXME: for precision sweep in resonator spectroscopy
-                            # change necessary to perform precision sweep
-                            # TODO: move this to instruments (ask Alvaro)
-                            # TODO: check if this will work with multiplex
-                            for sequencers in self.instruments[name]._sequencers.values():
-                                for sequencer in sequencers:
-                                    sequencer.pulses = instrument_pulses[name].ro_pulses
-                        results = self.instruments[name].acquire()
-                        existing_keys = set(acquisition_results.keys()) & set(results.keys())
-                        for key, value in results.items():
-                            if key in existing_keys:
-                                acquisition_results[key].update(value)
-                            else:
-                                acquisition_results[key] = value
+        for instrument in readout_instruments:
+            if instrument_pulses[instrument.name] and instrument_pulses[instrument.name].ro_pulses:
+                results = instrument.acquire()
+                existing_keys = set(acquisition_results.keys()) & set(results.keys())
+                for key, value in results.items():
+                    if key in existing_keys:
+                        acquisition_results[key].update(value)
+                    else:
+                        acquisition_results[key] = value
+
+        data = {}
+        for serial in acquisition_results:
+            for if_pulse, original in changed.items():
+                if serial == if_pulse.serial:
+                    data[original] = data[if_pulse.qubit] = ExecutionResults.from_components(
+                        *acquisition_results[serial]
+                    )
 
-        # change back the frequency of the pulses
-        for name in self.instruments:
-            roles[name] = self.settings["instruments"][name]["roles"]
-            if "readout" in roles[name]:
-                instrument_pulses[name] = sequence.get_channel_pulses(*self.instruments[name].channels)
-                for pulse in instrument_pulses[name]:
-                    if pulse.serial in changed:
-                        pippo = acquisition_results[pulse.serial]
-                        # if abs(pulse.frequency) > 300e6:
-                        pulse.frequency += self.get_lo_readout_frequency(pulse.qubit)
-                        acquisition_results[pulse.serial] = pippo
-            if "control" in roles[name]:
-                instrument_pulses[name] = sequence.get_channel_pulses(*self.instruments[name].channels)
-                for pulse in instrument_pulses[name]:
-                    if pulse.serial in changed:
-                        pulse.frequency += self.get_lo_drive_frequency(pulse.qubit)
-
-        for ro_pulse in ro_pulses.values():
-            data[ro_pulse.serial] = ExecutionResults.from_components(*acquisition_results[ro_pulse.serial])
-            data[ro_pulse.qubit] = copy.copy(data[ro_pulse.serial])
         return data
 
     def sweep(self, sequence, *sweepers, nshots=1024, average=True, relaxation_time=None):
         results = {}
         sweeper_pulses = {}
-
         # create copy of the sequence
         copy_sequence = copy.deepcopy(sequence)
         map_original_shifted = {pulse: pulse.serial for pulse in copy.deepcopy(copy_sequence).ro_pulses}
 
         # create dictionary containing pulses for each sweeper that point to the same original sequence
         # which is copy_sequence
         for sweeper in sweepers:
@@ -279,14 +364,15 @@
             nshots=nshots,
             average=average,
             relaxation_time=relaxation_time,
             results=results,
             sweeper_pulses=sweeper_pulses,
             map_original_shifted=map_original_shifted,
         )
+
         return results
 
     def _sweep_recursion(
         self,
         sequence,
         original_sequence,
         *sweepers,
@@ -296,16 +382,15 @@
         results=None,
         sweeper_pulses=None,
         map_original_shifted=None,
     ):
         sweeper = sweepers[0]
 
         # store values before starting to sweep
-        if sweeper.pulses is not None:
-            original_value = self._save_original_value(sweeper, sweeper_pulses)
+        original_value = self._save_original_value(sweeper, sweeper_pulses)
 
         # perform sweep recursively
         for value in sweeper.values:
             self._update_pulse_sequence_parameters(
                 sweeper, sweeper_pulses, original_sequence, map_original_shifted, value
             )
             if len(sweepers) > 1:
@@ -319,79 +404,84 @@
                     results=results,
                     sweeper_pulses=sweeper_pulses,
                     map_original_shifted=map_original_shifted,
                 )
             else:
                 new_sequence = copy.deepcopy(sequence)
                 result = self.execute_pulse_sequence(new_sequence, nshots)
-
                 # colllect result and append to original pulse
                 for original_pulse, new_serial in map_original_shifted.items():
-                    acquisition = result[new_serial].compute_average() if average else result[new_serial]
+                    acquisition = result[new_serial].average if average else result[new_serial]
 
-                    if results:
+                    if original_pulse.serial in results:
                         results[original_pulse.serial] += acquisition
                         results[original_pulse.qubit] += acquisition
                     else:
                         results[original_pulse.serial] = acquisition
                         results[original_pulse.qubit] = copy.copy(results[original_pulse.serial])
 
-        # restore initial value of the pul
-        if sweeper.pulses is not None:
-            self._restore_initial_value(sweeper, sweeper_pulses, original_value)
+        # restore initial value of the pulse
+        self._restore_initial_value(sweeper, sweeper_pulses, original_value)
 
     def _save_original_value(self, sweeper, sweeper_pulses):
         """Helper method for _sweep_recursion"""
         original_value = {}
-        pulses = sweeper_pulses[sweeper.parameter]
         # save original value of the parameter swept
-        for pulse in pulses:
-            if sweeper.parameter is Parameter.attenuation:
-                original_value[pulse] = self.get_attenuation(pulses[pulse].qubit)
-            elif sweeper.parameter is Parameter.gain:
-                original_value[pulse] = self.get_gain(pulses[pulse].qubit)
-            elif sweeper.parameter is Parameter.bias:
-                original_value[pulse] = self.get_bias(pulses[pulse].qubit)
-            else:
+        if sweeper.pulses is not None:
+            pulses = sweeper_pulses[sweeper.parameter]
+            for pulse in pulses:
                 original_value[pulse] = getattr(pulses[pulse], sweeper.parameter.name)
 
+        if sweeper.qubits is not None:
+            for qubit in sweeper.qubits:
+                if sweeper.parameter is Parameter.attenuation:
+                    original_value[qubit.name] = self.get_attenuation(qubit)
+                elif sweeper.parameter is Parameter.gain:
+                    original_value[qubit.name] = self.get_gain(qubit)
+                elif sweeper.parameter is Parameter.bias:
+                    original_value[qubit.name] = self.get_bias(qubit)
+
         return original_value
 
     def _restore_initial_value(self, sweeper, sweeper_pulses, original_value):
         """Helper method for _sweep_recursion"""
-        pulses = sweeper_pulses[sweeper.parameter]
-        for pulse in pulses:
-            if sweeper.parameter is Parameter.attenuation:
-                self.set_attenuation(pulses[pulse].qubit, original_value[pulse])
-            elif sweeper.parameter is Parameter.gain:
-                self.set_gain(pulses[pulse].qubit, original_value[pulse])
-            elif sweeper.parameter is Parameter.bias:
-                self.set_bias(pulses[pulse].qubit, original_value[pulse])
-            else:
+        if sweeper.pulses is not None:
+            pulses = sweeper_pulses[sweeper.parameter]
+            for pulse in pulses:
                 setattr(pulses[pulse], sweeper.parameter.name, original_value[pulse])
 
+        if sweeper.qubits is not None:
+            for qubit in sweeper.qubits:
+                if sweeper.parameter is Parameter.attenuation:
+                    self.set_attenuation(qubit, original_value[qubit.name])
+                elif sweeper.parameter is Parameter.gain:
+                    self.set_gain(qubit, original_value[qubit.name])
+                elif sweeper.parameter is Parameter.bias:
+                    self.set_bias(qubit, original_value[qubit.name])
+
     def _update_pulse_sequence_parameters(
         self, sweeper, sweeper_pulses, original_sequence, map_original_shifted, value
     ):
         """Helper method for _sweep_recursion"""
         if sweeper.pulses is not None:
             pulses = sweeper_pulses[sweeper.parameter]
             for pulse in pulses:
+                update_value = value
                 if sweeper.parameter is Parameter.frequency:
                     if pulses[pulse].type is PulseType.READOUT:
-                        value += self.qubits[pulses[pulse].qubit].readout_frequency
+                        update_value += self.qubits[pulses[pulse].qubit].readout_frequency
                     else:
-                        value += self.qubits[pulses[pulse].qubit].drive_frequency
-                    setattr(pulses[pulse], sweeper.parameter.name, value)
+                        update_value += self.qubits[pulses[pulse].qubit].drive_frequency
+                    setattr(pulses[pulse], sweeper.parameter.name, update_value)
                 elif sweeper.parameter is Parameter.amplitude:
                     if pulses[pulse].type is PulseType.READOUT:
                         current_amplitude = self.native_gates["single_qubit"][pulses[pulse].qubit]["MZ"]["amplitude"]
                     else:
                         current_amplitude = self.native_gates["single_qubit"][pulses[pulse].qubit]["RX"]["amplitude"]
-                    setattr(pulses[pulse], sweeper.parameter.name, float(current_amplitude * value))
+                    setattr(pulses[pulse], sweeper.parameter.name, float(current_amplitude * update_value))
                 if pulses[pulse].type is PulseType.READOUT:
                     to_modify = [
                         pulse1 for pulse1 in original_sequence.ro_pulses if pulse1.qubit == pulses[pulse].qubit
                     ]
                     if to_modify:
                         map_original_shifted[to_modify[0]] = pulses[pulse].serial
```

### Comparing `qibolab-0.0.2/src/qibolab/pulses.py` & `qibolab-0.0.3/src/qibolab/pulses.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,18 @@
 
         modulated_waveform_i = Waveform(mod_signals[:, 0])
         modulated_waveform_i.serial = f"Modulated_Waveform_I(num_samples = {num_samples}, amplitude = {format(pulse.amplitude, '.6f').rstrip('0').rstrip('.')}, shape = {str(pulse.shape)}, frequency = {format(pulse.frequency, '_')}, phase = {format(global_phase + pulse.relative_phase, '.6f').rstrip('0').rstrip('.')})"
         modulated_waveform_q = Waveform(mod_signals[:, 1])
         modulated_waveform_q.serial = f"Modulated_Waveform_Q(num_samples = {num_samples}, amplitude = {format(pulse.amplitude, '.6f').rstrip('0').rstrip('.')}, shape = {str(pulse.shape)}, frequency = {format(pulse.frequency, '_')}, phase = {format(global_phase + pulse.relative_phase, '.6f').rstrip('0').rstrip('.')})"
         return (modulated_waveform_i, modulated_waveform_q)
 
+    def __eq__(self, item) -> bool:
+        """Overloads == operator"""
+        return type(item) is self.__class__
+
 
 class Rectangular(PulseShape):
     """
     Rectangular pulse shape.
 
     """
 
@@ -223,14 +227,20 @@
     """
 
     def __init__(self, rel_sigma: float):
         self.name = "Gaussian"
         self.pulse: Pulse = None
         self.rel_sigma: float = float(rel_sigma)
 
+    def __eq__(self, item) -> bool:
+        """Overloads == operator"""
+        if super().__eq__(item):
+            return self.rel_sigma == item.rel_sigma
+        return False
+
     @property
     def envelope_waveform_i(self) -> Waveform:
         """The envelope waveform of the i component of the pulse."""
 
         if self.pulse:
             num_samples = int(np.rint(self.pulse.duration / 1e9 * PulseShape.SAMPLING_RATE))
             x = np.arange(0, num_samples, 1)
@@ -277,14 +287,20 @@
 
     def __init__(self, rel_sigma, beta):
         self.name = "Drag"
         self.pulse: Pulse = None
         self.rel_sigma = float(rel_sigma)
         self.beta = float(beta)
 
+    def __eq__(self, item) -> bool:
+        """Overloads == operator"""
+        if super().__eq__(item):
+            return self.rel_sigma == item.rel_sigma and self.beta == item.beta
+        return False
+
     @property
     def envelope_waveform_i(self) -> Waveform:
         """The envelope waveform of the i component of the pulse."""
 
         if self.pulse:
             num_samples = int(np.rint(self.pulse.duration / 1e9 * PulseShape.SAMPLING_RATE))
             x = np.arange(0, num_samples, 1)
@@ -346,14 +362,20 @@
         self.name = "IIR"
         self.target: PulseShape = target
         self._pulse: Pulse = None
         self.a: np.ndarray = np.array(a)
         self.b: np.ndarray = np.array(b)
         # Check len(a) = len(b) = 2
 
+    def __eq__(self, item) -> bool:
+        """Overloads == operator"""
+        if super().__eq__(item):
+            return self.target == item.target and (self.a == item.a).all() and (self.b == item.b).all()
+        return False
+
     @property
     def pulse(self):
         return self._pulse
 
     @pulse.setter
     def pulse(self, value):
         self._pulse = value
@@ -418,14 +440,20 @@
 
     def __init__(self, t_half_flux_pulse=None, b_amplitude=1):
         self.name = "SNZ"
         self.pulse: Pulse = None
         self.t_half_flux_pulse: float = t_half_flux_pulse
         self.b_amplitude: float = b_amplitude
 
+    def __eq__(self, item) -> bool:
+        """Overloads == operator"""
+        if super().__eq__(item):
+            return self.t_half_flux_pulse == item.t_half_flux_pulse and self.b_amplitude == item.b_amplitude
+        return False
+
     @property
     def envelope_waveform_i(self) -> Waveform:
         """The envelope waveform of the i component of the pulse."""
 
         if self.pulse:
             if not self.t_half_flux_pulse:
                 self.t_half_flux_pulse = self.pulse.duration / 2
@@ -481,14 +509,20 @@
     """
 
     def __init__(self, alpha: float):
         self.name = "eCap"
         self.pulse: Pulse = None
         self.alpha: float = float(alpha)
 
+    def __eq__(self, item) -> bool:
+        """Overloads == operator"""
+        if super().__eq__(item):
+            return self.alpha == item.alpha
+        return False
+
     @property
     def envelope_waveform_i(self) -> Waveform:
         if self.pulse:
             num_samples = int(self.pulse.duration / 1e9 * PulseShape.SAMPLING_RATE)
             x = np.arange(0, num_samples, 1)
             waveform = Waveform(
                 self.pulse.amplitude
@@ -600,45 +634,63 @@
         del self._duration
         del self._finish
         # del self._shape TODO activate when returning a deep copy of shape or when making a deep copy of shape in init
 
     @property
     def start(self) -> int:
         """Returns the time when the pulse is scheduled to be played, in ns."""
-
-        return self._start.value
+        if isinstance(self._start, se_int):
+            return self._start.value
+        else:
+            return self._start
 
     @start.setter
     def start(self, value):
         """Sets the time when the pulse is scheduled to be played.
 
         Args:
             value (se_int | int | np.integer): the time in ns.
         """
 
         if not isinstance(value, (se_int, int, np.integer)):
             raise TypeError(f"start argument type should be intSymbolicExpression or int, got {type(value).__name__}")
         elif not value >= 0:
             raise ValueError(f"start argument must be >= 0, got {value}")
+
         if isinstance(value, se_int):
-            # self._start = value
-            # self._start = intSymbolicExpression(value)
             self._start = se_int(value.symbol)["_p" + str(self._id) + "_start"]
-        elif isinstance(value, np.integer):
-            self._start = se_int(int(value))["_p" + str(self._id) + "_start"]
-        elif isinstance(value, int):
-            self._start = se_int(value)["_p" + str(self._id) + "_start"]
-        if self._duration:
-            self._finish = (self._start + self._duration)["_p" + str(self._id) + "_finish"]
+
+        elif isinstance(self._start, se_int):
+            if isinstance(value, np.integer):
+                self._start.value = int(value)
+            elif isinstance(value, int):
+                self._start.value = value
+        else:
+            if isinstance(value, np.integer):
+                self._start = int(value)
+            elif isinstance(value, int):
+                self._start = value
+
+        if not self._duration is None:
+            if (
+                isinstance(self._start, se_int)
+                or isinstance(self._duration, se_int)
+                or isinstance(self._finish, se_int)
+            ):
+                self._finish = se_int(self._start + self._duration)["_p" + str(self._id) + "_finish"]
+            else:
+                self._finish = self._start + self._duration
 
     @property
     def duration(self) -> int:
         """Returns the duration of the pulse, in ns."""
-
-        return self._duration.value
+        if isinstance(self._duration, se_int):
+            return self._duration.value
+        else:
+            return self._duration
 
     @duration.setter
     def duration(self, value):
         """Sets the duration of the pulse.
 
         Args:
             value (se_int | int | np.integer): the time in ns.
@@ -648,46 +700,69 @@
             raise TypeError(
                 f"duration argument type should be intSymbolicExpression or int, got {type(value).__name__}"
             )
         elif not value >= 0:
             raise ValueError(f"duration argument must be >= 0, got {value}")
         if isinstance(value, se_int):
             self._duration = se_int(value.symbol)["_p" + str(self._id) + "_duration"]
-        elif isinstance(value, np.integer):
-            self._duration = se_int(int(value))["_p" + str(self._id) + "_duration"]
-        elif isinstance(value, int):
-            self._duration = se_int(value)["_p" + str(self._id) + "_duration"]
-        if self._start:
-            self._finish = (self._start + self._duration)["_p" + str(self._id) + "_finish"]
+
+        elif isinstance(self._duration, se_int):
+            if isinstance(value, np.integer):
+                self._duration.value = int(value)
+            elif isinstance(value, int):
+                self._duration.value = value
+        else:
+            if isinstance(value, np.integer):
+                self._duration = int(value)
+            elif isinstance(value, int):
+                self._duration = value
+
+        if not self._start is None:
+            if (
+                isinstance(self._start, se_int)
+                or isinstance(self._duration, se_int)
+                or isinstance(self._finish, se_int)
+            ):
+                self._finish = se_int(self._start + self._duration)["_p" + str(self._id) + "_finish"]
+            else:
+                self._finish = self._start + self._duration
 
     @property
     def finish(self) -> int:
         """Returns the time when the pulse is scheduled to finish.
 
         Calculated as pulse.start - pulse finish.
         """
-
-        return self._finish.value
+        if isinstance(self._finish, se_int):
+            return self._finish.value
+        else:
+            return self._finish
 
     @property
     def se_start(self) -> se_int:
         """Returns a symbolic expression for the pulse start."""
 
+        if not isinstance(self._start, se_int):
+            self._start = se_int(self._start)["_p" + str(self._id) + "_start"]
         return self._start
 
     @property
     def se_duration(self) -> se_int:
         """Returns a symbolic expression for the pulse duration."""
 
+        if not isinstance(self._duration, se_int):
+            self._duration = se_int(self._duration)["_p" + str(self._id) + "_duration"]
         return self._duration
 
     @property
     def se_finish(self) -> se_int:
         """Returns a symbolic expression for the pulse finish."""
 
+        if not isinstance(self._finish, se_int):
+            self._finish = se_int(self._finish)["_p" + str(self._id) + "_finish"]
         return self._finish
 
     @property
     def amplitude(self) -> float:
         """Returns the amplitude of the pulse.
 
         Pulse amplitudes are normalised between -1 and 1.
@@ -739,15 +814,15 @@
     def global_phase(self):
         """Returns the global phase of the pulse, in radians.
 
         This phase is calculated from the pulse start time and frequency as `2 * pi * frequency * start`.
         """
 
         # pulse start, duration and finish are in ns
-        return 2 * np.pi * self._frequency * self._start.value / 1e9
+        return 2 * np.pi * self._frequency * self.start / 1e9
 
     @property
     def relative_phase(self) -> float:
         """Returns the relative phase of the pulse, in radians."""
 
         return self._relative_phase
 
@@ -768,15 +843,15 @@
 
     @property
     def phase(self) -> float:
         """Returns the total phase of the pulse, in radians.
 
         The total phase is computed as the sum of the global and relative phases.
         """
-        return 2 * np.pi * self._frequency * self._start.value / 1e9 + self._relative_phase
+        return 2 * np.pi * self._frequency * self.start / 1e9 + self._relative_phase
 
     @property
     def shape(self) -> PulseShape:
         """Returns the shape of the pulse, as a PulseShape object."""
 
         return self._shape
 
@@ -966,14 +1041,27 @@
             self._relative_phase,
             self._shape,
             self._channel,
             self._type,
             self._qubit,
         )
 
+    def is_equal_ignoring_start(self, item) -> bool:
+        """Check if two pulses are equal ignoring start time"""
+        return (
+            self.duration == item.duration
+            and self.amplitude == item.amplitude
+            and self.frequency == item.frequency
+            and self.relative_phase == item.relative_phase
+            and self.shape == item.shape
+            and self.channel == item.channel
+            and self.type == item.type
+            and self.qubit == item.qubit
+        )
+
     def plot(self, savefig_filename=None):
         """Plots the pulse envelope and modulated waveforms.
 
         Args:
             savefig_filename (str): a file path. If provided the plot is save to a file.
         """
 
@@ -1057,14 +1145,29 @@
 
     @property
     def global_phase(self):
         # readout pulses should have zero global phase so that we can
         # calculate probabilities in the i-q plane
         return 0
 
+    def copy(self):  # -> Pulse|ReadoutPulse|DrivePulse|FluxPulse:
+        """Returns a new Pulse object with the same attributes."""
+
+        # return eval(self.serial)
+        return ReadoutPulse(
+            self.start,
+            self.duration,
+            self.amplitude,
+            self.frequency,
+            self.relative_phase,
+            repr(self._shape),  # self._shape,
+            self.channel,
+            self.qubit,
+        )
+
 
 class DrivePulse(Pulse):
     """Describes a qubit drive pulse.
 
     See :class:`qibolab.pulses.Pulse` for argument desciption.
     """
 
@@ -1435,15 +1538,15 @@
             if isinstance(item, Pulse):
                 pulse = item
                 self.pulses.append(pulse)
             elif isinstance(item, PulseSequence):
                 ps = item
                 for pulse in ps.pulses:
                     self.pulses.append(pulse)
-        self.pulses.sort(key=lambda item: (item.channel, item.start))
+        self.pulses.sort(key=lambda item: (item.start, item.channel))
 
     def index(self, pulse):
         """Returns the index of a pulse in the sequence."""
 
         return self.pulses.index(pulse)
 
     def pop(self, index=-1):
@@ -1466,21 +1569,21 @@
         """Returns a shallow copy of the sequence.
 
         It returns a new PulseSequence object with references to the same Pulse objects.
         """
 
         return PulseSequence(*self.pulses)
 
-    def deep_copy(self):
+    def copy(self):
         """Returns a deep copy of the sequence.
 
         It returns a new PulseSequence with replicates of each of the pulses contained in the original sequence.
         """
 
-        return PulseSequence(*[pulse.deep_copy() for pulse in self.pulses])
+        return PulseSequence(*[pulse.copy() for pulse in self.pulses])
 
     @property
     def ro_pulses(self):
         """Returns a new PulseSequence containing only its readout pulses."""
 
         new_pc = PulseSequence()
         for pulse in self.pulses:
```

### Comparing `qibolab-0.0.2/src/qibolab/result.py` & `qibolab-0.0.3/src/qibolab/result.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,43 +5,14 @@
 import numpy as np
 import numpy.typing as npt
 
 ExecRes = np.dtype([("i", np.float64), ("q", np.float64)])
 
 
 @dataclass
-class AveragedResults:
-    """Data structure containing averages of ``ExecutionResults``."""
-
-    i: npt.NDArray[np.float64]
-    q: npt.NDArray[np.float64]
-
-    def __add__(self, data):
-        i = np.append(self.i, data.i)
-        q = np.append(self.q, data.q)
-
-        new_execution_results = self.__class__(i, q)
-
-        return new_execution_results
-
-    def to_dict(self):
-        """Serialize output in dict"""
-
-        return {
-            "MSR[V]": np.sqrt(self.i**2 + self.q**2),
-            "i[V]": self.i,
-            "q[V]": self.q,
-            "phase[rad]": np.angle(self.i + 1.0j * self.q),
-        }
-
-    def __len__(self):
-        return len(self.i)
-
-
-@dataclass
 class ExecutionResults:
     """Data structure to deal with the output of :func:`qibolab.platforms.abstract.AbstractPlatform.execute_pulse_sequence`"""
 
     array: npt.NDArray[ExecRes]
     shots: Optional[npt.NDArray[np.uint32]] = None
 
     @classmethod
@@ -57,18 +28,27 @@
         return self.array.i
 
     @property
     def q(self):
         return self.array.q
 
     def __add__(self, data):
-        i = np.append(self.i, data.i, axis=0)
-        q = np.append(self.q, data.q, axis=0)
+        assert len(data.i.shape) == len(data.q.shape)
+        if data.shots is not None:
+            assert len(data.i.shape) == len(data.shots.shape)
+        # concatenate on first dimension; if a scalar is passed, just append it
+        axis = 0 if len(data.i.shape) > 0 else None
+        i = np.append(self.i, data.i, axis=axis)
+        q = np.append(self.q, data.q, axis=axis)
+        if data.shots is not None:
+            shots = np.append(self.shots, data.shots, axis=axis)
+        else:
+            shots = None
 
-        new_execution_results = self.__class__.from_components(i, q)
+        new_execution_results = self.__class__.from_components(i, q, shots)
 
         return new_execution_results
 
     @cached_property
     def measurement(self):
         """Resonator signal voltage mesurement (MSR) in volts."""
         return np.sqrt(self.i**2 + self.q**2)
@@ -81,42 +61,41 @@
         # return signal.detrend(np.unwrap(phase))
 
     @cached_property
     def ground_state_probability(self):
         """Computes ground state probability"""
         return 1 - np.mean(self.shots)
 
-    def to_dict_probability(self, state=1):
+    def raw_probability(self, state=1):
         """Serialize probabilities in dict.
         Args:
             state (int): if 0 stores the probabilities of finding
                         the ground state. If 1 stores the
                         probabilities of finding the excited state.
         """
         if state == 1:
             return {"probability": 1 - self.ground_state_probability}
         elif state == 0:
             return {"probability": self.ground_state_probability}
 
-    def compute_average(self):
+    @property
+    def average(self):
         """Perform average over i and q"""
-        return AveragedResults(self.array.i.mean(), self.array.q.mean())
+        return AveragedResults.from_components(np.mean(self.i), np.mean(self.q))
 
-    def to_dict(self, average=True):
-        """Serialize output in dict.
-        Args:
-            average (bool): If `True` returns a dictionary of the form
-                            {'MSR[V]' : v, 'i[V]' : i, 'q[V]' : q, 'phase[rad]' : phase}.
-                            Where each value is averaged over the number shots. If `False`
-                            all the values for each shot are saved.
-        """
-        results = self.compute_average() if average else self
+    @property
+    def raw(self):
+        """Serialize output in dict."""
 
         return {
-            "MSR[V]": np.sqrt(results.i**2 + results.q**2),
-            "i[V]": results.i,
-            "q[V]": results.q,
-            "phase[rad]": np.angle(results.i + 1.0j * results.q),
+            "MSR[V]": self.measurement,
+            "i[V]": self.i,
+            "q[V]": self.q,
+            "phase[rad]": self.phase,
         }
 
     def __len__(self):
         return len(self.i)
+
+
+class AveragedResults(ExecutionResults):
+    """Data structure containing averages of ``ExecutionResults``."""
```

### Comparing `qibolab-0.0.2/src/qibolab/runcards/dummy.yml` & `qibolab-0.0.3/src/qibolab/runcards/dummy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 nqubits: 5
 description: QuantWare 5-qubit device.
 
 qubits: [0, 1, 2, 3, 4]
 
 settings:
     sampling_rate: 1000000000
-    repetition_duration: 0
+    relaxation_time: 0
 
 resonator_type: 2D
 
 topology: # qubit - qubit connections
 -   [ 1, 0, 1, 0, 0, 0]
 -   [ 0, 1, 1, 0, 0, 0]
 -   [ 1, 1, 1, 1, 1, 0]
@@ -154,25 +154,23 @@
               phase: -1.5707963267948966
               qubit: 3
 
 
 characterization:
     single_qubit:
         0:
-            readout_frequency: 0.0
+            readout_frequency: 7_226_500_000
             drive_frequency: 0.0
             T1: 0.0
             T2: 0.0
             sweetspot: 0.0
             filter: {}
             # parameters for single shot classification
             threshold: 0.0
             iq_angle: 0.0
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
             mixer_readout_g: 0.0
             mixer_readout_phi: 0.0
         1:
             readout_frequency: 7_453_265_000
@@ -180,16 +178,14 @@
             T1: 0.0
             T2: 0.0
             sweetspot: -0.047
             filter: {}
             # parameters for single shot classification
             threshold: 0.00028502261712637096
             iq_angle: 1.283105298787488
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 63.214
             # Software classifier
             # classifier:
             #     type: "scikit"
             #     model: "qw5q_gold/RBF_SVM_1.pkl"
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
@@ -207,54 +203,48 @@
             # parameters for single shot classification
             threshold: 0.0002694329123116206
             iq_angle: 4.912447775569025
             # Software classifier
             # classifier:
             #     type: "scikit"
             #     model: "qw5q_gold/RBF_SVM_2.pkl"
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
             mixer_readout_g: 0.0
             mixer_readout_phi: 0.0
         3:
-            readout_frequency: 7_802_391_000
+            readout_frequency: 7_802_191_000
             drive_frequency: 6_760_700_000
             T1: 0.0
             T2: 0.0
             sweetspot: 0.034
             filter: {}
             # parameters for single shot classification
             threshold: 0.0003363427381347193
             iq_angle: 1.6124890998581591
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
             # Software classifier
             # classifier:
             #     type: "scikit"
             #     model: "qw5q_gold/RBF_SVM_3.pkl"
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
             mixer_readout_g: 0.0
-            mixer_readout_phi: 0.0
+            mixer_readout_phi: 0.00
         4:
             readout_frequency: 8_057_668_000
             drive_frequency: 6_585_053_000
             T1: 0.0
             T2: 0.0
             sweetspot: -0.057
             filter: {}
             # parameters for single shot classification
             threshold: 0.00013079660165463033
             iq_angle: 5.6303684840135
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
             # Software classifier
             # classifier:
             #     type: "scikit"
             #     model: "qw5q_gold/RBF_SVM_4.pkl"
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
@@ -266,14 +256,12 @@
             T1: 0.0
             T2: 0.0
             sweetspot: 0.0
             filter: {}
             # parameters for single shot classification
             threshold: 0.0
             iq_angle: 0.0
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
             mixer_readout_g: 0.0
             mixer_readout_phi: 0.0
```

### Comparing `qibolab-0.0.2/src/qibolab/runcards/icarusq.yml` & `qibolab-0.0.3/src/qibolab/runcards/icarusq.yml`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/runcards/multiqubit_icarusq.yml` & `qibolab-0.0.3/src/qibolab/runcards/multiqubit_icarusq.yml`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/runcards/multiqubit_icarusqfpga.yml` & `qibolab-0.0.3/src/qibolab/runcards/multiqubit_icarusqfpga.yml`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.2/src/qibolab/runcards/qili1q_os2.yml` & `qibolab-0.0.3/src/qibolab/runcards/qili1q_os2.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 nqubits: 1
 description: 1-qubit device OS2 in XLD fridge, controlled with qblox cluster rf.
 
 settings:
     hardware_avg: 1024
-    repetition_duration: 200_000
+    relaxation_time: 200_000
     sampling_rate: 1_000_000_000
 
 qubits: [0]
 
 resonator_type: 3D
 
 topology: # qubit - qubit connections
@@ -63,15 +63,15 @@
         lib: qblox
         class: ClusterQCM_RF
         address: 192.168.0.6:8
         roles: [control]
         settings:
             ports:
                 o1:
-                    attenuation                  : 0 # (dB)
+                    attenuation                  : 12 # (dB)
                     lo_enabled                   : true
                     lo_frequency                 : 5_179_856_329 # (Hz) from 2e9 to 18e9
                     gain                         : 0.35 # for path0 and path1 -1.0<=v<=1.0
                     hardware_mod_en              : false
                 o2:
                     attenuation                  : 60 # (dB)
                     lo_enabled                   : true
@@ -79,17 +79,17 @@
                     gain                         : 0 # for path0 and path1 -1.0<=v<=1.0
                     hardware_mod_en              : false
 
             channel_port_map:
                 'L3-17_qd': o1 # IQ Port = out0 & out1
                 99: o2
     twpa_pump:
-        lib: rohde_schwarz
-        class: SGS100A
-        address: 192.168.0.37
+        lib: erasynth
+        class: ERA
+        address: /dev/ttyERA
         roles: [other]
         settings:
             frequency: 6.816e+9 # Hz
             power: 2.3 # dBm
 
 native_gates:
     single_qubit:
```

### Comparing `qibolab-0.0.2/src/qibolab/runcards/qw5q_gold.yml` & `qibolab-0.0.3/src/qibolab/runcards/qw5q_gold.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 nqubits: 5
 description: QuantWare 5-qubit device.
 
 qubits: [0, 1, 2, 3, 4, 5]
 
 settings:
     sampling_rate: 1000000000
-    repetition_duration: 50_000
+    relaxation_time: 50_000
 
 resonator_type: 2D
 
 topology: # qubit - qubit connections
 -   [ 1, 0, 1, 0, 0, 0]
 -   [ 0, 1, 1, 0, 0, 0]
 -   [ 1, 1, 1, 1, 1, 0]
@@ -163,17 +163,15 @@
             drive_frequency: 0.0
             T1: 0.0
             T2: 0.0
             sweetspot: 0.0
             filter: {}
             # parameters for single shot classification
             threshold: 0.0
-            iq_angle: 0.0
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
+            iq_angle: 0.00
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
             mixer_readout_g: 0.0
             mixer_readout_phi: 0.0
         1:
             readout_frequency: 7_453_265_000
@@ -181,16 +179,14 @@
             T1: 0.0
             T2: 0.0
             sweetspot: -0.047
             filter: {}
             # parameters for single shot classification
             threshold: 0.00028502261712637096
             iq_angle: 1.283105298787488
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 63.214
             # Software classifier
             # classifier:
             #     type: "scikit"
             #     model: "qw5q_gold/RBF_SVM_1.pkl"
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
@@ -208,16 +204,14 @@
             # parameters for single shot classification
             threshold: 0.0002694329123116206
             iq_angle: 4.912447775569025
             # Software classifier
             # classifier:
             #     type: "scikit"
             #     model: "qw5q_gold/RBF_SVM_2.pkl"
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
             mixer_readout_g: 0.0
             mixer_readout_phi: 0.0
         3:
             readout_frequency: 7_802_391_000
@@ -225,16 +219,14 @@
             T1: 0.0
             T2: 0.0
             sweetspot: 0.034
             filter: {}
             # parameters for single shot classification
             threshold: 0.0003363427381347193
             iq_angle: 1.6124890998581591
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
             # Software classifier
             # classifier:
             #     type: "scikit"
             #     model: "qw5q_gold/RBF_SVM_3.pkl"
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
@@ -246,16 +238,14 @@
             T1: 0.0
             T2: 0.0
             sweetspot: -0.057
             filter: {}
             # parameters for single shot classification
             threshold: 0.00013079660165463033
             iq_angle: 5.6303684840135
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
             # Software classifier
             # classifier:
             #     type: "scikit"
             #     model: "qw5q_gold/RBF_SVM_4.pkl"
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
@@ -267,14 +257,12 @@
             T1: 0.0
             T2: 0.0
             sweetspot: 0.0
             filter: {}
             # parameters for single shot classification
             threshold: 0.0
             iq_angle: 0.0
-            # required for integration weights (not sure if it should be here)
-            rotation_angle: 0.0
             # required for mixers (not sure if it should be here)
             mixer_drive_g: 0.0
             mixer_drive_phi: 0.0
             mixer_readout_g: 0.0
             mixer_readout_phi: 0.0
```

### Comparing `qibolab-0.0.2/src/qibolab/sweeper.py` & `qibolab-0.0.3/src/qibolab/sweeper.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 class Parameter(Enum):
     """Sweeping parameters."""
 
     frequency = auto()
     amplitude = auto()
     relative_phase = auto()
+    delay = auto()
 
     attenuation = auto()
     gain = auto()
     bias = auto()
 
 
 QubitParameter = {Parameter.bias, Parameter.attenuation, Parameter.gain}
```

### Comparing `qibolab-0.0.2/src/qibolab/symbolic.py` & `qibolab-0.0.3/src/qibolab/symbolic.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,27 @@
         import sys
 
         num_items = len(SymbolicExpression.instances)
         n = 0
         while len(SymbolicExpression.instances) > 0:
             symbol = list(SymbolicExpression.instances)[n]
             item = SymbolicExpression.instances[symbol]
-            if sys.getrefcount(item) < 4:
-                del SymbolicExpression.instances[symbol]
+
+            external_ref_count = sys.getrefcount(item)
+            import re
+
+            internal_ref_count = 0
+            for se in list(SymbolicExpression.instances):
+                if re.search(rf"\b{re.escape(symbol)}\b", SymbolicExpression.instances[se].expression):
+                    internal_ref_count += 1
+
+            if not internal_ref_count and external_ref_count < 4:
                 # DEBUG SymbolicExpression Garbage Collector Activity
-                # print(f'deleted {symbol}')
+                # print(f'deleting {symbol} with refcount {external_ref_count}')
+                del SymbolicExpression.instances[symbol]
                 num_items = len(SymbolicExpression.instances)
                 n = 0
             else:
                 n += 1
             if n == num_items:
                 break
```

### Comparing `qibolab-0.0.2/src/qibolab/transpilers/connectivity.py` & `qibolab-0.0.3/src/qibolab/transpilers/star_connectivity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+from dataclasses import dataclass
+
 from qibo import gates
 from qibo.config import log, raise_error
 
+from qibolab.transpilers.abstract import Transpiler
+
 
 def find_connected_qubit(qubits, queue, hardware_qubits):
     """Helper method for :meth:`qibolab.transpilers.fix_connecivity`.
 
     Finds which qubit should be mapped to hardware middle qubit
     by looking at the two-qubit gates that follow.
     """
@@ -17,126 +21,136 @@
                 return qubits[0]
             elif len(possible_qubits) == 1:
                 return possible_qubits.pop()
     # freedom of choice
     return qubits[0]
 
 
-def fix_connectivity(circuit, middle_qubit=2):
+@dataclass
+class StarConnectivity(Transpiler):
     """Transforms an arbitrary circuit to one that can be executed on hardware.
 
-    This method produces a circuit that respects the following connectivity:
-          q
-          |
-     q -- q -- q
-          |
-          q
-    by adding SWAP gates when needed.
-    It does not translate gates to native.
-
-    Args:
-        circuit (qibo.models.Circuit): The original Qibo circuit to transform.
-            This circuit must contain up to two-qubit gates.
-        middle_qubit (int): Hardware middle qubit.
-
-    Returns:
-        new (qibo.models.Circuit): Qibo circuit that performs the same operation
-            as the original but respects the hardware connectivity.
-        hardware_qubits (list): List that maps logical to hardware qubits.
-            This is required for transforming final measurements.
+    This transpiler produces a circuit that respects the following connectivity:
+        q
+        |
+    q -- q -- q
+        |
+        q
+    by adding SWAP gates when needed. It does not translate gates to native.
     """
-    # TODO: Change this to a more lightweight form that takes a list of pairs
-    # instead of the whole circuit.
 
-    # find the number of qubits for hardware circuit
-    if circuit.nqubits == 1:
-        nqubits = 1
-    else:
-        nqubits = max(circuit.nqubits, middle_qubit + 1)
-    # new circuit object that will be compatible with hardware connectivity
-    new = circuit.__class__(nqubits)
-    # list to maps logical to hardware qubits
-    hardware_qubits = list(range(nqubits))
-
-    # find initial qubit mapping
-    for i, gate in enumerate(circuit.queue):
-        if len(gate.qubits) == 2:
-            if middle_qubit not in gate.qubits:
-                new_middle = find_connected_qubit(gate.qubits, circuit.queue[i + 1 :], hardware_qubits)
+    middle_qubit: int
+    """Qubit id of the qubit that is in the middle of the star."""
+    verbose: bool = False
+
+    def tlog(self, message):
+        """Print messages only if ``verbose`` was set to ``True``."""
+        if self.verbose:
+            log.info(message)
+
+    def is_satisfied(self, circuit, middle_qubit=2, verbose=True):
+        """Checks if a circuit respects connectivity constraints.
+
+        Args:
+            circuit (qibo.models.Circuit): Circuit model to check.
+            middle_qubit (int): Hardware middle qubit.
+            verbose (bool): If ``True`` it prints debugging log messages.
+
+        Returns ``True`` if the following conditions are satisfied:
+            - Circuit does not contain more than two-qubit gates.
+            - All two-qubit gates have qubit 0 as target or control.
+        otherwise returns ``False``.
+        """
+        for gate in circuit.queue:
+            if len(gate.qubits) > 2 and not isinstance(gate, gates.M):
+                self.tlog(f"{gate.name} acts on more than two qubits.")
+                return False
+            elif len(gate.qubits) == 2:
+                if self.middle_qubit not in gate.qubits:
+                    self.tlog("Circuit does not respect connectivity. " f"{gate.name} acts on {gate.qubits}.")
+                    return False
+
+        self.tlog("Circuit respects connectivity.")
+        return True
+
+    def transpile(self, circuit):
+        """Apply the transpiler transformation on a given circuit.
+
+        Args:
+            circuit (qibo.models.Circuit): The original Qibo circuit to transform.
+                This circuit must contain up to two-qubit gates.
+
+        Returns:
+            new (qibo.models.Circuit): Qibo circuit that performs the same operation
+                as the original but respects the hardware connectivity.
+            hardware_qubits (list): List that maps logical to hardware qubits.
+                This is required for transforming final measurements.
+        """
+        # TODO: Change this to a more lightweight form that takes a list of pairs
+        # instead of the whole circuit.
+
+        middle_qubit = self.middle_qubit
+        # find the number of qubits for hardware circuit
+        if circuit.nqubits == 1:
+            nqubits = 1
+        else:
+            nqubits = max(circuit.nqubits, middle_qubit + 1)
+        # new circuit object that will be compatible with hardware connectivity
+        new = circuit.__class__(nqubits)
+        # list to maps logical to hardware qubits
+        hardware_qubits = list(range(nqubits))
+
+        # find initial qubit mapping
+        for i, gate in enumerate(circuit.queue):
+            if len(gate.qubits) == 2:
+                if middle_qubit not in gate.qubits:
+                    new_middle = find_connected_qubit(gate.qubits, circuit.queue[i + 1 :], hardware_qubits)
+                    hardware_qubits[middle_qubit], hardware_qubits[new_middle] = (
+                        hardware_qubits[new_middle],
+                        hardware_qubits[middle_qubit],
+                    )
+                break
+
+        # the first SWAP is not needed as it can be applied via virtual mapping
+        add_swap = False
+        for i, gate in enumerate(circuit.queue):
+            # map gate qubits to hardware
+            qubits = tuple(hardware_qubits.index(q) for q in gate.qubits)
+            if isinstance(gate, gates.M):
+                new_gate = gates.M(*qubits, **gate.init_kwargs)
+                new_gate.result = gate.result
+                new.add(new_gate)
+                continue
+
+            if len(qubits) > 2:
+                raise_error(
+                    NotImplementedError,
+                    "Transpiler does not support gates targeting more than two-qubits.",
+                )
+
+            elif len(qubits) == 2 and middle_qubit not in qubits:
+                # find which qubit should be moved to 0
+                new_middle = find_connected_qubit(qubits, circuit.queue[i + 1 :], hardware_qubits)
+                # update hardware qubits according to the swap
                 hardware_qubits[middle_qubit], hardware_qubits[new_middle] = (
                     hardware_qubits[new_middle],
                     hardware_qubits[middle_qubit],
                 )
-            break
-
-    # the first SWAP is not needed as it can be applied via virtual mapping
-    add_swap = False
-    for i, gate in enumerate(circuit.queue):
-        # map gate qubits to hardware
-        qubits = tuple(hardware_qubits.index(q) for q in gate.qubits)
-        if isinstance(gate, gates.M):
-            new_gate = gates.M(*qubits, **gate.init_kwargs)
-            new_gate.result = gate.result
-            new.add(new_gate)
-            continue
-
-        if len(qubits) > 2:
-            raise_error(
-                NotImplementedError,
-                "Transpiler does not support gates targeting more than two-qubits.",
-            )
-
-        elif len(qubits) == 2 and middle_qubit not in qubits:
-            # find which qubit should be moved to 0
-            new_middle = find_connected_qubit(qubits, circuit.queue[i + 1 :], hardware_qubits)
-            # update hardware qubits according to the swap
-            hardware_qubits[middle_qubit], hardware_qubits[new_middle] = (
-                hardware_qubits[new_middle],
-                hardware_qubits[middle_qubit],
-            )
-            if add_swap:
-                new.add(gates.SWAP(middle_qubit, new_middle))
-            # update gate qubits according to the new swap
-            qubits = tuple(hardware_qubits.index(q) for q in gate.qubits)
-
-        # add gate to the hardware circuit
-        if isinstance(gate, gates.Unitary):
-            # gates.Unitary requires matrix as first argument
-            from qibo.backends import NumpyBackend
-
-            backend = NumpyBackend()
-            matrix = gate.asmatrix(backend)
-            new.add(gate.__class__(matrix, *qubits, **gate.init_kwargs))
-        else:
-            new.add(gate.__class__(*qubits, **gate.init_kwargs))
-        if len(qubits) == 2:
-            add_swap = True
-
-    return new, hardware_qubits
-
-
-def respects_connectivity(circuit, middle_qubit=2, verbose=True):
-    """Checks if a circuit respects connectivity constraints.
-
-    Args:
-        circuit (qibo.models.Circuit): Circuit model to check.
-        middle_qubit (int): Hardware middle qubit.
-        verbose (bool): If ``True`` it prints debugging log messages.
-
-    Returns ``True`` if the following conditions are satisfied:
-        - Circuit does not contain more than two-qubit gates.
-        - All two-qubit gates have qubit 0 as target or control.
-    otherwise returns ``False``.
-    """
-    # pring messages only if ``verbose == True``
-    vlog = lambda msg: log.info(msg) if verbose else lambda msg: None
-    for gate in circuit.queue:
-        if len(gate.qubits) > 2 and not isinstance(gate, gates.M):
-            vlog(f"{gate.name} acts on more than two qubits.")
-            return False
-        elif len(gate.qubits) == 2:
-            if middle_qubit not in gate.qubits:
-                vlog("Circuit does not respect connectivity. " f"{gate.name} acts on {gate.qubits}.")
-                return False
+                if add_swap:
+                    new.add(gates.SWAP(middle_qubit, new_middle))
+                # update gate qubits according to the new swap
+                qubits = tuple(hardware_qubits.index(q) for q in gate.qubits)
+
+            # add gate to the hardware circuit
+            if isinstance(gate, gates.Unitary):
+                # gates.Unitary requires matrix as first argument
+                from qibo.backends import NumpyBackend
+
+                backend = NumpyBackend()
+                matrix = gate.asmatrix(backend)
+                new.add(gate.__class__(matrix, *qubits, **gate.init_kwargs))
+            else:
+                new.add(gate.__class__(*qubits, **gate.init_kwargs))
+            if len(qubits) == 2:
+                add_swap = True
 
-    vlog("Circuit respects connectivity.")
-    return True
+        return new, hardware_qubits
```

### Comparing `qibolab-0.0.2/src/qibolab/transpilers/general_connectivity.py` & `qibolab-0.0.3/src/qibolab/transpilers/general_connectivity.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,177 @@
 import random
+from dataclasses import dataclass
 from enum import Enum, auto
+from typing import Optional, Union
 
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 from more_itertools import pairwise
 from qibo import gates
 from qibo.config import log, raise_error
 from qibo.models import Circuit
 
+from qibolab.transpilers.abstract import Transpiler
+
 DEFAULT_INIT_SAMPLES = 100
 
 
 class QubitInitMethod(Enum):
     """A class to define the initial qubit mapping methods."""
 
     greedy = auto()
     subgraph = auto()
     custom = auto()
 
 
-class Transpiler:
+class GeneralConnectivity(Transpiler):
     """A class to perform initial qubit mapping and connectivity matching.
 
     Properties:
         connectivity (networkx.graph): chip connectivity.
-        init_method (string or QubitInitMethod): initial qubit mapping method.
+        init_method (str or QubitInitMethod): initial qubit mapping method.
         init_samples (int): number of random qubit initializations for greedy initial qubit mapping.
+        sampling_split (float): fraction of paths tested (between 0 and 1).
 
     Attributes:
         _circuit_repr (list): quantum circuit represented as a list (only 2 qubit gates).
         _mapping (dict): circuit to physical qubit mapping during transpiling.
         _graph (networkx.graph): qubit mapped as nodes of the connectivity graph.
         _qubit_map (np.array): circuit to physical qubit mapping during transpiling as vector.
         _circuit_position (int): position in the circuit.
         _added_swaps (int): number of swaps added to the circuit to match connectivity.
     """
 
-    def __init__(self, connectivity, init_method="greedy", init_samples=None):
+    def __init__(self, connectivity, init_method="greedy", init_samples=None, sampling_split=1.0, verbose=False):
         self.connectivity = connectivity
         self.init_method = init_method
         if self.init_method is QubitInitMethod.greedy and init_samples is None:
             init_samples = DEFAULT_INIT_SAMPLES
         self.init_samples = init_samples
+        self.sampling_split = sampling_split
+        self.verbose = verbose
 
         self._circuit_repr = None
         self._mapping = None
         self._graph = None
         self._qubit_map = None
+        self._transpiled_circuit = None
         self._circuit_position = 0
+
         self._added_swaps = 0
+        self._initial_map = None
+        self._final_map = None
+
+    def tlog(self, message):
+        """Print messages only if ``verbose`` was set to ``True``."""
+        if self.verbose:
+            log.info(message)
+
+    def is_satisfied(self, circuit):
+        """Checks if a circuit can be executed on Hardware.
+
+        Args:
+            circuit (qibo.models.Circuit): Circuit model to check.
+            connectivity (networkx.graph): chip connectivity.
+            verbose (bool): If ``True`` it prints debugging log messages.
+
+        Returns ``True`` if the following conditions are satisfied:
+            - Circuit does not contain more than two-qubit gates.
+            - All one-qubit gates are I, Z, RZ or U3.
+            - All two-qubit gates are CZ or iSWAP based on two_qubit_natives.
+            - Circuit matches connectivity.
+        otherwise returns ``False``.
+        """
+        for gate in circuit.queue:
+            if len(gate.qubits) > 2 and not isinstance(gate, gates.M):
+                self.tlog(f"{gate.name} acts on more than two qubits.")
+                return False
+            elif len(gate.qubits) == 2:
+                if gate.qubits not in self.connectivity.edges:
+                    self.tlog("Circuit does not respect connectivity. " f"{gate.name} acts on {gate.qubits}.")
+                    return False
+
+        self.tlog("Circuit respects connectivity.")
+        return True
 
-    def transpile(self, qibo_circuit):
-        """Qubit mapping initialization and circuit transpiling.
+    def transpile(self, circuit):
+        """Qubit mapping initialization and circuit connectivity matching.
 
         Args:
-            qibo_circuit (qibo.Circuit): circuit to be transpiled.
+            circuit (:class:`qibo.models.Circuit`): circuit to be matched to hardware connectivity.
 
         Returns:
             hardware_mapped_circuit (qibo.Circuit): circut mapped to hardware topology.
             final_mapping (dict): final qubit mapping.
             init_mapping (dict): initial qubit mapping.
             added_swaps (int): number of swap gates added.
         """
         self._circuit_position = 0
         self._added_swaps = 0
-        self.translate_circuit(qibo_circuit)
+        self.create_circuit_repr(circuit)
         keys = list(self._connectivity.nodes())
         if self._init_method is QubitInitMethod.greedy:
             self.greedy_init()
         elif self._init_method is QubitInitMethod.subgraph:
+            if len(self._circuit_repr) < 2:
+                raise_error(
+                    ValueError,
+                    "The circuit must contain at least two two-qubit gates in order to apply subgraph initialization",
+                )
             self.subgraph_init()
         elif self._init_method is QubitInitMethod.custom:
             self._mapping = dict(zip(keys, self._mapping.values()))
             self._graph = nx.relabel_nodes(self._connectivity, self._mapping)
         # Inverse permutation
         init_qubit_map = np.argsort(list(self._mapping.values()))
         init_mapping = dict(zip(keys, init_qubit_map))
         self._qubit_map = np.sort(init_qubit_map)
-        self.init_circuit(qibo_circuit)
-        self.first_transpiler_step(qibo_circuit)
+        self.init_circuit(circuit)
+        self.first_transpiler_step(circuit)
         while len(self._circuit_repr) != 0:
-            self.transpiler_step(qibo_circuit)
+            self.transpiler_step(circuit)
         final_mapping = {key: init_qubit_map[self._qubit_map[i]] for i, key in enumerate(keys)}
-        return (
-            self.init_mapping_circuit(self.transpiled_circuit, init_qubit_map),
-            final_mapping,
-            init_mapping,
-            self._added_swaps,
-        )
+        hardware_mapped_circuit = self.init_mapping_circuit(self._transpiled_circuit, init_qubit_map)
+
+        # TODO: Are all those returns needed?
+        # return hardware_mapped_circuit, final_mapping, init_mapping, self._added_swaps
+        self._initial_map = init_mapping
+        self._final_map = final_mapping
+        return hardware_mapped_circuit, [final_mapping[i] for i in range(circuit.nqubits)]
+
+    @property
+    def initial_map(self):
+        return self._initial_map
+
+    @property
+    def final_map(self):
+        return self._final_map
+
+    @property
+    def added_swaps(self):
+        return self._added_swaps
 
     def transpiler_step(self, qibo_circuit):
         """Transpilation step. Find new mapping, add swap gates and apply gates that can be run with this configuration.
 
         Args:
-            qibo_circuit (qibo.Circuit): circuit to be transpiled.
+            qibo_circuit (:class:`qibo.models.Circuit`): circuit to be transpiled.
         """
         len_2q_circuit = len(self._circuit_repr)
         path, meeting_point = self.relocate()
         self.add_swaps(path, meeting_point)
         self.update_qubit_map()
         self.add_gates(qibo_circuit, len_2q_circuit - len(self._circuit_repr))
 
     def first_transpiler_step(self, qibo_circuit):
         """First transpilation step. Apply gates that can be run with the initial qubit mapping.
 
         Args:
-            qibo_circuit (qibo.Circuit): circuit to be transpiled.
+            qibo_circuit (:class:`qibo.models.Circuit`): circuit to be transpiled.
         """
         len_2q_circuit = len(self._circuit_repr)
         self._circuit_repr = self.reduce(self._graph)
         self.add_gates(qibo_circuit, len_2q_circuit - len(self._circuit_repr))
 
     def custom_qubit_mapping(self, map):
         """Define a custom initial qubit mapping.
@@ -125,40 +186,56 @@
     @property
     def connectivity(self):
         return self._connectivity
 
     @connectivity.setter
     def connectivity(self, connectivity):
         """Set the hardware chip connectivity.
-
         Args:
             connectivity (networkx graph): define connectivity.
         """
 
         if isinstance(connectivity, nx.Graph):
             self._connectivity = connectivity
         else:
             raise_error(TypeError, "Use networkx graph for custom connectivity")
 
+    @property
+    def sampling_split(self):
+        return self._sampling_split
+
+    @sampling_split.setter
+    def sampling_split(self, sampling_split):
+        """Set the sampling split.
+
+        Args:
+            sampling_split (float): define fraction of shortest path tested.
+        """
+
+        if sampling_split > 0.0 and 1.0 >= sampling_split:
+            self._sampling_split = sampling_split
+        else:
+            raise_error(ValueError, "Sampling_split must be set greater than 0 and less or equal 1")
+
     def draw_connectivity(self):  # pragma: no cover
         """Show connectivity graph."""
         pos = nx.spectral_layout(self._connectivity)
         nx.draw(self._connectivity, pos=pos, with_labels=True)
         plt.show()
 
     @property
     def init_method(self):
         return self._init_method
 
     @init_method.setter
-    def init_method(self, init_method, init_samples=100):
+    def init_method(self, init_method):
         """Set the initial mapping method for the transpiler.
 
         Args:
-            init_method (string): Initial mapping method ("greedy" or "subgraph").
+            init_method (str): Initial mapping method ("greedy" or "subgraph").
         """
         if isinstance(init_method, str):
             init_method = QubitInitMethod[init_method]
         self._init_method = init_method
 
     @property
     def init_samples(self):
@@ -172,19 +249,19 @@
             init_samples (int): Number of random qubit mapping samples to be tested
             (required only for "greedy" initialization).
         """
         if init_samples is not None:
             self.init_method = QubitInitMethod.greedy
         self._init_samples = init_samples
 
-    def translate_circuit(self, qibo_circuit):
+    def create_circuit_repr(self, qibo_circuit):
         """Translate qibo circuit into a list of two qubit gates to be used by the transpiler.
 
         Args:
-            qibo_circuit (qibo.Circuit): circuit to be transpiled.
+            qibo_circuit (:class:`qibo.models.Circuit`): circuit to be transpiled.
         """
         translated_circuit = []
         for index, gate in enumerate(qibo_circuit.queue):
             if len(gate.qubits) == 2:
                 gate_qubits = list(gate.qubits)
                 gate_qubits.sort()
                 gate_qubits.append(index)
@@ -204,33 +281,40 @@
         """
         new_circuit = self._circuit_repr.copy()
         while new_circuit != [] and (new_circuit[0][0], new_circuit[0][1]) in graph.edges():
             del new_circuit[0]
         return new_circuit
 
     def subgraph_init(self):
-        """Subgraph isomorphism initialization, NP-complete it can take a long time for large circuits."""
+        # TODO fix networkx.GM.mapping for small subgraphs
+        """Subgraph isomorphism initialization, NP-complete it can take a long time for large circuits.
+        This initialization method may fail for very short circuits.
+        """
         H = nx.Graph()
         H.add_nodes_from([i for i in range(self._connectivity.number_of_nodes())])
         GM = nx.algorithms.isomorphism.GraphMatcher(self._connectivity, H)
         i = 0
         H.add_edge(self._circuit_repr[i][0], self._circuit_repr[i][1])
         while GM.subgraph_is_monomorphic() == True:
             result = GM
-            i = i + 1
+            i += 1
             H.add_edge(self._circuit_repr[i][0], self._circuit_repr[i][1])
             GM = nx.algorithms.isomorphism.GraphMatcher(self._connectivity, H)
             if self._connectivity.number_of_edges() == H.number_of_edges() or i == len(self._circuit_repr) - 1:
                 G = nx.relabel_nodes(self._connectivity, result.mapping)
+                keys = list(result.mapping.keys())
+                keys.sort()
                 self._graph = G
-                self._mapping = result.mapping
+                self._mapping = {i: result.mapping[i] for i in keys}
                 return
         G = nx.relabel_nodes(self._connectivity, result.mapping)
+        keys = list(result.mapping.keys())
+        keys.sort()
         self._graph = G
-        self._mapping = result.mapping
+        self._mapping = {i: result.mapping[i] for i in keys}
 
     def greedy_init(self):
         """Initialize the circuit with greedy algorithm let a maximum number of 2-qubit
         gates can be applied without introducing any SWAP gate"""
         nodes = self._connectivity.number_of_nodes()
         keys = list(self._connectivity.nodes())
         final_mapping = dict(zip(keys, list(range(nodes))))
@@ -248,28 +332,33 @@
                 final_graph = graph
                 final_mapping = mapping
                 final_cost = cost
         self._graph = final_graph
         self._mapping = final_mapping
 
     def map_list(self, path):
-        """Return all possible walks of qubits for a given path.
+        """Return all possible walks of qubits, or a fraction, for a given path.
 
         Args:
             path (list): path to move qubits.
 
         Returns:
-            mapping_list (list): all possible walks of qubits for a given path.
-            meeting_point_list (list): all possible qubit meeting point in the path.
+            mapping_list (list): all possible walks of qubits, or a fraction of them based on self.sampling_split, for a given path.
+            meeting_point_list (list): qubit meeting point for each path.
         """
         path_ends = [path[0], path[-1]]
         path_middle = path[1:-1]
         mapping_list = []
         meeting_point_list = []
-        for i in range(len(path) - 1):
+        test_paths = list(range(len(path) - 1))
+        if self.sampling_split != 1.0:
+            test_paths = np.random.choice(
+                test_paths, size=int(np.ceil(len(test_paths) * self.sampling_split)), replace=False
+            )
+        for i in test_paths:
             values = path_middle[:i] + path_ends + path_middle[i:]
             mapping = dict(zip(path, values))
             mapping_list.append(mapping)
             meeting_point_list.append(i)
         return mapping_list, meeting_point_list
 
     def relocate(self):
@@ -284,17 +373,17 @@
         final_circuit = circuit
         keys = list(range(nodes))
         final_graph = self._graph
         final_mapping = dict(zip(keys, keys))
         # Consider all shortest paths
         path_list = [p for p in nx.all_shortest_paths(self._graph, source=circuit[0][0], target=circuit[0][1])]
         self._added_swaps += len(path_list[0]) - 2
-        final_path = path_list[0]
-        # Reduce the number of paths to be faster
+        # Here test all paths
         for path in path_list:
+            # map_list uses self.sampling_split
             list_, meeting_point_list = self.map_list(path)
             for j, mapping in enumerate(list_):
                 new_graph = nx.relabel_nodes(self._graph, mapping)
                 new_circuit = self.reduce(new_graph)
                 # Greedy looking for the optimal path and the optimal walk on this path
                 if len(new_circuit) < len(final_circuit):
                     final_graph = new_graph
@@ -307,63 +396,63 @@
         self._circuit_repr = final_circuit
         return final_path, meeting_point
 
     def init_circuit(self, qibo_circuit):
         """Initialize the transpiled circuit
 
         Args:
-            Args: qibo_circuit (qibo.Circuit): circuit to be transpiled.
+            Args: qibo_circuit (:class:`qibo.models.Circuit`): circuit to be transpiled.
         """
         nodes = self._connectivity.number_of_nodes()
         qubits = qibo_circuit.nqubits
         if qubits > nodes:
             raise_error(ValueError, "There are not enough physical qubits in the hardware to map the circuit")
         elif qubits == nodes:
             new_circuit = Circuit(nodes)
         else:
             log.warning(
                 "You are using more physical qubits than required by the circuit, some qubits will be added to the circuit"
             )
             new_circuit = Circuit(nodes)
-        self.transpiled_circuit = new_circuit
+        self._transpiled_circuit = new_circuit
 
     def init_mapping_circuit(self, circuit, qubit_map):
         """Initial qubit mapping of the transpiled qibo circuit
 
         Args:
-            circuit (qibo.Circuit): transpiled qibo circuit.
+            circuit (:class:`qibo.models.Circuit`): transpiled qibo circuit.
             qubit_map (np.array): initial qubit mapping.
 
         Returns:
-            new_circuit (qibo.Circuit): transpiled circuit mapped with initial qubit mapping.
+            new_circuit (:class:`qibo.models.Circuit`): transpiled circuit mapped with initial qubit mapping.
         """
         new_circuit = Circuit(self._connectivity.number_of_nodes())
         for gate in circuit.queue:
             new_circuit.add(gate.on_qubits({q: qubit_map[q] for q in gate.qubits}))
         return new_circuit
 
     def add_gates(self, qibo_circuit, matched_gates):
         """Add one and two qubit gates to transpiled circuit until connectivity is matched
 
         Args:
-            qibo_circuit (qibo.Circuit): circuit to be transpiled.
+            qibo_circuit (:class:`qibo.models.Circuit`): circuit to be transpiled.
             matched_gates (int): number of two qubit gates that can be applied with the current qubit mapping
         """
         index = 0
         while self._circuit_position < len(qibo_circuit.queue):
             gate = qibo_circuit.queue[self._circuit_position]
             if len(gate.qubits) == 1:
-                self.transpiled_circuit.add(gate.on_qubits({gate.qubits[0]: self._qubit_map[gate.qubits[0]]}))
+                self._transpiled_circuit.add(gate.on_qubits({gate.qubits[0]: self._qubit_map[gate.qubits[0]]}))
                 self._circuit_position += 1
             else:
                 index += 1
                 if index == matched_gates + 1:
                     break
                 else:
-                    self.transpiled_circuit.add(
+                    self._transpiled_circuit.add(
                         gate.on_qubits(
                             {
                                 gate.qubits[0]: self._qubit_map[gate.qubits[0]],
                                 gate.qubits[1]: self._qubit_map[gate.qubits[1]],
                             }
                         )
                     )
@@ -373,20 +462,20 @@
         """Add swaps to the transpiled circuit to move qubits
 
         Args:
             path (list): path to move qubits.
             meeting_point (int): qubit meeting point in the path.
         """
         forward = path[0 : meeting_point + 1]
-        backward = path[meeting_point + 1 :: -1]
+        backward = list(reversed(path[meeting_point + 1 :]))
         if len(forward) > 1:
             for f1, f2 in pairwise(forward):
-                self.transpiled_circuit.add(gates.SWAP(self._qubit_map[f1], self._qubit_map[f2]))
+                self._transpiled_circuit.add(gates.SWAP(self._qubit_map[f1], self._qubit_map[f2]))
         if len(backward) > 1:
             for b1, b2 in pairwise(backward):
-                self.transpiled_circuit.add(gates.SWAP(self._qubit_map[b1], self._qubit_map[b2]))
+                self._transpiled_circuit.add(gates.SWAP(self._qubit_map[b1], self._qubit_map[b2]))
 
     def update_qubit_map(self):
         """Update the qubit mapping after adding swaps"""
         old_mapping = self._qubit_map.copy()
         for key, value in self._mapping.items():
             self._qubit_map[value] = old_mapping[key]
```

### Comparing `qibolab-0.0.2/src/qibolab/transpilers/unitary_decompositions.py` & `qibolab-0.0.3/src/qibolab/transpilers/unitary_decompositions.py`

 * *Files identical despite different names*

