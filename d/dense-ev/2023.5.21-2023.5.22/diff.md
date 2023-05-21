# Comparing `tmp/dense_ev-2023.5.21.tar.gz` & `tmp/dense_ev-2023.5.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dense_ev-2023.5.21.tar", last modified: Sun May 21 21:37:22 2023, max compression
+gzip compressed data, was "dense_ev-2023.5.22.tar", last modified: Sun May 21 23:31:56 2023, max compression
```

## Comparing `dense_ev-2023.5.21.tar` & `dense_ev-2023.5.22.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 atlytle   (1000) atlytle   (1000)        0 2023-05-21 21:37:22.067572 dense_ev-2023.5.21/
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)    11357 2023-05-17 18:55:58.000000 dense_ev-2023.5.21/LICENSE.txt
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)      197 2023-05-21 21:37:22.067572 dense_ev-2023.5.21/PKG-INFO
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)     1596 2023-05-17 22:05:42.000000 dense_ev-2023.5.21/README.md
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)      391 2023-05-21 21:03:08.000000 dense_ev-2023.5.21/pyproject.toml
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)       38 2023-05-21 21:37:22.067572 dense_ev-2023.5.21/setup.cfg
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)       92 2023-05-11 00:44:22.000000 dense_ev-2023.5.21/setup.py
-drwxr-xr-x   0 atlytle   (1000) atlytle   (1000)        0 2023-05-21 21:37:22.053572 dense_ev-2023.5.21/src/
-drwxr-xr-x   0 atlytle   (1000) atlytle   (1000)        0 2023-05-21 21:37:22.064572 dense_ev-2023.5.21/src/dense_ev/
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)        0 2023-05-07 20:22:18.000000 dense_ev-2023.5.21/src/dense_ev/__init__.py
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)     4764 2023-05-17 21:39:18.000000 dense_ev-2023.5.21/src/dense_ev/decompose_pauli.py
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)     5425 2023-05-21 20:44:09.000000 dense_ev-2023.5.21/src/dense_ev/dense_grouper.py
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)    33123 2023-05-17 21:35:44.000000 dense_ev-2023.5.21/src/dense_ev/dense_pauli_basis_change.py
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)     5813 2023-05-17 21:36:14.000000 dense_ev-2023.5.21/src/dense_ev/dense_pauli_expectation.py
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)     7951 2023-05-21 20:43:26.000000 dense_ev-2023.5.21/src/dense_ev/rmatrix.py
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)     3521 2023-05-21 20:21:40.000000 dense_ev-2023.5.21/src/dense_ev/test_ops.py
-drwxr-xr-x   0 atlytle   (1000) atlytle   (1000)        0 2023-05-21 21:37:22.066572 dense_ev-2023.5.21/src/dense_ev.egg-info/
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)      197 2023-05-21 21:37:22.000000 dense_ev-2023.5.21/src/dense_ev.egg-info/PKG-INFO
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)      441 2023-05-21 21:37:22.000000 dense_ev-2023.5.21/src/dense_ev.egg-info/SOURCES.txt
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)        1 2023-05-21 21:37:22.000000 dense_ev-2023.5.21/src/dense_ev.egg-info/dependency_links.txt
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)       20 2023-05-21 21:37:22.000000 dense_ev-2023.5.21/src/dense_ev.egg-info/requires.txt
--rw-r--r--   0 atlytle   (1000) atlytle   (1000)        9 2023-05-21 21:37:22.000000 dense_ev-2023.5.21/src/dense_ev.egg-info/top_level.txt
+drwxr-xr-x   0 atlytle   (1000) atlytle   (1000)        0 2023-05-21 23:31:56.354939 dense_ev-2023.5.22/
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)    11357 2023-05-17 18:55:58.000000 dense_ev-2023.5.22/LICENSE.txt
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)    15003 2023-05-21 23:31:56.354939 dense_ev-2023.5.22/PKG-INFO
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)     1731 2023-05-21 23:17:42.000000 dense_ev-2023.5.22/README.md
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)      512 2023-05-21 23:26:29.000000 dense_ev-2023.5.22/pyproject.toml
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)       38 2023-05-21 23:31:56.354939 dense_ev-2023.5.22/setup.cfg
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)       92 2023-05-11 00:44:22.000000 dense_ev-2023.5.22/setup.py
+drwxr-xr-x   0 atlytle   (1000) atlytle   (1000)        0 2023-05-21 23:31:56.340939 dense_ev-2023.5.22/src/
+drwxr-xr-x   0 atlytle   (1000) atlytle   (1000)        0 2023-05-21 23:31:56.351939 dense_ev-2023.5.22/src/dense_ev/
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)        0 2023-05-07 20:22:18.000000 dense_ev-2023.5.22/src/dense_ev/__init__.py
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)     4764 2023-05-17 21:39:18.000000 dense_ev-2023.5.22/src/dense_ev/decompose_pauli.py
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)     5425 2023-05-21 20:44:09.000000 dense_ev-2023.5.22/src/dense_ev/dense_grouper.py
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)    33123 2023-05-17 21:35:44.000000 dense_ev-2023.5.22/src/dense_ev/dense_pauli_basis_change.py
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)     5813 2023-05-17 21:36:14.000000 dense_ev-2023.5.22/src/dense_ev/dense_pauli_expectation.py
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)     7951 2023-05-21 20:43:26.000000 dense_ev-2023.5.22/src/dense_ev/rmatrix.py
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)     3521 2023-05-21 20:21:40.000000 dense_ev-2023.5.22/src/dense_ev/test_ops.py
+drwxr-xr-x   0 atlytle   (1000) atlytle   (1000)        0 2023-05-21 23:31:56.353939 dense_ev-2023.5.22/src/dense_ev.egg-info/
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)    15003 2023-05-21 23:31:56.000000 dense_ev-2023.5.22/src/dense_ev.egg-info/PKG-INFO
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)      441 2023-05-21 23:31:56.000000 dense_ev-2023.5.22/src/dense_ev.egg-info/SOURCES.txt
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)        1 2023-05-21 23:31:56.000000 dense_ev-2023.5.22/src/dense_ev.egg-info/dependency_links.txt
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)       20 2023-05-21 23:31:56.000000 dense_ev-2023.5.22/src/dense_ev.egg-info/requires.txt
+-rw-r--r--   0 atlytle   (1000) atlytle   (1000)        9 2023-05-21 23:31:56.000000 dense_ev-2023.5.22/src/dense_ev.egg-info/top_level.txt
```

### Comparing `dense_ev-2023.5.21/LICENSE.txt` & `dense_ev-2023.5.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dense_ev-2023.5.21/README.md` & `dense_ev-2023.5.22/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,32 @@
-# dense_EV
+# dense_ev
 **dense_ev** implements expectation value measurements in Qiskit using optimal
 dense grouping [arXiv:quant-ph/2305.xxxx](). For an $m$-qubit operator
 that includes all Pauli strings in its decomposition, 
 it provides a speedup of $2^m$ compared to naive evaluation of all strings,
 and $(3/2)^m$ compared to grouping based on qubit-wise commuting (QWC) families.
 
 ## Installation
 Create a virtual environment to sandbox the installation (optional):
 ```bash
 python3 -m venv test-env && source ./test-env/bin/activate
 ```
+To install,
+```bash
+pip install dense-ev
+```
 Install from GitHub:
 ```bash
-pip install git+ssh://git@github.com/atlytle/dense-ev-test.git
+pip install git+ssh://git@github.com/atlytle/dense-ev.git
+```
+To run unit tests,
+```python
+from dense_ev.test_op import run_unit_tests
+
+run_unit_tests()
 ```
 
 ### Qiskit version compatibility
 Note that **dense_ev** specifies `qiskit < 0.43.0`, as the `Opflow` and
 `QuantumInstance` packages have been deprecated as of `Qiskit 0.43.0`.
 We plan to update the code to function with the new `primitives` as this 
 migration continues and more documentation becomes available.
```

### Comparing `dense_ev-2023.5.21/src/dense_ev/decompose_pauli.py` & `dense_ev-2023.5.22/src/dense_ev/decompose_pauli.py`

 * *Files identical despite different names*

### Comparing `dense_ev-2023.5.21/src/dense_ev/dense_grouper.py` & `dense_ev-2023.5.22/src/dense_ev/dense_grouper.py`

 * *Files identical despite different names*

### Comparing `dense_ev-2023.5.21/src/dense_ev/dense_pauli_basis_change.py` & `dense_ev-2023.5.22/src/dense_ev/dense_pauli_basis_change.py`

 * *Files identical despite different names*

### Comparing `dense_ev-2023.5.21/src/dense_ev/dense_pauli_expectation.py` & `dense_ev-2023.5.22/src/dense_ev/dense_pauli_expectation.py`

 * *Files identical despite different names*

### Comparing `dense_ev-2023.5.21/src/dense_ev/rmatrix.py` & `dense_ev-2023.5.22/src/dense_ev/rmatrix.py`

 * *Files identical despite different names*

### Comparing `dense_ev-2023.5.21/src/dense_ev/test_ops.py` & `dense_ev-2023.5.22/src/dense_ev/test_ops.py`

 * *Files identical despite different names*

